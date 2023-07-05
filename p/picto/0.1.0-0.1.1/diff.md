# Comparing `tmp/picto-0.1.0.tar.gz` & `tmp/picto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picto-0.1.0.tar", last modified: Wed Jul  5 02:15:05 2023, max compression
+gzip compressed data, was "picto-0.1.1.tar", last modified: Wed Jul  5 02:19:24 2023, max compression
```

## Comparing `picto-0.1.0.tar` & `picto-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:15:05.078319 picto-0.1.0/
--rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-07-04 14:55:15.000000 picto-0.1.0/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       29 2023-07-04 15:01:35.000000 picto-0.1.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3989 2023-07-05 02:15:05.078319 picto-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-07-05 02:12:34.000000 picto-0.1.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:15:05.078319 picto-0.1.0/picto/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-04 15:05:19.000000 picto-0.1.0/picto/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      230 2023-07-04 21:25:04.000000 picto-0.1.0/picto/__main__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:15:05.078319 picto-0.1.0/picto/cli/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-04 18:22:55.000000 picto-0.1.0/picto/cli/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:15:05.078319 picto-0.1.0/picto/cli/snapshot/
--rw-rw-r--   0 user      (1000) user      (1000)      272 2023-07-05 01:52:51.000000 picto-0.1.0/picto/cli/snapshot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      528 2023-07-05 02:05:23.000000 picto-0.1.0/picto/cli/snapshot/extract.py
--rw-rw-r--   0 user      (1000) user      (1000)     4278 2023-07-05 02:05:29.000000 picto-0.1.0/picto/cli/snapshot/take.py
--rw-rw-r--   0 user      (1000) user      (1000)     5785 2023-07-05 02:05:30.000000 picto-0.1.0/picto/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:15:05.078319 picto-0.1.0/picto.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3989 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      415 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       45 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       44 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-05 02:15:05.000000 picto-0.1.0/picto.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 00:59:22.000000 picto-0.1.0/picto.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       76 2023-07-04 15:01:28.000000 picto-0.1.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)     1951 2023-07-05 02:15:05.078319 picto-0.1.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:19:24.124105 picto-0.1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-07-04 14:55:15.000000 picto-0.1.1/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2023-07-04 15:01:35.000000 picto-0.1.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3989 2023-07-05 02:19:24.124105 picto-0.1.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-07-05 02:12:34.000000 picto-0.1.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:19:24.124105 picto-0.1.1/picto/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-05 02:18:38.000000 picto-0.1.1/picto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      230 2023-07-04 21:25:04.000000 picto-0.1.1/picto/__main__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:19:24.124105 picto-0.1.1/picto/cli/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-04 18:22:55.000000 picto-0.1.1/picto/cli/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:19:24.124105 picto-0.1.1/picto/cli/snapshot/
+-rw-rw-r--   0 user      (1000) user      (1000)      272 2023-07-05 01:52:51.000000 picto-0.1.1/picto/cli/snapshot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      528 2023-07-05 02:05:23.000000 picto-0.1.1/picto/cli/snapshot/extract.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4278 2023-07-05 02:05:29.000000 picto-0.1.1/picto/cli/snapshot/take.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5785 2023-07-05 02:05:30.000000 picto-0.1.1/picto/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 02:19:24.124105 picto-0.1.1/picto.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3989 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      415 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       49 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-05 02:19:24.000000 picto-0.1.1/picto.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 00:59:22.000000 picto-0.1.1/picto.egg-info/zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)       76 2023-07-04 15:01:28.000000 picto-0.1.1/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)     1957 2023-07-05 02:19:24.124105 picto-0.1.1/setup.cfg
```

### Comparing `picto-0.1.0/LICENSE` & `picto-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picto-0.1.0/PKG-INFO` & `picto-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Take bookmarks.json, a URL list, or a single URL - convert those to screenshots
 Home-page: https://github.com/ArchiMoebius/picto
 Download-URL: https://github.com/ArchiMoebius/picto
 Author: Archi Moebius
 Author-email: ArchiMoebius@dojobebo.com
 Maintainer: Archi Moebius
 Maintainer-email: ArchiMoebius@dojobebo.com
```

### Comparing `picto-0.1.0/README.md` & `picto-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `picto-0.1.0/picto/cli/snapshot/extract.py` & `picto-0.1.1/picto/cli/snapshot/extract.py`

 * *Files identical despite different names*

### Comparing `picto-0.1.0/picto/cli/snapshot/take.py` & `picto-0.1.1/picto/cli/snapshot/take.py`

 * *Files identical despite different names*

### Comparing `picto-0.1.0/picto/utils.py` & `picto-0.1.1/picto/utils.py`

 * *Files identical despite different names*

### Comparing `picto-0.1.0/picto.egg-info/PKG-INFO` & `picto-0.1.1/picto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Take bookmarks.json, a URL list, or a single URL - convert those to screenshots
 Home-page: https://github.com/ArchiMoebius/picto
 Download-URL: https://github.com/ArchiMoebius/picto
 Author: Archi Moebius
 Author-email: ArchiMoebius@dojobebo.com
 Maintainer: Archi Moebius
 Maintainer-email: ArchiMoebius@dojobebo.com
```

### Comparing `picto-0.1.0/setup.cfg` & `picto-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 tests_require = isort
 setup_requires = pip
 install_requires = 
 	pytest-playwright
 	slugify
 	pillow
 	typer[all]
+	rich
 
 [options.entry_points]
 console_scripts = 
 	picto = picto.__main__:cli
 
 [options.packages.find]
 where = .
```

