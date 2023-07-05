# Comparing `tmp/opentok-3.6.0.tar.gz` & `tmp/opentok-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opentok-3.6.0.tar", last modified: Wed Jun  7 11:57:44 2023, max compression
+gzip compressed data, was "dist/opentok-3.6.1.tar", last modified: Wed Jul  5 12:34:27 2023, max compression
```

## Comparing `opentok-3.6.0.tar` & `opentok-3.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.6.0/LICENSE.txt
--rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-06-07 11:57:44.000000 opentok-3.6.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)    26549 2023-06-07 11:57:23.000000 opentok-3.6.0/README.rst
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok/
--rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.6.0/opentok/archives.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3973 2023-06-06 16:52:09.000000 opentok-3.6.0/opentok/broadcast.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6229 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/exceptions.py
--rw-r--r--   0 mkahan     (503) staff       (20)    96555 2023-06-06 16:56:02.000000 opentok-3.6.0/opentok/opentok.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.6.0/opentok/render.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/session.py
--rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/sip_call.py
--rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/stream.py
--rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/streamlist.py
--rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-06-07 11:40:16.000000 opentok-3.6.0/opentok/version.py
--rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/websocket_audio_connection.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/top_level.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-06-07 11:57:44.000000 opentok-3.6.0/setup.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.6.0/setup.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-05 12:34:27.000000 opentok-3.6.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.6.1/LICENSE.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-07-05 12:34:27.000000 opentok-3.6.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)    26549 2023-06-07 11:57:23.000000 opentok-3.6.1/README.rst
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok/
+-rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.6.1/opentok/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.6.1/opentok/archives.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3973 2023-07-04 16:30:25.000000 opentok-3.6.1/opentok/broadcast.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     6184 2023-07-05 12:33:55.000000 opentok-3.6.1/opentok/endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:39:57.000000 opentok-3.6.1/opentok/exceptions.py
+-rw-r--r--   0 mkahan     (503) staff       (20)    97034 2023-07-05 12:33:55.000000 opentok-3.6.1/opentok/opentok.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.6.1/opentok/render.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.6.1/opentok/session.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.6.1/opentok/sip_call.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.6.1/opentok/stream.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.6.1/opentok/streamlist.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-07-05 12:33:55.000000 opentok-3.6.1/opentok/version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.6.1/opentok/websocket_audio_connection.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-07-05 12:34:27.000000 opentok-3.6.1/opentok.egg-info/top_level.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-07-05 12:34:27.000000 opentok-3.6.1/setup.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.6.1/setup.py
```

### Comparing `opentok-3.6.0/LICENSE.txt` & `opentok-3.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/PKG-INFO` & `opentok-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.6.0
+Version: 3.6.1
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentok-3.6.0/README.rst` & `opentok-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/__init__.py` & `opentok-3.6.1/opentok/__init__.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/archives.py` & `opentok-3.6.1/opentok/archives.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/broadcast.py` & `opentok-3.6.1/opentok/broadcast.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/endpoints.py` & `opentok-3.6.1/opentok/endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 class Endpoints(object):
     """
     For internal use.
     Class that provides the endpoint urls
     """
 
-
     def __init__(self, api_url, api_key):
         self.api_url = api_url
         self.api_key = api_key
 
     def get_session_url(self):
         url = self.api_url + "/session/create"
         return url
@@ -53,15 +52,15 @@
             "endpoints.signaling_url is deprecated (use endpoints.get_signaling_url instead).",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.get_signaling_url(session_id, connection_id)
 
     def get_stream_url(self, session_id, stream_id=None):
-        """ this method returns the url to get streams information """
+        """this method returns the url to get streams information"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/stream"
@@ -75,142 +74,141 @@
             "endpoints.broadcast_url is deprecated (use endpoints.get_broadcast_url instead).",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.get_broadcast_url(broadcast_id, stop, layout)
 
     def force_disconnect_url(self, session_id, connection_id):
-        """ this method returns the force disconnect url endpoint """
+        """this method returns the force disconnect url endpoint"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/connection/"
             + connection_id
         )
         return url
 
     def set_archive_layout_url(self, archive_id):
-        """ this method returns the url to set the archive layout """
+        """this method returns the url to set the archive layout"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
             + "/archive/"
             + archive_id
             + "/layout"
         )
         return url
 
     def dial_url(self):
-        """ this method returns the url to initialize a SIP call """
+        """this method returns the url to initialize a SIP call"""
         url = self.api_url + "/v2/project/" + self.api_key + "/dial"
         return url
 
     def set_stream_class_lists_url(self, session_id):
-        """ this method returns the url to set the stream class list """
+        """this method returns the url to set the stream class list"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/stream"
         )
         return url
 
     def get_broadcast_url(self, broadcast_id=None, stop=False, layout=False):
-        """ this method returns urls for working with broadcast """
+        """this method returns urls for working with broadcast"""
         url = self.api_url + "/v2/project/" + self.api_key + "/broadcast"
 
         if broadcast_id:
             url = url + "/" + broadcast_id
         if stop:
             url = url + "/stop"
         if layout:
             url = url + "/layout"
-            
+
         return url
 
     def get_mute_all_url(self, session_id):
-        """ this method returns the urls for muting every stream in a session """
+        """this method returns the urls for muting every stream in a session"""
         url = (
-             self.api_url  
-            + "/v2/project/" 
+            self.api_url
+            + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/mute"
-
         )
 
         return url
 
     def get_dtmf_all_url(self, session_id):
-        """ this method returns the url for Play DTMF to all clients in the session """
+        """this method returns the url for Play DTMF to all clients in the session"""
         url = (
             self.api_url
-            + "/v2/project/" 
+            + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/play-dtmf"
         )
 
         return url
 
     def get_dtmf_specific_url(self, session_id, connection_id):
-        """ this method returns the url for Play DTMF to a specific client connection"""
+        """this method returns the url for Play DTMF to a specific client connection"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
             + "/session/"
             + session_id
             + "/connection/"
             + connection_id
             + "/play-dtmf"
         )
 
         return url
 
     def get_archive_stream(self, archive_id=None):
-        """ this method returns urls for working with streamModes in archives """
+        """this method returns urls for working with streamModes in archives"""
         url = (
             self.api_url
             + "/v2/project/"
             + self.api_key
-            + "archive/"
+            + "/archive/"
             + archive_id
             + "/streams"
         )
 
         return url
 
     def get_broadcast_stream(self, broadcast_id=None):
-        """ this method returns urls for working with streamModes in broadcasts """
+        """this method returns urls for working with streamModes in broadcasts"""
         url = (
             self.api_url
-            + "/v2/partner/"
+            + "/v2/project/"
             + self.api_key
-            + "broadcast/"
+            + "/broadcast/"
             + broadcast_id
             + "/streams"
         )
 
         return url
 
     def get_render_url(self, render_id: str = None):
-        "Returns URLs for working with the Render API."""
+        "Returns URLs for working with the Render API." ""
         url = self.api_url + "/v2/project/" + self.api_key + "/render"
         if render_id:
             url += "/" + render_id
 
         return url
 
     def get_audio_connector_url(self):
         """Returns URLs for working with the Audio Connector API."""
         url = self.api_url + "/v2/project/" + self.api_key + "/connect"
-        
+
         return url
```

### Comparing `opentok-3.6.0/opentok/exceptions.py` & `opentok-3.6.1/opentok/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/opentok.py` & `opentok-3.6.1/opentok/opentok.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,36 +860,37 @@
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
         if response:
-            return Archive(self, response.json())
-        elif response.status_code == 403:
-            raise AuthError()
-        elif response.status_code == 400:
-            """
-            The HTTP response has a 400 status code in the following cases:
-            You do not pass in a session ID or you pass in an invalid session ID.
-            No clients are actively connected to the OpenTok session.
-            You specify an invalid resolution value.
-            The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
-            """
-            raise RequestError(response.json().get("message"))
-        elif response.status_code == 404:
-            raise NotFoundError("Archive or Stream not found")
-        elif response.status_code == 405:
-            raise ArchiveStreamModeError(
-                "Your archive is configured with a streamMode that does not support stream manipulation."
-            )
-        elif response.status_code == 409:
-            raise ArchiveError(response.json().get("message"))
+            if response.status_code == 204:
+                return None
+            elif response.status_code == 403:
+                raise AuthError()
+            elif response.status_code == 400:
+                """
+                The HTTP response has a 400 status code in the following cases:
+                You do not pass in a session ID or you pass in an invalid session ID.
+                No clients are actively connected to the OpenTok session.
+                You specify an invalid resolution value.
+                The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
+                """
+                raise RequestError(response.json().get("message"))
+            elif response.status_code == 404:
+                raise NotFoundError("Archive or Stream not found")
+            elif response.status_code == 405:
+                raise ArchiveStreamModeError(
+                    "Your archive is configured with a streamMode that does not support stream manipulation."
+                )
+            elif response.status_code == 409:
+                raise ArchiveError(response.json().get("message"))
         else:
-            raise RequestError("An unexpected error occurred", response.status_code)
+            raise RequestError("An unexpected error occurred.", response.status_code)
 
     def remove_archive_stream(
         self, archive_id: str, stream_id: str
     ) -> requests.Response:
         """
         This method will remove streams from the archive with removeStream.
 
@@ -906,36 +907,37 @@
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
         if response:
-            return Archive(self, response.json())
-        elif response.status_code == 403:
-            raise AuthError()
-        elif response.status_code == 400:
-            """
-            The HTTP response has a 400 status code in the following cases:
-            You do not pass in a session ID or you pass in an invalid session ID.
-            No clients are actively connected to the OpenTok session.
-            You specify an invalid resolution value.
-            The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
-            """
-            raise RequestError(response.json().get("message"))
-        elif response.status_code == 404:
-            raise NotFoundError("Archive or Stream not found")
-        elif response.status_code == 405:
-            raise ArchiveStreamModeError(
-                "Your archive is configured with a streamMode that does not support stream manipulation."
-            )
-        elif response.status_code == 409:
-            raise ArchiveError(response.json().get("message"))
+            if response.status_code == 204:
+                return None
+            elif response.status_code == 403:
+                raise AuthError()
+            elif response.status_code == 400:
+                """
+                The HTTP response has a 400 status code in the following cases:
+                You do not pass in a session ID or you pass in an invalid session ID.
+                No clients are actively connected to the OpenTok session.
+                You specify an invalid resolution value.
+                The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
+                """
+                raise RequestError(response.json().get("message"))
+            elif response.status_code == 404:
+                raise NotFoundError("Archive or Stream not found")
+            elif response.status_code == 405:
+                raise ArchiveStreamModeError(
+                    "Your archive is configured with a streamMode that does not support stream manipulation."
+                )
+            elif response.status_code == 409:
+                raise ArchiveError(response.json().get("message"))
         else:
-            raise RequestError("An unexpected error occurred", response.status_code)
+            raise RequestError("An unexpected error occurred.", response.status_code)
 
     def send_signal(self, session_id, payload, connection_id=None):
         """
         Send signals to all participants in an active OpenTok session or to a specific client
         connected to that session.
 
         :param String session_id: The session ID of the OpenTok session that receives the signal
@@ -960,34 +962,35 @@
             self.endpoints.get_signaling_url(session_id, connection_id),
             data=json.dumps(payload),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
-        if response.status_code == 204:
-            pass
-        elif response.status_code == 400:
-            raise SignalingError(
-                "One of the signal properties - data, type, sessionId or connectionId - is invalid."
-            )
-        elif response.status_code == 403:
-            raise AuthError(
-                "You are not authorized to send the signal. Check your authentication credentials."
-            )
-        elif response.status_code == 404:
-            raise SignalingError(
-                "The client specified by the connectionId property is not connected to the session."
-            )
-        elif response.status_code == 413:
-            raise SignalingError(
-                "The type string exceeds the maximum length (128 bytes), or the data string exceeds the maximum size (8 kB)."
-            )
+        if response:
+            if response.status_code == 204:
+                return None
+            elif response.status_code == 400:
+                raise SignalingError(
+                    "One of the signal properties - data, type, sessionId or connectionId - is invalid."
+                )
+            elif response.status_code == 403:
+                raise AuthError(
+                    "You are not authorized to send the signal. Check your authentication credentials."
+                )
+            elif response.status_code == 404:
+                raise SignalingError(
+                    "The client specified by the connectionId property is not connected to the session."
+                )
+            elif response.status_code == 413:
+                raise SignalingError(
+                    "The type string exceeds the maximum length (128 bytes), or the data string exceeds the maximum size (8 kB)."
+                )
         else:
-            raise RequestError("An unexpected error occurred", response.status_code)
+            raise RequestError("An unexpected error occurred.", response.status_code)
 
     def signal(self, session_id, payload, connection_id=None):
         warnings.warn(
             "opentok.signal is deprecated (use opentok.send_signal instead).",
             DeprecationWarning,
             stacklevel=2,
         )
@@ -1555,32 +1558,33 @@
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
         if response:
-            return Broadcast(response.json())
-        elif response.status_code == 400:
-            raise BroadcastError(
-                "Invalid request. This response may indicate that data in your request data is "
-                "invalid JSON. It may also indicate that you passed in invalid layout options. "
-                "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
-                "session. Or you specified and invalid resolution."
-            )
-        elif response.status_code == 403:
-            raise AuthError("Authentication error.")
-        elif response.status_code == 405:
-            raise BroadcastStreamModeError(
-                "Your broadcast is configured with a streamMode that does not support stream manipulation."
-            )
-        elif response.status_code == 409:
-            raise BroadcastError("The broadcast has already started for the session.")
+            if response.status_code == 204:
+                return None
+            elif response.status_code == 400:
+                raise BroadcastError(
+                    "Invalid request. This response may indicate that data in your request data is "
+                    "invalid JSON. It may also indicate that you passed in invalid layout options. "
+                    "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
+                    "session. Or you specified and invalid resolution."
+                )
+            elif response.status_code == 403:
+                raise AuthError("Authentication error.")
+            elif response.status_code == 405:
+                raise BroadcastStreamModeError(
+                    "Your broadcast is configured with a streamMode that does not support stream manipulation."
+                )
+            elif response.status_code == 409:
+                raise BroadcastError("The broadcast has already started for the session.")
         else:
-            raise RequestError("OpenTok server error.", response.status_code)
+            raise RequestError("An unexpected error occurred.", response.status_code)
 
     def remove_broadcast_stream(
         self, broadcast_id: str, stream_id: str
     ) -> requests.Response:
         """
         This method will remove streams from the broadcast with removeStream.
 
@@ -1597,30 +1601,31 @@
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
         )
 
         if response:
-            return Broadcast(response.json())
-        elif response.status_code == 400:
-            raise BroadcastError(
-                "Invalid request. This response may indicate that data in your request data is "
-                "invalid JSON. It may also indicate that you passed in invalid layout options. "
-                "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
-                "session. Or you specified and invalid resolution."
-            )
-        elif response.status_code == 403:
-            raise AuthError("Authentication error.")
-        elif response.status_code == 405:
-            raise BroadcastStreamModeError(
-                "Your broadcast is configured with a streamMode that does not support stream manipulation."
-            )
-        elif response.status_code == 409:
-            raise BroadcastError("The broadcast has already started for the session.")
+            if response.status_code == 204:
+                return None
+            elif response.status_code == 400:
+                raise BroadcastError(
+                    "Invalid request. This response may indicate that data in your request data is "
+                    "invalid JSON. It may also indicate that you passed in invalid layout options. "
+                    "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
+                    "session. Or you specified and invalid resolution."
+                )
+            elif response.status_code == 403:
+                raise AuthError("Authentication error.")
+            elif response.status_code == 405:
+                raise BroadcastStreamModeError(
+                    "Your broadcast is configured with a streamMode that does not support stream manipulation."
+                )
+            elif response.status_code == 409:
+                raise BroadcastError("The broadcast has already started for the session.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
     def get_broadcast(self, broadcast_id):
         """
         Use this method to get details on a broadcast that is in-progress.
```

### Comparing `opentok-3.6.0/opentok/render.py` & `opentok-3.6.1/opentok/render.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/session.py` & `opentok-3.6.1/opentok/session.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/stream.py` & `opentok-3.6.1/opentok/stream.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/streamlist.py` & `opentok-3.6.1/opentok/streamlist.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok/websocket_audio_connection.py` & `opentok-3.6.1/opentok/websocket_audio_connection.py`

 * *Files identical despite different names*

### Comparing `opentok-3.6.0/opentok.egg-info/PKG-INFO` & `opentok-3.6.1/opentok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.6.0
+Version: 3.6.1
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentok-3.6.0/setup.py` & `opentok-3.6.1/setup.py`

 * *Files identical despite different names*

