# Comparing `tmp/havenpy-0.0.5.tar.gz` & `tmp/havenpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "havenpy-0.0.5.tar", last modified: Sun Jul  2 23:02:11 2023, max compression
+gzip compressed data, was "havenpy-0.0.6.tar", last modified: Wed Jul  5 19:30:02 2023, max compression
```

## Comparing `havenpy-0.0.5.tar` & `havenpy-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.553473 havenpy-0.0.5/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-02 23:02:11.553354 havenpy-0.0.5/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-30 05:08:05.000000 havenpy-0.0.5/README.md
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.551757 havenpy-0.0.5/havenpy/
--rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-30 05:08:05.000000 havenpy-0.0.5/havenpy/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-30 05:08:05.000000 havenpy-0.0.5/havenpy/interceptor.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.553065 havenpy-0.0.5/havenpy/pb/
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-07-02 03:44:58.000000 havenpy-0.0.5/havenpy/pb/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     4535 2023-07-02 06:06:39.000000 havenpy-0.0.5/havenpy/pb/manager_pb2.py
--rw-r--r--   0 konsti     (501) staff       (20)    13059 2023-07-02 03:44:58.000000 havenpy-0.0.5/havenpy/pb/manager_pb2_grpc.py
--rw-r--r--   0 konsti     (501) staff       (20)     2474 2023-07-02 22:41:14.000000 havenpy-0.0.5/havenpy/run.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-02 23:02:11.552472 havenpy-0.0.5/havenpy.egg-info/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)      310 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/SOURCES.txt
--rw-r--r--   0 konsti     (501) staff       (20)        1 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/dependency_links.txt
--rw-r--r--   0 konsti     (501) staff       (20)       32 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/requires.txt
--rw-r--r--   0 konsti     (501) staff       (20)        8 2023-07-02 23:02:11.000000 havenpy-0.0.5/havenpy.egg-info/top_level.txt
--rw-r--r--   0 konsti     (501) staff       (20)       38 2023-07-02 23:02:11.553514 havenpy-0.0.5/setup.cfg
--rw-r--r--   0 konsti     (501) staff       (20)      314 2023-07-02 23:02:07.000000 havenpy-0.0.5/setup.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 19:30:02.356411 havenpy-0.0.6/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-05 19:30:02.356296 havenpy-0.0.6/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-30 05:08:05.000000 havenpy-0.0.6/README.md
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 19:30:02.354932 havenpy-0.0.6/havenpy/
+-rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-30 05:08:05.000000 havenpy-0.0.6/havenpy/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-30 05:08:05.000000 havenpy-0.0.6/havenpy/interceptor.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 19:30:02.356090 havenpy-0.0.6/havenpy/pb/
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-07-04 05:30:32.000000 havenpy-0.0.6/havenpy/pb/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     4787 2023-07-05 19:02:13.000000 havenpy-0.0.6/havenpy/pb/manager_pb2.py
+-rw-r--r--   0 konsti     (501) staff       (20)    13083 2023-07-05 19:02:13.000000 havenpy-0.0.6/havenpy/pb/manager_pb2_grpc.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2614 2023-07-05 19:02:13.000000 havenpy-0.0.6/havenpy/run.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 19:30:02.355652 havenpy-0.0.6/havenpy.egg-info/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-05 19:30:02.000000 havenpy-0.0.6/havenpy.egg-info/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)      310 2023-07-05 19:30:02.000000 havenpy-0.0.6/havenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        1 2023-07-05 19:30:02.000000 havenpy-0.0.6/havenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       32 2023-07-05 19:30:02.000000 havenpy-0.0.6/havenpy.egg-info/requires.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        8 2023-07-05 19:30:02.000000 havenpy-0.0.6/havenpy.egg-info/top_level.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       38 2023-07-05 19:30:02.356447 havenpy-0.0.6/setup.cfg
+-rw-r--r--   0 konsti     (501) staff       (20)      314 2023-07-05 19:29:57.000000 havenpy-0.0.6/setup.py
```

### Comparing `havenpy-0.0.5/havenpy/interceptor.py` & `havenpy-0.0.6/havenpy/interceptor.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.5/havenpy/pb/manager_pb2.py` & `havenpy-0.0.6/havenpy/pb/manager_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,45 +9,47 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"\xdc\x01\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"&\n\x16\x43hatCompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xcc\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_count\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*<\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xb4\x04\n\x05Haven\x12,\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x0c.haven.Empty\"\x00\x12Q\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x1d.haven.ChatCompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"1\n\rSetupResponse\x12\x14\n\x07message\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_message\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"\xdc\x01\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"&\n\x16\x43hatCompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xe8\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12\x11\n\x04zone\x18\x07 \x01(\tH\x03\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_countB\x07\n\x05_zone\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*<\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xbc\x04\n\x05Haven\x12\x34\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x14.haven.SetupResponse\"\x00\x12Q\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x1d.haven.ChatCompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'manager_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ROLE._serialized_start=842
-  _ROLE._serialized_end=873
-  _STATUS._serialized_start=875
-  _STATUS._serialized_end=935
-  _GPUTYPE._serialized_start=937
-  _GPUTYPE._serialized_end=979
+  _ROLE._serialized_start=921
+  _ROLE._serialized_end=952
+  _STATUS._serialized_start=954
+  _STATUS._serialized_end=1014
+  _GPUTYPE._serialized_start=1016
+  _GPUTYPE._serialized_end=1058
   _EMPTY._serialized_start=24
   _EMPTY._serialized_end=31
   _SETUPREQUEST._serialized_start=33
   _SETUPREQUEST._serialized_end=83
-  _MESSAGE._serialized_start=85
-  _MESSAGE._serialized_end=138
-  _CHATCOMPLETIONREQUEST._serialized_start=141
-  _CHATCOMPLETIONREQUEST._serialized_end=361
-  _CHATCOMPLETIONRESPONSE._serialized_start=363
-  _CHATCOMPLETIONRESPONSE._serialized_end=401
-  _MODEL._serialized_start=403
-  _MODEL._serialized_end=424
-  _LISTMODELSRESPONSE._serialized_start=426
-  _LISTMODELSRESPONSE._serialized_end=476
-  _WORKER._serialized_start=478
-  _WORKER._serialized_end=538
-  _LISTWORKERSRESPONSE._serialized_start=540
-  _LISTWORKERSRESPONSE._serialized_end=593
-  _CREATEINFERENCEWORKERREQUEST._serialized_start=596
-  _CREATEINFERENCEWORKERREQUEST._serialized_end=800
-  _INFERENCEWORKER._serialized_start=802
-  _INFERENCEWORKER._serialized_end=840
-  _HAVEN._serialized_start=982
-  _HAVEN._serialized_end=1546
+  _SETUPRESPONSE._serialized_start=85
+  _SETUPRESPONSE._serialized_end=134
+  _MESSAGE._serialized_start=136
+  _MESSAGE._serialized_end=189
+  _CHATCOMPLETIONREQUEST._serialized_start=192
+  _CHATCOMPLETIONREQUEST._serialized_end=412
+  _CHATCOMPLETIONRESPONSE._serialized_start=414
+  _CHATCOMPLETIONRESPONSE._serialized_end=452
+  _MODEL._serialized_start=454
+  _MODEL._serialized_end=475
+  _LISTMODELSRESPONSE._serialized_start=477
+  _LISTMODELSRESPONSE._serialized_end=527
+  _WORKER._serialized_start=529
+  _WORKER._serialized_end=589
+  _LISTWORKERSRESPONSE._serialized_start=591
+  _LISTWORKERSRESPONSE._serialized_end=644
+  _CREATEINFERENCEWORKERREQUEST._serialized_start=647
+  _CREATEINFERENCEWORKERREQUEST._serialized_end=879
+  _INFERENCEWORKER._serialized_start=881
+  _INFERENCEWORKER._serialized_end=919
+  _HAVEN._serialized_start=1061
+  _HAVEN._serialized_end=1633
 # @@protoc_insertion_point(module_scope)
```

### Comparing `havenpy-0.0.5/havenpy/pb/manager_pb2_grpc.py` & `havenpy-0.0.6/havenpy/pb/manager_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         Args:
             channel: A grpc.Channel.
         """
         self.Setup = channel.unary_unary(
                 '/haven.Haven/Setup',
                 request_serializer=manager__pb2.SetupRequest.SerializeToString,
-                response_deserializer=manager__pb2.Empty.FromString,
+                response_deserializer=manager__pb2.SetupResponse.FromString,
                 )
         self.ChatCompletion = channel.unary_stream(
                 '/haven.Haven/ChatCompletion',
                 request_serializer=manager__pb2.ChatCompletionRequest.SerializeToString,
                 response_deserializer=manager__pb2.ChatCompletionResponse.FromString,
                 )
         self.ListModels = channel.unary_unary(
@@ -114,15 +114,15 @@
 
 
 def add_HavenServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Setup': grpc.unary_unary_rpc_method_handler(
                     servicer.Setup,
                     request_deserializer=manager__pb2.SetupRequest.FromString,
-                    response_serializer=manager__pb2.Empty.SerializeToString,
+                    response_serializer=manager__pb2.SetupResponse.SerializeToString,
             ),
             'ChatCompletion': grpc.unary_stream_rpc_method_handler(
                     servicer.ChatCompletion,
                     request_deserializer=manager__pb2.ChatCompletionRequest.FromString,
                     response_serializer=manager__pb2.ChatCompletionResponse.SerializeToString,
             ),
             'ListModels': grpc.unary_unary_rpc_method_handler(
@@ -174,15 +174,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/haven.Haven/Setup',
             manager__pb2.SetupRequest.SerializeToString,
-            manager__pb2.Empty.FromString,
+            manager__pb2.SetupResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ChatCompletion(request,
             target,
             options=(),
```

### Comparing `havenpy-0.0.5/havenpy/run.py` & `havenpy-0.0.6/havenpy/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 
 	def __init__(self, url: str, token: str):
 		channel = grpc.insecure_channel(url)
 		interceptor = add_header('authorization', f'Bearer {token}')
 		channel = grpc.intercept_channel(channel, interceptor)
 		self.client = manager_pb2_grpc.HavenStub(channel)
 
-	def setup(self, key_file: str) -> manager_pb2.Empty:
+		self.setup()
+
+	def setup(self, key_file: str = None) -> None:
 		request = manager_pb2.SetupRequest(key_file=key_file)
-		return self.client.Setup(request)
+		response: manager_pb2.SetupResponse = self.client.Setup(request)
+
+		if hasattr(response, "message"):
+			print(response.message)
 
 	def chat_completion(self, worker_name: str, messages: List[manager_pb2.Message], stream: bool = False, max_tokens: int = -1, top_p: float = -1, top_k: int = -1, temperature: float = -1) -> manager_pb2.ChatCompletionResponse or str:
 		request = manager_pb2.ChatCompletionRequest(worker_name=worker_name, messages=messages, max_tokens=max_tokens, top_p=top_p, top_k=top_k, temperature=temperature)
 		responseStream: manager_pb2.ChatCompletionResponse = self.client.ChatCompletion(request)
 
 		if stream:
 			return responseStream
@@ -35,16 +40,16 @@
 		request = manager_pb2.Empty()
 		return self.client.ListModels(request)
 	
 	def list_workers(self) -> manager_pb2.ListWorkersResponse:
 		request = manager_pb2.Empty()
 		return self.client.ListWorkers(request)
 	
-	def create_inference_worker(self, model_name: str, quantization: str, worker_name:str=None, gpu_type: manager_pb2.GpuType=None, gpu_count: int=None) -> manager_pb2.InferenceWorker:
-		request = manager_pb2.CreateInferenceWorkerRequest(model_name=model_name, quantization=quantization, worker_name=worker_name, gpu_type=gpu_type, gpu_count=gpu_count)
+	def create_inference_worker(self, model_name: str, quantization: str, worker_name: str = None, gpu_type: manager_pb2.GpuType = None, gpu_count: int = None, zone: str = None) -> manager_pb2.InferenceWorker:
+		request = manager_pb2.CreateInferenceWorkerRequest(model_name=model_name, quantization=quantization, worker_name=worker_name, gpu_type=gpu_type, gpu_count=gpu_count, zone=zone)
 		return self.client.CreateInferenceWorker(request)
 	
 	def pause_inference_worker(self, worker_name: str) -> manager_pb2.InferenceWorker:
 		request = manager_pb2.InferenceWorker(worker_name=worker_name)
 		return self.client.PauseInferenceWorker(request)
 	
 	def resume_inference_worker(self, worker_name: str) -> manager_pb2.InferenceWorker:
```

