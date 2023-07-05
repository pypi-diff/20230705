# Comparing `tmp/browser_driver_manager-1.0.1.tar.gz` & `tmp/browser_driver_manager-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browser_driver_manager-1.0.1.tar", last modified: Wed Jul  5 15:52:49 2023, max compression
+gzip compressed data, was "browser_driver_manager-1.0.3.tar", last modified: Wed Jul  5 17:07:34 2023, max compression
```

## Comparing `browser_driver_manager-1.0.1.tar` & `browser_driver_manager-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 15:52:49.042386 browser_driver_manager-1.0.1/
--rw-rw-rw-   0        0        0     4104 2023-07-05 15:52:49.040390 browser_driver_manager-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3234 2023-07-05 15:38:34.000000 browser_driver_manager-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 15:52:49.015457 browser_driver_manager-1.0.1/browser_driver_manager/
--rw-rw-rw-   0        0        0        0 2023-07-05 15:52:43.000000 browser_driver_manager-1.0.1/browser_driver_manager/__init__.py
--rw-rw-rw-   0        0        0     7742 2023-07-05 15:11:33.000000 browser_driver_manager-1.0.1/browser_driver_manager/browser_driver_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:52:49.038396 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/
--rw-rw-rw-   0        0        0     4104 2023-07-05 15:52:48.000000 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-05 15:52:48.000000 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 15:52:48.000000 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 15:52:48.000000 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-05 15:52:48.000000 browser_driver_manager-1.0.1/browser_driver_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 15:52:49.043391 browser_driver_manager-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-07-05 15:46:57.000000 browser_driver_manager-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 17:07:34.809792 browser_driver_manager-1.0.3/
+-rw-rw-rw-   0        0        0     4104 2023-07-05 17:07:34.808794 browser_driver_manager-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3234 2023-07-05 15:38:34.000000 browser_driver_manager-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 17:07:34.787852 browser_driver_manager-1.0.3/browser_driver_manager/
+-rw-rw-rw-   0        0        0     7742 2023-07-05 15:11:33.000000 browser_driver_manager-1.0.3/browser_driver_manager/browser_driver_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-05 17:07:34.806800 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/
+-rw-rw-rw-   0        0        0     4104 2023-07-05 17:07:34.000000 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-05 17:07:34.000000 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 17:07:34.000000 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 17:07:34.000000 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-05 17:07:34.000000 browser_driver_manager-1.0.3/browser_driver_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 17:07:34.809792 browser_driver_manager-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-07-05 17:07:16.000000 browser_driver_manager-1.0.3/setup.py
```

### Comparing `browser_driver_manager-1.0.1/PKG-INFO` & `browser_driver_manager-1.0.3/browser_driver_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: browser_driver_manager
-Version: 1.0.1
+Name: browser-driver-manager
+Version: 1.0.3
 Summary: 用于管理浏览器驱动程序的下载和安装
 Home-page: https://github.com/weqq2019/browser_driver_manager
 Author: 刘泉
 Author-email: soundless2023@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browser_driver_manager-1.0.1/README.md` & `browser_driver_manager-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `browser_driver_manager-1.0.1/browser_driver_manager/browser_driver_manager.py` & `browser_driver_manager-1.0.3/browser_driver_manager/browser_driver_manager.py`

 * *Files identical despite different names*

### Comparing `browser_driver_manager-1.0.1/browser_driver_manager.egg-info/PKG-INFO` & `browser_driver_manager-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: browser-driver-manager
-Version: 1.0.1
+Name: browser_driver_manager
+Version: 1.0.3
 Summary: 用于管理浏览器驱动程序的下载和安装
 Home-page: https://github.com/weqq2019/browser_driver_manager
 Author: 刘泉
 Author-email: soundless2023@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browser_driver_manager-1.0.1/setup.py` & `browser_driver_manager-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='browser_driver_manager',
-    version='1.0.1',
+    version='1.0.3',
     description='用于管理浏览器驱动程序的下载和安装',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='刘泉',
     author_email='soundless2023@gmail.com',
     url='https://github.com/weqq2019/browser_driver_manager',
     packages=['browser_driver_manager'],
```

