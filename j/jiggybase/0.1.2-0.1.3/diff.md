# Comparing `tmp/jiggybase-0.1.2.tar.gz` & `tmp/jiggybase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.1.2.tar", last modified: Wed Jun 21 05:32:34 2023, max compression
+gzip compressed data, was "jiggybase-0.1.3.tar", last modified: Wed Jul  5 16:51:12 2023, max compression
```

## Comparing `jiggybase-0.1.2.tar` & `jiggybase-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.811447 jiggybase-0.1.2/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.1.2/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-21 05:32:34.810977 jiggybase-0.1.2/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.1.2/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.794914 jiggybase-0.1.2/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.1.2/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.1.2/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     4385 2023-06-10 19:13:08.000000 jiggybase-0.1.2/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)    10188 2023-06-19 05:34:38.000000 jiggybase-0.1.2/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.798816 jiggybase-0.1.2/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1416 2023-06-13 01:56:18.000000 jiggybase-0.1.2/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      310 2023-06-11 03:47:40.000000 jiggybase-0.1.2/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     6851 2023-06-21 04:30:38.000000 jiggybase-0.1.2/jiggybase/examples/confluence_sync.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.1.2/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1392 2023-06-08 03:25:05.000000 jiggybase-0.1.2/jiggybase/examples/qa_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.1.2/jiggybase/examples/upload_email_example.py
--rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.1.2/jiggybase/ijiggy.py
--rw-r--r--   0 wsk        (501) staff       (20)     5887 2023-06-10 18:20:45.000000 jiggybase-0.1.2/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.1.2/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.808858 jiggybase-0.1.2/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.1.2/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.1.2/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.1.2/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.1.2/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.1.2/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     1833 2023-06-04 00:49:56.000000 jiggybase-0.1.2/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.1.2/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.1.2/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 23:09:48.000000 jiggybase-0.1.2/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     4858 2023-06-19 05:14:08.000000 jiggybase-0.1.2/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3411 2023-06-03 23:48:09.000000 jiggybase-0.1.2/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.1.2/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.1.2/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.1.2/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4799 2023-06-05 00:03:48.000000 jiggybase-0.1.2/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.796646 jiggybase-0.1.2/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     1089 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)      109 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      794 2023-06-19 02:49:26.000000 jiggybase-0.1.2/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-21 05:32:34.811577 jiggybase-0.1.2/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.810324 jiggybase-0.1.2/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.1.2/test/test.py
--rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.1.2/test/test_extract_typed_completion.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.058467 jiggybase-0.1.3/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.1.3/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-07-05 16:51:12.057958 jiggybase-0.1.3/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.1.3/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.049612 jiggybase-0.1.3/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.1.3/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.1.3/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4385 2023-06-10 19:13:08.000000 jiggybase-0.1.3/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    11184 2023-07-05 16:23:49.000000 jiggybase-0.1.3/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.052614 jiggybase-0.1.3/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1416 2023-06-13 01:56:18.000000 jiggybase-0.1.3/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      310 2023-06-11 03:47:40.000000 jiggybase-0.1.3/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     6851 2023-06-21 04:30:38.000000 jiggybase-0.1.3/jiggybase/examples/confluence_sync.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.1.3/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1392 2023-06-08 03:25:05.000000 jiggybase-0.1.3/jiggybase/examples/qa_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.1.3/jiggybase/examples/upload_email_example.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.1.3/jiggybase/ijiggy.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5887 2023-06-10 18:20:45.000000 jiggybase-0.1.3/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.1.3/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.056953 jiggybase-0.1.3/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.1.3/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.1.3/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.1.3/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.1.3/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.1.3/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1833 2023-06-04 00:49:56.000000 jiggybase-0.1.3/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.1.3/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.1.3/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 23:09:48.000000 jiggybase-0.1.3/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4858 2023-06-19 05:14:08.000000 jiggybase-0.1.3/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3411 2023-06-03 23:48:09.000000 jiggybase-0.1.3/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.1.3/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.1.3/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.1.3/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4799 2023-06-05 00:03:48.000000 jiggybase-0.1.3/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.051154 jiggybase-0.1.3/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     1089 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      109 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-07-05 16:51:12.000000 jiggybase-0.1.3/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      794 2023-07-05 16:14:13.000000 jiggybase-0.1.3/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-07-05 16:51:12.058643 jiggybase-0.1.3/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-07-05 16:51:12.057572 jiggybase-0.1.3/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.1.3/test/test.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.1.3/test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.1.2/LICENSE` & `jiggybase-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/PKG-INFO` & `jiggybase-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.1.2/README.md` & `jiggybase-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/chat_stream.py` & `jiggybase-0.1.3/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/client.py` & `jiggybase-0.1.3/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/collection.py` & `jiggybase-0.1.3/jiggybase/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional, List, Iterator
+from typing import Optional, List, Iterator, Tuple
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
 from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
 from .models import Message, CompletionRequest, ChatCompletion 
 from .chat_stream import extract_content_from_sse_bytes
@@ -138,14 +138,30 @@
         limit - Number of results to return starting from the offset
         reverse - Reverse the order of the items returned
         """
         params = {"start": start, "limit": limit, "reverse": reverse}
         rsp = self.plugin_session.get("/chunks", params=params)
         return [DocumentChunk.parse_obj(chunk) for chunk in rsp.json()]
 
+    def get_doc_chunks(self, 
+                       index: int = -1, 
+                       limit: int = 10, 
+                       reverse: bool = True,
+                       max_chunks_per_doc = 1) -> Tuple[List[List[DocumentChunk]], int]:
+         """
+         low level interface for iterating through the initial chunks for all docs in a collection
+         index - index of the first result to return, should be -1 to start at the end
+         limit - Number of results to return starting from the offset
+         reverse - Reverse the order of the items returned; True to return newest first
+         max_chunks_per_doc - maximum number of chunks to return for each document
+         """
+         params = {"index": index, "limit": limit, "reverse": reverse, "max_chunks_per_doc": max_chunks_per_doc}
+         rsp = self.plugin_session.get("/doc_chunks", params=params)
+         dcr_rsp = DocChunksResponse.parse_obj(rsp.json())
+         return dcr_rsp.docs, dcr_rsp.next_index
 
     def delete_docs(self, 
                     ids                      : Optional[List[str]] = None, 
                     document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
                     delete_all               : Optional[bool] = False) -> DeleteResponse:
         """
         Delete items in the collection by document id's or document metadata filter.
```

### Comparing `jiggybase-0.1.2/jiggybase/examples/chat_completion.py` & `jiggybase-0.1.3/jiggybase/examples/chat_completion.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/examples/confluence_sync.py` & `jiggybase-0.1.3/jiggybase/examples/confluence_sync.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.1.3/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/examples/qa_example.py` & `jiggybase-0.1.3/jiggybase/examples/qa_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/examples/upload_email_example.py` & `jiggybase-0.1.3/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/ijiggy.py` & `jiggybase-0.1.3/jiggybase/ijiggy.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/jiggybase_session.py` & `jiggybase-0.1.3/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/login.py` & `jiggybase-0.1.3/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/auth.py` & `jiggybase-0.1.3/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/chat.py` & `jiggybase-0.1.3/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/chunk.py` & `jiggybase-0.1.3/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/collection.py` & `jiggybase-0.1.3/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/metadata.py` & `jiggybase-0.1.3/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/org.py` & `jiggybase-0.1.3/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/plugin.py` & `jiggybase-0.1.3/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/plugin_config.py` & `jiggybase-0.1.3/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/prompt.py` & `jiggybase-0.1.3/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/providers.py` & `jiggybase-0.1.3/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/models/user.py` & `jiggybase-0.1.3/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase/org.py` & `jiggybase-0.1.3/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.1.3/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.1.2/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.1.3/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/pyproject.toml` & `jiggybase-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.1.2/test/test.py` & `jiggybase-0.1.3/test/test.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.2/test/test_extract_typed_completion.py` & `jiggybase-0.1.3/test/test_extract_typed_completion.py`

 * *Files identical despite different names*

