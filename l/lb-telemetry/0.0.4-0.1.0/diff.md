# Comparing `tmp/lb-telemetry-0.0.4.tar.gz` & `tmp/lb-telemetry-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb-telemetry-0.0.4.tar", last modified: Wed Jun 21 09:45:34 2023, max compression
+gzip compressed data, was "lb-telemetry-0.1.0.tar", last modified: Wed Jul  5 14:24:36 2023, max compression
```

## Comparing `lb-telemetry-0.0.4.tar` & `lb-telemetry-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 09:45:34.716152 lb-telemetry-0.0.4/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       30 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/.flake8
--rw-r--r--   0 cmcclymont   (501) staff       (20)       38 2023-06-20 07:46:54.000000 lb-telemetry-0.0.4/.gitignore
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1848 2023-06-19 13:53:10.000000 lb-telemetry-0.0.4/.gitlab-ci.yml
--rw-r--r--   0 cmcclymont   (501) staff       (20)       37 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/.mypy.ini
--rw-r--r--   0 cmcclymont   (501) staff       (20)      690 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 cmcclymont   (501) staff       (20)    18151 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/.pylintrc
--rw-r--r--   0 cmcclymont   (501) staff       (20)    35065 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/LICENSE
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1396 2023-06-21 09:45:34.716288 lb-telemetry-0.0.4/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      719 2023-06-21 07:35:51.000000 lb-telemetry-0.0.4/README.md
--rw-r--r--   0 cmcclymont   (501) staff       (20)      979 2023-06-21 09:45:19.000000 lb-telemetry-0.0.4/pyproject.toml
--rw-r--r--   0 cmcclymont   (501) staff       (20)      116 2023-06-20 07:41:21.000000 lb-telemetry-0.0.4/requirements.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)      250 2023-06-21 09:45:34.716675 lb-telemetry-0.0.4/setup.cfg
--rw-r--r--   0 cmcclymont   (501) staff       (20)      894 2023-06-09 07:44:16.000000 lb-telemetry-0.0.4/setup.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 09:45:34.711220 lb-telemetry-0.0.4/src/
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 09:45:34.714757 lb-telemetry-0.0.4/src/lb_telemetry/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       21 2023-06-20 14:20:00.000000 lb-telemetry-0.0.4/src/lb_telemetry/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     2984 2023-06-21 09:44:11.000000 lb-telemetry-0.0.4/src/lb_telemetry/logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 09:45:34.715926 lb-telemetry-0.0.4/src/lb_telemetry/tests/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       60 2023-06-19 12:43:48.000000 lb-telemetry-0.0.4/src/lb_telemetry/tests/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     2814 2023-06-21 09:44:11.000000 lb-telemetry-0.0.4/src/lb_telemetry/tests/test_logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-06-21 09:45:34.715553 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1396 2023-06-21 09:45:34.000000 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      474 2023-06-21 09:45:34.000000 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)        1 2023-06-21 09:45:34.000000 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       17 2023-06-21 09:45:34.000000 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/requires.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       13 2023-06-21 09:45:34.000000 lb-telemetry-0.0.4/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.366642 lb-telemetry-0.1.0/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     2191 2023-07-05 13:43:47.000000 lb-telemetry-0.1.0/.gitignore
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     2084 2023-07-05 13:55:01.000000 lb-telemetry-0.1.0/.gitlab-ci.yml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       37 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/.mypy.ini
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      657 2023-07-05 13:58:55.000000 lb-telemetry-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)    18151 2023-06-22 14:51:29.000000 lb-telemetry-0.1.0/.pylintrc
+-rw-r--r--   0 cmcclymont   (501) staff       (20)    35065 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/LICENSE
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     1359 2023-07-05 14:24:36.366470 lb-telemetry-0.1.0/PKG-INFO
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      705 2023-06-26 11:09:24.000000 lb-telemetry-0.1.0/README.md
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      979 2023-07-05 14:22:15.000000 lb-telemetry-0.1.0/pyproject.toml
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      156 2023-07-05 13:51:18.000000 lb-telemetry-0.1.0/requirements.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       38 2023-07-05 14:24:36.366687 lb-telemetry-0.1.0/setup.cfg
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.364670 lb-telemetry-0.1.0/src/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)        0 2023-06-26 11:25:27.000000 lb-telemetry-0.1.0/src/__init__.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.365282 lb-telemetry-0.1.0/src/lb_telemetry/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       21 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/src/lb_telemetry/__init__.py
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       41 2023-06-27 12:07:56.000000 lb-telemetry-0.1.0/src/lb_telemetry/log_fetch_error.py
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     5447 2023-07-05 12:56:41.000000 lb-telemetry-0.1.0/src/lb_telemetry/logger.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.366214 lb-telemetry-0.1.0/src/lb_telemetry/tests/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       60 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/src/lb_telemetry/tests/__init__.py
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     5203 2023-07-05 13:32:53.000000 lb-telemetry-0.1.0/src/lb_telemetry/tests/test_logger.py
+drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.365869 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/
+-rw-r--r--   0 cmcclymont   (501) staff       (20)     1359 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 cmcclymont   (501) staff       (20)      460 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)        1 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 cmcclymont   (501) staff       (20)       22 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/top_level.txt
```

### Comparing `lb-telemetry-0.0.4/.gitlab-ci.yml` & `lb-telemetry-0.1.0/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,33 +14,43 @@
 stages:
   - lint
   - test
   - build
   - deploy
 
 before_script:
-  - .venv/run pip install -r requirements.txt
+  - source /cvmfs/lhcb.cern.ch/lib/LbEnv
+  - python -m venv .venv
+  - source .venv/bin/activate
+  - pip install -r requirements.txt
+  - pip install -e .
 
-flake8:
+pre_commit:
   stage: lint
   script:
-    - .venv/run flake8 src/lb_telemetry
+    - pre-commit run --all-files
+  allow_failure: true
+
+ruff:
+  stage: lint
+  script:
+    - ruff check src/lb_telemetry --fix
   allow_failure: true
 
 mypy:
   stage: lint
   script:
-    - .venv/run mypy src/lb_telemetry
+    - mypy src/lb_telemetry --explicit-package-bases
   allow_failure: true
 
 tests:
   stage: test
   needs: []
   script:
-    - .venv/run pytest -v
+    - python -m pytest src/lb_telemetry/tests/ -v
   coverage: '/TOTAL.*\s+(\d+%)$/'
 
 package:
   stage: build
   image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.7
   script:
     - python -m build
```

### Comparing `lb-telemetry-0.0.4/.pre-commit-config.yaml` & `lb-telemetry-0.1.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.4.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
-        args: [--branch, main]
+        args: [--branch, master]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.7.0
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 20.8b1
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.8.4
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.277
     hooks:
-      - id: flake8
-        additional_dependencies: [flake8-bugbear]
+      - id: ruff
```

### Comparing `lb-telemetry-0.0.4/.pylintrc` & `lb-telemetry-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.4/LICENSE` & `lb-telemetry-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.0.4/PKG-INFO` & `lb-telemetry-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.0.4
+Version: 0.1.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lb-telemetry
 
 A utility for logging telemetry data about LHCb packages to [MONIT](https://monit.web.cern.ch/).
-Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46). 
+Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46).
 
 The package is not user-callable. It is intended to be imported and called by other LHCb packages such as [PIDCalib2](https://gitlab.cern.ch/lhcb-rta/pidcalib2).
 
 ## Setup
 
 ### Installing from PyPI
 
-The package is available on [PyPI](https://pypi.org/project/lhcb_package_usage_logger/).
+The package is available on [PyPI](https://pypi.org/project/lb-telemetry/).
 It can be installed on any computer via `pip` by running (preferably in a [virtual environment](https://docs.python.org/3/library/venv.html)):
 ```sh
-pip install lb_telemetry
+pip install lb-telemetry
 ```
```

### Comparing `lb-telemetry-0.0.4/README.md` & `lb-telemetry-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # lb-telemetry
 
 A utility for logging telemetry data about LHCb packages to [MONIT](https://monit.web.cern.ch/).
-Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46). 
+Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46).
 
 The package is not user-callable. It is intended to be imported and called by other LHCb packages such as [PIDCalib2](https://gitlab.cern.ch/lhcb-rta/pidcalib2).
 
 ## Setup
 
 ### Installing from PyPI
 
-The package is available on [PyPI](https://pypi.org/project/lhcb_package_usage_logger/).
+The package is available on [PyPI](https://pypi.org/project/lb-telemetry/).
 It can be installed on any computer via `pip` by running (preferably in a [virtual environment](https://docs.python.org/3/library/venv.html)):
 ```sh
-pip install lb_telemetry
+pip install lb-telemetry
 ```
```

### Comparing `lb-telemetry-0.0.4/pyproject.toml` & `lb-telemetry-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lb-telemetry"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
     {name="Cameron McClymont", email="cameron.duncan.mcclymont@cern.ch"},
     {name="Daniel Cervenkov", email="daniel.cervenkov@cern.ch"},
     {name="Chris Burr", email="christopher.burr@cern.ch"},
 ]
 description = "A utility for logging telemetry data from LHCb packages to MONIT"
 readme = "README.md"
```

### Comparing `lb-telemetry-0.0.4/src/lb_telemetry.egg-info/PKG-INFO` & `lb-telemetry-0.1.0/src/lb_telemetry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.0.4
+Version: 0.1.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lb-telemetry
 
 A utility for logging telemetry data about LHCb packages to [MONIT](https://monit.web.cern.ch/).
-Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46). 
+Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46).
 
 The package is not user-callable. It is intended to be imported and called by other LHCb packages such as [PIDCalib2](https://gitlab.cern.ch/lhcb-rta/pidcalib2).
 
 ## Setup
 
 ### Installing from PyPI
 
-The package is available on [PyPI](https://pypi.org/project/lhcb_package_usage_logger/).
+The package is available on [PyPI](https://pypi.org/project/lb-telemetry/).
 It can be installed on any computer via `pip` by running (preferably in a [virtual environment](https://docs.python.org/3/library/venv.html)):
 ```sh
-pip install lb_telemetry
+pip install lb-telemetry
 ```
```

