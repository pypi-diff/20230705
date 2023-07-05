# Comparing `tmp/dimjournal-1.0.5.tar.gz` & `tmp/dimjournal-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimjournal-1.0.5.tar", last modified: Wed Jul  5 01:57:43 2023, max compression
+gzip compressed data, was "dimjournal-1.0.6.tar", last modified: Wed Jul  5 02:02:51 2023, max compression
```

## Comparing `dimjournal-1.0.5.tar` & `dimjournal-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 01:57:32.000000 dimjournal-1.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 01:57:32.000000 dimjournal-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 01:57:32.000000 dimjournal-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 01:57:32.000000 dimjournal-1.0.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 01:57:32.000000 dimjournal-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 01:57:32.000000 dimjournal-1.0.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 01:57:32.000000 dimjournal-1.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-05 01:57:43.927776 dimjournal-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-05 01:57:32.000000 dimjournal-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 01:57:32.000000 dimjournal-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-05 01:57:43.931776 dimjournal-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 01:57:32.000000 dimjournal-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/src/dimjournal/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 01:57:32.000000 dimjournal-1.0.5/src/dimjournal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 01:57:32.000000 dimjournal-1.0.5/src/dimjournal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17122 2023-07-05 01:57:32.000000 dimjournal-1.0.5/src/dimjournal/dimjournal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/src/dimjournal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 01:57:43.000000 dimjournal-1.0.5/src/dimjournal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:43.927776 dimjournal-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 01:57:32.000000 dimjournal-1.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 01:57:32.000000 dimjournal-1.0.5/tests/test_dimjournal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 01:57:32.000000 dimjournal-1.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 02:02:37.000000 dimjournal-1.0.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 02:02:37.000000 dimjournal-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:02:51.152285 dimjournal-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-05 02:02:37.000000 dimjournal-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 02:02:37.000000 dimjournal-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 02:02:51.156285 dimjournal-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 02:02:37.000000 dimjournal-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/dimjournal/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17122 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/dimjournal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/dimjournal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:02:50.000000 dimjournal-1.0.6/src/dimjournal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tests/test_dimjournal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tox.ini
```

### Comparing `dimjournal-1.0.5/.coveragerc` & `dimjournal-1.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/.github/workflows/ci.yml` & `dimjournal-1.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/.gitignore` & `dimjournal-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/.pre-commit-config.yaml` & `dimjournal-1.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/LICENSE.txt` & `dimjournal-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/PKG-INFO` & `dimjournal-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.5
+Version: 1.0.6
 Summary: Archive utility for Midjourney
-Home-page: https://github.com/twardoch/dimjournal
+Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
-Project-URL: Documentation, https://github.com/twardoch/dimjournal
+Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
 Project-URL: Download, https://pypi.org/project/dimjournal
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,22 +21,31 @@
 
 # dimjournal
 
 dimjournal is a Python utility for automatically downloading upscaled images from Midjourney into a local archive (folder tree). 
 
 Note: the terms of use of Midjourney disallow any automation!
 
-dimjournal uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored a folder of your choice.
+dimjournal uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored in the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder, or in a folder of your choice if you specify it.
 
 ## Changelog
 
+- v1.0.6: Fixes
 - v1.0.3: Tested on macOS in July 2023
 
 ## Installation
 
+Stable version:
+
+```
+pip install dimjournal
+```
+
+Development version:
+
 ```
 python3 -m pip install git+https://github.com/twardoch/dimjournal
 ```
 
 ## Usage
 
 ### Command Line Interface (CLI)
```

### Comparing `dimjournal-1.0.5/setup.cfg` & `dimjournal-1.0.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 description = Archive utility for Midjourney
 author = Adam Twardoch
 author_email = adam+github@twardoch.com
 license = Apache-2.0
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
-url = https://github.com/twardoch/dimjournal
+url = https://pypi.org/project/dimjournal/
 project_urls = 
-	Documentation = https://github.com/twardoch/dimjournal
+	Documentation = https://twardoch.github.io/dimjournal/
 	Source = https://github.com/twardoch/dimjournal
 	Download = https://pypi.org/project/dimjournal
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `dimjournal-1.0.5/setup.py` & `dimjournal-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/src/dimjournal/__init__.py` & `dimjournal-1.0.6/src/dimjournal/__init__.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/src/dimjournal/dimjournal.py` & `dimjournal-1.0.6/src/dimjournal/dimjournal.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/src/dimjournal.egg-info/PKG-INFO` & `dimjournal-1.0.6/src/dimjournal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.5
+Version: 1.0.6
 Summary: Archive utility for Midjourney
-Home-page: https://github.com/twardoch/dimjournal
+Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
-Project-URL: Documentation, https://github.com/twardoch/dimjournal
+Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
 Project-URL: Download, https://pypi.org/project/dimjournal
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,22 +21,31 @@
 
 # dimjournal
 
 dimjournal is a Python utility for automatically downloading upscaled images from Midjourney into a local archive (folder tree). 
 
 Note: the terms of use of Midjourney disallow any automation!
 
-dimjournal uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored a folder of your choice.
+dimjournal uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored in the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder, or in a folder of your choice if you specify it.
 
 ## Changelog
 
+- v1.0.6: Fixes
 - v1.0.3: Tested on macOS in July 2023
 
 ## Installation
 
+Stable version:
+
+```
+pip install dimjournal
+```
+
+Development version:
+
 ```
 python3 -m pip install git+https://github.com/twardoch/dimjournal
 ```
 
 ## Usage
 
 ### Command Line Interface (CLI)
```

### Comparing `dimjournal-1.0.5/src/dimjournal.egg-info/SOURCES.txt` & `dimjournal-1.0.6/src/dimjournal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.5/tox.ini` & `dimjournal-1.0.6/tox.ini`

 * *Files identical despite different names*

