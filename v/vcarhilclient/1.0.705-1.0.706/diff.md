# Comparing `tmp/vcarhilclient-1.0.705.tar.gz` & `tmp/vcarhilclient-1.0.706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.705.tar", last modified: Wed Jul  5 09:44:35 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.706.tar", last modified: Wed Jul  5 10:04:05 2023, max compression
```

## Comparing `vcarhilclient-1.0.705.tar` & `vcarhilclient-1.0.706.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.230883 vcarhilclient-1.0.705/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.705/LICENSE
--rw-rw-rw-   0        0        0     2596 2023-07-05 09:44:35.231878 vcarhilclient-1.0.705/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.705/README.md
--rw-rw-rw-   0        0        0       86 2023-07-05 09:44:35.232875 vcarhilclient-1.0.705/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-07-05 09:40:42.000000 vcarhilclient-1.0.705/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.208185 vcarhilclient-1.0.705/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.705/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.705/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.705/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50918 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    14192 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.705/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2383 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.705/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.228887 vcarhilclient-1.0.705/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2596 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.855490 vcarhilclient-1.0.706/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.706/LICENSE
+-rw-rw-rw-   0        0        0     2596 2023-07-05 10:04:05.855490 vcarhilclient-1.0.706/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.706/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-05 10:04:05.856486 vcarhilclient-1.0.706/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-07-05 10:03:33.000000 vcarhilclient-1.0.706/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.838337 vcarhilclient-1.0.706/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.706/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.706/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.706/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50918 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    14192 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.706/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2383 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.706/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.852970 vcarhilclient-1.0.706/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2596 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.705/LICENSE` & `vcarhilclient-1.0.706/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/PKG-INFO` & `vcarhilclient-1.0.706/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.705
+Version: 1.0.706
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vcarhilclient-1.0.705/README.md` & `vcarhilclient-1.0.706/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/setup.py` & `vcarhilclient-1.0.706/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.705",
+    version="1.0.706",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
-    install_requires = ["minio==7.1.13"],
+    install_requires = ["minio==7.1.13","bitstring"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `vcarhilclient-1.0.705/vcarhilclient/Enums.py` & `vcarhilclient-1.0.706/vcarhilclient/Enums.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.706/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.706/vcarhilclient/kunyi_mrt.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.706/vcarhilclient/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.706/vcarhilclient/kunyi_util.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.706/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.706/vcarhilclient/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.706/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.705/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.706/vcarhilclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.705
+Version: 1.0.706
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

