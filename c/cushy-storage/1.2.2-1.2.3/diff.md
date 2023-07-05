# Comparing `tmp/cushy-storage-1.2.2.tar.gz` & `tmp/cushy-storage-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-worzx5zr/cushy-storage-1.2.2.tar", last modified: Fri Jun 23 06:50:15 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-pi3w3zv1/cushy-storage-1.2.3.tar", last modified: Wed Jul  5 15:05:03 2023, max compression
```

## Comparing `cushy-storage-1.2.2.tar` & `cushy-storage-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/cushy_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/cushy_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:50:15.000000 cushy-storage-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/tests/test_base_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/tests/test_cushy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/tests/test_dict_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-23 06:50:04.000000 cushy-storage-1.2.2/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:05:03.000000 cushy-storage-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/tests/test_dict_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-05 15:04:45.000000 cushy-storage-1.2.3/tests/test_orm.py
```

### Comparing `cushy-storage-1.2.2/LICENSE` & `cushy-storage-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/PKG-INFO` & `cushy-storage-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.2.2
+Version: 1.2.3
 Summary: A data local persistence ORM framework
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.2.2/README.md` & `cushy-storage-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage/__init__.py` & `cushy-storage-1.2.3/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage/_core.py` & `cushy-storage-1.2.3/cushy_storage/_core.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage/base.py` & `cushy-storage-1.2.3/cushy_storage/base.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage/logger.py` & `cushy-storage-1.2.3/cushy_storage/logger.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage/orm.py` & `cushy-storage-1.2.3/cushy_storage/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,18 @@
                     is_target = False
                     continue
             if is_target:
                 result.append(item)
 
         return self._from_filter(result, self.__name__)
 
-    def all(self) -> Optional[List[BaseORMModel]]:
+    def all(self) -> Optional[List]:
         return self._data
 
-    def first(self) -> Optional[BaseORMModel]:
+    def first(self):
         if len(self._data) == 0:
             return None
         return self._data[0]
 
     def print_all(self):
         for item in self._data:
             print(f"[cushy-storage orm] {item.__dict__}")
```

### Comparing `cushy-storage-1.2.2/cushy_storage/utils.py` & `cushy-storage-1.2.3/cushy_storage/utils.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.2.3/cushy_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.2.2
+Version: 1.2.3
 Summary: A data local persistence ORM framework
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.2.2/setup.py` & `cushy-storage-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.2.2",
+    version="1.2.3",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence ORM framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.2.2/tests/test_base_dict.py` & `cushy-storage-1.2.3/tests/test_base_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/tests/test_cushy_dict.py` & `cushy-storage-1.2.3/tests/test_cushy_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/tests/test_dict_cache.py` & `cushy-storage-1.2.3/tests/test_dict_cache.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.2/tests/test_orm.py` & `cushy-storage-1.2.3/tests/test_orm.py`

 * *Files identical despite different names*

