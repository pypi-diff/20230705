# Comparing `tmp/vban_cmd-2.1.0.tar.gz` & `tmp/vban_cmd-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.1.0.tar", max compression
+gzip compressed data, was "vban_cmd-2.1.1.tar", max compression
```

## Comparing `vban_cmd-2.1.0.tar` & `vban_cmd-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.1.0/LICENSE
--rw-r--r--   0        0        0      951 2023-07-05 01:52:46.657832 vban_cmd-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    11700 2023-07-05 01:51:51.856606 vban_cmd-2.1.0/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.1.0/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.1.0/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.1.0/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.1.0/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.1.0/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.1.0/vban_cmd/event.py
--rw-r--r--   0        0        0     6138 2023-07-05 01:47:58.253892 vban_cmd-2.1.0/vban_cmd/factory.py
--rw-r--r--   0        0        0     4168 2023-06-24 12:48:05.367943 vban_cmd-2.1.0/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.1.0/vban_cmd/kinds.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.1.0/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.1.0/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.1.0/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.1.0/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.1.0/vban_cmd/util.py
--rw-r--r--   0        0        0     6780 2023-07-05 01:48:57.026637 vban_cmd-2.1.0/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.1.0/vban_cmd/worker.py
--rw-r--r--   0        0        0    11856 1970-01-01 00:00:00.000000 vban_cmd-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.1.1/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-05 13:06:30.007528 vban_cmd-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11605 2023-07-05 13:04:56.374532 vban_cmd-2.1.1/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.1.1/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.1.1/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.1.1/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.1.1/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.1.1/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.1.1/vban_cmd/event.py
+-rw-r--r--   0        0        0     6133 2023-07-05 13:04:18.891728 vban_cmd-2.1.1/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4168 2023-06-24 12:48:05.367943 vban_cmd-2.1.1/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.1.1/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.1.1/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.1.1/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.1.1/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.1.1/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.1.1/vban_cmd/util.py
+-rw-r--r--   0        0        0     6773 2023-07-05 13:07:37.219851 vban_cmd-2.1.1/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.1.1/vban_cmd/worker.py
+-rw-r--r--   0        0        0    11763 1970-01-01 00:00:00.000000 vban_cmd-2.1.1/PKG-INFO
```

### Comparing `vban_cmd-2.1.0/LICENSE` & `vban_cmd-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/pyproject.toml` & `vban_cmd-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.1.0"
+version = "2.1.1"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.1.0/README.md` & `vban_cmd-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -456,16 +456,16 @@
 You may pass the following optional keyword arguments:
 
 -   `ip`: str, ip or hostname of remote machine
 -   `streamname`: str, name of the stream to connect to.
 -   `port`: int=6980, vban udp port of remote machine.
 -   `pdirty`: boolean=False, parameter updates
 -   `ldirty`: boolean=False, level updates
--   `timeout`: int=5, amount of time (seconds) you will wait for subscription response
--   `sendtext_only`: boolean=False, set `True` if you are only interested in sending script commands (no rt packets will be received)
+-   `timeout`: int=5, amount of time (seconds) to wait for an incoming RT data packet (parameter states).
+-   `outbound`: boolean=False, set `True` if you are only interested in sending commands. (no rt packets will be received)
 
 #### `vban.pdirty`
 
 True iff a parameter has been changed.
 
 #### `vban.ldirty`
 
@@ -475,16 +475,14 @@
 
 Sends a script block as a string request, for example:
 
 ```python
 vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
 ```
 
-note. if you are ONLY interested in sending script commands you may set sendtext_only kwarg to True
-
 #### `vban.public_packet`
 
 Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
 
 States not guaranteed to be current (requires use of dirty parameters to confirm).
 
 ### `Errors`
```

### Comparing `vban_cmd-2.1.0/vban_cmd/bus.py` & `vban_cmd-2.1.1/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/command.py` & `vban_cmd-2.1.1/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/config.py` & `vban_cmd-2.1.1/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/event.py` & `vban_cmd-2.1.1/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/factory.py` & `vban_cmd-2.1.1/vban_cmd/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             "ip": None,
             "port": 6980,
             "streamname": "Command1",
             "bps": 0,
             "channel": 0,
             "ratelimit": 0.01,
             "timeout": 5,
-            "sendtext_only": False,
+            "outbound": False,
             "sync": False,
             "pdirty": False,
             "ldirty": False,
         }
         if "subs" in kwargs:
             defaultkwargs |= kwargs.pop("subs")  # for backwards compatibility
         kwargs = defaultkwargs | kwargs
```

### Comparing `vban_cmd-2.1.0/vban_cmd/iremote.py` & `vban_cmd-2.1.1/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/kinds.py` & `vban_cmd-2.1.1/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/meta.py` & `vban_cmd-2.1.1/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/packet.py` & `vban_cmd-2.1.1/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/strip.py` & `vban_cmd-2.1.1/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/subject.py` & `vban_cmd-2.1.1/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/util.py` & `vban_cmd-2.1.1/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/vban_cmd/vbancmd.py` & `vban_cmd-2.1.1/vban_cmd/vbancmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             raise VBANCMDError("no ip provided and no vban.toml located.")
 
     def __enter__(self):
         self.login()
         return self
 
     def login(self):
-        """Starts the subscriber and updater threads (unless sendtext_only mode)"""
-        if not self.sendtext_only:
+        """Starts the subscriber and updater threads (unless in outbound mode)"""
+        if not self.outbound:
             self.running = True
             self.event.info()
 
             self.subscriber = Subscriber(self)
             self.subscriber.start()
 
             queue = Queue()
```

### Comparing `vban_cmd-2.1.0/vban_cmd/worker.py` & `vban_cmd-2.1.1/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.1.0/PKG-INFO` & `vban_cmd-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -473,16 +473,16 @@
 You may pass the following optional keyword arguments:
 
 -   `ip`: str, ip or hostname of remote machine
 -   `streamname`: str, name of the stream to connect to.
 -   `port`: int=6980, vban udp port of remote machine.
 -   `pdirty`: boolean=False, parameter updates
 -   `ldirty`: boolean=False, level updates
--   `timeout`: int=5, amount of time (seconds) you will wait for subscription response
--   `sendtext_only`: boolean=False, set `True` if you are only interested in sending script commands (no rt packets will be received)
+-   `timeout`: int=5, amount of time (seconds) to wait for an incoming RT data packet (parameter states).
+-   `outbound`: boolean=False, set `True` if you are only interested in sending commands. (no rt packets will be received)
 
 #### `vban.pdirty`
 
 True iff a parameter has been changed.
 
 #### `vban.ldirty`
 
@@ -492,16 +492,14 @@
 
 Sends a script block as a string request, for example:
 
 ```python
 vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
 ```
 
-note. if you are ONLY interested in sending script commands you may set sendtext_only kwarg to True
-
 #### `vban.public_packet`
 
 Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
 
 States not guaranteed to be current (requires use of dirty parameters to confirm).
 
 ### `Errors`
```

