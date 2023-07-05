# Comparing `tmp/searchium-0.0.1rc4.tar.gz` & `tmp/searchium-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchium-0.0.1rc4.tar", max compression
+gzip compressed data, was "searchium-0.0.1rc5.tar", max compression
```

## Comparing `searchium-0.0.1rc4.tar` & `searchium-0.0.1rc5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1423 2023-04-19 16:01:41.103149 searchium-0.0.1rc4/README.md
--rw-r--r--   0        0        0      380 2023-05-11 13:26:40.561220 searchium-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0      323 2023-05-11 12:14:21.577402 searchium-0.0.1rc4/searchium/__init__.py
--rw-r--r--   0        0        0       93 2023-04-04 10:24:52.278850 searchium-0.0.1rc4/searchium/client/__init__.py
--rw-r--r--   0        0        0     6395 2023-05-11 11:27:09.343472 searchium-0.0.1rc4/searchium/client/func.py
--rw-r--r--   0        0        0     1176 2023-04-18 14:33:48.839524 searchium-0.0.1rc4/searchium/client/init.py
--rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc4/searchium/fvs/__init__.py
--rw-r--r--   0        0        0     5331 2023-04-03 12:04:06.397449 searchium-0.0.1rc4/searchium/fvs/client.py
--rw-r--r--   0        0        0     1989 2023-05-11 11:18:52.346561 searchium-0.0.1rc4/searchium/fvs/model.py
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 searchium-0.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0     1423 2023-04-19 16:01:41.103149 searchium-0.0.1rc5/README.md
+-rw-r--r--   0        0        0      398 2023-07-05 08:41:11.102216 searchium-0.0.1rc5/pyproject.toml
+-rw-r--r--   0        0        0      329 2023-07-05 08:40:43.705829 searchium-0.0.1rc5/searchium/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-04 10:24:52.278850 searchium-0.0.1rc5/searchium/client/__init__.py
+-rw-r--r--   0        0        0     6395 2023-07-05 08:40:43.729829 searchium-0.0.1rc5/searchium/client/func.py
+-rw-r--r--   0        0        0     1176 2023-04-18 14:33:48.839524 searchium-0.0.1rc5/searchium/client/init.py
+-rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc5/searchium/fvs/__init__.py
+-rw-r--r--   0        0        0     5331 2023-04-03 12:04:06.397449 searchium-0.0.1rc5/searchium/fvs/client.py
+-rw-r--r--   0        0        0     2041 2023-07-05 12:12:59.668153 searchium-0.0.1rc5/searchium/fvs/model.py
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 searchium-0.0.1rc5/PKG-INFO
```

### Comparing `searchium-0.0.1rc4/README.md` & `searchium-0.0.1rc5/README.md`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc4/searchium/client/func.py` & `searchium-0.0.1rc5/searchium/client/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,16 @@
     if get.status_code == 200:
         obj_as = parse_obj_as(Response, get.json())
         return obj_as
     else:
         raise Exception(get.json())
 
 
-def train_status(dataset_id: str) -> TrainStatus:
-    link = f"{Config.link}/dataset/train/status/{dataset_id}"
+def get_dataset_status(dataset_id: str) -> TrainStatus:
+    link = f"{Config.link}/dataset/status/{dataset_id}"
     get = requests.get(link, headers=Config.headers)
     if get.status_code == 200:
         obj_as = parse_obj_as(TrainStatus, get.json())
         return obj_as
     else:
         raise Exception(get.json())
```

### Comparing `searchium-0.0.1rc4/searchium/client/init.py` & `searchium-0.0.1rc5/searchium/client/init.py`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc4/searchium/fvs/client.py` & `searchium-0.0.1rc5/searchium/fvs/client.py`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc4/searchium/fvs/model.py` & `searchium-0.0.1rc5/searchium/fvs/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 class Document(BaseModel):
     document_id: str = None
     vector: List[float] = None
     metadata: Optional[List[dict]] = None
 
 
 class DatasetStatus(str, Enum):
-    completed = 'completed'
-    training = 'training'
-    error = 'error'
-    loaded = 'loaded'
-    pending = 'pending'
+    COMPLETED = 'completed'
+    TRAINING = 'training'
+    ERROR = 'error'
+    LOADED = 'loaded'
+    PENDING = 'pending'
+    ADDING = 'adding'
+    NOT_LOADED = 'not_loaded'
 
 
 class TrainStatus(BaseModel):
     datasetStatus: DatasetStatus
 
 
 class Response(BaseModel):
```

### Comparing `searchium-0.0.1rc4/PKG-INFO` & `searchium-0.0.1rc5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: searchium
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: 
 Author: GSI Technology, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Clients of Searchium cloud platform
 #### FVS - is fast vector search
 ##### get more info https://www.searchium.ai/
```

