# Comparing `tmp/dingtalk-stream-0.6.0.tar.gz` & `tmp/dingtalk-stream-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.6.0.tar", last modified: Fri Jun 30 03:44:34 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.6.1.tar", last modified: Wed Jul  5 07:37:45 2023, max compression
```

## Comparing `dingtalk-stream-0.6.0.tar` & `dingtalk-stream-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.856657 dingtalk-stream-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:44:34.856657 dingtalk-stream-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.344431 dingtalk-stream-0.6.1/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/setup.py
```

### Comparing `dingtalk-stream-0.6.0/LICENSE` & `dingtalk-stream-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/PKG-INFO` & `dingtalk-stream-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.0/README.md` & `dingtalk-stream-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/__init__.py` & `dingtalk-stream-0.6.1/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.6.1/dingtalk_stream/card_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding:utf-8 -*-
 
 """
 这里提供了一些常用的卡片模板及其封装类
 """
 
 from .card_replier import CardReplier, AICardReplier, AICardStatus
+import json
 
 
 class MarkdownCardInstance(CardReplier):
     """
     一款超级通用的markdown卡片
     """
 
@@ -66,15 +67,15 @@
     """
     一款超级通用的AI Markdown卡片
     ai_start --> ai_streaming --> ai_streaming --> ai_finish/ai_fail
     """
 
     def __init__(self, dingtalk_client, incoming_message):
         super(AIMarkdownCardInstance, self).__init__(dingtalk_client, incoming_message)
-        self.card_template_id = "533f959a-8b28-4d29-8856-77a18d3ad3c2.schema"
+        self.card_template_id = "382e4302-551d-4880-bf29-a30acfab2e71.schema"
         self.card_instance_id = None
         self.title = None
         self.logo = None
         self.markdown = ""
         self.inputing_status = False
 
     def set_title_and_logo(self, title: str, logo: str):
@@ -99,56 +100,75 @@
         if self.card_instance_id is None or self.card_instance_id == "":
             self.logger.error('AIMarkdownCardInstance.ai_streaming failed, you should send card first.')
             return
 
         if not self.inputing_status:
             card_data = {
                 "flowStatus": AICardStatus.INPUTING,
-                "messageContent": ""
+                "msgContent": ""
             }
 
             if self.title is not None and self.title != "":
-                card_data["title"] = self.title
+                card_data["msgTitle"] = self.title
 
             if self.logo is not None and self.logo != "":
                 card_data["logo"] = self.logo
 
+            order = [
+                "msgTitle",
+                "msgButtons",
+                "msgImages",
+                "msgTextList",
+                "msgContent"
+            ]
+
+            card_data["sys_full_json_obj"] = json.dumps({"order": order})
+
             self.put_card_data(self.card_instance_id, card_data)
 
             self.inputing_status = True
 
         if append:
             self.markdown = self.markdown + markdown
         else:
             self.markdown = markdown
 
-        self.streaming(self.card_instance_id, "messageContent", self.markdown, append=False, finished=False,
+        self.streaming(self.card_instance_id, "msgContent", self.markdown, append=False, finished=False,
                        failed=False)
 
     def ai_finish(self, markdown: str = ""):
         """
         完成态
         :param markdown:
         :return:
         """
         if self.card_instance_id is None or self.card_instance_id == "":
             self.logger.error('AIMarkdownCardInstance.ai_finish failed, you should send card first.')
             return
 
-        if markdown == "":
+        if markdown == "" or markdown is None:
             markdown = self.markdown
         else:
             self.markdown = markdown
 
+        order = [
+            "msgTitle",
+            "msgButtons",
+            "msgImages",
+            "msgTextList",
+            "msgContent"
+        ]
+
         card_data = {
-            "messageContent": markdown,
+            "msgContent": markdown,
+            "sys_full_json_obj": json.dumps({"order": order})
         }
 
         if self.title is not None and self.title != "":
-            card_data["title"] = self.title
+            card_data["msgTitle"] = self.title
 
         if self.logo is not None and self.logo != "":
             card_data["logo"] = self.logo
 
         self.finish(self.card_instance_id, card_data)
 
     def ai_fail(self):
@@ -160,13 +180,13 @@
         if self.card_instance_id is None or self.card_instance_id == "":
             self.logger.error('AIMarkdownCardInstance.ai_fail failed, you should send card first.')
             return
 
         card_data = {}
 
         if self.title is not None and self.title != "":
-            card_data["title"] = self.title
+            card_data["msgTitle"] = self.title
 
         if self.logo is not None and self.logo != "":
             card_data["logo"] = self.logo
 
         self.fail(self.card_instance_id, card_data)
```

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.6.1/dingtalk_stream/card_replier.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
             "key": content_key,
             "content": content_value,
             "isFull": not append,
             "isFinalize": finished,
             "isError": failed,
         }
 
-        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/card/update/streaming'
+        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/card/streaming'
         try:
             response = requests.put(url,
                                     headers=self.get_request_header(access_token),
                                     json=body)
 
             response.raise_for_status()
         except Exception as e:
```

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.6.1/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.6.1/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.6.1/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.6.1/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.6.1/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.6.1/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.0/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.6.1/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.0/setup.py` & `dingtalk-stream-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.6.0',
+    version='0.6.1',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

