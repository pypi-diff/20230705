# Comparing `tmp/mtls-0.16.0.tar.gz` & `tmp/mtls-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtls-0.16.0.tar", last modified: Mon Apr 11 21:49:33 2022, max compression
+gzip compressed data, was "mtls-0.17.0.tar", last modified: Wed Jul  5 06:22:37 2023, max compression
```

## Comparing `mtls-0.16.0.tar` & `mtls-0.17.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.771293 mtls-0.16.0/
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.767960 mtls-0.16.0/.circleci/
--rw-r--r--   0 groved    (1000) groved    (1000)     4527 2020-10-18 21:11:29.000000 mtls-0.16.0/.circleci/config.yml
--rw-r--r--   0 groved    (1000) groved    (1000)      244 2019-11-22 05:27:47.000000 mtls-0.16.0/.coveragerc
--rw-r--r--   0 groved    (1000) groved    (1000)      408 2019-11-23 05:19:13.000000 mtls-0.16.0/.editorconfig
--rw-r--r--   0 groved    (1000) groved    (1000)       43 2022-04-11 02:27:15.000000 mtls-0.16.0/.env
--rw-r--r--   0 groved    (1000) groved    (1000)      119 2022-02-08 07:30:11.000000 mtls-0.16.0/.flake8
--rw-r--r--   0 groved    (1000) groved    (1000)      107 2020-06-13 01:48:05.000000 mtls-0.16.0/.gitignore
--rw-r--r--   0 groved    (1000) groved    (1000)      664 2020-10-18 21:11:29.000000 mtls-0.16.0/.travis.yml
--rw-r--r--   0 groved    (1000) groved    (1000)      589 2022-04-11 02:27:15.000000 mtls-0.16.0/LICENSE
--rw-r--r--   0 groved    (1000) groved    (1000)     1764 2022-04-11 19:49:33.000000 mtls-0.16.0/Makefile
--rw-r--r--   0 groved    (1000) groved    (1000)     9557 2022-04-11 21:49:33.771293 mtls-0.16.0/PKG-INFO
--rw-r--r--   0 groved    (1000) groved    (1000)      337 2022-04-11 02:27:15.000000 mtls-0.16.0/Pipfile
--rw-r--r--   0 groved    (1000) groved    (1000)    20988 2022-04-11 02:27:15.000000 mtls-0.16.0/Pipfile.lock
--rw-r--r--   0 groved    (1000) groved    (1000)     8389 2020-06-30 04:38:37.000000 mtls-0.16.0/README.md
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.767960 mtls-0.16.0/bin/
--rwxr-xr-x   0 groved    (1000) groved    (1000)      407 2019-11-22 05:27:47.000000 mtls-0.16.0/bin/mtls
--rw-r--r--   0 groved    (1000) groved    (1000)      352 2019-03-08 06:13:43.000000 mtls-0.16.0/config.ini.example
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.767960 mtls-0.16.0/mtls/
--rw-r--r--   0 groved    (1000) groved    (1000)      436 2022-03-06 04:12:46.000000 mtls-0.16.0/mtls/__init__.py
--rw-r--r--   0 groved    (1000) groved    (1000)       28 2022-03-06 04:12:46.000000 mtls-0.16.0/mtls/__main__.py
--rw-r--r--   0 groved    (1000) groved    (1000)    12952 2022-04-11 07:23:26.000000 mtls-0.16.0/mtls/cli.py
--rw-r--r--   0 groved    (1000) groved    (1000)    39107 2022-04-11 06:56:27.000000 mtls-0.16.0/mtls/mtls.py
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.767960 mtls-0.16.0/mtls/share/
--rw-r--r--   0 groved    (1000) groved    (1000)  1151553 2022-03-06 04:12:46.000000 mtls-0.16.0/mtls/share/password_word_list
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.767960 mtls-0.16.0/mtls.egg-info/
--rw-r--r--   0 groved    (1000) groved    (1000)     9557 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/PKG-INFO
--rw-r--r--   0 groved    (1000) groved    (1000)      601 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/SOURCES.txt
--rw-r--r--   0 groved    (1000) groved    (1000)        1 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/dependency_links.txt
--rw-r--r--   0 groved    (1000) groved    (1000)       38 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/entry_points.txt
--rw-r--r--   0 groved    (1000) groved    (1000)       59 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/requires.txt
--rw-r--r--   0 groved    (1000) groved    (1000)        5 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/top_level.txt
--rw-r--r--   0 groved    (1000) groved    (1000)        1 2022-04-11 21:49:33.000000 mtls-0.16.0/mtls.egg-info/zip-safe
--rw-r--r--   0 groved    (1000) groved    (1000)      174 2022-04-11 07:21:54.000000 mtls-0.16.0/pyproject.toml
--rw-r--r--   0 groved    (1000) groved    (1000)     1223 2022-04-11 02:27:15.000000 mtls-0.16.0/requirements.txt
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.771293 mtls-0.16.0/scripts/
--rwxr-xr-x   0 groved    (1000) groved    (1000)      424 2019-06-06 06:44:41.000000 mtls-0.16.0/scripts/get_build_version.sh
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.771293 mtls-0.16.0/scripts/git-hooks/
--rwxr-xr-x   0 groved    (1000) groved    (1000)       10 2019-03-08 06:13:43.000000 mtls-0.16.0/scripts/git-hooks/pre-commit.sh
--rw-r--r--   0 groved    (1000) groved    (1000)       79 2022-04-11 21:49:33.771293 mtls-0.16.0/setup.cfg
--rw-r--r--   0 groved    (1000) groved    (1000)     1690 2022-03-06 04:12:46.000000 mtls-0.16.0/setup.py
-drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2022-04-11 21:49:33.771293 mtls-0.16.0/test/
--rw-r--r--   0 groved    (1000) groved    (1000)       75 2019-06-06 06:44:41.000000 mtls-0.16.0/test/.coverage
--rw-r--r--   0 groved    (1000) groved    (1000)        0 2019-06-06 06:44:41.000000 mtls-0.16.0/test/__init__.py
--rw-r--r--   0 groved    (1000) groved    (1000)    41219 2022-04-11 06:56:27.000000 mtls-0.16.0/test/test_cli.py
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.902817 mtls-0.17.0/
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.899484 mtls-0.17.0/.circleci/
+-rw-r--r--   0 groved    (1000) groved    (1000)     4398 2023-07-05 04:29:17.000000 mtls-0.17.0/.circleci/config.yml
+-rw-r--r--   0 groved    (1000) groved    (1000)      244 2019-11-22 05:27:47.000000 mtls-0.17.0/.coveragerc
+-rw-r--r--   0 groved    (1000) groved    (1000)      408 2019-11-23 05:19:13.000000 mtls-0.17.0/.editorconfig
+-rw-r--r--   0 groved    (1000) groved    (1000)       43 2022-04-11 02:27:15.000000 mtls-0.17.0/.env
+-rw-r--r--   0 groved    (1000) groved    (1000)      119 2022-02-08 07:30:11.000000 mtls-0.17.0/.flake8
+-rw-r--r--   0 groved    (1000) groved    (1000)      132 2023-07-05 04:29:17.000000 mtls-0.17.0/.gitignore
+-rw-r--r--   0 groved    (1000) groved    (1000)      664 2023-07-05 06:20:33.000000 mtls-0.17.0/.travis.yml
+-rw-r--r--   0 groved    (1000) groved    (1000)      589 2022-04-11 02:27:15.000000 mtls-0.17.0/LICENSE
+-rw-r--r--   0 groved    (1000) groved    (1000)     1383 2023-07-05 04:29:17.000000 mtls-0.17.0/Makefile
+-rw-r--r--   0 groved    (1000) groved    (1000)    10338 2023-07-05 06:22:37.902817 mtls-0.17.0/PKG-INFO
+-rw-r--r--   0 groved    (1000) groved    (1000)      448 2023-07-05 04:29:17.000000 mtls-0.17.0/Pipfile
+-rw-r--r--   0 groved    (1000) groved    (1000)    24725 2023-07-05 04:29:17.000000 mtls-0.17.0/Pipfile.lock
+-rw-r--r--   0 groved    (1000) groved    (1000)     8389 2020-06-30 04:38:37.000000 mtls-0.17.0/README.md
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.899484 mtls-0.17.0/bin/
+-rwxr-xr-x   0 groved    (1000) groved    (1000)      407 2023-07-02 00:43:08.000000 mtls-0.17.0/bin/mtls
+-rw-r--r--   0 groved    (1000) groved    (1000)      352 2019-03-08 06:13:43.000000 mtls-0.17.0/config.ini.example
+-rw-r--r--   0 groved    (1000) groved    (1000)     1577 2023-07-05 04:29:17.000000 mtls-0.17.0/pyproject.toml
+-rw-r--r--   0 groved    (1000) groved    (1000)     8664 2023-07-05 04:29:17.000000 mtls-0.17.0/requirements.txt
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.899484 mtls-0.17.0/scripts/
+-rwxr-xr-x   0 groved    (1000) groved    (1000)      424 2019-06-06 06:44:41.000000 mtls-0.17.0/scripts/get_build_version.sh
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.899484 mtls-0.17.0/scripts/git-hooks/
+-rwxr-xr-x   0 groved    (1000) groved    (1000)       10 2019-03-08 06:13:43.000000 mtls-0.17.0/scripts/git-hooks/pre-commit.sh
+-rw-r--r--   0 groved    (1000) groved    (1000)      532 2023-07-05 06:22:37.902817 mtls-0.17.0/setup.cfg
+-rw-r--r--   0 groved    (1000) groved    (1000)       56 2023-07-05 04:29:17.000000 mtls-0.17.0/setup.py
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.899484 mtls-0.17.0/src/
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.902817 mtls-0.17.0/src/mtls/
+-rw-r--r--   0 groved    (1000) groved    (1000)      314 2023-07-05 04:29:17.000000 mtls-0.17.0/src/mtls/__init__.py
+-rw-r--r--   0 groved    (1000) groved    (1000)       28 2023-07-05 04:29:17.000000 mtls-0.17.0/src/mtls/__main__.py
+-rw-r--r--   0 groved    (1000) groved    (1000)      144 2023-07-05 06:22:36.000000 mtls-0.17.0/src/mtls/__version__.py
+-rw-r--r--   0 groved    (1000) groved    (1000)    12952 2023-07-05 04:29:17.000000 mtls-0.17.0/src/mtls/cli.py
+-rw-r--r--   0 groved    (1000) groved    (1000)    38778 2023-07-05 04:29:17.000000 mtls-0.17.0/src/mtls/mtls.py
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.902817 mtls-0.17.0/src/mtls.egg-info/
+-rw-r--r--   0 groved    (1000) groved    (1000)    10338 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/PKG-INFO
+-rw-r--r--   0 groved    (1000) groved    (1000)      639 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/SOURCES.txt
+-rw-r--r--   0 groved    (1000) groved    (1000)        1 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/dependency_links.txt
+-rw-r--r--   0 groved    (1000) groved    (1000)       38 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/entry_points.txt
+-rw-r--r--   0 groved    (1000) groved    (1000)       59 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/requires.txt
+-rw-r--r--   0 groved    (1000) groved    (1000)        5 2023-07-05 06:22:37.000000 mtls-0.17.0/src/mtls.egg-info/top_level.txt
+-rw-r--r--   0 groved    (1000) groved    (1000)        1 2023-07-04 05:57:30.000000 mtls-0.17.0/src/mtls.egg-info/zip-safe
+drwxr-xr-x   0 groved    (1000) groved    (1000)        0 2023-07-05 06:22:37.902817 mtls-0.17.0/test/
+-rw-r--r--   0 groved    (1000) groved    (1000)       75 2019-06-06 06:44:41.000000 mtls-0.17.0/test/.coverage
+-rw-r--r--   0 groved    (1000) groved    (1000)        0 2019-06-06 06:44:41.000000 mtls-0.17.0/test/__init__.py
+-rw-r--r--   0 groved    (1000) groved    (1000)    41219 2022-04-11 06:56:27.000000 mtls-0.17.0/test/test_cli.py
```

### Comparing `mtls-0.16.0/.circleci/config.yml` & `mtls-0.17.0/.circleci/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         default: /root/.local/share/virtualenvs/
     steps:
       - restore_cache:
           key: pip-<< parameters.key >>-{{ .Branch }}-{{ checksum "Pipfile" }}-{{ checksum "Pipfile.lock" }}
       - run:
           name: Pipenv Install
           command: |
-            python -m pip install --user pip==18.0
+            python -m pip install --user pip
             python -m pip install --user pipenv
-            python -m pipenv --three install --dev
+            python -m pipenv install --dev
           environment:
             PIP_SHIMS_BASE_MODULE: pipenv.patched.notpip
       - save_cache:
           key: pip-<< parameters.key >>-{{ .Branch }}-{{ checksum "Pipfile" }}-{{ checksum "Pipfile.lock" }}
           paths:
           - << parameters.dir >>
   test:
@@ -57,15 +57,15 @@
             brew upgrade
             brew update
             brew install python3 gnupg pipenv || true
 
 executors:
   linux:
     docker:
-      - image: circleci/python:3.7-stretch
+      - image: cimg/python:3.11
         environment:
           PIPENV_VENV_IN_PROJECT: true
   osx:
     macos:
       xcode: "10.0.0"
 
 jobs:
@@ -115,19 +115,16 @@
     executor: linux
     working_directory: ~/mtls-cli
     steps:
       - attach_workspace:
           at: ~/mtls-cli
       - pip_install
       - run:
-          name: Update requirements.txt
-          command: pipenv lock -r > requirements.txt
-      - run:
           name: Create Distribution
-          command: make pkg
+          command: make build
       - store_artifacts:
           path: dist/
 
   test:
     executor: linux
     working_directory: ~/mtls-cli
     steps:
```

### Comparing `mtls-0.16.0/.travis.yml` & `mtls-0.17.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `mtls-0.16.0/LICENSE` & `mtls-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mtls-0.16.0/Makefile` & `mtls-0.17.0/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 SHELL := /bin/bash
 PIP_ENV:=$(shell pipenv --venv)
 ROOT_DIR:=$(shell dirname $(realpath $(lastword $(MAKEFILE_LIST))))
 DESTDIR ?= ~/.local/bin/
 SIGN := 1
-VERSION := $(shell pipenv run python3 setup.py --version)
 
 ifeq ($(OS),Windows_NT)
     UNAME := Windows
 else
     UNAME := $(shell uname -s)
 endif
 
@@ -23,15 +22,15 @@
 Pipfile.lock:
 	@pipenv lock
 
 .PHONY: requirements.txt
 requirements.txt:
 	@echo "Generating requirements.txt"
 	@echo "# DO NOT EDIT. This file is generated by running 'make requirements.txt'" > requirements.txt
-	@jq -r '.default|to_entries|map("\(.key)\(.value.version) --hash=\(.value.hashes[0])")[]' Pipfile.lock >> requirements.txt
+	@pipenv requirements --hash >> requirements.txt
 
 .PHONY: set-hooks
 set-hooks:
 	@echo "Setting commit hooks"
 	@ ([ ! -L ".git/hooks/pre-commit" ] && \
 		ln -s $(PWD)/scripts/git-hooks/pre-commit.sh .git/hooks/pre-commit) \
 		|| true
@@ -41,25 +40,17 @@
 	@pipenv run black -l 79 ./mtls/*.py
 	@pipenv run black -l 79 ./test/*.py
 
 .PHONY: lint
 lint:
 	@pipenv run pycodestyle **/*.py
 
-.PHONY: build-develop
-build-develop:
-	@pipenv run python setup.py develop
-
-.PHONY: build-pypi
-build-pypi:
-	@pipenv run python setup.py sdist bdist_wheel
-
 .PHONY: build
 build: setup
-	@pipenv run python setup.py build
+	@pipenv run python -m build
 
 .PHONY: run
 run:
 	@pipenv run python3 bin/mtls $(ARGS)
 
 .PHONY: test
 test: setup
@@ -73,14 +64,11 @@
 coverage:
 	-@pipenv run coverage report -m
 
 .PHONY: coveralls
 coveralls:
 	@pipenv run coveralls
 
-.PHONY: pkg
-pkg: build
-	@pipenv run python setup.py sdist bdist_wheel
-
 .PHONY: clean
 clean:
-	@rm -r build dist mtls.egg-info .eggs $(PIP_ENV)
+	@rm dist || true
+	@pipenv clean
```

### Comparing `mtls-0.16.0/PKG-INFO` & `mtls-0.17.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 Metadata-Version: 2.1
 Name: mtls
-Version: 0.16.0
+Version: 0.17.0
 Summary: A short-lived certificate tool based on the Zero Trust network mode
 Home-page: https://github.com/drGrove/mtls-cli
-Author: Danny Grove
-Author-email: danny@drgrovellc.com
-License: UNKNOWN
+Author-email: Danny Grove <danny@drgrovellc.com>
+License: Copyright 2018-2022 Danny Grove
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+        http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+                    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+                    See the License for the specific language governing permissions and
+                    limitations under the License.
+        
 Project-URL: Homepage, https://github.com/drGrove/mtls-cli
 Project-URL: Source, https://github.com/drGrove/mtls-cli
 Project-URL: Tracker, https://github.com/drGrove/mtls-cli/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -17,17 +29,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mutual TLS Client (mtls) #
 
 [![Known Vulnerabilities](https://snyk.io/test/github/drGrove/mtls-cli/badge.svg)](https://snyk.io/test/github/drGrove/mtls-cli)
 [![CircleCI](https://circleci.com/gh/drGrove/mtls-cli/tree/master.svg?style=svg)](https://circleci.com/gh/drGrove/mtls-cli/tree/master)
```

### Comparing `mtls-0.16.0/Pipfile.lock` & `mtls-0.17.0/Pipfile.lock`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9221230158730158%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'5846ae9dbcd797624d30a516bbaae5664afb3d407fac2c18515a85e4ebea31a4'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              '\'version\': \'==2023.5.7\', \'markers\': "python_version >= \'3.6\'"}, \'cffi\': '*

 * *              "{'hashes': "*

 * *              "['sha256:00a9ed42e88df81f […]*

```diff
@@ -1,92 +1,107 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "072f91e54b836c0197a9db9c4b14ce356d387ed1cdad776c86e539196a51140d"
+            "sha256": "5846ae9dbcd797624d30a516bbaae5664afb3d407fac2c18515a85e4ebea31a4"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
-                "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3",
-                "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2",
-                "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636",
-                "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20",
-                "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728",
-                "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27",
-                "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66",
-                "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443",
-                "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0",
-                "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7",
-                "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39",
-                "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605",
-                "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a",
-                "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37",
-                "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029",
-                "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139",
-                "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc",
-                "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df",
-                "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14",
-                "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880",
-                "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2",
-                "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a",
-                "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e",
-                "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474",
-                "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024",
-                "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8",
-                "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0",
-                "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e",
-                "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a",
-                "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e",
-                "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032",
-                "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6",
-                "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e",
-                "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b",
-                "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e",
-                "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954",
-                "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962",
-                "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c",
-                "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4",
-                "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55",
-                "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962",
-                "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023",
-                "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c",
-                "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6",
-                "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8",
-                "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382",
-                "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7",
-                "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc",
-                "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
-                "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
-            "version": "==1.15.0"
+            "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2842d8f5e82a1f6aa437380934d5e1cd4fcf2003b06fed6940769c164a480a45",
-                "sha256:98398a9d69ee80548c762ba991a4728bfc3836768ed226b3945908d1a688371c"
+                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
+                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
             ],
             "markers": "python_version >= '3'",
-            "version": "==2.0.11"
+            "version": "==2.0.12"
         },
         "click": {
             "hashes": [
                 "sha256:8c04c11192119b1ef78ea049e0a6f0463e4c48ef00a30160c704337586f3ad7a",
                 "sha256:fba402a4a47334742d782209a7c79bc448911afe1149d07bdabdf480b3e2f4b6"
             ],
             "index": "pypi",
@@ -116,19 +131,19 @@
                 "sha256:ec63da4e7e4a5f924b90af42eddf20b698a70e58d86a72d943857c4c6045b3ee"
             ],
             "index": "pypi",
             "version": "==36.0.1"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "version": "==3.4"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
@@ -158,15 +173,15 @@
             "version": "==2.27.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:000ca7f471a233c2251c6c7023ee85305721bfdf18621ebff4fd17a8653427ed",
                 "sha256:0e7c33d9a63e7ddfcb86780aac87befc2fbddf46c58dbb487e0855f7ceec283c"
             ],
@@ -179,28 +194,37 @@
             "hashes": [
                 "sha256:77b80f693a569e2e527958459634f18df9b0ba2625ba4e0c2d5da5be42e6f2b3",
                 "sha256:a615e69ae185e08fdd73e4715e260e2479c861b5740057fde6e8b4e3b7dd589f"
             ],
             "index": "pypi",
             "version": "==21.12b0"
         },
+        "build": {
+            "hashes": [
+                "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
+                "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
+            ],
+            "index": "pypi",
+            "version": "==0.10.0"
+        },
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2842d8f5e82a1f6aa437380934d5e1cd4fcf2003b06fed6940769c164a480a45",
-                "sha256:98398a9d69ee80548c762ba991a4728bfc3836768ed226b3945908d1a688371c"
+                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
+                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
             ],
             "markers": "python_version >= '3'",
-            "version": "==2.0.11"
+            "version": "==2.0.12"
         },
         "click": {
             "hashes": [
                 "sha256:8c04c11192119b1ef78ea049e0a6f0463e4c48ef00a30160c704337586f3ad7a",
                 "sha256:fba402a4a47334742d782209a7c79bc448911afe1149d07bdabdf480b3e2f4b6"
             ],
             "index": "pypi",
@@ -287,48 +311,66 @@
                 "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
             ],
             "index": "pypi",
             "version": "==4.0.1"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "version": "==3.4"
+        },
+        "installer": {
+            "hashes": [
+                "sha256:05d1933f0a5ba7d8d6296bb6d5018e7c94fa473ceb10cf198a92ccea19c27b53",
+                "sha256:a26d3e3116289bb08216e0d0f7d925fcef0b0194eedfa0c944bcaaa106c4b631"
+            ],
+            "index": "pypi",
+            "version": "==0.7.0"
         },
         "mccabe": {
             "hashes": [
                 "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
                 "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
             ],
             "version": "==0.6.1"
         },
         "mypy-extensions": {
             "hashes": [
-                "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
-                "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==0.4.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
+        },
+        "packaging": {
+            "hashes": [
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
-                "sha256:7d15c4ddb0b5c802d161efc417ec1a2558ea2653c2e8ad9c19098201dc1c993a",
-                "sha256:e564499435a2673d586f6b2130bb5b95f04a3ba06f81b8f895b651a3c76aabb1"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
-            "version": "==0.9.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:1d7385c7db91728b83efd0ca99a5afb296cab9d0ed8313a45ed8ba17967ecfca",
-                "sha256:440633ddfebcc36264232365d7840a970e75e1018d15b4327d11f91909045fda"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.4.1"
+            "version": "==3.8.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
                 "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -338,49 +380,81 @@
             "hashes": [
                 "sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c",
                 "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.4.0"
         },
+        "pyproject-hooks": {
+            "hashes": [
+                "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
+                "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.0.0"
+        },
         "requests": {
             "hashes": [
                 "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
                 "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
             ],
             "index": "pypi",
             "version": "==2.27.1"
         },
+        "setuptools": {
+            "hashes": [
+                "sha256:26ead7d1f93efc0f8c804d9fafafbe4a44b179580a7105754b245155f9af05a8",
+                "sha256:47c7b0c0f8fc10eec4cf1e71c6fdadf8decaa74ffa087e68cd1c20db7ad6a592"
+            ],
+            "index": "pypi",
+            "version": "==62.1.0"
+        },
+        "setuptools-scm": {
+            "hashes": [
+                "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
+                "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
+            ],
+            "index": "pypi",
+            "version": "==6.4.2"
+        },
         "tomli": {
             "hashes": [
                 "sha256:05b6166bff487dc068d322585c7ea4ef78deed501cc124060e0f238e89a9231f",
                 "sha256:e3069e4be3ead9668e21cb9b074cd948f7b3113fd9c8bba083f48247aab8b11c"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.2.3"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
-                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
-            "markers": "python_version >= '3.10'",
-            "version": "==4.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:000ca7f471a233c2251c6c7023ee85305721bfdf18621ebff4fd17a8653427ed",
                 "sha256:0e7c33d9a63e7ddfcb86780aac87befc2fbddf46c58dbb487e0855f7ceec283c"
             ],
             "index": "pypi",
             "version": "==1.26.8"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:1315816c0acc508997eb3ae03b9d3ff619c9d12d544c9a9b553704b1cc4f6af5",
-                "sha256:2eed4cc58e4d65613ed6114af2f380f7910ff416fc8c46947f6e76b6815f56c0"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.2.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.6.1"
+        },
+        "wheel": {
+            "hashes": [
+                "sha256:4bdcd7d840138086126cd09254dc6195fb4fc6f01c050a1d7236f2630db1d22a",
+                "sha256:e9a504e793efbca1b8e0e9cb979a249cf4a0a7b5b8c9e8b65a5e39d49529c1c4"
+            ],
+            "index": "pypi",
+            "version": "==0.37.1"
         }
     }
 }
```

### Comparing `mtls-0.16.0/README.md` & `mtls-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `mtls-0.16.0/mtls/cli.py` & `mtls-0.17.0/src/mtls/cli.py`

 * *Files identical despite different names*

### Comparing `mtls-0.16.0/mtls/mtls.py` & `mtls-0.17.0/src/mtls/mtls.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from configparser import ConfigParser
 from json.decoder import JSONDecodeError
 from pathlib import Path
 import base64
 import binascii
 import json
 import os
-import pkg_resources
 import platform
 import random
+import secrets
 import subprocess
 import sys
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
@@ -459,24 +459,15 @@
             click.secho("Failed to decrypt CSR, invalid password.", fg="red")
             sys.exit(1)
         return x509.load_pem_x509_csr(
             bytes(csr_str, "utf-8"), default_backend()
         )
 
     def _genPW(self):
-        wordList = []
-        with pkg_resources.resource_stream(
-            __name__, "share/password_word_list"
-        ) as wordFile:
-            for line in wordFile:
-                wordList.append(line.decode().rstrip("\n"))
-        pw = []
-        for _ in range(10):
-            pw.append(random.choice(wordList))
-        return " ".join(pw).rstrip()
+        return secrets.token_hex(32)
 
     def convert_to_cert(self, cert):
         try:
             cert = bytes(str(cert), "utf-8")
             cert = x509.load_pem_x509_certificate(
                 cert, backend=default_backend()
             )
```

### Comparing `mtls-0.16.0/mtls.egg-info/PKG-INFO` & `mtls-0.17.0/src/mtls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 Metadata-Version: 2.1
 Name: mtls
-Version: 0.16.0
+Version: 0.17.0
 Summary: A short-lived certificate tool based on the Zero Trust network mode
 Home-page: https://github.com/drGrove/mtls-cli
-Author: Danny Grove
-Author-email: danny@drgrovellc.com
-License: UNKNOWN
+Author-email: Danny Grove <danny@drgrovellc.com>
+License: Copyright 2018-2022 Danny Grove
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+        http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+                    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+                    See the License for the specific language governing permissions and
+                    limitations under the License.
+        
 Project-URL: Homepage, https://github.com/drGrove/mtls-cli
 Project-URL: Source, https://github.com/drGrove/mtls-cli
 Project-URL: Tracker, https://github.com/drGrove/mtls-cli/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -17,17 +29,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mutual TLS Client (mtls) #
 
 [![Known Vulnerabilities](https://snyk.io/test/github/drGrove/mtls-cli/badge.svg)](https://snyk.io/test/github/drGrove/mtls-cli)
 [![CircleCI](https://circleci.com/gh/drGrove/mtls-cli/tree/master.svg?style=svg)](https://circleci.com/gh/drGrove/mtls-cli/tree/master)
```

### Comparing `mtls-0.16.0/mtls.egg-info/SOURCES.txt` & `mtls-0.17.0/src/mtls.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 config.ini.example
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .circleci/config.yml
 bin/mtls
-mtls/__init__.py
-mtls/__main__.py
-mtls/cli.py
-mtls/mtls.py
-mtls.egg-info/PKG-INFO
-mtls.egg-info/SOURCES.txt
-mtls.egg-info/dependency_links.txt
-mtls.egg-info/entry_points.txt
-mtls.egg-info/requires.txt
-mtls.egg-info/top_level.txt
-mtls.egg-info/zip-safe
-mtls/share/password_word_list
 scripts/get_build_version.sh
 scripts/git-hooks/pre-commit.sh
+src/mtls/__init__.py
+src/mtls/__main__.py
+src/mtls/__version__.py
+src/mtls/cli.py
+src/mtls/mtls.py
+src/mtls.egg-info/PKG-INFO
+src/mtls.egg-info/SOURCES.txt
+src/mtls.egg-info/dependency_links.txt
+src/mtls.egg-info/entry_points.txt
+src/mtls.egg-info/requires.txt
+src/mtls.egg-info/top_level.txt
+src/mtls.egg-info/zip-safe
 test/.coverage
 test/__init__.py
 test/test_cli.py
```

### Comparing `mtls-0.16.0/setup.py` & `mtls-0.17.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,67 @@
-from setuptools import setup, find_packages
+[project]
+name = "mtls"
+dynamic = [
+    "entry-points",
+    "version",
+]
+authors = [
+    { name="Danny Grove", email="danny@drgrovellc.com" }
+]
+description = "A short-lived certificate tool based on the Zero Trust network mode"
+readme = "README.md"
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Topic :: Internet",
+    "Topic :: Security :: Cryptography",
+    "Topic :: Security",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3 :: Only",
+]
 
-desc = "A short-lived certificate tool based on the Zero Trust network mode"
+[project.scripts]
+mtls = "mtls.cli:cli"
 
-setup(
-    name="mtls",
-    author="Danny Grove",
-    author_email="danny@drgrovellc.com",
-    url="https://github.com/drGrove/mtls-cli",
-    description=desc,
-    long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
-    project_urls={
-        "Homepage": "https://github.com/drGrove/mtls-cli",
-        "Source": "https://github.com/drGrove/mtls-cli",
-        "Tracker": "https://github.com/drGrove/mtls-cli/issues",
-    },
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Intended Audience :: End Users/Desktop",
-        "Intended Audience :: System Administrators",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-        "Topic :: Internet",
-        "Topic :: Security :: Cryptography",
-        "Topic :: Security",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-    python_requires='>=3.6',
-    setup_requires=["setuptools_scm"],
-    use_scm_version=True,
-    packages=find_packages(exclude=["test"]),
-    package_data={"mtls": ["share/*"]},
-    entry_points={
-        "console_scripts": [
-            "mtls = mtls.cli:cli"
-        ]
-    },
-    install_requires=[
-        "cryptography",
-        "python-gnupg",
-        "urllib3",
-        "requests",
-        "click",
-        "pyOpenSSL",
-    ],
-    zip_safe=True
-)
+[project.urls]
+Homepage = "https://github.com/drGrove/mtls-cli"
+Source = "https://github.com/drGrove/mtls-cli"
+Tracker = "https://github.com/drGrove/mtls-cli/issues"
+
+
+[build-system]
+requires = [
+    "setuptools==62.1.0",
+    "wheel==0.37.1",
+    "setuptools_scm==6.4.2",
+]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+write_to = "src/mtls/__version__.py"
+
+[tool.black]
+line-length = 79
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+)/
+'''
```

### Comparing `mtls-0.16.0/test/test_cli.py` & `mtls-0.17.0/test/test_cli.py`

 * *Files identical despite different names*

