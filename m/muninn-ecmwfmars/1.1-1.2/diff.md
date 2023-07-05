# Comparing `tmp/muninn-ecmwfmars-1.1.tar.gz` & `tmp/muninn-ecmwfmars-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muninn-ecmwfmars-1.1.tar", last modified: Wed Nov  3 16:46:17 2021, max compression
+gzip compressed data, was "dist/muninn-ecmwfmars-1.2.tar", last modified: Wed Jul  5 12:09:37 2023, max compression
```

## Comparing `muninn-ecmwfmars-1.1.tar` & `muninn-ecmwfmars-1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/
--rw-r--r--   0 sander     (501) staff       (20)      601 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)     1513 2021-01-21 17:10:35.000000 muninn-ecmwfmars-1.1/LICENSE
--rw-r--r--   0 sander     (501) staff       (20)      678 2021-11-03 16:44:09.000000 muninn-ecmwfmars-1.1/setup.py
--rw-r--r--   0 sander     (501) staff       (20)       38 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/setup.cfg
--rw-r--r--   0 sander     (501) staff       (20)    19446 2021-05-14 10:50:35.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.py
--rw-r--r--   0 sander     (501) staff       (20)      588 2021-01-21 17:10:35.000000 muninn-ecmwfmars-1.1/README.rst
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/
--rw-r--r--   0 sander     (501) staff       (20)      601 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)      246 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/SOURCES.txt
--rw-r--r--   0 sander     (501) staff       (20)        7 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/requires.txt
--rw-r--r--   0 sander     (501) staff       (20)       17 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/top_level.txt
--rw-r--r--   0 sander     (501) staff       (20)        1 2021-11-03 16:46:17.000000 muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/dependency_links.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/
+-rw-r--r--   0 sander     (501) staff       (20)      601 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)      678 2023-07-05 12:04:34.000000 muninn-ecmwfmars-1.2/setup.py
+-rw-r--r--   0 sander     (501) staff       (20)       38 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/setup.cfg
+-rw-r--r--   0 sander     (501) staff       (20)    19548 2023-03-27 14:41:28.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.py
+-rw-r--r--   0 sander     (501) staff       (20)      588 2021-04-01 08:09:08.000000 muninn-ecmwfmars-1.2/README.rst
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/
+-rw-r--r--   0 sander     (501) staff       (20)      601 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)      238 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/SOURCES.txt
+-rw-r--r--   0 sander     (501) staff       (20)        7 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/requires.txt
+-rw-r--r--   0 sander     (501) staff       (20)       17 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/top_level.txt
+-rw-r--r--   0 sander     (501) staff       (20)        1 2023-07-05 12:09:37.000000 muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/dependency_links.txt
```

### Comparing `muninn-ecmwfmars-1.1/PKG-INFO` & `muninn-ecmwfmars-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: muninn-ecmwfmars
-Version: 1.1
+Version: 1.2
 Summary: Muninn extension for ECMWF GRIB products from the mars archive
 Home-page: https://github.com/stcorp/muninn-ecmwfmars
 Author: S[&]T
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `muninn-ecmwfmars-1.1/setup.py` & `muninn-ecmwfmars-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="muninn-ecmwfmars",
-    version="1.1",
+    version="1.2",
     description="Muninn extension for ECMWF GRIB products from the mars archive",
     url="https://github.com/stcorp/muninn-ecmwfmars",
     author="S[&]T",
     license="BSD",
     py_modules=["muninn_ecmwfmars"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `muninn-ecmwfmars-1.1/muninn_ecmwfmars.py` & `muninn-ecmwfmars-1.2/muninn_ecmwfmars.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,15 +448,15 @@
             coda.cursor_goto_parent(cursor)
             if i < num_messages - 1:
                 coda.cursor_goto_next_array_element(cursor)
 
     return ecmwfmars, levtype_options
 
 
-def get_remote_url(filename, ecmwfmars, levtype_options):
+def get_remote_url(filename, ecmwfmars, levtype_options, packing=None):
     """
         levtype_options should be a dict with for each 'levtype' field a dict containing:
         - string 'param'
             '/' separated list of parameters for the given level type
             https://software.ecmwf.int/wiki/display/UDOC/Identification+keywords#Identificationkeywords-param
         - string 'levelist' (optional)
             '/' separated list of levels for the given level type
@@ -479,14 +479,16 @@
         request['step'] = str(ecmwfmars.step)
     if 'resol' in ecmwfmars:
         request['resol'] = ecmwfmars.resol
     if 'grid' in ecmwfmars:
         request['grid'] = ecmwfmars.grid
     if 'area' in ecmwfmars:
         request['area'] = ecmwfmars.area
+    if packing is not None:
+        request['packing'] = packing
 
     first = True
     for levtype in levtype_options:
         if first:
             first = False
         else:
             # The '&concatenate&' is a muninn-specific way of combining multiple requests in one
@@ -498,15 +500,15 @@
         elif 'levelist' in request:
             del request['levelist']
         remote_url += "&".join(["%s=%s" % (key, str(request[key])) for key in request])
 
     return remote_url
 
 
-def get_core_properties(product_type, ecmwfmars, levtype_options=None):
+def get_core_properties(product_type, ecmwfmars, levtype_options=None, packing=None):
     date = datetime.datetime.strptime(ecmwfmars.date.replace('-', ''), "%Y%m%d")
     time = ecmwfmars.time.replace(':', '')
     if len(time) >= 2:
         if len(time) >= 4:
             date += datetime.timedelta(hours=int(time[0:2]), minutes=int(time[2:4]))
         else:
             date += datetime.timedelta(hours=int(time[0:2]))
@@ -522,15 +524,15 @@
     core.validity_start = date
     if 'step' in ecmwfmars:
         core.validity_start += datetime.timedelta(hours=ecmwfmars.step)
     core.validity_stop = core.validity_start
     # the creation date is set to the base time of the model
     core.creation_date = date
     if levtype_options:
-        core.remote_url = get_remote_url(core.physical_name, ecmwfmars, levtype_options)
+        core.remote_url = get_remote_url(core.physical_name, ecmwfmars, levtype_options, packing)
     return core
 
 
 class ECMWFBackend(RemoteBackend):
     """
     'ecmwfapi' urls are custom defined urls for retrieving data from ECMWF MARS.
     It uses the following format:
```

### Comparing `muninn-ecmwfmars-1.1/README.rst` & `muninn-ecmwfmars-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `muninn-ecmwfmars-1.1/muninn_ecmwfmars.egg-info/PKG-INFO` & `muninn-ecmwfmars-1.2/muninn_ecmwfmars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: muninn-ecmwfmars
-Version: 1.1
+Version: 1.2
 Summary: Muninn extension for ECMWF GRIB products from the mars archive
 Home-page: https://github.com/stcorp/muninn-ecmwfmars
 Author: S[&]T
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

