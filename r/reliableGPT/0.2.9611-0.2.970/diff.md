# Comparing `tmp/reliableGPT-0.2.9611.tar.gz` & `tmp/reliableGPT-0.2.970.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.9611.tar", last modified: Mon Jul  3 15:41:38 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.970.tar", last modified: Wed Jul  5 20:48:51 2023, max compression
```

## Comparing `reliableGPT-0.2.9611.tar` & `reliableGPT-0.2.970.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:41:38.219202 reliableGPT-0.2.9611/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.9611/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      157 2023-07-03 15:41:38.219080 reliableGPT-0.2.9611/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.9611/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.9611/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:41:38.216616 reliableGPT-0.2.9611/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      157 2023-07-03 15:41:38.000000 reliableGPT-0.2.9611/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-03 15:41:38.000000 reliableGPT-0.2.9611/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-03 15:41:38.000000 reliableGPT-0.2.9611/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-03 15:41:38.000000 reliableGPT-0.2.9611/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-03 15:41:38.000000 reliableGPT-0.2.9611/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:41:38.218897 reliableGPT-0.2.9611/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.9611/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.9611/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.9611/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11549 2023-07-03 15:14:41.000000 reliableGPT-0.2.9611/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.9611/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.9611/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-03 15:14:41.000000 reliableGPT-0.2.9611/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      429 2023-07-03 15:41:24.000000 reliableGPT-0.2.9611/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3900 2023-07-03 15:26:34.000000 reliableGPT-0.2.9611/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.9611/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-03 15:41:38.219252 reliableGPT-0.2.9611/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      399 2023-07-03 15:41:29.000000 reliableGPT-0.2.9611/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:48:51.708411 reliableGPT-0.2.970/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.970/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-05 20:48:51.708304 reliableGPT-0.2.970/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8271 2023-07-03 21:43:04.000000 reliableGPT-0.2.970/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.970/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:48:51.706153 reliableGPT-0.2.970/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-05 20:48:51.000000 reliableGPT-0.2.970/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      514 2023-07-05 20:48:51.000000 reliableGPT-0.2.970/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-05 20:48:51.000000 reliableGPT-0.2.970/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-05 20:48:51.000000 reliableGPT-0.2.970/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-05 20:48:51.000000 reliableGPT-0.2.970/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:48:51.707932 reliableGPT-0.2.970/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.970/reliablegpt/APICallHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3120 2023-06-28 23:12:14.000000 reliableGPT-0.2.970/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.970/reliablegpt/CustomQueue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    11802 2023-07-05 20:47:04.000000 reliableGPT-0.2.970/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.970/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.970/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7119 2023-07-03 21:43:04.000000 reliableGPT-0.2.970/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      374 2023-07-03 21:43:04.000000 reliableGPT-0.2.970/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5667 2023-07-05 20:46:57.000000 reliableGPT-0.2.970/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-03 21:42:46.000000 reliableGPT-0.2.970/reliablegpt/reliableQuery.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-05 20:48:51.708450 reliableGPT-0.2.970/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-05 20:48:38.000000 reliableGPT-0.2.970/setup.py
```

### Comparing `reliableGPT-0.2.9611/LICENSE` & `reliableGPT-0.2.970/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/README.md` & `reliableGPT-0.2.970/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.970/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.970/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/Alerting.py` & `reliableGPT-0.2.970/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.970/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.970/reliablegpt/IndividualRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,35 +256,41 @@
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.recovered_request_exception',
           result=result,
           posthog_metadata={
             'error': str(e),
             'recovered_response': result
           },
-          errors=[e])
+          errors=[e],
+          function_name=str(self.model_function),
+          kwargs=kwargs)
       else:
         # No errors, successfull retry
         self.save_request(user_email=self.user_email,
                           graceful_string=self.graceful_string,
                           posthog_event="reliableGPT.recovered_request",
                           result=result,
                           posthog_metadata={
                             'error': str(e),
                             'recovered_response': result
                           },
-                          errors=[e])
+                          errors=[e],
+                          function_name=str(self.model_function),
+                          kwargs=kwargs)
     except Exception as e2:
       # Exception 2, After trying to rescue
       print("gets 2nd error: ", e2)
       self.save_request(
         user_email=self.user_email,
         graceful_string=self.graceful_string,
         posthog_event='reliableGPT.recovered_request_exception',
         result="",
         posthog_metadata={
           'original_error': str(e),
           'error2': str(e2),
           'recovered_response': self.graceful_string
         },
-        errors=[e, e2])
+        errors=[e, e2],
+        function_name=str(self.model_function),
+        kwargs=kwargs)
       return result
     return result
```

### Comparing `reliableGPT-0.2.9611/reliablegpt/Model.py` & `reliableGPT-0.2.970/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.970/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.970/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9611/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.970/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

