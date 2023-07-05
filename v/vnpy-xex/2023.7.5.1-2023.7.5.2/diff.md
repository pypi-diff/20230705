# Comparing `tmp/vnpy_xex-2023.7.5.1.tar.gz` & `tmp/vnpy_xex-2023.7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.7.5.1.tar", last modified: Wed Jul  5 07:50:04 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.7.5.2.tar", last modified: Wed Jul  5 08:01:09 2023, max compression
```

## Comparing `vnpy_xex-2023.7.5.1.tar` & `vnpy_xex-2023.7.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 07:50:04.387660 vnpy_xex-2023.7.5.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.7.5.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-07-05 07:50:04.387774 vnpy_xex-2023.7.5.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.7.5.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-07-05 07:50:04.388338 vnpy_xex-2023.7.5.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.7.5.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 07:50:04.384395 vnpy_xex-2023.7.5.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.7.5.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25292 2023-07-05 07:48:58.000000 vnpy_xex-2023.7.5.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 07:50:04.387422 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-07-05 07:50:04.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-07-05 07:50:04.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-07-05 07:50:04.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-07-05 07:50:04.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-07-05 07:50:04.000000 vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 08:01:09.730019 vnpy_xex-2023.7.5.2/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.7.5.2/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-07-05 08:01:09.730148 vnpy_xex-2023.7.5.2/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.7.5.2/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-07-05 08:01:09.730788 vnpy_xex-2023.7.5.2/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.7.5.2/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 08:01:09.726947 vnpy_xex-2023.7.5.2/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      645 2023-07-05 08:00:16.000000 vnpy_xex-2023.7.5.2/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    25292 2023-07-05 07:48:58.000000 vnpy_xex-2023.7.5.2/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-07-05 08:01:09.729786 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-07-05 08:01:09.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-07-05 08:01:09.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-07-05 08:01:09.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-07-05 08:01:09.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-07-05 08:01:09.000000 vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.7.5.1/LICENSE` & `vnpy_xex-2023.7.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.7.5.1/PKG-INFO` & `vnpy_xex-2023.7.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.7.5.1
+Version: 2023.7.5.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.7.5.1/setup.cfg` & `vnpy_xex-2023.7.5.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.7.5.1
+version = 2023.7.5.2
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.7.5.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.7.5.2/vnpy_xex/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from enum import Enum
 from vnpy.trader.constant import Exchange
 
 # Extract original exchange name list
 exchange_names = [e.name for e in Exchange]
+if "XEX" not in exchange_names:
+    # Add crypto currency exchanges
+    exchange_names.extend([
+        "XEX",
+    ])
+    # Generate new enum class
+    Exchange = Enum("Exchange", zip(exchange_names, exchange_names))
 
-# Add crypto currency exchanges
-exchange_names.extend([
-    "XEX",
-])
-
-# Generate new enum class
-Exchange = Enum("Exchange", zip(exchange_names, exchange_names))
-import vnpy.trader.constant
-
-vnpy.trader.constant.Exchange = Exchange
+    import vnpy.trader.constant
+    vnpy.trader.constant.Exchange = Exchange
 
 import importlib_metadata
 
 from .xex_gateway import XEXSpotGateway
 
 try:
     __version__ = importlib_metadata.version("vnpy_xex")
```

### Comparing `vnpy_xex-2023.7.5.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.7.5.2/vnpy_xex/xex_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.7.5.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.7.5.2/vnpy_xex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.7.5.1
+Version: 2023.7.5.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

