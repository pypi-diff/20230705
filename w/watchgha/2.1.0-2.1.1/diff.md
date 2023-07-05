# Comparing `tmp/watchgha-2.1.0.tar.gz` & `tmp/watchgha-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-m52gzbl2/watchgha-2.1.0.tar", last modified: Wed Jul  5 11:04:28 2023, max compression
+gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-t25lph3t/watchgha-2.1.1.tar", last modified: Wed Jul  5 11:28:20 2023, max compression
```

## Comparing `watchgha-2.1.0.tar` & `watchgha-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-2.1.0/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-2.1.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       86 2023-07-02 23:07:34.000000 watchgha-2.1.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2597 2023-07-01 16:34:52.000000 watchgha-2.1.0/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:04:28.000000 watchgha-2.1.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9739 2023-07-05 10:59:17.000000 watchgha-2.1.0/README.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2023-06-30 21:19:24.000000 watchgha-2.1.0/dev-requirements.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1443 2023-07-05 10:55:33.000000 watchgha-2.1.0/pyproject.toml
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-05 11:04:28.000000 watchgha-2.1.0/setup.cfg
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-07-05 11:00:24.000000 watchgha-2.1.0/src/watchgha/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-2.1.0/src/watchgha/bucketer.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6273 2023-07-02 20:54:10.000000 watchgha-2.1.0/src/watchgha/data_core.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3077 2023-07-02 20:03:45.000000 watchgha-2.1.0/src/watchgha/demo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      404 2023-06-29 12:20:29.000000 watchgha-2.1.0/src/watchgha/git_help.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3247 2023-07-05 10:54:08.000000 watchgha-2.1.0/src/watchgha/http_help.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1108 2023-06-30 21:19:24.000000 watchgha-2.1.0/src/watchgha/utils.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4232 2023-07-02 23:12:28.000000 watchgha-2.1.0/src/watchgha/watch_runs.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      518 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       53 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-05 11:04:28.000000 watchgha-2.1.0/src/watchgha.egg-info/top_level.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)   393385 2023-07-02 21:07:54.000000 watchgha-2.1.0/watch.gif
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:28:20.000000 watchgha-2.1.1/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-2.1.1/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-2.1.1/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       86 2023-07-02 23:07:34.000000 watchgha-2.1.1/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2972 2023-07-05 11:22:32.000000 watchgha-2.1.1/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:28:20.000000 watchgha-2.1.1/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9739 2023-07-05 11:25:57.000000 watchgha-2.1.1/README.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2023-06-30 21:19:24.000000 watchgha-2.1.1/dev-requirements.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1443 2023-07-05 11:21:51.000000 watchgha-2.1.1/pyproject.toml
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-05 11:28:20.000000 watchgha-2.1.1/setup.cfg
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-07-05 11:26:10.000000 watchgha-2.1.1/src/watchgha/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-2.1.1/src/watchgha/bucketer.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6273 2023-07-02 20:54:10.000000 watchgha-2.1.1/src/watchgha/data_core.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3077 2023-07-02 20:03:45.000000 watchgha-2.1.1/src/watchgha/demo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      404 2023-06-29 12:20:29.000000 watchgha-2.1.1/src/watchgha/git_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3247 2023-07-05 11:23:52.000000 watchgha-2.1.1/src/watchgha/http_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1108 2023-06-30 21:19:24.000000 watchgha-2.1.1/src/watchgha/utils.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4232 2023-07-05 11:23:17.000000 watchgha-2.1.1/src/watchgha/watch_runs.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10687 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      518 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       53 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-05 11:28:20.000000 watchgha-2.1.1/src/watchgha.egg-info/top_level.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)   393385 2023-07-02 21:07:54.000000 watchgha-2.1.1/watch.gif
```

### Comparing `watchgha-2.1.0/.editorconfig` & `watchgha-2.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/LICENSE.txt` & `watchgha-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/Makefile` & `watchgha-2.1.1/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 	pipx install --force -e .
 
 .PHONY: cog_docs
 
 cog_docs:	## Run cog to get docs right
 	python -m cogapp -crP --verbosity=1 README.rst
 
+.PHONY: test_release release check_release
+
 test_release: clean check_release dist test_pypi	## Do all the steps for a test release
 
-release: clean check_release dist pypi tag gh_release	## Do all the steps for a release
+release: clean check_release dist pypi tag gh_release comment	## Do all the steps for a release
 
 check_release: _check_manifest _check_tree _check_readme _check_version	## Check that we are ready for a release
 	@echo "Release checks passed"
 
 _pip_install_e:
 	python -m pip install -q -e .
 
@@ -59,22 +61,29 @@
 	@export VER="$$(python -c "import watchgha as me; print(me.__version__)")" && \
 	if grep -q $$VER README.rst; then \
 		echo 'Current version is in the README.rst'; \
 	else \
 		echo "No entry in README.rst for version $$VER!"; \
 		exit 1; \
 	fi
+	python -m cogapp -cP --check --verbosity=1 README.rst
 
 _check_version: _pip_install_e
 	@export VER="$$(python -c "import watchgha as me; print(me.__version__)")" && \
 	if [[ $$(git tags | grep -q -w $$VER && echo "x") == "x" ]]; then \
 		echo 'A git tag for this version exists! Did you forget to bump the version in src/watchgha/__init__.py?'; \
 		exit 1; \
 	fi
 
+.PHONY: tag gh_release comment
+
 tag: _pip_install_e ## Make a git tag with the version number
 	@export VER="$$(python -c "import watchgha as me; print(me.__version__)")" && \
 	git tag -a -m "Version $$VER" $$VER
 	git push --all
 
 gh_release:	## Publish a GitHub release
 	python -m scriv github-release --all
+
+comment:	## Show the markdown for a "shipped" comment.
+	@export VER="$$(python -c "import watchgha as me; print(me.__version__)")" && \
+	echo "This is now released as part of [watchgha $$VER](https://pypi.org/project/watchgha/$$VER)."
```

### Comparing `watchgha-2.1.0/PKG-INFO` & `watchgha-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.1.0
+Version: 2.1.1
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -188,15 +188,15 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
-2.1.0 — 2023-07-05
+2.1.1 — 2023-07-05
 ------------------
 
 - Implicit .netrc authentication stopped working, but has been fixed. Thanks,
   `Rob Weir <pull 11_>`_.
 
 .. _pull 11: https://github.com/nedbat/watchgha/pull/11
```

### Comparing `watchgha-2.1.0/README.rst` & `watchgha-2.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
-2.1.0 — 2023-07-05
+2.1.1 — 2023-07-05
 ------------------
 
 - Implicit .netrc authentication stopped working, but has been fixed. Thanks,
   `Rob Weir <pull 11_>`_.
 
 .. _pull 11: https://github.com/nedbat/watchgha/pull/11
```

### Comparing `watchgha-2.1.0/pyproject.toml` & `watchgha-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 requires-python = ">= 3.7"
 
 dependencies = [
     "click",
     "dulwich",
     "exceptiongroup",
-    "httpx>=0.24.0",    # 0.24.0 added NetRCAuth()
+    "httpx>=0.24.1",    # 0.24.1 added NetRCAuth()
     "rich",
     "trio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `watchgha-2.1.0/src/watchgha/bucketer.py` & `watchgha-2.1.1/src/watchgha/bucketer.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha/data_core.py` & `watchgha-2.1.1/src/watchgha/data_core.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha/demo.py` & `watchgha-2.1.1/src/watchgha/demo.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha/http_help.py` & `watchgha-2.1.1/src/watchgha/http_help.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha/utils.py` & `watchgha-2.1.1/src/watchgha/utils.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha/watch_runs.py` & `watchgha-2.1.1/src/watchgha/watch_runs.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/src/watchgha.egg-info/PKG-INFO` & `watchgha-2.1.1/src/watchgha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.1.0
+Version: 2.1.1
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -188,15 +188,15 @@
 
 
 Changelog
 =========
 
 .. scriv-start-here
 
-2.1.0 — 2023-07-05
+2.1.1 — 2023-07-05
 ------------------
 
 - Implicit .netrc authentication stopped working, but has been fixed. Thanks,
   `Rob Weir <pull 11_>`_.
 
 .. _pull 11: https://github.com/nedbat/watchgha/pull/11
```

### Comparing `watchgha-2.1.0/src/watchgha.egg-info/SOURCES.txt` & `watchgha-2.1.1/src/watchgha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.1.0/watch.gif` & `watchgha-2.1.1/watch.gif`

 * *Files identical despite different names*

