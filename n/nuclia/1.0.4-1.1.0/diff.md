# Comparing `tmp/nuclia-1.0.4.tar.gz` & `tmp/nuclia-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.0.4.tar", last modified: Thu Jun 29 07:30:18 2023, max compression
+gzip compressed data, was "nuclia-1.1.0.tar", last modified: Wed Jul  5 15:13:26 2023, max compression
```

## Comparing `nuclia-1.0.4.tar` & `nuclia-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041690 nuclia-1.0.4/
--rw-r--r--   0 ramon      (501) staff       (20)       39 2023-06-29 07:30:17.000000 nuclia-1.0.4/.gitignore
--rw-r--r--   0 ramon      (501) staff       (20)       10 2023-06-29 07:30:17.000000 nuclia-1.0.4/.python-version
--rw-r--r--   0 ramon      (501) staff       (20)      271 2023-06-29 07:30:17.000000 nuclia-1.0.4/CHANGELOG.md
--rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-06-29 07:30:17.000000 nuclia-1.0.4/LICENSE
--rw-r--r--   0 ramon      (501) staff       (20)       83 2023-06-29 07:30:17.000000 nuclia-1.0.4/MANIFEST.in
--rw-r--r--   0 ramon      (501) staff       (20)      236 2023-06-29 07:30:17.000000 nuclia-1.0.4/Makefile
--rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-29 07:30:18.041735 nuclia-1.0.4/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)      847 2023-06-29 07:30:17.000000 nuclia-1.0.4/README.md
--rw-r--r--   0 ramon      (501) staff       (20)        6 2023-06-29 07:30:17.000000 nuclia-1.0.4/VERSION
--rw-r--r--   0 ramon      (501) staff       (20)       24 2023-06-29 07:30:17.000000 nuclia-1.0.4/code-requirements.txt
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.037909 nuclia-1.0.4/docs/
--rw-r--r--   0 ramon      (501) staff       (20)      941 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/AUTH.md
--rw-r--r--   0 ramon      (501) staff       (20)     1580 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/CONVERSATION.md
--rw-r--r--   0 ramon      (501) staff       (20)      892 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/DEFAULT.md
--rw-r--r--   0 ramon      (501) staff       (20)      648 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/README.md
--rw-r--r--   0 ramon      (501) staff       (20)     1057 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/SEARCH.md
--rw-r--r--   0 ramon      (501) staff       (20)     1993 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/UPLOAD.md
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.038378 nuclia-1.0.4/nuclia/
--rw-r--r--   0 ramon      (501) staff       (20)      303 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039316 nuclia-1.0.4/nuclia/cli/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      660 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/run.py
--rw-r--r--   0 ramon      (501) staff       (20)      526 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/utils.py
--rw-r--r--   0 ramon      (501) staff       (20)     6257 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/config.py
--rw-r--r--   0 ramon      (501) staff       (20)      739 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/data.py
--rw-r--r--   0 ramon      (501) staff       (20)     2569 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/decorators.py
--rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/exceptions.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039768 nuclia-1.0.4/nuclia/lib/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      253 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/conversations.py
--rw-r--r--   0 ramon      (501) staff       (20)     5996 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/kb.py
--rw-r--r--   0 ramon      (501) staff       (20)      868 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/nua.py
--rw-r--r--   0 ramon      (501) staff       (20)      123 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/nua_responses.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.040965 nuclia-1.0.4/nuclia/sdk/
--rw-r--r--   0 ramon      (501) staff       (20)      343 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      229 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/accounts.py
--rw-r--r--   0 ramon      (501) staff       (20)     7800 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/auth.py
--rw-r--r--   0 ramon      (501) staff       (20)     1075 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/kb.py
--rw-r--r--   0 ramon      (501) staff       (20)     2251 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/kbs.py
--rw-r--r--   0 ramon      (501) staff       (20)      410 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/nua.py
--rw-r--r--   0 ramon      (501) staff       (20)     1092 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/nuas.py
--rw-r--r--   0 ramon      (501) staff       (20)      499 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/predict.py
--rw-r--r--   0 ramon      (501) staff       (20)      190 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/process.py
--rw-r--r--   0 ramon      (501) staff       (20)     2245 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/search.py
--rw-r--r--   0 ramon      (501) staff       (20)      188 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/train.py
--rw-r--r--   0 ramon      (501) staff       (20)     5846 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/upload.py
--rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/zones.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041503 nuclia-1.0.4/nuclia/tests/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041601 nuclia-1.0.4/nuclia/tests/assets/
--rw-r--r--   0 ramon      (501) staff       (20)      761 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ramon      (501) staff       (20)       50 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/conftest.py
--rw-r--r--   0 ramon      (501) staff       (20)     1200 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/fixtures.py
--rw-r--r--   0 ramon      (501) staff       (20)      492 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_auth.py
--rw-r--r--   0 ramon      (501) staff       (20)      659 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_conversation.py
--rw-r--r--   0 ramon      (501) staff       (20)      247 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_predict.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039046 nuclia-1.0.4/nuclia.egg-info/
--rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)     1201 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ramon      (501) staff       (20)       47 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ramon      (501) staff       (20)      133 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/requires.txt
--rw-r--r--   0 ramon      (501) staff       (20)        7 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/zip-safe
--rw-r--r--   0 ramon      (501) staff       (20)      132 2023-06-29 07:30:17.000000 nuclia-1.0.4/requirements.txt
--rw-r--r--   0 ramon      (501) staff       (20)      204 2023-06-29 07:30:18.041931 nuclia-1.0.4/setup.cfg
--rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-06-29 07:30:17.000000 nuclia-1.0.4/setup.py
--rw-r--r--   0 ramon      (501) staff       (20)       32 2023-06-29 07:30:17.000000 nuclia-1.0.4/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.636134 nuclia-1.1.0/
+-rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-05 15:13:25.000000 nuclia-1.1.0/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-05 15:13:25.000000 nuclia-1.1.0/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)      479 2023-07-05 15:13:25.000000 nuclia-1.1.0/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-05 15:13:25.000000 nuclia-1.1.0/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-05 15:13:25.000000 nuclia-1.1.0/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-05 15:13:25.000000 nuclia-1.1.0/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-05 15:13:26.636398 nuclia-1.1.0/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-05 15:13:25.000000 nuclia-1.1.0/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-05 15:13:25.000000 nuclia-1.1.0/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-05 15:13:25.000000 nuclia-1.1.0/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.620929 nuclia-1.1.0/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      648 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1993 2023-07-05 15:13:25.000000 nuclia-1.1.0/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.622733 nuclia-1.1.0/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.626142 nuclia-1.1.0/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1280 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2971 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.627652 nuclia-1.1.0/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/lib/nua_responses.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.632790 nuclia-1.1.0/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1341 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8910 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.635230 nuclia-1.1.0/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.635669 nuclia-1.1.0/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      682 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-05 15:13:25.000000 nuclia-1.1.0/nuclia/tests/test_predict.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-05 15:13:26.625066 nuclia-1.1.0/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1222 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-05 15:13:26.000000 nuclia-1.1.0/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-05 15:13:25.000000 nuclia-1.1.0/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-05 15:13:26.637172 nuclia-1.1.0/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-05 15:13:25.000000 nuclia-1.1.0/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-05 15:13:25.000000 nuclia-1.1.0/test-requirements.txt
```

### Comparing `nuclia-1.0.4/LICENSE` & `nuclia-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/PKG-INFO` & `nuclia-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.4
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
+Description: # Nuclia Python Client
+        
+        In order to install
+        
+        ```bash
+        pip install nuclia
+        ```
+        
+        ## Authentication
+        
+        ### Nuclia
+        
+        You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
+        
+        ```bash
+        nuclia auth login
+        ```
+        
+        
+        ### Nuclia Knowledgebox
+        
+        You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
+        
+        ```bash
+        nuclia auth kb --url KB_URL --token SERVICE_TOKEN
+        ```
+        
+        KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
+        
+        
+        ### Nuclia Understanding API
+        
+        You can login with a Nuclia Understanding API key to process files, predict and train using our system
+        
+        ```bash
+        nuclia auth nua --key ZZZZ
+        ```
+        
+        ## Documentation
+        
+        You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
 Keywords: search,semantic,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Nuclia Python Client
-
-In order to install
-
-```bash
-pip install nuclia
-```
-
-## Authentication
-
-### Nuclia
-
-You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
-
-```bash
-nuclia auth login
-```
-
-
-### Nuclia Knowledgebox
-
-You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
-
-```bash
-nuclia auth kb --url KB_URL --token SERVICE_TOKEN
-```
-
-KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
-
-
-### Nuclia Understanding API
-
-You can login with a Nuclia Understanding API key to process files, predict and train using our system
-
-```bash
-nuclia auth nua --key ZZZZ
-```
-
-
```

### Comparing `nuclia-1.0.4/README.md` & `nuclia-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,7 +31,11 @@
 ### Nuclia Understanding API
 
 You can login with a Nuclia Understanding API key to process files, predict and train using our system
 
 ```bash
 nuclia auth nua --key ZZZZ
 ```
+
+## Documentation
+
+You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
```

### Comparing `nuclia-1.0.4/docs/AUTH.md` & `nuclia-1.1.0/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/docs/DEFAULT.md` & `nuclia-1.1.0/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/docs/README.md` & `nuclia-1.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/docs/SEARCH.md` & `nuclia-1.1.0/docs/SEARCH.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 # Search
 
 ## Search experience
 
 Its the most basic search experience at Nuclia. You can search resources and paragraphs that match a query by a fulltext match, a fuzzy match or a semantic match. The results will be ordered by each search using BM25, fuzzy distance and semantic distance.
 
 ```bash
-nuclia search search --query="My search"
+nuclia kb search search --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
 search.search(query="My search")
 ```
 
+Get JSON output:
+
+```bash
+nuclia kb search search --query="My search" --json
+```
+
+Get YAML output:
+
+```bash
+nuclia kb search search --query="My search" --yaml
+```
+
 ## Find experience
 
 You get the list of paragraphs matching semantically and by keywords ordered together with a generic reranking strategy.
 
 ```bash
-nuclia search find --query="My search"
+nuclia kb search find --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
 search.find(query="My search")
 ```
 
-## Ask experience
+It also supports indented and YAML output.
+
+## Chat experience
 
 Based on the find experience we use a generative AI to answer the question based on the context without hallucinations and with the find result and relations
 
 ```bash
-nuclia search ask --query="My search"
+nuclia kb search chat --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
-search.ask(query="My search")
+search.chat(query="My search")
 ```
```

### Comparing `nuclia-1.0.4/docs/UPLOAD.md` & `nuclia-1.1.0/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/config.py` & `nuclia-1.1.0/nuclia/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,18 @@
                 )
             )
         return kb_obj
 
     def set_user_token(self, code: str):
         self.token = code
 
+    def remove_user_token(self):
+        self.token = None
+        self.save()
+
     def set_nua_token(
         self,
         client_id: str,
         account: str,
         region: str,
         token: str,
         account_type: Optional[str] = None,
```

### Comparing `nuclia-1.0.4/nuclia/data.py` & `nuclia-1.1.0/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/decorators.py` & `nuclia-1.1.0/nuclia/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
+from functools import wraps
+
+import yaml
+
 from nuclia.data import get_auth
 from nuclia.exceptions import NotDefinedDefault
 from nuclia.lib.kb import Environment, NucliaDBClient
 from nuclia.lib.nua import NuaClient
 
 
 def accounts(func):
+    @wraps(func)
     def wrapper_checkout_accounts(*args, **kwargs):
         auth = get_auth()
         auth.accounts()
         return func(*args, **kwargs)
 
     return wrapper_checkout_accounts
 
 
 def kbs(func):
+    @wraps(func)
     def wrapper_checkout_kbs(*args, **kwargs):
         if "account" in kwargs:
             auth = get_auth()
             auth.kbs(kwargs["account"])
         return func(*args, **kwargs)
 
     return wrapper_checkout_kbs
 
 
 def kb(func):
+    @wraps(func)
     def wrapper_checkout_kb(*args, **kwargs):
         url = kwargs.get("url")
         api_key = kwargs.get("api_key")
         auth = get_auth()
         if url is None:
             # Get default KB
             kbid = auth._config.get_default_kb()
@@ -65,21 +72,35 @@
         kwargs["ndb"] = ndb
         return func(*args, **kwargs)
 
     return wrapper_checkout_kb
 
 
 def nua(func):
+    @wraps(func)
     def wrapper_checkout_nua(*args, **kwargs):
         auth = get_auth()
         nua_id = auth._config.get_default_nua()
         if nua_id is None:
             raise NotDefinedDefault()
 
         nua_obj = auth._config.get_nua(nua_id)
         nc = NuaClient(
             region=nua_obj.region, account=nua_obj.account, token=nua_obj.token
         )
         kwargs["nc"] = nc
         return func(*args, **kwargs)
 
     return wrapper_checkout_nua
+
+
+def pretty(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        if kwargs.get("json"):
+            return result.json(indent=2)
+        if kwargs.get("yaml"):
+            return yaml.dump(result)
+        return result
+
+    return wrapper
```

### Comparing `nuclia-1.0.4/nuclia/lib/kb.py` & `nuclia-1.1.0/nuclia/lib/kb.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Optional
 
 import httpx
 import requests
 from nucliadb_models.search import ChatRequest
 from nucliadb_sdk import NucliaDB, Region
 
+from nuclia.exceptions import NeedUserToken
+
 RESOURCE_PATH = "/resource/{rid}"
 RESOURCE_PATH_BY_SLUG = "/slug/{slug}"
 SEARCH_PATH = "/search"
 CREATE_RESOURCE_PATH = "/resources"
 CREATE_VECTORSET = "/vectorset/{vectorset}"
 VECTORSETS = "/vectorsets"
 COUNTER = "/counters"
@@ -83,15 +85,15 @@
             writer_headers = {
                 "Authorization": f"Bearer {user_token}",
                 "X-SYNCHRONOUS": "True",
             }
         elif (
             environment == Environment.CLOUD and api_key is None and user_token is None
         ):
-            raise AttributeError("On Cloud you need to provide API Key")
+            raise NeedUserToken("On Cloud you need to provide API Key")
         else:
             reader_headers = {
                 "X-NUCLIADB-ROLES": f"READER",
             }
             writer_headers = {
                 "X-NUCLIADB-ROLES": f"WRITER",
                 "X-SYNCHRONOUS": "True",
```

### Comparing `nuclia-1.0.4/nuclia/lib/nua.py` & `nuclia-1.1.0/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/sdk/auth.py` & `nuclia-1.1.0/nuclia/sdk/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,25 @@
         Lets redirect the user to the UI to capture a token
         """
         if self._validate_user_token():
             print("Logged in!")
             self._show_user()
             return
 
-        webbrowser.open(get_global_url("/redirect?display=token&ident={ident}"))
+        webbrowser.open(get_global_url("/redirect?display=token"))
         code = input("Follow the browser flow and copy the token and paste it here:")
         print("Checking...")
         self.set_user_token(code)
 
+    def logout(self):
+        """
+        Remove the current user token.
+        """
+        self._config.remove_user_token()
+
     def set_user_token(self, code: str):
         if self._validate_user_token(code):
             self._config.set_user_token(code)
             print("Auth completed!")
             self.post_login()
         else:
             print("Invalid token auth not completed")
```

### Comparing `nuclia-1.0.4/nuclia/sdk/kb.py` & `nuclia-1.1.0/nuclia/sdk/kb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from nucliadb_models.resource import Resource, ResourceList
 
 from nuclia.data import get_auth
-from nuclia.decorators import kb
-from nuclia.lib.kb import NucliaDBClient
+from nuclia.decorators import kb, pretty
 from nuclia.sdk.auth import NucliaAuth
 from nuclia.sdk.search import NucliaSearch
 from nuclia.sdk.upload import NucliaUpload
 
 
 class NucliaKB:
     @property
@@ -15,21 +14,33 @@
         return auth
 
     def __init__(self):
         self.upload = NucliaUpload()
         self.search = NucliaSearch()
 
     @kb
-    def list(self, *, ndb: NucliaDBClient):
+    def list(self, **kwargs):
+        ndb = kwargs["ndb"]
         data: ResourceList = ndb.ndb.list_resources(kbid=ndb.kbid)
         for resource in data.resources:
             print(f"{resource.id} {resource.icon:30} {resource.title}")
 
     @kb
-    def get_resource_by_slug(self, *, ndb: NucliaDBClient, slug: str) -> Resource:
+    @pretty
+    def get_resource_by_id(self, *, rid: str, **kwargs) -> Resource:
+        ndb = kwargs["ndb"]
+        return ndb.ndb.get_resource_by_id(
+            kbid=ndb.kbid, rid=rid, query_params={"show": "values"}
+        )
+
+    @kb
+    @pretty
+    def get_resource_by_slug(self, *, slug: str, **kwargs) -> Resource:
+        ndb = kwargs["ndb"]
         return ndb.ndb.get_resource_by_slug(
             kbid=ndb.kbid, slug=slug, query_params={"show": "values"}
         )
 
     @kb
-    def delete(self, *, ndb: NucliaDBClient, rid: str):
+    def delete(self, *, rid: str, **kwargs):
+        ndb = kwargs["ndb"]
         ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
```

### Comparing `nuclia-1.0.4/nuclia/sdk/kbs.py` & `nuclia-1.1.0/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/sdk/nuas.py` & `nuclia-1.1.0/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/sdk/search.py` & `nuclia-1.1.0/nuclia/sdk/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     FindRequest,
     KnowledgeboxFindResults,
     Relations,
     SearchRequest,
 )
 
 from nuclia.data import get_auth
-from nuclia.decorators import kb
-from nuclia.lib.kb import NucliaDBClient
+from nuclia.decorators import kb, pretty
 from nuclia.sdk.auth import NucliaAuth
 
 
 @dataclass
 class ChatAnswer:
     answer: bytes
     learning_id: str
@@ -24,39 +23,68 @@
     find_result: Optional[KnowledgeboxFindResults]
 
     def __str__(self):
         return self.answer.decode()
 
 
 class NucliaSearch:
+    """
+    Perform search on a Knowledge Box.
+
+    `find` and `search` accept the following parameters:
+    - `json`: return results in JSON format
+    - `yaml`: return results in YAML format
+    """
+
     @property
     def _auth(self) -> NucliaAuth:
         auth = get_auth()
         return auth
 
     @kb
-    def search(self, *, ndb: NucliaDBClient, query: Union[str, SearchRequest]):
+    @pretty
+    def search(self, *, query: Union[str, SearchRequest], **kwargs):
+        """
+        Perform a search query.
+
+        See https://docs.nuclia.dev/docs/api#tag/Search/operation/Search_Knowledge_Box_kb__kbid__search_post
+        """
+        ndb = kwargs["ndb"]
         if isinstance(query, str):
             req = SearchRequest(query=query)
         else:
             req = query
 
         return ndb.ndb.search(req, kbid=ndb.kbid)
 
     @kb
-    def find(self, *, ndb: NucliaDBClient, query: Union[str, FindRequest]):
+    @pretty
+    def find(self, *, query: Union[str, FindRequest], **kwargs):
+        """
+        Perform a find query.
+
+        See https://docs.nuclia.dev/docs/api#tag/Search/operation/Find_Knowledge_Box_kb__kbid__find_post
+        """
+
+        ndb = kwargs["ndb"]
         if isinstance(query, str):
             req = FindRequest(query=query)
         else:
             req = query
 
         return ndb.ndb.find(req, kbid=ndb.kbid)
 
     @kb
-    def ask(self, *, ndb: NucliaDBClient, query: Union[str, ChatRequest]):
+    def chat(self, *, query: Union[str, ChatRequest], **kwargs):
+        """
+        Answer a question.
+
+        See https://docs.nuclia.dev/docs/api#tag/Search/operation/Chat_Knowledge_Box_kb__kbid__chat_post
+        """
+        ndb = kwargs["ndb"]
         if isinstance(query, str):
             req = ChatRequest(query=query)
         else:
             req = query
         response = ndb.chat(req)
         header = response.raw.read(4)
         payload_size = int.from_bytes(header, byteorder="big", signed=False)
```

### Comparing `nuclia-1.0.4/nuclia/tests/fixtures.py` & `nuclia-1.1.0/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.4/nuclia/tests/test_conversation.py` & `nuclia-1.1.0/nuclia/tests/test_conversation.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     except NotFoundError:
         pass
 
     res = nkb.list()
     assert res is None
 
     nu = NucliaUpload()
-    nu.conversation(path=path)
+    nu.conversation(path=path, slug="conversation1", field="c1")
 
     resource = nkb.get_resource_by_slug(slug="conversation1")
     assert resource
-    assert resource.data.conversations["conversation1"]
+    assert resource.data.conversations["c1"]
```

### Comparing `nuclia-1.0.4/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.0/nuclia.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.4
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
+Description: # Nuclia Python Client
+        
+        In order to install
+        
+        ```bash
+        pip install nuclia
+        ```
+        
+        ## Authentication
+        
+        ### Nuclia
+        
+        You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
+        
+        ```bash
+        nuclia auth login
+        ```
+        
+        
+        ### Nuclia Knowledgebox
+        
+        You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
+        
+        ```bash
+        nuclia auth kb --url KB_URL --token SERVICE_TOKEN
+        ```
+        
+        KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
+        
+        
+        ### Nuclia Understanding API
+        
+        You can login with a Nuclia Understanding API key to process files, predict and train using our system
+        
+        ```bash
+        nuclia auth nua --key ZZZZ
+        ```
+        
+        ## Documentation
+        
+        You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
 Keywords: search,semantic,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Nuclia Python Client
-
-In order to install
-
-```bash
-pip install nuclia
-```
-
-## Authentication
-
-### Nuclia
-
-You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
-
-```bash
-nuclia auth login
-```
-
-
-### Nuclia Knowledgebox
-
-You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
-
-```bash
-nuclia auth kb --url KB_URL --token SERVICE_TOKEN
-```
-
-KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
-
-
-### Nuclia Understanding API
-
-You can login with a Nuclia Understanding API key to process files, predict and train using our system
-
-```bash
-nuclia auth nua --key ZZZZ
-```
-
-
```

### Comparing `nuclia-1.0.4/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.0/nuclia.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 nuclia/lib/nua.py
 nuclia/lib/nua_responses.py
 nuclia/sdk/__init__.py
 nuclia/sdk/accounts.py
 nuclia/sdk/auth.py
 nuclia/sdk/kb.py
 nuclia/sdk/kbs.py
+nuclia/sdk/logger.py
 nuclia/sdk/nua.py
 nuclia/sdk/nuas.py
 nuclia/sdk/predict.py
 nuclia/sdk/process.py
 nuclia/sdk/search.py
 nuclia/sdk/train.py
 nuclia/sdk/upload.py
```

### Comparing `nuclia-1.0.4/setup.py` & `nuclia-1.1.0/setup.py`

 * *Files identical despite different names*

