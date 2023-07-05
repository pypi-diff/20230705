# Comparing `tmp/quickbolt-0.1.3.tar.gz` & `tmp/quickbolt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.1.3.tar", max compression
+gzip compressed data, was "quickbolt-0.1.4.tar", max compression
```

## Comparing `quickbolt-0.1.3.tar` & `quickbolt-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.3/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.3/README.md
--rw-r--r--   0        0        0     1238 2023-07-04 19:20:56.864321 quickbolt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.3/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.3/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    11241 2023-07-04 05:37:57.116510 quickbolt-0.1.3/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.3/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.3/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.3/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.3/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.3/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.3/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.3/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.3/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     7394 2023-07-03 21:01:01.356118 quickbolt-0.1.3/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.3/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     4266 2023-07-03 21:01:01.356324 quickbolt-0.1.3/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.3/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.3/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.3/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.3/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.3/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.4/README.md
+-rw-r--r--   0        0        0     1238 2023-07-05 05:53:30.375693 quickbolt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.4/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.4/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    11311 2023-07-05 02:39:06.705757 quickbolt-0.1.4/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.4/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.4/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.4/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.4/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.4/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.4/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.4/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.4/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     7522 2023-07-05 05:48:43.803436 quickbolt-0.1.4/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.4/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.1.4/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.4/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.4/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.4/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.4/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.4/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.4/PKG-INFO
```

### Comparing `quickbolt-0.1.3/LICENSE` & `quickbolt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/README.md` & `quickbolt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/pyproject.toml` & `quickbolt-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.1.3"
+version = "0.1.4"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.1.3/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.1.4/quickbolt/batch_generation/batch_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,20 @@
         "get": "200",
         "patch": "200",
         "post": "201",
         "put": "204",
         "delete": "204",
     }[method]
 
+    headers = headers or {}
+    bad_headers = []
+    if headers:
+        bad_headers = generate_bad_bodies(headers, min=min)[:bad_header_count]
+
     invalid_sub_values = {"str": "aaa", "digit": "999"}
-    bad_headers = generate_bad_bodies(headers, min=min)[:bad_header_count]
     invalid_urls = generate_bad_urls(url, invalid_sub_values, corrupt_query_params, min)
     not_found_urls = generate_bad_urls(
         url, corrupt_query_params=corrupt_query_params, min=min
     )
 
     clean_url = url.replace(";", "")
     if description:
```

### Comparing `quickbolt-0.1.3/quickbolt/clients/aio_requests.py` & `quickbolt-0.1.4/quickbolt/clients/aio_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/clients/httpx_requests.py` & `quickbolt-0.1.4/quickbolt/clients/httpx_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/logging/async_logger.py` & `quickbolt-0.1.4/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.1.4/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/reporting/response_csv.py` & `quickbolt-0.1.4/quickbolt/reporting/response_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,27 @@
     This reads a csv.
 
     Args:
         csv_path: The path to the csv file. If path is None the default one is found and used.
     Returns:
         data: The rows of a csv file.
     """
+
+    def try_ast_eval(item):
+        try:
+            return ast.literal_eval(item)
+        except:
+            return item
+
     async with aopen(csv_path, encoding="ascii", newline="") as csv_file:
         data = [row async for row in AsyncReader(csv_file)]
 
     return [
         [
-            ast.literal_eval(item)
+            try_ast_eval(item)
             if (
                 not ("MultiDict" in item or "BufferedReader" in item)
                 and ("[" in item or "{" in item)
             )
             else item
             for item in row
         ]
@@ -48,18 +55,20 @@
 
     Returns:
         scrubbed_text: The scrubbed text.
     """
     # need to do better here
     text_dict = jh.deserialize(text)
     flat_scrubbed_text = dh.flatten(text_dict)
+
     for key, value in flat_scrubbed_text.items():
-        if not isinstance(value, str):
+        if isinstance(value, (int, float)):
             val_type = type(value).__name__
-            flat_scrubbed_text[key] = f"{value} ({val_type})"
+            flat_scrubbed_text[key] = f"{value} <{val_type}>"
+
     unflat_scrubbed_text = dh.unflatten(flat_scrubbed_text)
     scrubbed_text = jh.serialize(unflat_scrubbed_text)
 
     targets = re.findall(
         r"([A-Za-z]+[\d@]+[\w@]*|[\d@]+[A-Za-z]+[\w@]*|\d+)", scrubbed_text
     )
     targets.sort(key=len, reverse=True)
```

### Comparing `quickbolt-0.1.3/quickbolt/utils/dictionary.py` & `quickbolt-0.1.4/quickbolt/utils/dictionary.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 
     Returns:
         flat_d: The flattened object.
     """
 
     def recurse(value, parent_key=""):
         if isinstance(value, list):
-            for i, v in enumerate(value):
-                recurse(v, f"{parent_key}.{i}" if parent_key else str(i))
+            if not value:
+                obj[parent_key] = value
+            else:
+                for i, v in enumerate(value):
+                    recurse(v, f"{parent_key}.{i}" if parent_key else str(i))
         elif isinstance(value, dict):
-            for k, v in value.items():
-                recurse(v, f"{parent_key}.{k}" if parent_key else k)
+            if not value:
+                obj[parent_key] = value
+            else:
+                for k, v in value.items():
+                    recurse(v, f"{parent_key}.{k}" if parent_key else k)
         else:
             obj[parent_key] = value
 
     obj = {}
     recurse(d)
     return obj
 
@@ -33,15 +39,14 @@
 
     Args:
         flat_dict: The flat dictionary to unflatten.
 
     Returns:
         unflattened_dict: The unflattened dict.
     """
-    unflattened_dict = {}
 
     def assign(keys, value, d):
         key = keys.pop(0)
         if len(keys) == 0:
             if key.isdigit():
                 while len(d) <= int(key):
                     d.append(None)
@@ -60,14 +65,19 @@
             else:
                 if key in d.keys():
                     assign(keys, value, d[key])
                 else:
                     d[key] = [{}] if keys[0].isdigit() else {}
                     assign(keys, value, d[key])
 
+    if len(flat_dict) == 1 and "" in flat_dict:
+        return flat_dict[""]
+
+    unflattened_dict = {}
+
     for flat_key, value in flat_dict.items():
         keys = flat_key.split(".")
         assign(keys, value, unflattened_dict)
 
     return unflattened_dict
```

### Comparing `quickbolt-0.1.3/quickbolt/utils/directory.py` & `quickbolt-0.1.4/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/utils/json.py` & `quickbolt-0.1.4/quickbolt/utils/json.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/quickbolt/validations/validations.py` & `quickbolt-0.1.4/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.3/PKG-INFO` & `quickbolt-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
```

