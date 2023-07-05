# Comparing `tmp/batch-mailchimp-1.1.3.tar.gz` & `tmp/batch-mailchimp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-mailchimp-1.1.3.tar", last modified: Wed Jul  5 15:36:42 2023, max compression
+gzip compressed data, was "batch-mailchimp-1.2.0.tar", last modified: Wed Jul  5 18:40:32 2023, max compression
```

## Comparing `batch-mailchimp-1.1.3.tar` & `batch-mailchimp-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:36:42.268843 batch-mailchimp-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 15:36:42.268843 batch-mailchimp-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:36:42.264843 batch-mailchimp-1.1.3/batch_mailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/batch_mailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/batch_mailchimp/batches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/batch_mailchimp/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/batch_mailchimp/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:36:42.268843 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 15:36:42.000000 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 15:36:42.000000 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:36:42.000000 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 15:36:42.000000 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 15:36:42.000000 batch-mailchimp-1.1.3/batch_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:36:42.268843 batch-mailchimp-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 15:36:34.000000 batch-mailchimp-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/batch_mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/batch_mailchimp/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 18:40:32.000000 batch-mailchimp-1.2.0/batch_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:40:32.535920 batch-mailchimp-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 18:40:24.000000 batch-mailchimp-1.2.0/setup.py
```

### Comparing `batch-mailchimp-1.1.3/LICENSE` & `batch-mailchimp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.3/PKG-INFO` & `batch-mailchimp-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.1.3
+Version: 1.2.0
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `batch-mailchimp-1.1.3/README.rst` & `batch-mailchimp-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.3/batch_mailchimp/__init__.py` & `batch-mailchimp-1.2.0/batch_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.3/batch_mailchimp/batches_api.py` & `batch-mailchimp-1.2.0/batch_mailchimp/batches_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         )
 
 
 class Batch:
     def __init__(self, batches_api, **kwargs):
         self._batches_api = batches_api
         self._operations = kwargs.get("operations")
-        self._response = None
+        self._responses = None
         self.update(**kwargs)
 
     def update(self, **kwargs):
         self.batch_id = kwargs.get("id")
         self.total_operations = kwargs.get("total_operations")
         self.finished_operations = kwargs.get("finished_operations")
         self.errored_operations = kwargs.get("errored_operations")
@@ -51,32 +51,32 @@
         )
 
     def status(self, refresh=False):
         if refresh:
             self._batches_api.status(self.batch_id, refresh=refresh)
         return self
 
-    def response(self):
-        if self._response:
-            return self._response
+    def responses(self):
+        if self._responses:
+            return self._responses
         batch = self.status(refresh=True)
         if batch._status == "finished" and batch.response_body_url:
             content = requests.get(batch.response_body_url).content
             tf = tarfile.open(fileobj=BytesIO(content))
             output = []
             for member in tf.getmembers():
                 file_content = tf.extractfile(member)
                 if file_content is None:
                     continue
                 output += json.load(file_content)
-            self._response = ResponseCollection({
+            self._responses = ResponseCollection({
                 o["operation_id"]: Response(**o)
                 for o in output
             })
-            return self._response
+            return self._responses
 
     def delete(self):
         return self._batches_api.delete_request(self.batch_id)
 
 
 class BatchesApi(batches_api.BatchesApi):
     _max_operations = 1_000
```

### Comparing `batch-mailchimp-1.1.3/batch_mailchimp/collections.py` & `batch-mailchimp-1.2.0/batch_mailchimp/collections.py`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.3/batch_mailchimp.egg-info/PKG-INFO` & `batch-mailchimp-1.2.0/batch_mailchimp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.1.3
+Version: 1.2.0
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `batch-mailchimp-1.1.3/setup.py` & `batch-mailchimp-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="batch-mailchimp",
     description="A python client for MailChimp Marketing API, with batch support",
     url="https://github.com/FullFact/python-batchmailchimp",
     author="Andy Lulham",
     author_email="andy.lulham@fullfact.org",
-    version="1.1.3",
+    version="1.2.0",
     packages=find_packages(),
     license="MIT",
     keywords="mailchimp marketing api client wrapper",
     long_description=readme,
     install_requires=["mailchimp-marketing>=3.0.80"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

