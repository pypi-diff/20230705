# Comparing `tmp/git-dummy-0.0.8.tar.gz` & `tmp/git-dummy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-dummy-0.0.8.tar", last modified: Wed Jun 14 06:23:49 2023, max compression
+gzip compressed data, was "git-dummy-0.0.9.tar", last modified: Wed Jul  5 01:56:23 2023, max compression
```

## Comparing `git-dummy-0.0.8.tar` & `git-dummy-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.824033 git-dummy-0.0.8/
--rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5804 2023-06-14 06:23:49.824033 git-dummy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5092 2023-06-14 06:01:15.000000 git-dummy-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.816033 git-dummy-0.0.8/git_dummy/
--rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.0.8/git_dummy/__init__.py
--rw-rw-rw-   0        0        0     5146 2023-06-14 06:17:47.000000 git-dummy-0.0.8/git_dummy/__main__.py
--rw-rw-rw-   0        0        0      345 2023-06-14 05:53:40.000000 git-dummy-0.0.8/git_dummy/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:23:49.824033 git-dummy-0.0.8/git_dummy.egg-info/
--rw-rw-rw-   0        0        0     5804 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 06:23:49.000000 git-dummy-0.0.8/git_dummy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:23:49.824033 git-dummy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1214 2023-06-14 06:22:50.000000 git-dummy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.680722 git-dummy-0.0.9/
+-rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5804 2023-07-05 01:56:23.680722 git-dummy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5092 2023-06-14 06:01:15.000000 git-dummy-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.671844 git-dummy-0.0.9/git_dummy/
+-rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.0.9/git_dummy/__init__.py
+-rw-rw-rw-   0        0        0     5146 2023-06-14 06:17:47.000000 git-dummy-0.0.9/git_dummy/__main__.py
+-rw-rw-rw-   0        0        0      405 2023-07-05 01:19:31.000000 git-dummy-0.0.9/git_dummy/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.679507 git-dummy-0.0.9/git_dummy.egg-info/
+-rw-rw-rw-   0        0        0     5804 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 01:56:23.680722 git-dummy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1223 2023-07-05 01:55:53.000000 git-dummy-0.0.9/setup.py
```

### Comparing `git-dummy-0.0.8/LICENSE` & `git-dummy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.8/PKG-INFO` & `git-dummy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
```

### Comparing `git-dummy-0.0.8/README.md` & `git-dummy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.8/git_dummy/__main__.py` & `git-dummy-0.0.9/git_dummy/__main__.py`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.8/git_dummy.egg-info/PKG-INFO` & `git-dummy-0.0.9/git_dummy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
```

### Comparing `git-dummy-0.0.8/setup.py` & `git-dummy-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="git-dummy",
-    version="0.0.8",
+    version="0.0.9",
     author="Jacob Stopak",
     author_email="jacob@initialcommit.io",
     description="Generate dummy Git repositories populated with the desired number of commits, branches, and structure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://initialcommit.com/tools/git-dummy",
     packages=setuptools.find_packages(),
@@ -18,15 +18,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=[
         "gitpython",
         "typer",
-        "pydantic",
+        "pydantic_settings",
     ],
     keywords="git dummy generate populate repo repository",
     project_urls={
         "Homepage": "https://initialcommit.com/tools/git-dummy",
         "Source": "https://github.com/initialcommit-com/git-dummy",
     },
     entry_points={
```

