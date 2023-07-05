# Comparing `tmp/dimjournal-1.0.8.tar.gz` & `tmp/dimjournal-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimjournal-1.0.8.tar", last modified: Wed Jul  5 08:13:03 2023, max compression
+gzip compressed data, was "dimjournal-1.0.9.tar", last modified: Wed Jul  5 08:17:49 2023, max compression
```

## Comparing `dimjournal-1.0.8.tar` & `dimjournal-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.591322 dimjournal-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 08:12:47.000000 dimjournal-1.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.587322 dimjournal-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.591322 dimjournal-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 08:12:47.000000 dimjournal-1.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:12:47.000000 dimjournal-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 08:12:47.000000 dimjournal-1.0.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 08:12:47.000000 dimjournal-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 08:12:47.000000 dimjournal-1.0.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 08:12:47.000000 dimjournal-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-05 08:13:03.591322 dimjournal-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 08:12:47.000000 dimjournal-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 08:12:47.000000 dimjournal-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-05 08:13:03.591322 dimjournal-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 08:12:47.000000 dimjournal-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.587322 dimjournal-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.591322 dimjournal-1.0.8/src/dimjournal/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 08:12:47.000000 dimjournal-1.0.8/src/dimjournal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 08:12:47.000000 dimjournal-1.0.8/src/dimjournal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17404 2023-07-05 08:12:47.000000 dimjournal-1.0.8/src/dimjournal/dimjournal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.591322 dimjournal-1.0.8/src/dimjournal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 08:13:03.000000 dimjournal-1.0.8/src/dimjournal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:13:03.591322 dimjournal-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 08:12:47.000000 dimjournal-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 08:12:47.000000 dimjournal-1.0.8/tests/test_dimjournal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 08:12:47.000000 dimjournal-1.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.707382 dimjournal-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 08:17:37.000000 dimjournal-1.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.703382 dimjournal-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.703382 dimjournal-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 08:17:37.000000 dimjournal-1.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:17:37.000000 dimjournal-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 08:17:37.000000 dimjournal-1.0.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 08:17:37.000000 dimjournal-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 08:17:37.000000 dimjournal-1.0.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 08:17:37.000000 dimjournal-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-05 08:17:49.707382 dimjournal-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-05 08:17:37.000000 dimjournal-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 08:17:37.000000 dimjournal-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-05 08:17:49.707382 dimjournal-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 08:17:37.000000 dimjournal-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.703382 dimjournal-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.703382 dimjournal-1.0.9/src/dimjournal/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 08:17:37.000000 dimjournal-1.0.9/src/dimjournal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 08:17:37.000000 dimjournal-1.0.9/src/dimjournal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17404 2023-07-05 08:17:37.000000 dimjournal-1.0.9/src/dimjournal/dimjournal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.707382 dimjournal-1.0.9/src/dimjournal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 08:17:49.000000 dimjournal-1.0.9/src/dimjournal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:17:49.707382 dimjournal-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 08:17:37.000000 dimjournal-1.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 08:17:37.000000 dimjournal-1.0.9/tests/test_dimjournal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 08:17:37.000000 dimjournal-1.0.9/tox.ini
```

### Comparing `dimjournal-1.0.8/.coveragerc` & `dimjournal-1.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/.github/workflows/ci.yml` & `dimjournal-1.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/.gitignore` & `dimjournal-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/.pre-commit-config.yaml` & `dimjournal-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/LICENSE.txt` & `dimjournal-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/PKG-INFO` & `dimjournal-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.8
+Version: 1.0.9
 Summary: Archive utility for Midjourney
 Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
@@ -15,21 +15,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-# DimJournal
+# Dimjournal
 
-DimJournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
+Dimjournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
 
 _Note: the terms of use of Midjourney disallow any automation._
 
-DimJournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored in the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder, or in a folder that specify.
+Dimjournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. 
 
 ## Changelog
 
 - v1.0.8: Fixes
 - v1.0.3: Tested on macOS in July 2023
 
 ## Installation
@@ -52,22 +52,22 @@
 
 In Terminal, run:
 
 ```bash
 dimjournal
 ```
 
-or:
+Dimjournal will open a browser where you need to log into MidJourney. The tool will create the backup folder, which by default is the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder. It will operate the browser, download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs), and save it in JSON files in the backup folder. Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
+
+To specify a different backup folder, use: 
 
 ```bash
 python3 -m dimjournal --archive_folder /path/to/your/archive/folder
 ```
 
-This should open a browser where you need to log into MidJourney. Then the tool will operate the browser and download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs). Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
-
 ### Python
 
 You can also use Dimjournal in your Python scripts. Here is an example of how to import and use the `download` function:
 
 ```python
 from dimjournal import download
```

### Comparing `dimjournal-1.0.8/README.md` & `dimjournal-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# DimJournal
+# Dimjournal
 
-DimJournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
+Dimjournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
 
 _Note: the terms of use of Midjourney disallow any automation._
 
-DimJournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored in the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder, or in a folder that specify.
+Dimjournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. 
 
 ## Changelog
 
 - v1.0.8: Fixes
 - v1.0.3: Tested on macOS in July 2023
 
 ## Installation
@@ -31,22 +31,22 @@
 
 In Terminal, run:
 
 ```bash
 dimjournal
 ```
 
-or:
+Dimjournal will open a browser where you need to log into MidJourney. The tool will create the backup folder, which by default is the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder. It will operate the browser, download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs), and save it in JSON files in the backup folder. Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
+
+To specify a different backup folder, use: 
 
 ```bash
 python3 -m dimjournal --archive_folder /path/to/your/archive/folder
 ```
 
-This should open a browser where you need to log into MidJourney. Then the tool will operate the browser and download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs). Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
-
 ### Python
 
 You can also use Dimjournal in your Python scripts. Here is an example of how to import and use the `download` function:
 
 ```python
 from dimjournal import download
```

### Comparing `dimjournal-1.0.8/setup.cfg` & `dimjournal-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/setup.py` & `dimjournal-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/src/dimjournal/__init__.py` & `dimjournal-1.0.9/src/dimjournal/__init__.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/src/dimjournal/dimjournal.py` & `dimjournal-1.0.9/src/dimjournal/dimjournal.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/src/dimjournal.egg-info/PKG-INFO` & `dimjournal-1.0.9/src/dimjournal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.8
+Version: 1.0.9
 Summary: Archive utility for Midjourney
 Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
@@ -15,21 +15,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-# DimJournal
+# Dimjournal
 
-DimJournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
+Dimjournal is a Midjourney backup tool. It automatically downloads the metadata archive and the upscaled images from Midjourney into a local archive (folder tree). It also embeds some basic metadata (like the prompt) into the PNG files. 
 
 _Note: the terms of use of Midjourney disallow any automation._
 
-DimJournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. The files are stored in the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder, or in a folder that specify.
+Dimjournal is a Python tool uses the Selenium WebDriver to log into the Midjourney website, fetch user data, and download job information and images. 
 
 ## Changelog
 
 - v1.0.8: Fixes
 - v1.0.3: Tested on macOS in July 2023
 
 ## Installation
@@ -52,22 +52,22 @@
 
 In Terminal, run:
 
 ```bash
 dimjournal
 ```
 
-or:
+Dimjournal will open a browser where you need to log into MidJourney. The tool will create the backup folder, which by default is the `midjourney/dimjournal` subfolder inside your `Pictures`/`My Pictures` folder. It will operate the browser, download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs), and save it in JSON files in the backup folder. Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
+
+To specify a different backup folder, use: 
 
 ```bash
 python3 -m dimjournal --archive_folder /path/to/your/archive/folder
 ```
 
-This should open a browser where you need to log into MidJourney. Then the tool will operate the browser and download all metadata (up to 2,500 last upscale jobs, and up to 2,500 jobs). Then it will use the browser to download all upscales that are not in the backup folder. If you run the tool again, it will only download new metadata, and new images. 
-
 ### Python
 
 You can also use Dimjournal in your Python scripts. Here is an example of how to import and use the `download` function:
 
 ```python
 from dimjournal import download
```

### Comparing `dimjournal-1.0.8/src/dimjournal.egg-info/SOURCES.txt` & `dimjournal-1.0.9/src/dimjournal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.8/tox.ini` & `dimjournal-1.0.9/tox.ini`

 * *Files identical despite different names*

