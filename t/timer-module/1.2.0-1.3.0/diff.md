# Comparing `tmp/timer-module-1.2.0.tar.gz` & `tmp/timer-module-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-module-1.2.0.tar", last modified: Mon Jul  3 22:10:19 2023, max compression
+gzip compressed data, was "timer-module-1.3.0.tar", last modified: Wed Jul  5 00:09:24 2023, max compression
```

## Comparing `timer-module-1.2.0.tar` & `timer-module-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.649897 timer-module-1.2.0/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2428 2023-07-03 22:10:19.648897 timer-module-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 22:10:19.649897 timer-module-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-07-03 22:04:41.000000 timer-module-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.624860 timer-module-1.2.0/timer_module/
--rw-rw-rw-   0        0        0      120 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/__init__.py
--rw-rw-rw-   0        0        0      357 2023-07-03 21:10:46.000000 timer-module-1.2.0/timer_module/hasher.py
--rw-rw-rw-   0        0        0     3797 2023-07-03 22:06:14.000000 timer-module-1.2.0/timer_module/logger.py
--rw-rw-rw-   0        0        0     6332 2023-07-03 21:14:38.000000 timer-module-1.2.0/timer_module/metrics.py
--rw-rw-rw-   0        0        0     7070 2023-07-03 22:07:45.000000 timer-module-1.2.0/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1296 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/terminal.py
--rw-rw-rw-   0        0        0     1405 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.647897 timer-module-1.2.0/timer_module.egg-info/
--rw-rw-rw-   0        0        0     2428 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 00:09:24.439508 timer-module-1.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2809 2023-07-05 00:09:24.438004 timer-module-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2240 2023-07-04 23:44:17.000000 timer-module-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 00:09:24.439508 timer-module-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-05 00:06:52.000000 timer-module-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:09:24.415477 timer-module-1.3.0/timer_module/
+-rw-rw-rw-   0        0        0      120 2023-07-02 20:41:30.000000 timer-module-1.3.0/timer_module/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-07-03 21:10:46.000000 timer-module-1.3.0/timer_module/hasher.py
+-rw-rw-rw-   0        0        0     3797 2023-07-03 22:06:14.000000 timer-module-1.3.0/timer_module/logger.py
+-rw-rw-rw-   0        0        0     6376 2023-07-05 00:06:38.000000 timer-module-1.3.0/timer_module/metrics.py
+-rw-rw-rw-   0        0        0     7070 2023-07-05 00:06:32.000000 timer-module-1.3.0/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1296 2023-07-02 20:41:30.000000 timer-module-1.3.0/timer_module/terminal.py
+-rw-rw-rw-   0        0        0     2508 2023-07-05 00:06:26.000000 timer-module-1.3.0/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:09:24.438004 timer-module-1.3.0/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2809 2023-07-05 00:09:24.000000 timer-module-1.3.0/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-05 00:09:24.000000 timer-module-1.3.0/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 00:09:24.000000 timer-module-1.3.0/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 00:09:24.000000 timer-module-1.3.0/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-05 00:09:24.000000 timer-module-1.3.0/timer_module.egg-info/top_level.txt
```

### Comparing `timer-module-1.2.0/LICENSE` & `timer-module-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.2.0/PKG-INFO` & `timer-module-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: timer-module
-Version: 1.2.0
-Summary: Timer Module with performance profiling features
-Home-page: https://github.com/syn-chromatic/timer-module
-Author: syn-chromatic
-Author-email: synchromatic.github@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Utilities
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ___
 ## 📋 Prerequisite:
 ```
 Requires Python >= 3.10
 TimeProfiler makes use of new features from Python's typing module.
 ```
 
@@ -26,43 +9,69 @@
 ## 🛠️ Installation:
 ```
 pip install timer-module
 ```
 
 ___
 ## 🖥️ Timer Usage:
+### Example Usage:
 ```python
 import time
 from timer_module import TimerModule
 
 timer_module = TimerModule().start()
 
 timer_module.pause()
-time.sleep(2)
+time.sleep(0.2)
 
 timer_module.start()
-time.sleep(2)
+time.sleep(0.5)
+
+seconds = timer_module.get_time()
+print(seconds)
+```
+
+#### Get the current time
+```python
+# Seconds
+TimerModule().get_time() # float
+
+# Milliseconds
+TimerModule().get_time_ms() # float
+
+# Nanoseconds
+TimerModule().get_time_ns() # float
+```
+
+
+#### Set the starting time
+```python
+# Seconds
+TimerModule().set_time(1.0)
 
-time_seconds = timer_module.get_time()
-print(time_seconds)
+# Milliseconds
+TimerModule().set_time_ms(1.0)
+
+# Nanoseconds
+TimerModule().set_time_ns(1.0)
 ```
 
-#### Set the timer
+#### Pause timer:
 ```python
-timer_module = TimerModule().set_time(5).start()
+TimerModule().pause()
 ```
 
-#### Refresh time (preserves timer state):
+#### Refresh timer (preserves timer run state):
 ```python
-timer_module.refresh()
+TimerModule().refresh()
 ```
 
-#### Reset time (resets everyting)
+#### Reset timer (resets everything)
 ```python
-timer_module.reset()
+TimerModule().reset()
 ```
 
 ___
 ## 🖥️ Profiler Usage:
 TimeProfiler also includes a "function_profiler" and "async_function_profiler", in a class the asynchronous methods are handled automatically, but for functions you need to select the appropriate decorator.
 
 ```python
@@ -100,9 +109,7 @@
 ec = ExampleClass()
 ec.method_1()
 ```
 
 #### Output:
 ![profiler_output](https://github.com/syn-chromatic/timer-module/assets/68112904/155f7515-fc5a-480b-b7eb-d1e710acae3f)
 
-
-
```

### Comparing `timer-module-1.2.0/setup.py` & `timer-module-1.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
 long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
```

### Comparing `timer-module-1.2.0/timer_module/logger.py` & `timer-module-1.3.0/timer_module/logger.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.2.0/timer_module/metrics.py` & `timer-module-1.3.0/timer_module/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,27 +35,27 @@
         elif nanos >= 1e3:
             return self.format_microseconds()
 
         return self.format_nanoseconds()
 
 
 class CallableMetrics:
-    __slots__ = ("name", "module", "suffix", "call_hash", "ncalls", "time_ns")
+    __slots__ = ("name", "module", "notice", "call_hash", "ncalls", "time_ns")
 
     def __init__(
         self,
         name: str,
         module: str,
-        suffix: str,
+        notice: str,
         ncalls: int,
         time_ns: float,
     ):
         self.name = name
         self.module = module
-        self.suffix = suffix
+        self.notice = notice
         self.ncalls = ncalls
         self.time_ns = time_ns
         self.call_hash = self.get_hash()
 
     def __hash__(self) -> int:
         return self.call_hash
 
@@ -105,20 +105,23 @@
 
     def get_relative_percentage(self, pcall_ns: float, call_ns: float) -> float:
         percentage = 0.0
         if pcall_ns > 0.0 and call_ns > 0.0:
             percentage = (call_ns / pcall_ns) * 100
         return percentage
 
-    def write_primary_call_header(self, call_metrics: CallableMetrics):
+    def get_call_name(self, call_metrics: CallableMetrics):
         pcall_name = call_metrics.name
-        pcall_suffix = call_metrics.suffix
-        if pcall_suffix:
-            pcall_name += f" ({pcall_suffix})"
+        pcall_notice = call_metrics.notice
+        if pcall_notice:
+            pcall_name += f" ({pcall_notice})"
+        return pcall_name
 
+    def write_primary_call_header(self, call_metrics: CallableMetrics):
+        pcall_name = self.get_call_name(call_metrics)
         profile_header = "█ PROFILE: {} █"
         profile_header = profile_header.format(pcall_name)
         separator = "=" * len(profile_header)
         string = "\n{}\n{}"
         string = string.format(profile_header, separator)
         self.terminal.set_ansi_color(self.header_color)
         self.terminal.write(string)
@@ -132,18 +135,15 @@
         percall_time = TimeFormatterNs(percall_time_ns).auto_format()
         string = "Profile Time: [{}]\nNCalls: [{}] — PerCall: [{}]\n——————\n"
         string = string.format(pcall_time, pcall_ncalls, percall_time)
         self.terminal.set_ansi_color(self.call_color)
         self.terminal.write(string)
 
     def write_call_report(self, call_metrics: CallableMetrics, pcall_time: float):
-        call_name = call_metrics.name
-        call_suffix = call_metrics.suffix
-        if call_suffix:
-            call_name += f" ({call_suffix})"
+        call_name = self.get_call_name(call_metrics)
         call_time_ns = call_metrics.time_ns
         call_ncalls = call_metrics.ncalls
         percall_time_ns = call_metrics.get_percall_time()
 
         prc = self.get_relative_percentage(pcall_time, call_time_ns)
         call_time = TimeFormatterNs(call_time_ns).auto_format()
         percall_time = TimeFormatterNs(percall_time_ns).auto_format()
```

### Comparing `timer-module-1.2.0/timer_module/profiler.py` & `timer-module-1.3.0/timer_module/profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,22 +58,22 @@
                 call_metrics = self._timing_refs[pcall_hash][call_hash]
                 call_metrics.time_ns += time_ns
                 call_metrics.ncalls += 1
                 if self._verbose:
                     self._profiler_logger.subcall_event(call_metrics)
 
     @staticmethod
-    def _create_callable_metrics(call: Callable, suffix: str) -> CallableMetrics:
+    def _create_callable_metrics(call: Callable, notice: str) -> CallableMetrics:
         name = call.__qualname__
         module = call.__module__
 
         call_metrics = CallableMetrics(
             name=name,
             module=module,
-            suffix=suffix,
+            notice=notice,
             ncalls=0,
             time_ns=0.0,
         )
         return call_metrics
 
     def _set_pcall_hash(self, call_hash: int):
         pcall_hash = self._pcall_hash
@@ -91,16 +91,16 @@
 
         pcall_timing = self._timing_refs[pcall_hash]
         if call_hash not in pcall_timing:
             call_metrics = self._callable_refs[call_hash]
             new_metrics = call_metrics.fresh_copy()
             pcall_timing.update({call_hash: new_metrics})
 
-    def _add_call_ref(self, call: Callable, suffix: str = "") -> int:
-        call_metrics = self._create_callable_metrics(call, suffix)
+    def _add_call_ref(self, call: Callable, notice: str = "") -> int:
+        call_metrics = self._create_callable_metrics(call, notice)
         call_hash = call_metrics.call_hash
         self._callable_refs[call_hash] = call_metrics
         if self._verbose:
             self._profiler_logger.add_call_reference(call_metrics)
         return call_hash
 
     def _get_method_wrapper(
```

### Comparing `timer-module-1.2.0/timer_module/terminal.py` & `timer-module-1.3.0/timer_module/terminal.py`

 * *Files identical despite different names*

