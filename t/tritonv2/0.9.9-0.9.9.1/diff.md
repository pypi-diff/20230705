# Comparing `tmp/tritonv2-0.9.9.tar.gz` & `tmp/tritonv2-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.9.tar", last modified: Tue Jul  4 18:10:41 2023, max compression
+gzip compressed data, was "tritonv2-0.9.9.1.tar", last modified: Wed Jul  5 10:19:23 2023, max compression
```

## Comparing `tritonv2-0.9.9.tar` & `tritonv2-0.9.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 18:10:41.298120 tritonv2-0.9.9/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-07-04 18:10:41.298215 tritonv2-0.9.9/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-07-04 18:10:40.000000 tritonv2-0.9.9/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      770 2023-07-04 18:10:41.298663 tritonv2-0.9.9/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-04 18:10:40.000000 tritonv2-0.9.9/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 18:10:41.296856 tritonv2-0.9.9/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.9/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.9/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.9/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/grpc_interceptor.py
--rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.9/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     7704 2023-07-04 18:07:20.000000 tritonv2-0.9.9/tritonv2/model.py
--rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-04 11:53:35.000000 tritonv2-0.9.9/tritonv2/model_config.py
--rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.9/tritonv2/module.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.9/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.9/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 18:10:41.297861 tritonv2-0.9.9/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-04 18:10:41.000000 tritonv2-0.9.9/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:19:23.323968 tritonv2-0.9.9.1/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-05 10:19:23.324058 tritonv2-0.9.9.1/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-05 10:19:22.000000 tritonv2-0.9.9.1/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-05 10:19:23.324488 tritonv2-0.9.9.1/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-05 10:19:22.000000 tritonv2-0.9.9.1/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:19:23.323047 tritonv2-0.9.9.1/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.9.1/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.9.1/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.9.1/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.9.1/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7590 2023-07-05 10:18:58.000000 tritonv2-0.9.9.1/tritonv2/model.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-04 11:53:35.000000 tritonv2-0.9.9.1/tritonv2/model_config.py
+-rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.9.1/tritonv2/module.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.9.1/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.9.1/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:19:23.323819 tritonv2-0.9.9.1/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-05 10:19:23.000000 tritonv2-0.9.9.1/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.9/PKG-INFO` & `tritonv2-0.9.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9
+pip install tritonv2==0.9.9.1
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9/README.md` & `tritonv2-0.9.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9
+pip install tritonv2==0.9.9.1
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9/setup.cfg` & `tritonv2-0.9.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.9
+version = 0.9.9.1
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

### Comparing `tritonv2-0.9.9/tritonv2/client.py` & `tritonv2-0.9.9.1/tritonv2/client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/client_factory.py` & `tritonv2-0.9.9.1/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/constants.py` & `tritonv2-0.9.9.1/tritonv2/constants.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.9.1/tritonv2/grpc_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/grpc_client.py` & `tritonv2-0.9.9.1/tritonv2/grpc_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/grpc_interceptor.py` & `tritonv2-0.9.9.1/tritonv2/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/http_aio_client.py` & `tritonv2-0.9.9.1/tritonv2/http_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/http_client.py` & `tritonv2-0.9.9.1/tritonv2/http_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/model.py` & `tritonv2-0.9.9.1/tritonv2/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 # Copyright (c) 2022 Baidu.com, Inc. All Rights Reserved
 """
 Model For Triton
 """
 import os
 import json
 import base64
-import shutil
-from typing import Any, Optional,List
+from typing import Any, Optional, List
 
 from .module import CustomModule
 from .client_factory import TritonClientFactory
 from .constants import BENCHMARK_TASK, TESTING_TASK
 
 try:
     from tritonclient.http import _get_inference_request
 except ImportError:
     from tritonclient.http._utils import _get_inference_request
 
+
 class Model(object):
     """
     Model Class
     Args:
         object (_type_): _description_
     """
-    def __init__(self, 
-                 custom_module_class: Optional[CustomModule], 
+
+    def __init__(self,
+                 custom_module_class: Optional[CustomModule],
                  input_file_path: str,
                  server_url: str,
                  kind: str,
                  model_name: str = 'ensemble',
                  model_version: str = '1',
                  **kwargs) -> None:
         """
@@ -44,37 +45,37 @@
             model_version (str, optional): Defaults to '1'.
             output_file_path (str, optional): Defaults to './request.json'.
         """
         self.input_file_path = str(input_file_path)
         self.model_name = str(model_name)
         self.server_url = str(server_url)
         self.model_version = str(model_version)
-        
-        assert kind in [BENCHMARK_TASK, TESTING_TASK], "kind must be one of benchmark or testing"
+
+        assert kind in [BENCHMARK_TASK,
+                        TESTING_TASK], "kind must be one of benchmark or testing"
         self.kind = kind
         if self.kind == BENCHMARK_TASK:
             self.output_file_path = './request.json'
         elif self.kind == TESTING_TASK:
             self.output_file_path = './result/'
             if not os.path.exists(self.output_file_path):
                 os.makedirs(self.output_file_path)
-                
-        self.client = TritonClientFactory.create_http_client(server_url=self.server_url)
+
+        self.client = TritonClientFactory.create_http_client(
+            server_url=self.server_url)
         self.input_metadata, self.output_metadata, self.batch_size = self.client.get_inputs_and_outputs_detail(
             model_name=self.model_name, model_version=self.model_version)
-        
+
         self.input_file_path_list = self.get_input_file_path_list()
-        
+
         self.custom_module_instance = custom_module_class(
             input_metadata=self.input_metadata,
             output_metadata=self.output_metadata,
             **kwargs)
-        
-        
-    
+
     def get_input_file_path_list(self) -> List[str]:
         """
         Scan input file path
         Returns:
             List[str]: path list
         """
         file_extensions = {'.jpeg', '.png', '.jpg'}
@@ -89,108 +90,111 @@
             _, ext = os.path.splitext(self.input_file_path)
             if ext.lower() in file_extensions:
                 file_paths.append(self.input_file_path)
         else:
             return file_paths
 
         return file_paths
-    
+
     def save_benchmark_request(self, model_inputs, model_outputs):
         """
         Save perf analysis input data json file
         Args:
             model_inputs (_type_): triton model inputs
             model_outputs (_type_): triton model outputs
 
         Returns:
             _type_: _description_
         """
         request_body_list = []
         for k, v in enumerate(model_inputs):
             request_body, json_size = _get_inference_request(inputs=v,
-                                                            outputs=model_outputs[k],
-                                                            request_id=str(k),
-                                                            sequence_id=None,
-                                                            sequence_start=None,
-                                                            sequence_end=None,
-                                                            priority=None,
-                                                            timeout=None,
-                                                            custom_parameters=None)
+                                                             outputs=model_outputs[k],
+                                                             request_id=str(k),
+                                                             sequence_id=None,
+                                                             sequence_start=None,
+                                                             sequence_end=None,
+                                                             priority=None,
+                                                             timeout=None,
+                                                             custom_parameters=None)
             if json_size is not None:
                 return self._save_binary_benchmark_request(model_inputs)
 
             request_body_list.append(request_body)
-            
+
         result = {'data': []}
-        
+
         for k, body in enumerate(request_body_list):
             infer_req = json.loads(body)
             single_input = {}
             for i in range(len(infer_req['inputs'])):
                 shape = infer_req['inputs'][i]['shape']
                 if self.batch_size > 0:
                     shape.pop(0)
                 single_input[infer_req['inputs'][i]['name']] = {
                     'shape': shape,
                     'content': infer_req['inputs'][i]['data']
                 }
-                
+
             result['data'].append(single_input)
-        
+
         perf_req = json.dumps(result)
         with open(self.output_file_path, 'w') as f:
             f.write(perf_req)
-            
+
     def save_testing_result(self, model_inputs, model_outputs):
         """
         Save inference result json file
         Args:
             model_inputs (_type_): _description_
             model_outputs (_type_): _description_
         """
         for k, model_input in enumerate(model_inputs):
             model_output = model_outputs[k]
-            response = self.client.model_infer(model_name=self.model_name, model_version=self.model_version, inputs=model_input, outputs=model_output)
+            response = self.client.model_infer(
+                model_name=self.model_name,
+                model_version=self.model_version,
+                inputs=model_input, outputs=model_output)
             response_str = self.custom_module_instance.postprocess(response)
-            result_file_path = os.path.join(self.output_file_path, os.path.basename(self.input_file_path_list[k]).split('.')[0] + '.json')
+            result_file_path = os.path.join(
+                self.output_file_path, self.input_file_path_list[k] + '.json')
             with open(result_file_path, 'w') as f:
                 f.write(response_str)
-            
+
     def _save_binary_benchmark_request(self, model_inputs):
         """
         Save binary perf analysis input data json file
         Args:
             model_inputs (_type_): _description_
         """
         result = {'data': []}
-        
+
         for k, v in enumerate(model_inputs):
             single_input = {}
             for i in v:
-                shape = i.shape() 
+                shape = i.shape()
                 if self.batch_size > 0:
                     shape.pop(0)
                 single_input[i.name()] = {
-                    'content': {'b64': base64.b64encode(i._get_binary_data()).decode('utf-8')}, 
+                    'content': {'b64': base64.b64encode(i._get_binary_data()).decode('utf-8')},
                     'shape': shape,
                 }
             result['data'].append(single_input)
-        
+
         perf_req = json.dumps(result)
         with open(self.output_file_path, 'w') as f:
             f.write(perf_req)
-    
+
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         model_inputs = []
         model_outputs = []
-        
+
         for input_path in self.input_file_path_list:
             model_input = self.custom_module_instance.prepare_input(input_path)
             model_inputs.append(model_input)
             model_output = self.custom_module_instance.prepare_output()
             model_outputs.append(model_output)
-        
+
         if self.kind == BENCHMARK_TASK:
             self.save_benchmark_request(model_inputs, model_outputs)
         elif self.kind == TESTING_TASK:
             self.save_testing_result(model_inputs, model_outputs)
-
```

### Comparing `tritonv2-0.9.9/tritonv2/model_config.py` & `tritonv2-0.9.9.1/tritonv2/model_config.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/module.py` & `tritonv2-0.9.9.1/tritonv2/module.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2/utils.py` & `tritonv2-0.9.9.1/tritonv2/utils.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.9.1/tritonv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9
+pip install tritonv2==0.9.9.1
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9/tritonv2.egg-info/SOURCES.txt` & `tritonv2-0.9.9.1/tritonv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

