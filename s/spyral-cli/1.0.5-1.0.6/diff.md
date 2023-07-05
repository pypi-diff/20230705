# Comparing `tmp/spyral_cli-1.0.5.tar.gz` & `tmp/spyral_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.5.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.6.tar", max compression
```

## Comparing `spyral_cli-1.0.5.tar` & `spyral_cli-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-05 08:53:24.745054 spyral_cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.5/src/spyral/__init__.py
--rw-r--r--   0        0        0     5793 2023-07-05 08:53:24.745227 spyral_cli-1.0.5/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-05 15:33:45.110669 spyral_cli-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.6/src/spyral/__init__.py
+-rw-r--r--   0        0        0     7007 2023-07-05 15:32:14.537063 spyral_cli-1.0.6/src/spyral/cli.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.6/PKG-INFO
```

### Comparing `spyral_cli-1.0.5/pyproject.toml` & `spyral_cli-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.0.5/src/spyral/cli.py` & `spyral_cli-1.0.6/src/spyral/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, IO, Optional
 import subprocess as sp
 import sys
+import re
 from datetime import datetime
 from pathlib import Path
 import time
 import threading
 import csv
 import platform
 
@@ -51,15 +52,18 @@
         self.time: List[float] = [0]
         self.rss: List[float] = [0]
         self.vms: List[float] = [0]
 
     def run(self, p: psutil.Process):
         try:
             start = datetime.now()
-            while p.is_running() and p.status() in (psutil.STATUS_RUNNING, psutil.STATUS_SLEEPING):
+            while p.is_running() and p.status() in (
+                psutil.STATUS_RUNNING,
+                psutil.STATUS_SLEEPING,
+            ):
                 if self.terminate:
                     return
                 delta = (datetime.now() - start).total_seconds()
                 rss = p.memory_info().rss
                 vms = p.memory_info().vms
                 for subp in p.children(recursive=True):
                     try:
@@ -97,28 +101,34 @@
 
 @app.command()
 def run(
     cmd: List[str],
     interval: float = typer.Option(0.5, "--interval", "-i"),
     output: Path = typer.Option("spyral.csv", "--output", "-o"),
     summary: bool = sys.stdout.isatty(),
+    label: Optional[str] = typer.Option(None, "--label", "-l"),
 ):
     p = psutil.Popen(cmd, stdout=sp.PIPE, stderr=sp.STDOUT)
     console = rich.console.Console()
 
     with rich.live.Live(console=console, transient=not summary) as live, output.open(
         "w"
     ) as ofh:
-        ofh.write("# " + " ".join(cmd) + "\n")
+        ofh.write("# spyral-cmd: " + " ".join(cmd) + "\n")
+        if label is not None:
+            ofh.write("# spyral-label: " + label + "\n")
         mon = Monitor(interval=interval, live=live, output=ofh, command=cmd)
         t = threading.Thread(target=mon.run, args=(p,))
         t.start()
 
         try:
-            while p.is_running() and p.status() in (psutil.STATUS_RUNNING, psutil.STATUS_SLEEPING):
+            while p.is_running() and p.status() in (
+                psutil.STATUS_RUNNING,
+                psutil.STATUS_SLEEPING,
+            ):
                 for line in iter(p.stdout.readline, b""):
                     if not t.is_alive() and mon.exception is not None:
                         print("Monitoring thread has died")
                         print("Exception:", str(mon.exception))
                         raise RuntimeError("Monitoring thread has died")
                     live.console.out(line.decode("utf-8"), highlight=False, end="")
         except KeyboardInterrupt:
@@ -185,7 +195,36 @@
     ax.axhline(df.vms.iloc[vms_imax], ls="--", c="tab:blue")
 
     ax.set(xlabel="time [s]", ylabel="memory [M]")
 
     fig.tight_layout()
     for f in formats:
         fig.savefig(output / f"{csv.stem}.{f.name}")
+
+
+@app.command()
+def maxima(
+    output: Path = typer.Argument(..., dir_okay=False),
+    inputs: List[Path] = typer.Argument(...),
+    extra_columns: List[str] = typer.Option([], "--extra-column", "-e"),
+):
+    import pandas as pd
+
+    with output.open("a") as fh:
+        writer = csv.writer(fh)
+
+        for i in inputs:
+            cmd = None
+            label = None
+            with i.open("r") as ifh:
+                for _, line in zip(range(10), ifh):
+                    if m := re.match(r" *# spyral-cmd: (.*)", line):
+                        cmd = m.group(1).strip()
+                    if m := re.match(r" *# spyral-label: (.*)", line):
+                        label = m.group(1).strip()
+                        break
+            assert cmd or label
+            if label is None:
+                label = cmd
+
+            df = pd.read_csv(i, comment="#")
+            writer.writerow(extra_columns + [label, df.rss.max(), df.vms.max()])
```

### Comparing `spyral_cli-1.0.5/PKG-INFO` & `spyral_cli-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

