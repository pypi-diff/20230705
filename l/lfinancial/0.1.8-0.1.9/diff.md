# Comparing `tmp/lfinancial-0.1.8.tar.gz` & `tmp/lfinancial-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.8.tar", last modified: Wed Jul  5 13:19:08 2023, max compression
+gzip compressed data, was "lfinancial-0.1.9.tar", last modified: Wed Jul  5 13:23:49 2023, max compression
```

## Comparing `lfinancial-0.1.8.tar` & `lfinancial-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:19:08.391719 lfinancial-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-05 13:18:51.000000 lfinancial-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-05 13:19:08.391719 lfinancial-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-05 13:18:51.000000 lfinancial-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:19:08.387719 lfinancial-0.1.8/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 13:18:51.000000 lfinancial-0.1.8/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-05 13:18:51.000000 lfinancial-0.1.8/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 13:18:51.000000 lfinancial-0.1.8/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:19:08.391719 lfinancial-0.1.8/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-05 13:19:08.000000 lfinancial-0.1.8/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 13:19:08.000000 lfinancial-0.1.8/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:19:08.000000 lfinancial-0.1.8/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 13:19:08.000000 lfinancial-0.1.8/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:19:08.391719 lfinancial-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-05 13:18:51.000000 lfinancial-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:19:08.391719 lfinancial-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 13:18:51.000000 lfinancial-0.1.8/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-05 13:23:25.000000 lfinancial-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-05 13:23:49.309429 lfinancial-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 13:23:25.000000 lfinancial-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:23:49.309429 lfinancial-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-05 13:23:25.000000 lfinancial-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 13:23:25.000000 lfinancial-0.1.9/tests/test_document.py
```

### Comparing `lfinancial-0.1.8/LICENSE.txt` & `lfinancial-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.8/PKG-INFO` & `lfinancial-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |    
 } '--. } '_}  | } | }\  { /  /\  \ | }\  { | },-. | } /  /\  \ } '--. 
 `----' `--'   `-' `-' `-' `-'  `-' `-' `-' `----' `-' `-'  `-' `----' 
 ```
 [![pypi](https://img.shields.io/pypi/v/lfinancial)](https://pypi.org/project/lfinancial/)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)
+[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)](https://github.com/LemonLzy/lfinancial/actions)
 [![GitHub](https://img.shields.io/github/license/LemonLzy/lfinancial)](https://github.com/LemonLzy/lfinancial/blob/main/LICENSE.txt)
 ---
 
 #### How to install?
 ```shell
 pip install lfinancial
 ```
```

### Comparing `lfinancial-0.1.8/README.md` & `lfinancial-0.1.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |    
 } '--. } '_}  | } | }\  { /  /\  \ | }\  { | },-. | } /  /\  \ } '--. 
 `----' `--'   `-' `-' `-' `-'  `-' `-' `-' `----' `-' `-'  `-' `----' 
 ```
 [![pypi](https://img.shields.io/pypi/v/lfinancial)](https://pypi.org/project/lfinancial/)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)
+[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)](https://github.com/LemonLzy/lfinancial/actions)
 [![GitHub](https://img.shields.io/github/license/LemonLzy/lfinancial)](https://github.com/LemonLzy/lfinancial/blob/main/LICENSE.txt)
 ---
 
 #### How to install?
 ```shell
 pip install lfinancial
 ```
```

### Comparing `lfinancial-0.1.8/lfinancial/factory.py` & `lfinancial-0.1.9/lfinancial/factory.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.8/lfinancial/financial.py` & `lfinancial-0.1.9/lfinancial/financial.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.8/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.1.9/lfinancial.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |    
 } '--. } '_}  | } | }\  { /  /\  \ | }\  { | },-. | } /  /\  \ } '--. 
 `----' `--'   `-' `-' `-' `-'  `-' `-' `-' `----' `-' `-'  `-' `----' 
 ```
 [![pypi](https://img.shields.io/pypi/v/lfinancial)](https://pypi.org/project/lfinancial/)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)
+[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/LemonLzy/lfinancial/publish.yml)](https://github.com/LemonLzy/lfinancial/actions)
 [![GitHub](https://img.shields.io/github/license/LemonLzy/lfinancial)](https://github.com/LemonLzy/lfinancial/blob/main/LICENSE.txt)
 ---
 
 #### How to install?
 ```shell
 pip install lfinancial
 ```
```

### Comparing `lfinancial-0.1.8/setup.py` & `lfinancial-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.1.8',
+    version='0.1.9',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

