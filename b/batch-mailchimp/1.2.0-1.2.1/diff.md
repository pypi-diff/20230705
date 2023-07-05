# Comparing `tmp/batch-mailchimp-1.2.0.tar.gz` & `tmp/batch-mailchimp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-mailchimp-1.2.0.tar", last modified: Wed Jul  5 18:40:32 2023, max compression
+gzip compressed data, was "batch-mailchimp-1.2.1.tar", last modified: Wed Jul  5 21:18:24 2023, max compression
```

## Comparing `batch-mailchimp-1.2.0.tar` & `batch-mailchimp-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/batch_mailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/batches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:24.523309 batch-mailchimp-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 21:18:24.523309 batch-mailchimp-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:24.523309 batch-mailchimp-1.2.1/batch_mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/batch_mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/batch_mailchimp/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/batch_mailchimp/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/batch_mailchimp/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:24.523309 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 21:18:24.000000 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 21:18:24.000000 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:18:24.000000 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 21:18:24.000000 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 21:18:24.000000 batch-mailchimp-1.2.1/batch_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:18:24.523309 batch-mailchimp-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 21:18:17.000000 batch-mailchimp-1.2.1/setup.py
```

### Comparing `batch-mailchimp-1.2.0/LICENSE` & `batch-mailchimp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.2.0/PKG-INFO` & `batch-mailchimp-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `batch-mailchimp-1.2.0/README.rst` & `batch-mailchimp-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.2.0/batch_mailchimp/__init__.py` & `batch-mailchimp-1.2.1/batch_mailchimp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,13 +109,18 @@
         self.searchCampaigns = SearchCampaignsApi(self.api_client)
         self.searchMembers = SearchMembersApi(self.api_client)
         self.templateFolders = TemplateFoldersApi(self.api_client)
         self.templates = TemplatesApi(self.api_client)
         self.verifiedDomains = VerifiedDomainsApi(self.api_client)
         self.batches = BatchesApi(self.api_client)
 
+    def __str__(self):
+        return "batch mode {batch_mode_toggle}".format(
+            batch_mode_toggle="ON" if self.api_client.batch_mode else "OFF",
+        )
+
     def __repr__(self):
-        return "<{module}.{name}: batch mode {batch_mode_toggle}>".format(
+        return "<{module}.{name}: {str_rep}>".format(
             module=self.__class__.__module__,
             name=self.__class__.__name__,
-            batch_mode_toggle="ON" if self.api_client.batch_mode else "OFF",
+            str_rep=str(self),
         )
```

### Comparing `batch-mailchimp-1.2.0/batch_mailchimp/batches_api.py` & `batch-mailchimp-1.2.1/batch_mailchimp/batches_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import json
 from io import BytesIO
 import tarfile
-from itertools import islice
 from mailchimp_marketing.api import batches_api
 import requests
 from .decorators import no_batch
 from .collections import BatchCollection, ResponseCollection
 
 
 class Response:
     def __init__(self, **kwargs):
         self.operation_id = kwargs["operation_id"]
         self.status_code = kwargs["status_code"]
         self.body = json.loads(kwargs["response"])
 
+    def __str__(self):
+        return "{operation_id} ({status_code}".format(
+            operation_id=self.operation_id,
+            status_code=self.status_code,
+        )
+
     def __repr__(self):
-        return "<{module}.{name}: {operation_id} ({status_code})>".format(
+        return "<{module}.{name}: {str_rep}>".format(
             module=self.__class__.__module__,
             name=self.__class__.__name__,
-            operation_id=self.operation_id,
-            status_code=self.status_code,
+            str_rep=str(self),
         )
 
 
 class Batch:
     def __init__(self, batches_api, **kwargs):
         self._batches_api = batches_api
         self._operations = kwargs.get("operations")
@@ -36,24 +40,29 @@
         self.finished_operations = kwargs.get("finished_operations")
         self.errored_operations = kwargs.get("errored_operations")
         self.submitted_at = kwargs.get("submitted_at")
         self.completed_at = kwargs.get("completed_at")
         self.response_body_url = kwargs.get("response_body_url")
         self._status = kwargs.get("status")
 
-    def __repr__(self):
-        return "<{module}.{name}: {finished}/{total} operation{s} ({status})>".format(
-            module=self.__class__.__module__,
-            name=self.__class__.__name__,
+    def __str__(self):
+        return "{finished}/{total} operation{s} ({status})".format(
             finished=self.finished_operations,
             total=self.total_operations,
             s="s" if self.total_operations != 1 else "",
             status=self._status,
         )
 
+    def __repr__(self):
+        return "<{module}.{name}: {str_rep}>".format(
+            module=self.__class__.__module__,
+            name=self.__class__.__name__,
+            str_rep=str(self),
+        )
+
     def status(self, refresh=False):
         if refresh:
             self._batches_api.status(self.batch_id, refresh=refresh)
         return self
 
     def responses(self):
         if self._responses:
@@ -106,21 +115,22 @@
         batch = Batch(self, operations=operations, **batch_data)
         self._batches[batch.batch_id] = batch
         self.api_client.operations = []
         return batch
 
     @no_batch
     def bulk_run(self):
-        if len(self.api_client.operations) == 0:
+        if self.api_client.operations == []:
             raise Exception("No operations to run")
-        operations = iter(self.api_client.operations)
-        while operations_chunk := list(islice(operations, self._max_operations)):
+        while self.api_client.operations:
+            operations_chunk = self.api_client.operations[:self._max_operations]
             batch_data = self.start({"operations": operations_chunk})
             batch = Batch(self, operations=operations_chunk, **batch_data)
             self._batches[batch.batch_id] = batch
+            self.api_client.operations = self.api_client.operations[self._max_operations:]
         return self._batches
 
     def delete_all(self, refresh=False, **kwargs):
         batches = self.list(refresh=refresh)
         batch_ids = [batch.batch_id for batch in batches]
         for batch_id in batch_ids:
             self.delete_request(batch_id)
```

### Comparing `batch-mailchimp-1.2.0/batch_mailchimp/collections.py` & `batch-mailchimp-1.2.1/batch_mailchimp/collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from collections import UserDict
 
 
 class MyCollection(UserDict):
+    def __str__(self):
+        return str(list(self.data.values())),
+
     def __repr__(self):
-        return "<{module}.{name}: {data}>".format(
+        return "<{module}.{name}: {str_rep}>".format(
             module=self.__class__.__module__,
             name=self.__class__.__name__,
-            data=list(self.data.values()),
+            str_rep=str(self),
         )
 
     def __getitem__(self, item):
         if type(item) is str:
             return super().__getitem__(item)
         return list(self.data.values())[item]
```

### Comparing `batch-mailchimp-1.2.0/batch_mailchimp.egg-info/PKG-INFO` & `batch-mailchimp-1.2.1/batch_mailchimp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `batch-mailchimp-1.2.0/setup.py` & `batch-mailchimp-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="batch-mailchimp",
     description="A python client for MailChimp Marketing API, with batch support",
     url="https://github.com/FullFact/python-batchmailchimp",
     author="Andy Lulham",
     author_email="andy.lulham@fullfact.org",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     license="MIT",
     keywords="mailchimp marketing api client wrapper",
     long_description=readme,
     install_requires=["mailchimp-marketing>=3.0.80"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

