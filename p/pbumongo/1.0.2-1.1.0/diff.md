# Comparing `tmp/pbumongo-1.0.2.tar.gz` & `tmp/pbumongo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbumongo-1.0.2.tar", last modified: Tue Jun  6 23:19:47 2023, max compression
+gzip compressed data, was "pbumongo-1.1.0.tar", last modified: Wed Jul  5 07:25:04 2023, max compression
```

## Comparing `pbumongo-1.0.2.tar` & `pbumongo-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.065248 pbumongo-1.0.2/
--rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-06-06 23:19:47.065248 pbumongo-1.0.2/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7981 2023-06-06 23:18:57.000000 pbumongo-1.0.2/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.064248 pbumongo-1.0.2/pbumongo/
--rw-r--r--   0 peter     (1000) peter     (1000)      183 2023-01-24 06:59:15.000000 pbumongo-1.0.2/pbumongo/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      679 2023-06-06 23:07:59.000000 pbumongo-1.0.2/pbumongo/mongo_connection.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2130 2023-01-24 08:05:48.000000 pbumongo-1.0.2/pbumongo/mongo_document.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12202 2023-06-06 23:13:09.000000 pbumongo-1.0.2/pbumongo/mongo_store.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.065248 pbumongo-1.0.2/pbumongo.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      309 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-01-24 06:59:18.000000 pbumongo-1.0.2/pbumongo.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       19 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        9 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-06 23:19:47.065248 pbumongo-1.0.2/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)      667 2023-06-06 23:19:08.000000 pbumongo-1.0.2/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:25:04.078668 pbumongo-1.1.0/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-07-05 07:25:04.078668 pbumongo-1.1.0/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7981 2023-06-06 23:18:57.000000 pbumongo-1.1.0/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:25:04.078668 pbumongo-1.1.0/pbumongo/
+-rw-r--r--   0 peter     (1000) peter     (1000)      183 2023-01-24 06:59:15.000000 pbumongo-1.1.0/pbumongo/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      678 2023-07-05 07:23:58.000000 pbumongo-1.1.0/pbumongo/mongo_connection.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1802 2023-07-05 07:22:14.000000 pbumongo-1.1.0/pbumongo/mongo_document.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12202 2023-07-05 07:23:38.000000 pbumongo-1.1.0/pbumongo/mongo_store.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:25:04.078668 pbumongo-1.1.0/pbumongo.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-07-05 07:25:04.000000 pbumongo-1.1.0/pbumongo.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      309 2023-07-05 07:25:04.000000 pbumongo-1.1.0/pbumongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-05 07:25:04.000000 pbumongo-1.1.0/pbumongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-01-24 06:59:18.000000 pbumongo-1.1.0/pbumongo.egg-info/not-zip-safe
+-rw-rw-r--   0 peter     (1000) peter     (1000)       19 2023-07-05 07:25:04.000000 pbumongo-1.1.0/pbumongo.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        9 2023-07-05 07:25:04.000000 pbumongo-1.1.0/pbumongo.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-05 07:25:04.079668 pbumongo-1.1.0/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      667 2023-07-05 07:23:04.000000 pbumongo-1.1.0/setup.py
```

### Comparing `pbumongo-1.0.2/PKG-INFO` & `pbumongo-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbumongo
-Version: 1.0.2
+Version: 1.1.0
 Summary: Basic MongoDB wrapper for object-oriented collection handling
 Home-page: https://github.com/ilfrich/pbu-mongo
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities - Mongo `pbumongo`
```

### Comparing `pbumongo-1.0.2/README.md` & `pbumongo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pbumongo-1.0.2/pbumongo/mongo_connection.py` & `pbumongo-1.1.0/pbumongo/mongo_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,8 @@
             raise ValueError("Parameter 'mongo_db' cannot be None")
         if mongo_url is None:
             raise ValueError("Parameter 'mongo_url' cannot be None")
         self.mongo_url = mongo_url
         self.mongo_db = mongo_db
 
     def create_store(self, store_class: Type[AbstractMongoStore], collection_name: str) -> AbstractMongoStore:
-        return store_class(mongo_url=self.mongo_url, mongo_db=self.mongo_db, collection_name=collection_name)
+        return store_class(mongo_url=self.mongo_url, db_name=self.mongo_db, collection_name=collection_name)
```

### Comparing `pbumongo-1.0.2/pbumongo/mongo_document.py` & `pbumongo-1.1.0/pbumongo/mongo_document.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,7 @@
         result = super().to_json()
         if self.id is not None:
             result["_id"] = str(self.id)
         if getattr(self, "data_model_version", None) is not None:
             result["dataModelVersion"] = self.data_model_version
 
         return result
-
-    @staticmethod
-    @abstractmethod
-    def from_json(json: dict):
-        """
-        Receives a dictionary or JSON object and returns an instance of this MongoDocument sub-class.
-        :param json: a dictionary or JSON object instance
-        :return: an instance of a sub-class of MongoDocument
-        """
-        pass
```

### Comparing `pbumongo-1.0.2/pbumongo/mongo_store.py` & `pbumongo-1.1.0/pbumongo/mongo_store.py`

 * *Files identical despite different names*

### Comparing `pbumongo-1.0.2/pbumongo.egg-info/PKG-INFO` & `pbumongo-1.1.0/pbumongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbumongo
-Version: 1.0.2
+Version: 1.1.0
 Summary: Basic MongoDB wrapper for object-oriented collection handling
 Home-page: https://github.com/ilfrich/pbu-mongo
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities - Mongo `pbumongo`
```

### Comparing `pbumongo-1.0.2/setup.py` & `pbumongo-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="pbumongo",
-      version="1.0.2",
+      version="1.1.0",
       description="Basic MongoDB wrapper for object-oriented collection handling",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/ilfrich/pbu-mongo",
       author="Peter Ilfrich",
       author_email="das-peter@gmx.de",
       license="Apache-2.0",
       packages=[
           "pbumongo"
       ],
       install_requires=[
           "pymongo",
-          "pbu>=1.0.0"
+          "pbu>=1.1.0"
       ],
       tests_require=[
           "pytest",
       ],
       zip_safe=False)
```

