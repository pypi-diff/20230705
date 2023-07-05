# Comparing `tmp/dream_river-0.0.6.tar.gz` & `tmp/dream_river-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream_river-0.0.6.tar", last modified: Tue Jun 13 08:23:25 2023, max compression
+gzip compressed data, was "dream_river-0.0.7.tar", last modified: Wed Jul  5 02:14:41 2023, max compression
```

## Comparing `dream_river-0.0.6.tar` & `dream_river-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.328014 dream_river-0.0.6/
--rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1413 2023-06-13 08:23:25.328014 dream_river-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.294487 dream_river-0.0.6/dream_river/
--rw-rw-rw-   0        0        0     8516 2023-06-13 08:14:56.000000 dream_river-0.0.6/dream_river/ML.py
--rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.6/dream_river/__init__.py
--rw-rw-rw-   0        0        0     7139 2023-06-13 08:17:08.000000 dream_river-0.0.6/dream_river/convertools.py
--rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.6/dream_river/geobox.py
--rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.6/dream_river/indices.py
--rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.6/dream_river/plotimg.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.326379 dream_river-0.0.6/dream_river.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 08:23:25.330011 dream_river-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1773 2023-06-13 08:15:59.000000 dream_river-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.079277 dream_river-0.0.7/
+-rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1392 2023-07-05 02:14:41.080277 dream_river-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.058275 dream_river-0.0.7/dream_river/
+-rw-rw-rw-   0        0        0     8528 2023-07-05 02:11:46.000000 dream_river-0.0.7/dream_river/ML.py
+-rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.7/dream_river/__init__.py
+-rw-rw-rw-   0        0        0     7139 2023-06-13 08:17:08.000000 dream_river-0.0.7/dream_river/convertools.py
+-rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.7/dream_river/geobox.py
+-rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.7/dream_river/indices.py
+-rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.7/dream_river/plotimg.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.078277 dream_river-0.0.7/dream_river.egg-info/
+-rw-rw-rw-   0        0        0     1392 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-05 02:14:41.082277 dream_river-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-07-05 02:12:31.000000 dream_river-0.0.7/setup.py
```

### Comparing `dream_river-0.0.6/LICENSE` & `dream_river-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/LICENSE.txt` & `dream_river-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/PKG-INFO` & `dream_river-0.0.7/dream_river.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: dream_river
-Version: 0.0.6
+Name: dream-river
+Version: 0.0.7
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
+Download-URL: https://pypi.org/project/dream_river/
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -20,8 +19,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: LICENSE.txt
 
 This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.
-
```

### Comparing `dream_river-0.0.6/README.rst` & `dream_river-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/dream_river/ML.py` & `dream_river-0.0.7/dream_river/ML.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from sklearn import model_selection
 from sklearn.metrics import accuracy_score
 from IPython.display import Image
 from datacube.utils import geometry
 from datacube.utils.cog import write_cog
 from dea_tools.classification import collect_training_data, predict_xr
 from dea_tools.bandindices import calculate_indices
-from convertools import vectorize
+from dream_river.convertools import vectorize
 import warnings
 warnings.filterwarnings("ignore")
 
 def custom_loadband(query):
 
     # Initialise datacube
     dc = datacube.Datacube(app='extract_VI')
```

### Comparing `dream_river-0.0.6/dream_river/convertools.py` & `dream_river-0.0.7/dream_river/convertools.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/dream_river/geobox.py` & `dream_river-0.0.7/dream_river/geobox.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/dream_river/indices.py` & `dream_river-0.0.7/dream_river/indices.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/dream_river/plotimg.py` & `dream_river-0.0.7/dream_river/plotimg.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.6/dream_river.egg-info/PKG-INFO` & `dream_river-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: dream-river
-Version: 0.0.6
+Name: dream_river
+Version: 0.0.7
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
+Download-URL: https://pypi.org/project/dream_river/
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -20,8 +19,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: LICENSE.txt
 
 This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.
-
```

### Comparing `dream_river-0.0.6/setup.py` & `dream_river-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESC ='This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.'
 
 setup(
     name='dream_river',
     packages=['dream_river'],
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     author_email='dreamusaha@gmail.com',
     description= 'This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube',
     long_description= DESC,
     author='Pathakorn Usaha',
     url= 'https://github.com/Pathakorn40/rice-detection',
     download_url= 'https://pypi.org/project/dream_river/',
```

