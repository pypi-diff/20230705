# Comparing `tmp/ome-zarr-0.7.1.tar.gz` & `tmp/ome-zarr-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ome-zarr-0.7.1.tar", last modified: Mon May  8 08:49:11 2023, max compression
+gzip compressed data, was "ome-zarr-0.8.0.tar", last modified: Wed Jul  5 09:48:27 2023, max compression
```

## Comparing `ome-zarr-0.7.1.tar` & `ome-zarr-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.956908 ome-zarr-0.7.1/ome_zarr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/axes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5628 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/ome_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:48:27.515112 ome-zarr-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-05 09:48:27.515112 ome-zarr-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:48:27.515112 ome-zarr-0.8.0/ome_zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6079 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/ome_zarr/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:48:27.515112 ome-zarr-0.8.0/ome_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 09:48:27.000000 ome-zarr-0.8.0/ome_zarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:48:27.515112 ome-zarr-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-05 09:48:24.000000 ome-zarr-0.8.0/setup.py
```

### Comparing `ome-zarr-0.7.1/LICENSE` & `ome-zarr-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/PKG-INFO` & `ome-zarr-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.7.1
+Version: 0.8.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ome-zarr-0.7.1/README.rst` & `ome-zarr-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/axes.py` & `ome-zarr-0.8.0/ome_zarr/axes.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/cli.py` & `ome-zarr-0.8.0/ome_zarr/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List, Union
 
 from .csv import csv_to_zarr
 from .data import astronaut, coins, create_zarr
 from .scale import Scaler
 from .utils import download as zarr_download
 from .utils import info as zarr_info
+from .utils import view as zarr_view
 
 
 def config_logging(loglevel: int, args: argparse.Namespace) -> None:
     """Configure logging taking the `verbose` and `quiet` arguments into account.
 
     Each `-v` increases the `loglevel` by 10 and each `-q` reduces the loglevel by 10.
     For example, an initial loglevel of `INFO` will be converted to `DEBUG` via `-qqv`.
@@ -25,14 +26,20 @@
 
 def info(args: argparse.Namespace) -> None:
     """Wrap the :func:`~ome_zarr.utils.info` method."""
     config_logging(logging.WARN, args)
     list(zarr_info(args.path, stats=args.stats))
 
 
+def view(args: argparse.Namespace) -> None:
+    """Wrap the :func:`~ome_zarr.utils.view` method."""
+    config_logging(logging.WARN, args)
+    zarr_view(args.path, args.port)
+
+
 def download(args: argparse.Namespace) -> None:
     """Wrap the :func:`~ome_zarr.utils.download` method."""
     config_logging(logging.WARN, args)
     zarr_download(args.path, args.output)
 
 
 def create(args: argparse.Namespace) -> None:
@@ -101,14 +108,20 @@
 
     # download
     parser_download = subparsers.add_parser("download")
     parser_download.add_argument("path")
     parser_download.add_argument("--output", default=".")
     parser_download.set_defaults(func=download)
 
+    # view (in ome-ngff-validator in a browser)
+    parser_view = subparsers.add_parser("view")
+    parser_view.add_argument("path")
+    parser_view.add_argument("--port", type=int, default=8000)
+    parser_view.set_defaults(func=view)
+
     # create
     parser_create = subparsers.add_parser("create")
     parser_create.add_argument(
         "--method", choices=("coins", "astronaut"), default="coins"
     )
     parser_create.add_argument("path")
     parser_create.set_defaults(func=create)
```

### Comparing `ome-zarr-0.7.1/ome_zarr/conversions.py` & `ome-zarr-0.8.0/ome_zarr/conversions.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/csv.py` & `ome-zarr-0.8.0/ome_zarr/csv.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/dask_utils.py` & `ome-zarr-0.8.0/ome_zarr/dask_utils.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/data.py` & `ome-zarr-0.8.0/ome_zarr/data.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/format.py` & `ome-zarr-0.8.0/ome_zarr/format.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/io.py` & `ome-zarr-0.8.0/ome_zarr/io.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/reader.py` & `ome-zarr-0.8.0/ome_zarr/reader.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/scale.py` & `ome-zarr-0.8.0/ome_zarr/scale.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr/utils.py` & `ome-zarr-0.8.0/ome_zarr/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """Utility methods for ome_zarr access."""
 
 import json
 import logging
+import os
+import webbrowser
+from http.server import (  # type: ignore[attr-defined]
+    HTTPServer,
+    SimpleHTTPRequestHandler,
+    test,
+)
 from pathlib import Path
 from typing import Iterator, List
 
 import dask
 import dask.array as da
 import zarr
 from dask.diagnostics import ProgressBar
@@ -41,14 +48,43 @@
             if stats:
                 minmax = f" minmax={dask.compute(array.min(), array.max())}"
             print(f"   - {array.shape}{minmax}")
         LOGGER.debug(node.data)
         yield node
 
 
+def view(input_path: str, port: int = 8000) -> None:
+    # serve the parent directory in a simple server with CORS. Open browser
+
+    parent_dir, image_name = os.path.split(input_path)
+    parent_dir = str(parent_dir)
+
+    class CORSRequestHandler(SimpleHTTPRequestHandler):
+        def end_headers(self) -> None:
+            self.send_header("Access-Control-Allow-Origin", "*")
+            SimpleHTTPRequestHandler.end_headers(self)
+
+        def translate_path(self, path: str) -> str:
+            # Since we don't call the class constructor ourselves,
+            # we set the directory here instead
+            self.directory = parent_dir
+            super_path = super().translate_path(path)
+            return super_path
+
+    # open ome-ngff-validator in a web browser...
+    url = (
+        f"https://ome.github.io/ome-ngff-validator/"
+        f"?source=http://localhost:{port}/{image_name}"
+    )
+    webbrowser.open(url)
+
+    # ...then start serving content
+    test(CORSRequestHandler, HTTPServer, port=port)
+
+
 def download(input_path: str, output_dir: str = ".") -> None:
     """Download an OME-Zarr from the given path.
 
     All :class:`Nodes <ome_utils.reader.Node>` that are found from the given path will
     be included in the download.
     """
     location = parse_url(input_path)
```

### Comparing `ome-zarr-0.7.1/ome_zarr/writer.py` & `ome-zarr-0.8.0/ome_zarr/writer.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.1/ome_zarr.egg-info/PKG-INFO` & `ome-zarr-0.8.0/ome_zarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.7.1
+Version: 0.8.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ome-zarr-0.7.1/setup.py` & `ome-zarr-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 install_requires += (["requests"],)
 install_requires += (["scikit-image"],)
 install_requires += (["toolz"],)
 
 
 setup(
     name="ome-zarr",
-    version="0.7.1",
+    version="0.8.0",
     author="The Open Microscopy Team",
     url="https://github.com/ome/ome-zarr-py",
     description="Implementation of images in Zarr files.",
     long_description=read("README.rst"),
     packages=["ome_zarr"],
     py_modules=["ome_zarr"],
     python_requires=">=3.6",
```

