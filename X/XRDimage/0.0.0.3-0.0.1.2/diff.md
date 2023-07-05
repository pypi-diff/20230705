# Comparing `tmp/XRDimage-0.0.0.3.tar.gz` & `tmp/XRDimage-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XRDimage-0.0.0.3.tar", last modified: Mon Aug  1 22:51:46 2022, max compression
+gzip compressed data, was "XRDimage-0.0.1.2.tar", last modified: Mon Jul  3 16:04:52 2023, max compression
```

## Comparing `XRDimage-0.0.0.3.tar` & `XRDimage-0.0.1.2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxrwxr-x   0 pawancw   (1000) pawancw   (1000)        0 2022-08-01 22:51:46.687137 XRDimage-0.0.0.3/
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)     1074 2022-07-22 17:41:41.000000 XRDimage-0.0.0.3/LICENSE
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)      558 2022-08-01 22:51:46.687137 XRDimage-0.0.0.3/PKG-INFO
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)     2019 2022-07-21 20:08:06.000000 XRDimage-0.0.0.3/README.md
-drwxrwxr-x   0 pawancw   (1000) pawancw   (1000)        0 2022-08-01 22:51:46.687137 XRDimage-0.0.0.3/XRDimage.egg-info/
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)      558 2022-08-01 22:51:46.000000 XRDimage-0.0.0.3/XRDimage.egg-info/PKG-INFO
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)      200 2022-08-01 22:51:46.000000 XRDimage-0.0.0.3/XRDimage.egg-info/SOURCES.txt
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)        1 2022-08-01 22:51:46.000000 XRDimage-0.0.0.3/XRDimage.egg-info/dependency_links.txt
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)       39 2022-08-01 22:51:46.000000 XRDimage-0.0.0.3/XRDimage.egg-info/requires.txt
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)        1 2022-08-01 22:51:46.000000 XRDimage-0.0.0.3/XRDimage.egg-info/top_level.txt
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)       88 2022-08-01 22:33:02.000000 XRDimage-0.0.0.3/pyproject.toml
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)       38 2022-08-01 22:51:46.687137 XRDimage-0.0.0.3/setup.cfg
--rw-rw-r--   0 pawancw   (1000) pawancw   (1000)      921 2022-08-01 22:51:41.000000 XRDimage-0.0.0.3/setup.py
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.403882 XRDimage-0.0.1.2/
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/.keep
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/LICENSE
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      665 2023-07-03 16:04:52.401608 XRDimage-0.0.1.2/PKG-INFO
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2019 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/README.md
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.363072 XRDimage-0.0.1.2/XRDimage/
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/__init__.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      819 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/dark_correction.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     3874 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/find_center.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2040 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/image_processing_function.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1711 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/image_registration.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1138 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/mask.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     3513 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/temperature_independent.py
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.394410 XRDimage-0.0.1.2/XRDimage.egg-info/
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      665 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/PKG-INFO
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      430 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       46 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/requires.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/top_level.txt
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimageDescription.txt
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      855 2023-07-03 15:14:46.000000 XRDimage-0.0.1.2/pyproject.toml
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-03 16:04:52.406385 XRDimage-0.0.1.2/setup.cfg
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1010 2023-07-03 15:27:28.000000 XRDimage-0.0.1.2/setup.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/test
```

### Comparing `XRDimage-0.0.0.3/LICENSE` & `XRDimage-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.0.3/PKG-INFO` & `XRDimage-0.0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.0.3
-Summary: package for image processing on XRD images
+Version: 0.0.1.2
+Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
+Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `XRDimage-0.0.0.3/README.md` & `XRDimage-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.0.3/XRDimage.egg-info/PKG-INFO` & `XRDimage-0.0.1.2/XRDimage.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: XRDimage
-Version: 0.0.0.3
-Summary: package for image processing on XRD images
+Version: 0.0.1.2
+Summary: XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.
 Home-page: http://engineering.case.edu/centers/sdle/
 Author: Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French
 Author-email: wxy215@case.edu, pkt19@case.edu, roger.french@case.edu
 License: MIT License
 Project-URL: Documentation, https://xrdimage-doc.readthedocs.io/en/latest/
 Project-URL: Bugtracker, https://bitbucket.org/cwrusdle/xrd-image/src/main/
+Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `XRDimage-0.0.0.3/setup.py` & `XRDimage-0.0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 
 setup(name='XRDimage',
-      version='0.0.0.3',
-      description='package for image processing on XRD images',
+      version='0.0.1.2',
+      description='XRDImage is a Python 3 package developed by the SDLE Research Center at Case Western Reserve University in Cleveland, OH.',
       url='http://engineering.case.edu/centers/sdle/',
       author='Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak, Pawan K. Tripathi, Roger H. French',
       author_email='wxy215@case.edu, pkt19@case.edu, roger.french@case.edu',
       license='MIT License',
       packages=[''],
       package_dir={'XRDimage': './XRDimage'},
 #      package_data={'XRDimage': ['data','files/data/FullSizeModules/*','files/tutorials/*','files/data/out','README.rst']},
       python_requires='>=3.8',
-      install_requires=['numpy', 'PIL','scikit-image','scikit-image','os'],
+      install_requires=['numpy', 'PIL','scikit-image','scikit-image','os', 'pandas'],
 #      include_package_data=True,
       project_urls={"Documentation":"https://xrdimage-doc.readthedocs.io/en/latest/","Bugtracker": "https://bitbucket.org/cwrusdle/xrd-image/src/main/"},
       )
```

