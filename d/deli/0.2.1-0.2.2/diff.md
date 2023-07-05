# Comparing `tmp/deli-0.2.1.tar.gz` & `tmp/deli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deli-0.2.1.tar", last modified: Sat Jun 24 14:45:50 2023, max compression
+gzip compressed data, was "deli-0.2.2.tar", last modified: Wed Jul  5 16:43:01 2023, max compression
```

## Comparing `deli-0.2.1.tar` & `deli-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.339832 deli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-24 14:45:47.000000 deli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:45:47.000000 deli-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 14:45:50.339832 deli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 14:45:47.000000 deli-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.335832 deli-0.2.1/deli/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 14:45:47.000000 deli-0.2.1/deli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 14:45:47.000000 deli-0.2.1/deli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-24 14:45:47.000000 deli-0.2.1/deli/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.339832 deli-0.2.1/deli/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/nifty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/numpy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/packaged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.335832 deli-0.2.1/deli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 14:45:47.000000 deli-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 14:45:47.000000 deli-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:45:50.339832 deli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-24 14:45:47.000000 deli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.870432 deli-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 16:42:49.000000 deli-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 16:42:49.000000 deli-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-05 16:43:01.870432 deli-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-05 16:42:49.000000 deli-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-05 16:42:49.000000 deli-0.2.2/deli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 16:42:49.000000 deli-0.2.2/deli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-05 16:42:49.000000 deli-0.2.2/deli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/nifty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/numpy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/packaged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-05 16:42:49.000000 deli-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:42:49.000000 deli-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:43:01.870432 deli-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-05 16:42:49.000000 deli-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-05 16:42:49.000000 deli-0.2.2/tests/test_serializers.py
```

### Comparing `deli-0.2.1/LICENSE` & `deli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/interface.py` & `deli-0.2.2/deli/interface.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializer.py` & `deli-0.2.2/deli/serializer.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/choice.py` & `deli-0.2.2/deli/serializers/choice.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/csv.py` & `deli-0.2.2/deli/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/dicom.py` & `deli-0.2.2/deli/serializers/dicom.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/helpers.py` & `deli-0.2.2/deli/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/images.py` & `deli-0.2.2/deli/serializers/images.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/nifty.py` & `deli-0.2.2/deli/serializers/nifty.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/numpy_.py` & `deli-0.2.2/deli/serializers/numpy_.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli/serializers/packaged.py` & `deli-0.2.2/deli/serializers/packaged.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.1/deli.egg-info/SOURCES.txt` & `deli-0.2.2/deli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 deli/serializers/choice.py
 deli/serializers/csv.py
 deli/serializers/dicom.py
 deli/serializers/helpers.py
 deli/serializers/images.py
 deli/serializers/nifty.py
 deli/serializers/numpy_.py
-deli/serializers/packaged.py
+deli/serializers/packaged.py
+tests/test_serializers.py
```

### Comparing `deli-0.2.1/pyproject.toml` & `deli-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,23 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3 :: Only',
     'Operating System :: OS Independent',
 ]
 
+[project.optional-dependencies]
+all = [
+    'pandas',
+    'pydicom',
+    'nibabel',
+    'numpy',
+    'imageio>=2.0.0',
+]
+
 [project.urls]
 'Homepage' = 'https://github.com/maxme1/deli'
 'Issues' = 'https://github.com/maxme1/deli/issues'
 'Source' = 'https://github.com/maxme1/deli'
 
 [build-system]
 requires = ['setuptools>=43.0.0', 'wheel']
```

### Comparing `deli-0.2.1/setup.py` & `deli-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,11 +43,20 @@
     license=LICENSE,
     version=VERSION,
     url=URL,
     download_url=DOWNLOAD_URL,
     packages=find_packages(include=(NAME,)),
     include_package_data=True,
     install_requires=REQUIREMENTS,
+    extras_require={
+        'all': [
+            'pandas',
+            'pydicom',
+            'nibabel',
+            'numpy',
+            'imageio>=2.0.0',
+        ]
+    },
     classifiers=CLASSIFIERS,
     keywords=KEYWORDS,
     python_requires='>=3.6',
 )
```

