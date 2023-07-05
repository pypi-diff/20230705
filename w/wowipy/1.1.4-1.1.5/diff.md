# Comparing `tmp/wowipy-1.1.4.tar.gz` & `tmp/wowipy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.4.tar", last modified: Mon Jul  3 14:23:09 2023, max compression
+gzip compressed data, was "wowipy-1.1.5.tar", last modified: Wed Jul  5 08:07:24 2023, max compression
```

## Comparing `wowipy-1.1.4.tar` & `wowipy-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.090977 wowipy-1.1.4/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.4/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-07-03 14:23:09.090977 wowipy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-03 14:23:09.090977 wowipy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-03 14:23:07.000000 wowipy-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.073994 wowipy-1.1.4/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.4/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.4/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    49213 2023-06-30 09:34:21.000000 wowipy-1.1.4/wowipy/models.py
--rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.4/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    43528 2023-06-30 09:41:11.000000 wowipy-1.1.4/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.089979 wowipy-1.1.4/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.483780 wowipy-1.1.5/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.5/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-07-05 08:07:24.482816 wowipy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:07:24.483780 wowipy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-05 08:07:22.000000 wowipy-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.465828 wowipy-1.1.5/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.5/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.5/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    49213 2023-06-30 09:34:21.000000 wowipy-1.1.5/wowipy/models.py
+-rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.5/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    43536 2023-07-05 08:07:06.000000 wowipy-1.1.5/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:07:24.481785 wowipy-1.1.5/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 08:07:24.000000 wowipy-1.1.5/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.4/COPYING` & `wowipy-1.1.5/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.4/LICENSE` & `wowipy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.4/PKG-INFO` & `wowipy-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.4
+Version: 1.1.5
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.4/setup.py` & `wowipy-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.4',
+    version='1.1.5',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.4/wowipy/models.py` & `wowipy-1.1.5/wowipy/models.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.4/wowipy/rest_adapter.py` & `wowipy-1.1.5/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.4/wowipy/wowipy.py` & `wowipy-1.1.5/wowipy/wowipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,25 +693,25 @@
         filter_params['includePaymentOrder'] = 'true'
 
         if add_args is not None:
             filter_params.update(add_args)
         retlist = []
 
         if not fetch_all:
-            result = self._rest_adapter.get(endpoint='Commissioning/InvoiceReceipt/CommissionItems',
+            result = self._rest_adapter.get(endpoint='CommissioningRead/InvoiceReceipt/CommissionItems',
                                             ep_params=filter_params)
         else:
             result = Result(0, "", [])
             merge_schema = {"mergeStrategy": "append"}
             merger = Merger(schema=merge_schema)
             filter_params['offset'] = 0
             filter_params['limit'] = 100
             response_count = 100
             while response_count == 100:
-                part_result = self._rest_adapter.get(endpoint='Commissioning/InvoiceReceipt/CommissionItems',
+                part_result = self._rest_adapter.get(endpoint='CommissioningRead/InvoiceReceipt/CommissionItems',
                                                      ep_params=filter_params)
                 result.data = merger.merge(result.data, part_result.data)
                 filter_params['offset'] += 100
                 response_count = len(part_result.data)
                 print(f"Receipt-Count: {len(result.data)}")
 
         for entry in result.data:
```

### Comparing `wowipy-1.1.4/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.5/wowipy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.4
+Version: 1.1.5
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

