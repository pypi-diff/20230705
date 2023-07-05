# Comparing `tmp/github-deploy-1.1.1.tar.gz` & `tmp/github-deploy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/github-deploy/github-deploy/dist/.tmp-u1p_6mtn/github-deploy-1.1.1.tar", last modified: Mon May  1 17:26:57 2023, max compression
+gzip compressed data, was "/home/runner/work/github-deploy/github-deploy/dist/.tmp-lft7evpl/github-deploy-1.1.2.tar", last modified: Wed Jul  5 18:08:59 2023, max compression
```

## Comparing `github-deploy-1.1.1.tar` & `github-deploy-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:26:57.000000 github-deploy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 17:26:16.000000 github-deploy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-01 17:26:16.000000 github-deploy-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-01 17:26:57.000000 github-deploy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-01 17:26:16.000000 github-deploy-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/_http_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/_repo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 17:26:16.000000 github-deploy-1.1.1/github_deploy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 17:26:57.000000 github-deploy-1.1.1/github_deploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:26:57.000000 github-deploy-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 17:26:39.000000 github-deploy-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:59.000000 github-deploy-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 18:08:31.000000 github-deploy-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:08:31.000000 github-deploy-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-05 18:08:59.000000 github-deploy-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-05 18:08:31.000000 github-deploy-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:59.000000 github-deploy-1.1.2/github_deploy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/_http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/_repo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-05 18:08:31.000000 github-deploy-1.1.2/github_deploy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 18:08:58.000000 github-deploy-1.1.2/github_deploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:08:59.000000 github-deploy-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-05 18:08:46.000000 github-deploy-1.1.2/setup.py
```

### Comparing `github-deploy-1.1.1/LICENSE` & `github-deploy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/PKG-INFO` & `github-deploy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-deploy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Deploy yaml files to a large number of repositories in seconds.
 Home-page: https://github.com/tj-python/github-deploy
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 License: MIT
 Keywords: yaml,deploy,poly repository,github,single configuration
 Requires-Python: >=3.7
```

### Comparing `github-deploy-1.1.1/README.md` & `github-deploy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy/commands/_http_utils.py` & `github-deploy-1.1.2/github_deploy/commands/_http_utils.py`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy/commands/_repo_utils.py` & `github-deploy-1.1.2/github_deploy/commands/_repo_utils.py`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy/commands/delete.py` & `github-deploy-1.1.2/github_deploy/commands/delete.py`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy/commands/upload.py` & `github-deploy-1.1.2/github_deploy/commands/upload.py`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy/main.py` & `github-deploy-1.1.2/github_deploy/main.py`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/github_deploy.egg-info/PKG-INFO` & `github-deploy-1.1.2/github_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-deploy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Deploy yaml files to a large number of repositories in seconds.
 Home-page: https://github.com/tj-python/github-deploy
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 License: MIT
 Keywords: yaml,deploy,poly repository,github,single configuration
 Requires-Python: >=3.7
```

### Comparing `github-deploy-1.1.1/github_deploy.egg-info/SOURCES.txt` & `github-deploy-1.1.2/github_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `github-deploy-1.1.1/setup.py` & `github-deploy-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 extras_require = {
     "deploy": deploy_requires,
 }
 
 
 setup(
     name="github-deploy",
-    version="1.1.1",
+    version="1.1.2",
     description="Deploy yaml files to a large number of repositories in seconds.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_TYPE,
     url="https://github.com/tj-python/github-deploy",
     entry_points={
         "console_scripts": [
             "github-deploy=github_deploy.main:main",
```

