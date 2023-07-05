# Comparing `tmp/watchgha-2.0.0.tar.gz` & `tmp/watchgha-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-ie4eys2t/watchgha-2.0.0.tar", last modified: Sun Jul  2 23:16:07 2023, max compression
+gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-m52gzbl2/watchgha-2.1.0.tar", last modified: Wed Jul  5 11:04:28 2023, max compression
```

## Comparing `watchgha-2.0.0.tar` & `watchgha-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-2.0.0/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-2.0.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       86 2023-07-02 23:07:34.000000 watchgha-2.0.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2597 2023-07-01 16:34:52.000000 watchgha-2.0.0/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10472 2023-07-02 23:16:07.000000 watchgha-2.0.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9524 2023-07-02 23:09:11.000000 watchgha-2.0.0/README.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2023-06-30 21:19:24.000000 watchgha-2.0.0/dev-requirements.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1405 2023-06-29 12:20:29.000000 watchgha-2.0.0/pyproject.toml
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-02 23:16:07.000000 watchgha-2.0.0/setup.cfg
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-07-02 23:10:57.000000 watchgha-2.0.0/src/watchgha/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-2.0.0/src/watchgha/bucketer.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6273 2023-07-02 20:54:10.000000 watchgha-2.0.0/src/watchgha/data_core.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3077 2023-07-02 20:03:45.000000 watchgha-2.0.0/src/watchgha/demo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      404 2023-06-29 12:20:29.000000 watchgha-2.0.0/src/watchgha/git_help.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3152 2023-06-30 21:19:24.000000 watchgha-2.0.0/src/watchgha/http_help.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1108 2023-06-30 21:19:24.000000 watchgha-2.0.0/src/watchgha/utils.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4232 2023-07-02 23:12:28.000000 watchgha-2.0.0/src/watchgha/watch_runs.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10472 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      518 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       45 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/top_level.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)   393385 2023-07-02 21:07:54.000000 watchgha-2.0.0/watch.gif
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-2.1.0/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-2.1.0/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       86 2023-07-02 23:07:34.000000 watchgha-2.1.0/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2597 2023-07-01 16:34:52.000000 watchgha-2.1.0/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:04:28.000000 watchgha-2.1.0/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9739 2023-07-05 10:59:17.000000 watchgha-2.1.0/README.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2023-06-30 21:19:24.000000 watchgha-2.1.0/dev-requirements.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1443 2023-07-05 10:55:33.000000 watchgha-2.1.0/pyproject.toml
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-05 11:04:28.000000 watchgha-2.1.0/setup.cfg
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-07-05 11:00:24.000000 watchgha-2.1.0/src/watchgha/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-2.1.0/src/watchgha/bucketer.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6273 2023-07-02 20:54:10.000000 watchgha-2.1.0/src/watchgha/data_core.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3077 2023-07-02 20:03:45.000000 watchgha-2.1.0/src/watchgha/demo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      404 2023-06-29 12:20:29.000000 watchgha-2.1.0/src/watchgha/git_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3247 2023-07-05 10:54:08.000000 watchgha-2.1.0/src/watchgha/http_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1108 2023-06-30 21:19:24.000000 watchgha-2.1.0/src/watchgha/utils.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4232 2023-07-02 23:12:28.000000 watchgha-2.1.0/src/watchgha/watch_runs.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      518 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       53 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/top_level.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)   393385 2023-07-02 21:07:54.000000 watchgha-2.1.0/watch.gif
```

### Comparing `watchgha-2.0.0/.editorconfig` & `watchgha-2.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/LICENSE.txt` & `watchgha-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/Makefile` & `watchgha-2.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/PKG-INFO` & `watchgha-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.0.0
+Version: 2.1.0
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -188,14 +188,23 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
+2.1.0 — 2023-07-05
+------------------
+
+- Implicit .netrc authentication stopped working, but has been fixed. Thanks,
+  `Rob Weir <pull 11_>`_.
+
+.. _pull 11: https://github.com/nedbat/watchgha/pull/11
+
+
 2.0.0 — 2023-07-02
 ------------------
 
 - The default polling interval is now 15 seconds.
 
 - Now the GitHub repo location and branch name are defaulted from the current
   git repo.  The repo location can be a local directory or GitHub URL. Closes
@@ -278,14 +287,15 @@
 The code is a bit messy and undocumented, and there are no tests.  If you want
 to change the code, open an issue and let's talk about it.
 
 Contributors:
 
 - Ned Batchelder
 - Hugo van Kemenade
+- Rob Weir
 
 
 Back Story
 ==========
 
 This started as a formatter for the output of ``gh run list`` from the `gh
 run command`_.  Then I tried ``gh run watch``, but wasn't happy with its
```

### Comparing `watchgha-2.0.0/README.rst` & `watchgha-2.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,23 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
+2.1.0 — 2023-07-05
+------------------
+
+- Implicit .netrc authentication stopped working, but has been fixed. Thanks,
+  `Rob Weir <pull 11_>`_.
+
+.. _pull 11: https://github.com/nedbat/watchgha/pull/11
+
+
 2.0.0 — 2023-07-02
 ------------------
 
 - The default polling interval is now 15 seconds.
 
 - Now the GitHub repo location and branch name are defaulted from the current
   git repo.  The repo location can be a local directory or GitHub URL. Closes
@@ -255,14 +264,15 @@
 The code is a bit messy and undocumented, and there are no tests.  If you want
 to change the code, open an issue and let's talk about it.
 
 Contributors:
 
 - Ned Batchelder
 - Hugo van Kemenade
+- Rob Weir
 
 
 Back Story
 ==========
 
 This started as a formatter for the output of ``gh run list`` from the `gh
 run command`_.  Then I tried ``gh run watch``, but wasn't happy with its
```

### Comparing `watchgha-2.0.0/pyproject.toml` & `watchgha-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 requires-python = ">= 3.7"
 
 dependencies = [
     "click",
     "dulwich",
     "exceptiongroup",
-    "httpx",
+    "httpx>=0.24.0",    # 0.24.0 added NetRCAuth()
     "rich",
     "trio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `watchgha-2.0.0/src/watchgha/bucketer.py` & `watchgha-2.1.0/src/watchgha/bucketer.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/src/watchgha/data_core.py` & `watchgha-2.1.0/src/watchgha/data_core.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/src/watchgha/demo.py` & `watchgha-2.1.0/src/watchgha/demo.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/src/watchgha/http_help.py` & `watchgha-2.1.0/src/watchgha/http_help.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,24 @@
     def __init__(self):
         # $set_env.py: SAVE_DATA - save all fetched data to get_* files.
         self.save = bool(int(os.environ.get("SAVE_DATA", "0")))
         if self.save:
             with open("get_index.txt", "w") as index:
                 index.write("# URLs fetched:\n")
             self.count = itertools.count()
+        self.auth = None
         self.headers = {}
         token = os.environ.get("GITHUB_TOKEN", "")
         if token:
             self.headers["Authorization"] = f"Bearer {token}"
+        else:
+            self.auth = httpx.NetRCAuth()
 
     async def get_data(self, url):
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(auth=self.auth) as client:
             resp = None
             try:
                 for ntry in range(3):
                     resp = await client.get(
                         url,
                         headers=self.headers,
                         timeout=30,
```

### Comparing `watchgha-2.0.0/src/watchgha/utils.py` & `watchgha-2.1.0/src/watchgha/utils.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/src/watchgha/watch_runs.py` & `watchgha-2.1.0/src/watchgha/watch_runs.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/src/watchgha.egg-info/PKG-INFO` & `watchgha-2.1.0/src/watchgha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.0.0
+Version: 2.1.0
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -188,14 +188,23 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
+2.1.0 — 2023-07-05
+------------------
+
+- Implicit .netrc authentication stopped working, but has been fixed. Thanks,
+  `Rob Weir <pull 11_>`_.
+
+.. _pull 11: https://github.com/nedbat/watchgha/pull/11
+
+
 2.0.0 — 2023-07-02
 ------------------
 
 - The default polling interval is now 15 seconds.
 
 - Now the GitHub repo location and branch name are defaulted from the current
   git repo.  The repo location can be a local directory or GitHub URL. Closes
@@ -278,14 +287,15 @@
 The code is a bit messy and undocumented, and there are no tests.  If you want
 to change the code, open an issue and let's talk about it.
 
 Contributors:
 
 - Ned Batchelder
 - Hugo van Kemenade
+- Rob Weir
 
 
 Back Story
 ==========
 
 This started as a formatter for the output of ``gh run list`` from the `gh
 run command`_.  Then I tried ``gh run watch``, but wasn't happy with its
```

### Comparing `watchgha-2.0.0/src/watchgha.egg-info/SOURCES.txt` & `watchgha-2.1.0/src/watchgha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.0.0/watch.gif` & `watchgha-2.1.0/watch.gif`

 * *Files identical despite different names*

