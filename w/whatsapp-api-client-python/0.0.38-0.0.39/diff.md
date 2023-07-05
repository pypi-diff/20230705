# Comparing `tmp/whatsapp-api-client-python-0.0.38.tar.gz` & `tmp/whatsapp-api-client-python-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-client-python-0.0.38.tar", last modified: Mon Jul  3 08:55:20 2023, max compression
+gzip compressed data, was "whatsapp-api-client-python-0.0.39.tar", last modified: Wed Jul  5 15:42:59 2023, max compression
```

## Comparing `whatsapp-api-client-python-0.0.38.tar` & `whatsapp-api-client-python-0.0.39.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:55:20.009895 whatsapp-api-client-python-0.0.38/
--rw-rw-rw-   0        0        0    18132 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/LICENSE
--rw-rw-rw-   0        0        0    21313 2023-07-03 08:55:20.009895 whatsapp-api-client-python-0.0.38/PKG-INFO
--rw-rw-rw-   0        0        0    20328 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 08:55:20.010898 whatsapp-api-client-python-0.0.38/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.992850 whatsapp-api-client-python-0.0.38/tests/
--rw-rw-rw-   0        0        0     3965 2023-07-03 08:51:05.000000 whatsapp-api-client-python-0.0.38/tests/test_methods.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.995859 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/
--rw-rw-rw-   0        0        0     2058 2023-07-03 08:41:02.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/API.py
--rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/__init__.py
--rw-rw-rw-   0        0        0      363 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/response.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:55:20.008892 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/
--rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-07-01 10:03:15.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/account.py
--rw-rw-rw-   0        0        0      595 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/device.py
--rw-rw-rw-   0        0        0     4518 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/groups.py
--rw-rw-rw-   0        0        0     2174 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/journals.py
--rw-rw-rw-   0        0        0      743 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/marking.py
--rw-rw-rw-   0        0        0      928 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/queues.py
--rw-rw-rw-   0        0        0     1238 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/receiving.py
--rw-rw-rw-   0        0        0     8002 2023-07-03 08:50:13.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/sending.py
--rw-rw-rw-   0        0        0     3599 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/serviceMethods.py
--rw-rw-rw-   0        0        0     2640 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/webhooks.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.999868 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/
--rw-rw-rw-   0        0        0    21313 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      902 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.751853 whatsapp-api-client-python-0.0.39/
+-rw-rw-rw-   0        0        0    18132 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/LICENSE
+-rw-rw-rw-   0        0        0    21777 2023-07-05 15:42:59.750849 whatsapp-api-client-python-0.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0    20328 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 15:42:59.751853 whatsapp-api-client-python-0.0.39/setup.cfg
+-rw-rw-rw-   0        0        0     1802 2023-07-05 15:41:59.000000 whatsapp-api-client-python-0.0.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.735968 whatsapp-api-client-python-0.0.39/tests/
+-rw-rw-rw-   0        0        0     4261 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/tests/test_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.737973 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/
+-rw-rw-rw-   0        0        0     2211 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/API.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/__init__.py
+-rw-rw-rw-   0        0        0      363 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/response.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.749847 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-07-01 10:03:15.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/account.py
+-rw-rw-rw-   0        0        0      595 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/device.py
+-rw-rw-rw-   0        0        0     4518 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/groups.py
+-rw-rw-rw-   0        0        0     2134 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/journals.py
+-rw-rw-rw-   0        0        0      763 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/marking.py
+-rw-rw-rw-   0        0        0      928 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/queues.py
+-rw-rw-rw-   0        0        0     1437 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/receiving.py
+-rw-rw-rw-   0        0        0     8004 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/sending.py
+-rw-rw-rw-   0        0        0     3599 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/serviceMethods.py
+-rw-rw-rw-   0        0        0     2676 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.741829 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/
+-rw-rw-rw-   0        0        0    21777 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      902 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-client-python-0.0.38/LICENSE` & `whatsapp-api-client-python-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/PKG-INFO` & `whatsapp-api-client-python-0.0.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.38
+Version: 0.0.39
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# whatsapp-api-client-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
```

### Comparing `whatsapp-api-client-python-0.0.38/README.md` & `whatsapp-api-client-python-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/setup.py` & `whatsapp-api-client-python-0.0.39/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-client-python",
-    version="0.0.38",
+    version="0.0.39",
     description=(
         "This library helps you easily create"
         " a Python application with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -17,21 +17,31 @@
     url="https://github.com/green-api/whatsapp-api-client-python",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
+        "Natural Language :: English",
+        "Natural Language :: Russian",
         "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Communications",
+        "Topic :: Communications :: Chat",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
     install_requires=["requests==2.31.0"],
-    python_requires=">=3.8"
+    python_requires=">=3.7"
 )
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/API.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/API.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,27 @@
     serviceMethods,
     webhooks
 )
 
 
 class GreenApi:
     host: str
+    media: str
     idInstance: str
     apiTokenInstance: str
 
     def __init__(
             self,
             idInstance: str,
             apiTokenInstance: str,
-            host: str = "https://api.green-api.com"
+            host: str = "https://api.green-api.com",
+            media: str = "https://media.green-api.com"
     ):
         self.host = host
+        self.media = media
         self.idInstance = idInstance
         self.apiTokenInstance = apiTokenInstance
 
         self.account = account.Account(self)
         self.device = device.Device(self)
         self.groups = groups.Groups(self)
         self.journals = journals.Journals(self)
@@ -47,14 +50,15 @@
             self,
             method: str,
             url: str,
             payload: Optional[dict] = None,
             files: Optional[dict] = None
     ) -> Response:
         url = url.replace("{{host}}", self.host)
+        url = url.replace("{{media}}", self.media)
         url = url.replace("{{idInstance}}", self.idInstance)
         url = url.replace("{{apiTokenInstance}}", self.apiTokenInstance)
 
         try:
             with Session() as session:
                 if not files:
                     response = session.request(
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/account.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/account.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/device.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/device.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/groups.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/groups.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/journals.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/journals.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "getMessage/{{apiTokenInstance}}"
             ), request_body
         )
 
-    def lastIncomingMessages(
-            self, minutes: Optional[int] = None
-    ) -> Response:
+    def lastIncomingMessages(self, minutes: Optional[int] = None) -> Response:
         """
         The method returns the last incoming messages of the account.
         """
 
         request_body = None
         if minutes is not None:
             request_body = {"minutes": minutes}
@@ -54,17 +52,15 @@
         return self.api.request(
             "GET", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "lastIncomingMessages/{{apiTokenInstance}}"
             ), request_body
         )
 
-    def lastOutgoingMessages(
-            self, minutes: Optional[int] = None
-    ) -> Response:
+    def lastOutgoingMessages(self, minutes: Optional[int] = None) -> Response:
         """
         The method returns the last outgoing messages of the account.
         """
 
         request_body = None
         if minutes is not None:
             request_body = {"minutes": minutes}
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/marking.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/marking.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 class Marking:
     def __init__(self, api: "GreenApi"):
         self.api = api
 
     def readChat(
             self, chatId: str, idMessage: Optional[str] = None
     ) -> Response:
-        """The method is aimed for marking messages in a chat as read."""
+        """
+        The method is aimed for marking messages in a chat as read.
+        """
 
         request_body = locals()
         if idMessage is None:
             request_body.pop("idMessage")
         request_body.pop("self")
 
         return self.api.request(
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/queues.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/queues.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/receiving.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/receiving.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,25 +20,30 @@
             "GET", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "receiveNotification/{{apiTokenInstance}}"
             )
         )
 
     def deleteNotification(self, receiptId: int) -> Response:
-        """"""
+        """
+        The method is aimed for deleting an incoming notification from
+        the notification queue.
+        """
 
         url = (
             "{{host}}/waInstance{{idInstance}}/"
             "deleteNotification/{{apiTokenInstance}}"
         )
 
         return self.api.request("DELETE", f"{url}/{receiptId}")
 
     def downloadFile(self, chatId: str, idMessage: str) -> Response:
-        """"""
+        """
+        The method is aimed for downloading incoming and outgoing files.
+        """
 
         request_body = locals()
         request_body.pop("self")
 
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/sending.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/sending.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
         files = {"file": (file_name, open(path, "rb"), content_type)}
 
         request_body.pop("path")
 
         return self.api.request(
             "POST", (
-                "{{host}}/waInstance{{idInstance}}/"
+                "{{media}}/waInstance{{idInstance}}/"
                 "sendFileByUpload/{{apiTokenInstance}}"
             ), request_body, files
         )
 
     def sendFileByUrl(
             self,
             chatId: str,
@@ -163,15 +163,15 @@
         file_name = pathlib.Path(path).name
         content_type = mimetypes.guess_type(file_name)[0]
 
         files = {"file": (file_name, open(path, "rb"), content_type)}
 
         return self.api.request(
             "POST", (
-                "{{host}}/waInstance{{idInstance}}/"
+                "{{media}}/waInstance{{idInstance}}/"
                 "uploadFile/{{apiTokenInstance}}"
             ), files=files
         )
 
     def sendLocation(
             self,
             chatId: str,
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/serviceMethods.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/serviceMethods.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/webhooks.py` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/webhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Webhooks:
     _running: Optional[bool] = None
 
     def __init__(self, api: "GreenApi"):
         self.api = api
 
     @property
-    def started(self) -> bool:
+    def started(self) -> Optional[bool]:
         return self._running
 
     @started.setter
     def started(self, value: bool) -> None:
         self._running = value
 
     def startReceivingNotifications(
@@ -31,15 +31,15 @@
 
     def stopReceivingNotifications(self) -> None:
         self._running = False
 
     def job(self, onEvent: Callable[[str, dict], Any]) -> None:
         """Deprecated"""
 
-        logger.log(logging.WARNING, "Deprecated")
+        logger.log(logging.WARNING, "This function is deprecated.")
 
         print((
             "Started receiving incoming notifications."
             " To stop the process, press Ctrl + C."
         ))
 
         while self.started:
@@ -59,15 +59,15 @@
                         response["receiptId"]
                     )
             except KeyboardInterrupt:
                 break
 
         print("Stopped receiving incoming notifications.")
 
-    def _start_polling(self, handler: Callable[[str, dict], Any]):
+    def _start_polling(self, handler: Callable[[str, dict], Any]) -> None:
         logger.log(logging.INFO, "Started receiving incoming notifications.")
 
         while self._running:
             try:
                 response = self.api.receiving.receiveNotification()
                 if response.code == 200:
                     if not response.data:
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/PKG-INFO` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.38
+Version: 0.0.39
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# whatsapp-api-client-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
```

### Comparing `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/SOURCES.txt` & `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

