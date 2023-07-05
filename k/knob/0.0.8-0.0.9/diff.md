# Comparing `tmp/knob-0.0.8.tar.gz` & `tmp/knob-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/knob-0.0.8.tar", last modified: Mon Aug  6 08:33:42 2018, max compression
+gzip compressed data, was "dist/knob-0.0.9.tar", last modified: Mon Aug  6 10:05:10 2018, max compression
```

## Comparing `knob-0.0.8.tar` & `knob-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 08:33:42.000000 knob-0.0.8/
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 08:33:42.000000 knob-0.0.8/knob.egg-info/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       11 2018-08-06 08:33:41.000000 knob-0.0.8/knob.egg-info/top_level.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      418 2018-08-06 08:33:41.000000 knob-0.0.8/knob.egg-info/PKG-INFO
--rw-r--r--   0 dodo      (1000) dodo      (1000)       31 2018-08-06 08:33:41.000000 knob-0.0.8/knob.egg-info/requires.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)        1 2018-08-06 08:33:41.000000 knob-0.0.8/knob.egg-info/dependency_links.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      338 2018-08-06 08:33:41.000000 knob-0.0.8/knob.egg-info/SOURCES.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      418 2018-08-06 08:33:42.000000 knob-0.0.8/PKG-INFO
--rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-08-06 08:33:42.000000 knob-0.0.8/setup.cfg
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 08:33:42.000000 knob-0.0.8/knob/
--rw-r--r--   0 dodo      (1000) dodo      (1000)      805 2018-07-10 07:15:58.000000 knob-0.0.8/knob/setting.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-07-09 07:34:28.000000 knob-0.0.8/knob/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      209 2018-07-09 07:48:32.000000 knob-0.0.8/knob/dt.py
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 08:33:42.000000 knob-0.0.8/knob/http/
--rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-09 07:46:45.000000 knob-0.0.8/knob/http/__init__.py
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2198 2018-07-09 08:14:44.000000 knob-0.0.8/knob/http/response.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1853 2018-08-06 08:33:33.000000 knob-0.0.8/knob/model.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1737 2018-07-09 07:41:08.000000 knob-0.0.8/knob/db_router.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      258 2018-07-09 08:36:23.000000 knob-0.0.8/knob/validators.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1001 2018-07-20 02:55:09.000000 knob-0.0.8/knob/crypt.py
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 08:33:42.000000 knob-0.0.8/tests/
--rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-20 02:27:32.000000 knob-0.0.8/tests/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      674 2018-07-20 02:54:05.000000 knob-0.0.8/tests/test_crypt.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      772 2018-08-06 08:31:10.000000 knob-0.0.8/setup.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 10:05:10.000000 knob-0.0.9/
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       11 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/top_level.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      418 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/PKG-INFO
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       31 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/requires.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)        1 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/dependency_links.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      338 2018-08-06 10:05:10.000000 knob-0.0.9/knob.egg-info/SOURCES.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      418 2018-08-06 10:05:10.000000 knob-0.0.9/PKG-INFO
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-08-06 10:05:10.000000 knob-0.0.9/setup.cfg
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 10:05:10.000000 knob-0.0.9/knob/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      805 2018-07-10 07:15:58.000000 knob-0.0.9/knob/setting.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2018-07-09 07:34:28.000000 knob-0.0.9/knob/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      209 2018-07-09 07:48:32.000000 knob-0.0.9/knob/dt.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 10:05:10.000000 knob-0.0.9/knob/http/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-09 07:46:45.000000 knob-0.0.9/knob/http/__init__.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2198 2018-07-09 08:14:44.000000 knob-0.0.9/knob/http/response.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1848 2018-08-06 10:04:51.000000 knob-0.0.9/knob/model.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1737 2018-07-09 07:41:08.000000 knob-0.0.9/knob/db_router.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      258 2018-07-09 08:36:23.000000 knob-0.0.9/knob/validators.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1001 2018-07-20 02:55:09.000000 knob-0.0.9/knob/crypt.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-08-06 10:05:10.000000 knob-0.0.9/tests/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-20 02:27:32.000000 knob-0.0.9/tests/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      674 2018-07-20 02:54:05.000000 knob-0.0.9/tests/test_crypt.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      772 2018-08-06 10:05:03.000000 knob-0.0.9/setup.py
```

### Comparing `knob-0.0.8/knob/setting.py` & `knob-0.0.9/knob/setting.py`

 * *Files identical despite different names*

### Comparing `knob-0.0.8/knob/http/response.py` & `knob-0.0.9/knob/http/response.py`

 * *Files identical despite different names*

### Comparing `knob-0.0.8/knob/model.py` & `knob-0.0.9/knob/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     """
     Updates an object of Django model instance with given info, optionally limited to certain fields only.
     :param obj: a Django model instance
     :param info: a dict
     :param fields: optional, only update these fields.
     :return: updated obj (saved)
     """
-    updated_fields = set()
+    update_fields = set()
     for key, val in six.iteritems(info):
         if fields is None or key in fields:
             setattr(obj, key, val)
-        updated_fields.add(key)
+        update_fields.add(key)
 
-    if updated_fields:
-        obj.save(updated_fields=list(updated_fields))
+    if update_fields:
+        obj.save(update_fields=list(update_fields))
 
     return obj
 
 
 def get_model_class(model):
     """
     Deduct the model class from given input.
```

### Comparing `knob-0.0.8/knob/db_router.py` & `knob-0.0.9/knob/db_router.py`

 * *Files identical despite different names*

### Comparing `knob-0.0.8/knob/crypt.py` & `knob-0.0.9/knob/crypt.py`

 * *Files identical despite different names*

### Comparing `knob-0.0.8/tests/test_crypt.py` & `knob-0.0.9/tests/test_crypt.py`

 * *Files identical despite different names*

### Comparing `knob-0.0.8/setup.py` & `knob-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 
 setuptools.setup(
     name="knob",
-    version="0.0.8",
+    version="0.0.9",
     author="claydodo and his little friends (xiao huo ban)",
     author_email="claydodo@foxmail.com",
     description="Django utils collection",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/claydodo/knob",
     packages=setuptools.find_packages(),
```

