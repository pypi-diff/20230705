# Comparing `tmp/autoconf-2023.6.18.3.tar.gz` & `tmp/autoconf-2023.7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-2023.6.18.3.tar", last modified: Sun Jun 18 22:19:09 2023, max compression
+gzip compressed data, was "autoconf-2023.7.5.2.tar", last modified: Wed Jul  5 14:50:43 2023, max compression
```

## Comparing `autoconf-2023.6.18.3.tar` & `autoconf-2023.7.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/autoconf/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/class_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/dictable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/directory_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/autoconf/json_prior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/json_prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/json_prior/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/json_prior/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/autoconf/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/mock/mock_real.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/autoconf/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/autoconf/tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/autoconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-18 22:19:09.000000 autoconf-2023.6.18.3/autoconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 22:19:09.589834 autoconf-2023.6.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-18 22:18:55.000000 autoconf-2023.6.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.483229 autoconf-2023.7.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 14:50:43.483229 autoconf-2023.7.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.479229 autoconf-2023.7.5.2/autoconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/class_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/dictable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/directory_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.479229 autoconf-2023.7.5.2/autoconf/json_prior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/json_prior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/json_prior/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/json_prior/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.479229 autoconf-2023.7.5.2/autoconf/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/mock/mock_real.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.483229 autoconf-2023.7.5.2/autoconf/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/autoconf/tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.483229 autoconf-2023.7.5.2/autoconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 14:50:43.000000 autoconf-2023.7.5.2/autoconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 14:50:43.483229 autoconf-2023.7.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-05 14:50:30.000000 autoconf-2023.7.5.2/setup.py
```

### Comparing `autoconf-2023.6.18.3/LICENSE` & `autoconf-2023.7.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/PKG-INFO` & `autoconf-2023.7.5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf
-Version: 2023.6.18.3
+Version: 2023.7.5.2
 Summary: PyAuto Configration
 Home-page: https://github.com/rhayes777/PyAutoConf
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoconf-2023.6.18.3/autoconf/class_path.py` & `autoconf-2023.7.5.2/autoconf/class_path.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/conf.py` & `autoconf-2023.7.5.2/autoconf/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/dictable.py` & `autoconf-2023.7.5.2/autoconf/dictable.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/directory_config.py` & `autoconf-2023.7.5.2/autoconf/directory_config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/json_prior/config.py` & `autoconf-2023.7.5.2/autoconf/json_prior/config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/json_prior/generate.py` & `autoconf-2023.7.5.2/autoconf/json_prior/generate.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/mock/mock_real.py` & `autoconf-2023.7.5.2/autoconf/mock/mock_real.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/autoconf/tools/decorators.py` & `autoconf-2023.7.5.2/autoconf/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.18.3/setup.py` & `autoconf-2023.7.5.2/setup.py`

 * *Files identical despite different names*

