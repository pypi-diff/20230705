# Comparing `tmp/netorca-sdk-0.1.1.tar.gz` & `tmp/netorca-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netorca-sdk-0.1.1.tar", last modified: Fri Jun 16 10:08:57 2023, max compression
+gzip compressed data, was "netorca-sdk-0.1.2.tar", last modified: Wed Jul  5 10:02:37 2023, max compression
```

## Comparing `netorca-sdk-0.1.1.tar` & `netorca-sdk-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.131534 netorca-sdk-0.1.1/netorca_sdk/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5492 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10705 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8375 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/netorca.py
--rw-rw-rw-   0 root         (0) root         (0)    10442 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/serviceowner.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/netorca_sdk/validations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.131534 netorca-sdk-0.1.1/netorca_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-16 10:08:57.000000 netorca-sdk-0.1.1/netorca_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 10:08:57.132534 netorca-sdk-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    10410 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)    11854 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_netorca.py
--rw-rw-rw-   0 root         (0) root         (0)     7998 2023-06-16 10:08:42.000000 netorca-sdk-0.1.1/tests/test_serviceowner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:02:37.085648 netorca-sdk-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-05 10:02:37.085648 netorca-sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:02:37.084648 netorca-sdk-0.1.2/netorca_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5493 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11475 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8375 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/serviceowner.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/netorca_sdk/validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:02:37.084648 netorca-sdk-0.1.2/netorca_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-05 10:02:37.000000 netorca-sdk-0.1.2/netorca_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-05 10:02:37.000000 netorca-sdk-0.1.2/netorca_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:02:37.000000 netorca-sdk-0.1.2/netorca_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-05 10:02:37.000000 netorca-sdk-0.1.2/netorca_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-05 10:02:37.000000 netorca-sdk-0.1.2/netorca_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:02:37.085648 netorca-sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:02:37.084648 netorca-sdk-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/tests/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    10410 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/tests/test_netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)     7998 2023-07-05 10:02:21.000000 netorca-sdk-0.1.2/tests/test_serviceowner.py
```

### Comparing `netorca-sdk-0.1.1/LICENSE` & `netorca-sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/PKG-INFO` & `netorca-sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netorca-sdk-0.1.1/netorca_sdk/auth.py` & `netorca-sdk-0.1.2/netorca_sdk/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         if not url or not data:
             raise NetorcaException("URL or data not provided!")
 
         if authentication_required:
             response = requests.patch(url=url, data=data, headers=self.headers, verify=False)
         else:
             response = requests.patch(url=url, data=data, verify=False)
+
         if 200 <= response.status_code < 500:
             return response
         raise NetorcaException(
             f"Failed to send PATCH request. PATCH details: {args, kwargs}. Response details: {response.json()}"
         )
 
     def delete(self, *args, **kwargs):
```

### Comparing `netorca-sdk-0.1.1/netorca_sdk/config.py` & `netorca-sdk-0.1.2/netorca_sdk/config.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/netorca_sdk/consumer.py` & `netorca-sdk-0.1.2/netorca_sdk/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,55 +142,68 @@
         full_request = {team["name"]: self.consumer_submission}
 
         if metadata is not None:
             full_request[team["name"]]["metadata"] = metadata
 
         return full_request
 
-    def validate(self, pretty_print=False) -> Tuple[bool, dict]:
+    def validate(self, pretty_print=False, partial=False) -> Tuple[bool, dict]:
         """
         Validate consume request.
         NOTE: Data must be first imported with `load_from_repository` method
-
+        Parameters:
+            pretty_print:   (optional) pretty print errors, default: False
+            partial:        (optional) partial validation, default: False
         Returns:
             Tuple[bool, str]    ->  is_valid, validation_errors
         """
         if not (self.config and self.auth):
             raise NetorcaException("Use `load_from_repository(repository_path)` method to load configuration.")
         VALIDATE_REQUEST_PATH = f"{self.auth.fqdn}{VALIDATE_CONSUMER_SUBMISSION_ENDPOINT}"
         full_request = self.prepare_request()
 
-        response = self.auth.post(
-            url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True
-        )
+        if partial:
+            response = self.auth.patch(url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request),
+                                       authentication_required=True)
+        else:
+            response = self.auth.post(url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request),
+                                      authentication_required=True)
 
         response = response.json()
         if response.get("is_valid"):
             return True, {}
         errors = response.get("errors")
 
         if pretty_print:
             ConsumerSubmission.pretty_print_errors(errors)
         return False, errors
 
-    def submit(self) -> Tuple[bool, str]:
+    def submit(self, partial=False) -> Tuple[bool, str]:
         """
         Validate and submit consumer request.
         NOTE: Data must be first imported with `load_from_repository` method
 
+        Parameters:
+            partial:        (optional) partial submission, default: False
         Returns:
             bool, str    ->  submission successful, submission messages
         """
-        is_valid = self.validate(pretty_print=True)
+        is_valid = self.validate(pretty_print=True, partial=partial)
         if not is_valid[0]:
             return False, "Consumer request is invalid and cannot be submitted."
 
         SUBMIT_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_CONSUMER_SUBMISSION_ENDPOINT}"
         full_request = self.prepare_request()
-        response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True)
+        if partial:
+            response = self.auth.patch(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request),
+                                       authentication_required=True)
+        else:
+            response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request),
+                                      authentication_required=True)
+
         if response.status_code == 201:
             return True, "Submitted successfuly."
         return False, response.text
 
     @staticmethod
     def pretty_print_errors(errors: dict) -> None:
         """
```

### Comparing `netorca-sdk-0.1.1/netorca_sdk/netorca.py` & `netorca-sdk-0.1.2/netorca_sdk/netorca.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/netorca_sdk/serviceowner.py` & `netorca-sdk-0.1.2/netorca_sdk/serviceowner.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/netorca_sdk.egg-info/PKG-INFO` & `netorca-sdk-0.1.2/netorca_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netorca-sdk-0.1.1/setup.py` & `netorca-sdk-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="netorca-sdk",
     packages=["netorca_sdk"],
-    version="0.1.1",
+    version="0.1.2",
     license="MIT",
     description="A package for interacting with the NetOrca API",
     author="Scott Rowlandson",
     author_email="scott@netautomate.org",
     url="https://gitlab.com/netorca_public/netorca_sdk/",
     keywords=["netorca", "orchestration", "netautomate"],
     install_requires=[
```

### Comparing `netorca-sdk-0.1.1/tests/test_auth.py` & `netorca-sdk-0.1.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/tests/test_consumer.py` & `netorca-sdk-0.1.2/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/tests/test_netorca.py` & `netorca-sdk-0.1.2/tests/test_netorca.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.1/tests/test_serviceowner.py` & `netorca-sdk-0.1.2/tests/test_serviceowner.py`

 * *Files identical despite different names*

