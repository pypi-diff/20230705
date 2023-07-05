# Comparing `tmp/stocks-cli-0.2.1.tar.gz` & `tmp/stocks-cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocks-cli-0.2.1.tar", last modified: Wed Jul  5 10:03:20 2023, max compression
+gzip compressed data, was "stocks-cli-0.2.2.tar", last modified: Wed Jul  5 12:47:54 2023, max compression
```

## Comparing `stocks-cli-0.2.1.tar` & `stocks-cli-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.596109 stocks-cli-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 10:03:20.596109 stocks-cli-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.594109 stocks-cli-0.2.1/cli/
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    60865 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/export.py
--rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/export_eln_website_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    64937 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)    37169 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/register.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/stockscli.ini
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:03:20.596109 stocks-cli-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.594109 stocks-cli-0.2.1/stocks/
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.595109 stocks-cli-0.2.1/stocks/assaysniffer/
--rw-rw-rw-   0 root         (0) root         (0)     3787 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocks/assaysniffer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3639 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocks/assaysniffer/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    39729 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocks/assaysniffer/sniffers.py
--rw-rw-rw-   0 root         (0) root         (0)    30404 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocks/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.595109 stocks-cli-0.2.1/stocks_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      647 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 10:03:20.000000 stocks-cli-0.2.1/stocks_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:03:20.596109 stocks-cli-0.2.1/stocksapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocksapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10815 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocksapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocksapi/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    74940 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocksapi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    27299 2023-07-05 10:03:12.000000 stocks-cli-0.2.1/stocksapi/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.173620 stocks-cli-0.2.2/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    60865 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export_eln_website_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    64937 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)    37169 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/stockscli.ini
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks/
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks/assaysniffer/
+-rw-rw-rw-   0 root         (0) root         (0)     3787 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3639 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    39729 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/sniffers.py
+-rw-rw-rw-   0 root         (0) root         (0)    30404 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      647 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/stocksapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10815 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    74940 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    27299 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/models.py
```

### Comparing `stocks-cli-0.2.1/LICENSE.txt` & `stocks-cli-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/PKG-INFO` & `stocks-cli-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.2.1/README.md` & `stocks-cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/__init__.py` & `stocks-cli-0.2.2/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/__main__.py` & `stocks-cli-0.2.2/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/config.py` & `stocks-cli-0.2.2/cli/config.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/export.py` & `stocks-cli-0.2.2/cli/export.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/export_eln_website_utils.py` & `stocks-cli-0.2.2/cli/export_eln_website_utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/export_utils.py` & `stocks-cli-0.2.2/cli/export_utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/fetch.py` & `stocks-cli-0.2.2/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/register.py` & `stocks-cli-0.2.2/cli/register.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/cli/utils.py` & `stocks-cli-0.2.2/cli/utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/setup.py` & `stocks-cli-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="stocks-cli",
-    version="0.2.1",
+    version="0.2.2",
     author="GBCS",
     author_email="gbcs@embl.de",
     packages=["cli", "stocks", "stocks.assaysniffer", "stocksapi"],
     data_files=[('cli', ['cli/stockscli.ini'])],
     include_package_data=True,
     install_requires=requirements,
     extras_require={
```

### Comparing `stocks-cli-0.2.1/stocks/__init__.py` & `stocks-cli-0.2.2/stocks/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocks/assaysniffer/__init__.py` & `stocks-cli-0.2.2/stocks/assaysniffer/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocks/assaysniffer/registry.py` & `stocks-cli-0.2.2/stocks/assaysniffer/registry.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocks/assaysniffer/sniffers.py` & `stocks-cli-0.2.2/stocks/assaysniffer/sniffers.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocks/models.py` & `stocks-cli-0.2.2/stocks/models.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocks_cli.egg-info/PKG-INFO` & `stocks-cli-0.2.2/stocks_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.2.1/stocks_cli.egg-info/SOURCES.txt` & `stocks-cli-0.2.2/stocks_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocksapi/client.py` & `stocks-cli-0.2.2/stocksapi/client.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocksapi/exceptions.py` & `stocks-cli-0.2.2/stocksapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocksapi/manager.py` & `stocks-cli-0.2.2/stocksapi/manager.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.1/stocksapi/models.py` & `stocks-cli-0.2.2/stocksapi/models.py`

 * *Files identical despite different names*

