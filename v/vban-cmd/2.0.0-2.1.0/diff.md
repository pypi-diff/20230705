# Comparing `tmp/vban-cmd-2.0.0.tar.gz` & `tmp/vban_cmd-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban-cmd-2.0.0.tar", max compression
+gzip compressed data, was "vban_cmd-2.1.0.tar", max compression
```

## Comparing `vban-cmd-2.0.0.tar` & `vban_cmd-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban-cmd-2.0.0/LICENSE
--rw-r--r--   0        0        0      951 2023-06-25 12:12:54.738275 vban-cmd-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    11211 2023-06-25 17:44:51.494900 vban-cmd-2.0.0/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban-cmd-2.0.0/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban-cmd-2.0.0/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban-cmd-2.0.0/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban-cmd-2.0.0/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban-cmd-2.0.0/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban-cmd-2.0.0/vban_cmd/event.py
--rw-r--r--   0        0        0     6101 2023-06-25 02:42:35.162285 vban-cmd-2.0.0/vban_cmd/factory.py
--rw-r--r--   0        0        0     4168 2023-06-24 12:48:05.367943 vban-cmd-2.0.0/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban-cmd-2.0.0/vban_cmd/kinds.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban-cmd-2.0.0/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban-cmd-2.0.0/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban-cmd-2.0.0/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban-cmd-2.0.0/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban-cmd-2.0.0/vban_cmd/util.py
--rw-r--r--   0        0        0     6680 2023-06-25 10:52:32.659395 vban-cmd-2.0.0/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban-cmd-2.0.0/vban_cmd/worker.py
--rw-r--r--   0        0        0    12178 2023-06-25 20:58:40.663927 vban-cmd-2.0.0/setup.py
--rw-r--r--   0        0        0    11322 2023-06-25 20:58:40.664927 vban-cmd-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.1.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-05 01:52:46.657832 vban_cmd-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11700 2023-07-05 01:51:51.856606 vban_cmd-2.1.0/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.1.0/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.1.0/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.1.0/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban_cmd-2.1.0/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.1.0/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.1.0/vban_cmd/event.py
+-rw-r--r--   0        0        0     6138 2023-07-05 01:47:58.253892 vban_cmd-2.1.0/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4168 2023-06-24 12:48:05.367943 vban_cmd-2.1.0/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.1.0/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.1.0/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.1.0/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.1.0/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.1.0/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.1.0/vban_cmd/util.py
+-rw-r--r--   0        0        0     6780 2023-07-05 01:48:57.026637 vban_cmd-2.1.0/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.1.0/vban_cmd/worker.py
+-rw-r--r--   0        0        0    11856 1970-01-01 00:00:00.000000 vban_cmd-2.1.0/PKG-INFO
```

### Comparing `vban-cmd-2.0.0/LICENSE` & `vban_cmd-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/pyproject.toml` & `vban_cmd-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban-cmd-2.0.0/README.md` & `vban_cmd-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 -   `knee`: float, from 0.0 to 1.0
 -   `gainout`: float, from -24.0 to 24.0
 -   `makeup`: boolean
 
 example:
 
 ```python
-print(vm.strip[4].comp.knob)
+print(vban.strip[4].comp.knob)
 ```
 
 Strip Comp properties are defined as write only.
 
 `knob` defined for all versions, all other parameters potato only.
 
 ##### Strip.Gate
@@ -185,15 +185,15 @@
 -   `attack`: float, from 0.0 to 1000.0
 -   `hold`: float, from 0.0 to 5000.0
 -   `release`: float, from 0.0 to 5000.0
 
 example:
 
 ```python
-vm.strip[2].gate.attack = 300.8
+vban.strip[2].gate.attack = 300.8
 ```
 
 Strip Gate properties are defined as write only, potato version only.
 
 `knob` defined for all versions, all other parameters potato only.
 
 ##### Strip.Denoiser
@@ -347,14 +347,15 @@
     Set many strip/bus parameters at once, for example:
 
 ```python
 vban.apply(
     {
         "strip-0": {"A1": True, "B1": True, "gain": -6.0},
         "bus-1": {"mute": True, "mode": "composite"},
+        "bus-2": {"eq": {"on": True}},
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
@@ -382,15 +383,14 @@
 
 Level updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.
 
 example:
 
 ```python
 import vban_cmd
-# Listen for level updates
 opts = {
     "ip": "<ip address>",
     "streamname": "Command1",
     "port": 6980,
 }
 with vban_cmd.api('banana', ldirty=True, **opts) as vban:
     ...
@@ -454,16 +454,18 @@
 `vban_cmd.api(kind_id: str, **opts)`
 
 You may pass the following optional keyword arguments:
 
 -   `ip`: str, ip or hostname of remote machine
 -   `streamname`: str, name of the stream to connect to.
 -   `port`: int=6980, vban udp port of remote machine.
--   `pdirty`: parameter updates
--   `ldirty`: level updates
+-   `pdirty`: boolean=False, parameter updates
+-   `ldirty`: boolean=False, level updates
+-   `timeout`: int=5, amount of time (seconds) you will wait for subscription response
+-   `sendtext_only`: boolean=False, set `True` if you are only interested in sending script commands (no rt packets will be received)
 
 #### `vban.pdirty`
 
 True iff a parameter has been changed.
 
 #### `vban.ldirty`
 
@@ -473,21 +475,26 @@
 
 Sends a script block as a string request, for example:
 
 ```python
 vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
 ```
 
+note. if you are ONLY interested in sending script commands you may set sendtext_only kwarg to True
+
 #### `vban.public_packet`
 
-Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).
+Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
+
+States not guaranteed to be current (requires use of dirty parameters to confirm).
 
 ### `Errors`
 
--   `errors.VBANCMDError`: Base VMCMD error class.
+-   `errors.VBANCMDError`: Exception raised when general errors occur.
+-   `errors.VBANCMDConnectionError`: Exception raised when connection/timeout errors occur.
 
 ### `Tests`
 
 First make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)
 
 Then from tests directory:
```

### Comparing `vban-cmd-2.0.0/vban_cmd/bus.py` & `vban_cmd-2.1.0/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/command.py` & `vban_cmd-2.1.0/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/config.py` & `vban_cmd-2.1.0/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/event.py` & `vban_cmd-2.1.0/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/factory.py` & `vban_cmd-2.1.0/vban_cmd/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             "ip": None,
             "port": 6980,
             "streamname": "Command1",
             "bps": 0,
             "channel": 0,
             "ratelimit": 0.01,
             "timeout": 5,
+            "sendtext_only": False,
             "sync": False,
             "pdirty": False,
             "ldirty": False,
         }
         if "subs" in kwargs:
             defaultkwargs |= kwargs.pop("subs")  # for backwards compatibility
         kwargs = defaultkwargs | kwargs
```

### Comparing `vban-cmd-2.0.0/vban_cmd/iremote.py` & `vban_cmd-2.1.0/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/kinds.py` & `vban_cmd-2.1.0/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/meta.py` & `vban_cmd-2.1.0/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/packet.py` & `vban_cmd-2.1.0/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/strip.py` & `vban_cmd-2.1.0/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/subject.py` & `vban_cmd-2.1.0/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/util.py` & `vban_cmd-2.1.0/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/vban_cmd/vbancmd.py` & `vban_cmd-2.1.0/vban_cmd/vbancmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,26 +81,27 @@
             raise VBANCMDError("no ip provided and no vban.toml located.")
 
     def __enter__(self):
         self.login()
         return self
 
     def login(self):
-        """Starts the subscriber and updater threads"""
-        self.running = True
-        self.event.info()
-
-        self.subscriber = Subscriber(self)
-        self.subscriber.start()
-
-        queue = Queue()
-        self.updater = Updater(self, queue)
-        self.updater.start()
-        self.producer = Producer(self, queue)
-        self.producer.start()
+        """Starts the subscriber and updater threads (unless sendtext_only mode)"""
+        if not self.sendtext_only:
+            self.running = True
+            self.event.info()
+
+            self.subscriber = Subscriber(self)
+            self.subscriber.start()
+
+            queue = Queue()
+            self.updater = Updater(self, queue)
+            self.updater.start()
+            self.producer = Producer(self, queue)
+            self.producer.start()
 
         self.logger.info(f"{type(self).__name__}: Successfully logged into {self}")
 
     def _set_rt(
         self,
         id_: str,
         param: Optional[str] = None,
```

### Comparing `vban-cmd-2.0.0/vban_cmd/worker.py` & `vban_cmd-2.1.0/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-2.0.0/setup.py` & `vban_cmd-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,525 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: vban-cmd
+Version: 2.1.0
+Summary: Python interface for the VBAN RT Packet Service (Sendtext)
+Home-page: https://github.com/onyx-and-iris/vban-cmd-python
+License: MIT
+Author: onyx-and-iris
+Author-email: code@onyxandiris.online
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Project-URL: Repository, https://github.com/onyx-and-iris/vban-cmd-python
+Description-Content-Type: text/markdown
 
-packages = \
-['vban_cmd']
+[![PyPI version](https://badge.fury.io/py/vban-cmd.svg)](https://badge.fury.io/py/vban-cmd)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/vban-cmd-python/blob/dev/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![Tests Status](./tests/basic.svg?dummy=8484744)
+![Tests Status](./tests/banana.svg?dummy=8484744)
+![Tests Status](./tests/potato.svg?dummy=8484744)
 
-package_data = \
-{'': ['*']}
+# VBAN CMD
 
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['gui = scripts:ex_gui',
-                     'obs = scripts:ex_obs',
-                     'observer = scripts:ex_observer',
-                     'test = scripts:test']}
-
-setup_kwargs = {
-    'name': 'vban-cmd',
-    'version': '2.0.0',
-    'description': 'Python interface for the VBAN RT Packet Service (Sendtext)',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/vban-cmd.svg)](https://badge.fury.io/py/vban-cmd)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/vban-cmd-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# VBAN CMD\n\nThis python interface allows you to get and set Voicemeeter parameter values over a network.\n\nIt may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)\n\nThere is no support for audio transfer in this package, only parameters.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.8\n-   Banana 2.0.6.8\n-   Potato 3.0.2.8\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install vban-cmd`\n\n## `Use`\n\n#### Connection\n\nLoad VBAN connection info from toml config. A valid `vban.toml` might look like this:\n\n```toml\n[connection]\nip = "gamepc.local"\nport = 6980\nstreamname = "Command1"\n```\n\nIt should be placed next to your `__main__.py` file.\n\nAlternatively you may pass `ip`, `port`, `streamname` as keyword arguments.\n\n#### `__main__.py`\n\nSimplest use case, use a context manager to request a VbanCmd class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n```python\nimport vban_cmd\n\n\nclass ManyThings:\n    def __init__(self, vban):\n        self.vban = vban\n\n    def things(self):\n        self.vban.strip[0].label = "podmic"\n        self.vban.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vban.bus[3].gain = -6.3\n        self.vban.bus[4].eq.on = True\n        info = (\n            f"bus 3 gain has been set to {self.vban.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vban.bus[4].eq.on}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    KIND_ID = "banana"\n\n    with vban_cmd.api(\n        KIND_ID, ip="gamepc.local", port=6980, streamname="Command1"\n    ) as vban:\n        do = ManyThings(vban)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vban.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True, "eq": {"on": True}},\n            }\n        )\n\n\nif __name__ == "__main__":\n    main()\n```\n\nOtherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.\n\n## `KIND_ID`\n\nPass the kind of Voicemeeter as an argument. KIND_ID may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `limit`: int, from -40 to 12\n\nexample:\n\n```python\nvban.strip[3].gain = 3.7\nprint(vban.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvban.strip[5].appmute("Spotify", True)\nvban.strip[5].appgain("Spotify", 0.5)\n```\n\n##### Strip.Comp\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `gainin`: float, from -24.0 to 24.0\n-   `ratio`: float, from 1.0 to 8.0\n-   `threshold`: float, from -40.0 to -3.0\n-   `attack`: float, from 0.0 to 200.0\n-   `release`: float, from 0.0 to 5000.0\n-   `knee`: float, from 0.0 to 1.0\n-   `gainout`: float, from -24.0 to 24.0\n-   `makeup`: boolean\n\nexample:\n\n```python\nprint(vm.strip[4].comp.knob)\n```\n\nStrip Comp properties are defined as write only.\n\n`knob` defined for all versions, all other parameters potato only.\n\n##### Strip.Gate\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `threshold`: float, from -60.0 to -10.0\n-   `damping`: float, from -60.0 to -10.0\n-   `bpsidechain`: int, from 100 to 4000\n-   `attack`: float, from 0.0 to 1000.0\n-   `hold`: float, from 0.0 to 5000.0\n-   `release`: float, from 0.0 to 5000.0\n\nexample:\n\n```python\nvm.strip[2].gate.attack = 300.8\n```\n\nStrip Gate properties are defined as write only, potato version only.\n\n`knob` defined for all versions, all other parameters potato only.\n\n##### Strip.Denoiser\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n\nstrip.denoiser properties are defined as write only, potato version only.\n\n##### Strip.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nStrip EQ properties are defined as write only, potato version only.\n\n##### Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvban.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Levels\n\nThe following properties are available.\n\n-   `prefader`\n\nexample:\n\n```python\nprint(vban.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n\nexample:\n\n```python\nvban.bus[4].eq = true\nprint(vban.bus[0].label)\n```\n\n##### Bus.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\n##### Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvban.bus[4].mode.amix = True\n\nprint(vban.bus[2].mode.get())\n```\n\n##### Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vban.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvban.strip[0].fadeto(-10.3, 1000)\nvban.bus[3].fadeby(-5.6, 500)\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values. The following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are write only and accept boolean values.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvban.command.restart()\nvban.command.showvbanchat = true\n```\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus parameters at once, for example:\n\n```python\nvban.apply(\n    {\n        "strip-0": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-1": {"mute": True, "mode": "composite"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvban.strip[0].apply(mute: true, gain: 3.2, A1: true)\nvban.bus[0].apply(A1: true)\n```\n\n## Config Files\n\n`vban.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport vban_cmd\nwith vban_cmd.api(\'banana\') as vban:\n    vban.apply_config(\'example\')\n```\n\nwill load a config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nLevel updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.\n\nexample:\n\n```python\nimport vban_cmd\n# Listen for level updates\nopts = {\n    "ip": "<ip address>",\n    "streamname": "Command1",\n    "port": 6980,\n}\nwith vban_cmd.api(\'banana\', ldirty=True, **opts) as vban:\n    ...\n```\n\n#### `vban.subject`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vban):\n        vban.subject.add(self)\n        ...\n```\n\n#### `vban.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvban.event.ldirty = True\n\nvban.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvban.event.remove(["pdirty", "ldirty"])\n\n# get a list of currently subscribed\nprint(vban.event.get())\n```\n\n## VbanCmd class\n\n`vban_cmd.api(kind_id: str, **opts)`\n\nYou may pass the following optional keyword arguments:\n\n-   `ip`: str, ip or hostname of remote machine\n-   `streamname`: str, name of the stream to connect to.\n-   `port`: int=6980, vban udp port of remote machine.\n-   `pdirty`: parameter updates\n-   `ldirty`: level updates\n\n#### `vban.pdirty`\n\nTrue iff a parameter has been changed.\n\n#### `vban.ldirty`\n\nTrue iff a level value has been changed.\n\n#### `vban.sendtext(script)`\n\nSends a script block as a string request, for example:\n\n```python\nvban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")\n```\n\n#### `vban.public_packet`\n\nReturns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).\n\n### `Errors`\n\n-   `errors.VBANCMDError`: Base VMCMD error class.\n\n### `Tests`\n\nFirst make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)\n\nThen from tests directory:\n\n`pytest -v`\n\n## Resources\n\n-   [Voicemeeter VBAN TEXT](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=19)\n\n-   [Voicemeeter RT Packet Service](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=27)\n',
-    'author': 'onyx-and-iris',
-    'author_email': 'code@onyxandiris.online',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/onyx-and-iris/vban-cmd-python',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+This python interface allows you to get and set Voicemeeter parameter values over a network.
+
+It may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)
+
+There is no support for audio transfer in this package, only parameters.
+
+For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
+
+## Tested against
+
+-   Basic 1.0.8.8
+-   Banana 2.0.6.8
+-   Potato 3.0.2.8
+
+## Requirements
+
+-   [Voicemeeter](https://voicemeeter.com/)
+-   Python 3.10 or greater
+
+## Installation
+
+`pip install vban-cmd`
+
+## `Use`
+
+#### Connection
+
+Load VBAN connection info from toml config. A valid `vban.toml` might look like this:
+
+```toml
+[connection]
+ip = "gamepc.local"
+port = 6980
+streamname = "Command1"
+```
+
+It should be placed next to your `__main__.py` file.
+
+Alternatively you may pass `ip`, `port`, `streamname` as keyword arguments.
+
+#### `__main__.py`
+
+Simplest use case, use a context manager to request a VbanCmd class of a kind.
+
+Login and logout are handled for you in this scenario.
+
+```python
+import vban_cmd
+
+
+class ManyThings:
+    def __init__(self, vban):
+        self.vban = vban
+
+    def things(self):
+        self.vban.strip[0].label = "podmic"
+        self.vban.strip[0].mute = True
+        print(
+            f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"
+        )
+
+    def other_things(self):
+        self.vban.bus[3].gain = -6.3
+        self.vban.bus[4].eq.on = True
+        info = (
+            f"bus 3 gain has been set to {self.vban.bus[3].gain}",
+            f"bus 4 eq has been set to {self.vban.bus[4].eq.on}",
+        )
+        print("\n".join(info))
+
+
+def main():
+    KIND_ID = "banana"
+
+    with vban_cmd.api(
+        KIND_ID, ip="gamepc.local", port=6980, streamname="Command1"
+    ) as vban:
+        do = ManyThings(vban)
+        do.things()
+        do.other_things()
+
+        # set many parameters at once
+        vban.apply(
+            {
+                "strip-2": {"A1": True, "B1": True, "gain": -6.0},
+                "bus-2": {"mute": True, "eq": {"on": True}},
+            }
+        )
+
+
+if __name__ == "__main__":
+    main()
+```
+
+Otherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.
+
+## `KIND_ID`
+
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
+
+-   `basic`
+-   `banana`
+-   `potato`
+
+## `Available commands`
+
+### Strip
+
+The following properties are available.
+
+-   `mono`: boolean
+-   `solo`: boolean
+-   `mute`: boolean
+-   `label`: string
+-   `gain`: float, -60 to 12
+-   `A1 - A5`, `B1 - B3`: boolean
+-   `limit`: int, from -40 to 12
+
+example:
+
+```python
+vban.strip[3].gain = 3.7
+print(vban.strip[0].label)
+```
+
+The following methods are available.
+
+-   `appgain(name, value)`: string, float, from 0.0 to 1.0
+
+Set the gain in db by value for the app matching name.
+
+-   `appmute(name, value)`: string, bool
+
+Set mute state as value for the app matching name.
+
+example:
+
+```python
+vban.strip[5].appmute("Spotify", True)
+vban.strip[5].appgain("Spotify", 0.5)
+```
+
+##### Strip.Comp
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+-   `gainin`: float, from -24.0 to 24.0
+-   `ratio`: float, from 1.0 to 8.0
+-   `threshold`: float, from -40.0 to -3.0
+-   `attack`: float, from 0.0 to 200.0
+-   `release`: float, from 0.0 to 5000.0
+-   `knee`: float, from 0.0 to 1.0
+-   `gainout`: float, from -24.0 to 24.0
+-   `makeup`: boolean
+
+example:
+
+```python
+print(vban.strip[4].comp.knob)
+```
+
+Strip Comp properties are defined as write only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Gate
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+-   `threshold`: float, from -60.0 to -10.0
+-   `damping`: float, from -60.0 to -10.0
+-   `bpsidechain`: int, from 100 to 4000
+-   `attack`: float, from 0.0 to 1000.0
+-   `hold`: float, from 0.0 to 5000.0
+-   `release`: float, from 0.0 to 5000.0
+
+example:
+
+```python
+vban.strip[2].gate.attack = 300.8
+```
+
+Strip Gate properties are defined as write only, potato version only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Denoiser
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+
+strip.denoiser properties are defined as write only, potato version only.
+
+##### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+Strip EQ properties are defined as write only, potato version only.
+
+##### Gainlayers
+
+-   `gain`: float, from -60.0 to 12.0
+
+example:
+
+```python
+vban.strip[3].gainlayer[3].gain = 3.7
+```
+
+Gainlayers are defined for potato version only.
+
+##### Levels
+
+The following properties are available.
+
+-   `prefader`
+
+example:
+
+```python
+print(vban.strip[3].levels.prefader)
+```
+
+Level properties will return -200.0 if no audio detected.
+
+### Bus
+
+The following properties are available.
+
+-   `mono`: boolean
+-   `mute`: boolean
+-   `label`: string
+-   `gain`: float, -60 to 12
+
+example:
+
+```python
+vban.bus[4].eq = true
+print(vban.bus[0].label)
+```
+
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+##### Modes
+
+The following properties are available.
+
+-   `normal`: boolean
+-   `amix`: boolean
+-   `bmix`: boolean
+-   `composite`: boolean
+-   `tvmix`: boolean
+-   `upmix21`: boolean
+-   `upmix41`: boolean
+-   `upmix61`: boolean
+-   `centeronly`: boolean
+-   `lfeonly`: boolean
+-   `rearonly`: boolean
+
+The following methods are available.
+
+-   `get()`: Returns the current bus mode
+
+example:
+
+```python
+vban.bus[4].mode.amix = True
+
+print(vban.bus[2].mode.get())
+```
+
+##### Levels
+
+The following properties are available.
+
+-   `all`
+
+example:
+
+```python
+print(vban.bus[0].levels.all)
+```
+
+`levels.all` will return -200.0 if no audio detected.
+
+### Strip | Bus
+
+The following methods are available.
+
+-   `fadeto(amount, time)`: float, int
+-   `fadeby(amount, time)`: float, int
+
+Modify gain to or by the selected amount in db over a time interval in ms.
+
+example:
+
+```python
+vban.strip[0].fadeto(-10.3, 1000)
+vban.bus[3].fadeby(-5.6, 500)
+```
+
+### Command
+
+Certain 'special' commands are defined by the API as performing actions rather than setting values. The following methods are available:
+
+-   `show()` : Bring Voiceemeter GUI to the front
+-   `shutdown()` : Shuts down the GUI
+-   `restart()` : Restart the audio engine
+-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)
+
+The following properties are write only and accept boolean values.
+
+-   `showvbanchat`: boolean
+-   `lock`: boolean
+
+example:
+
+```python
+vban.command.restart()
+vban.command.showvbanchat = true
+```
+
+### Multiple parameters
+
+-   `apply`
+    Set many strip/bus parameters at once, for example:
+
+```python
+vban.apply(
+    {
+        "strip-0": {"A1": True, "B1": True, "gain": -6.0},
+        "bus-1": {"mute": True, "mode": "composite"},
+        "bus-2": {"eq": {"on": True}},
+    }
+)
+```
+
+Or for each class you may do:
+
+```python
+vban.strip[0].apply(mute: true, gain: 3.2, A1: true)
+vban.bus[0].apply(A1: true)
+```
+
+## Config Files
+
+`vban.apply_config(<configname>)`
+
+You may load config files in TOML format.
+Three example configs have been included with the package. Remember to save
+current settings before loading a user config. To set one you may do:
+
+```python
+import vban_cmd
+with vban_cmd.api('banana') as vban:
+    vban.apply_config('example')
+```
+
+will load a config file at configs/banana/example.toml for Voicemeeter Banana.
+
+## Events
+
+Level updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.
+
+example:
+
+```python
+import vban_cmd
+opts = {
+    "ip": "<ip address>",
+    "streamname": "Command1",
+    "port": 6980,
 }
+with vban_cmd.api('banana', ldirty=True, **opts) as vban:
+    ...
+```
+
+#### `vban.subject`
+
+Use the Subject class to register an app as event observer.
+
+The following methods are available:
+
+-   `add`: registers an app as an event observer
+-   `remove`: deregisters an app as an event observer
+
+example:
+
+```python
+# register an app to receive updates
+class App():
+    def __init__(self, vban):
+        vban.subject.add(self)
+        ...
+```
+
+#### `vban.event`
+
+Use the event class to toggle updates as necessary.
+
+The following properties are available:
+
+-   `pdirty`: boolean
+-   `ldirty`: boolean
+
+example:
+
+```python
+vban.event.ldirty = True
+
+vban.event.pdirty = False
+```
+
+Or add, remove a list of events.
+
+The following methods are available:
+
+-   `add()`
+-   `remove()`
+-   `get()`
+
+example:
+
+```python
+vban.event.remove(["pdirty", "ldirty"])
+
+# get a list of currently subscribed
+print(vban.event.get())
+```
+
+## VbanCmd class
+
+`vban_cmd.api(kind_id: str, **opts)`
+
+You may pass the following optional keyword arguments:
+
+-   `ip`: str, ip or hostname of remote machine
+-   `streamname`: str, name of the stream to connect to.
+-   `port`: int=6980, vban udp port of remote machine.
+-   `pdirty`: boolean=False, parameter updates
+-   `ldirty`: boolean=False, level updates
+-   `timeout`: int=5, amount of time (seconds) you will wait for subscription response
+-   `sendtext_only`: boolean=False, set `True` if you are only interested in sending script commands (no rt packets will be received)
+
+#### `vban.pdirty`
+
+True iff a parameter has been changed.
+
+#### `vban.ldirty`
+
+True iff a level value has been changed.
+
+#### `vban.sendtext(script)`
+
+Sends a script block as a string request, for example:
+
+```python
+vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
+```
+
+note. if you are ONLY interested in sending script commands you may set sendtext_only kwarg to True
+
+#### `vban.public_packet`
+
+Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
+
+States not guaranteed to be current (requires use of dirty parameters to confirm).
+
+### `Errors`
+
+-   `errors.VBANCMDError`: Exception raised when general errors occur.
+-   `errors.VBANCMDConnectionError`: Exception raised when connection/timeout errors occur.
+
+### `Tests`
+
+First make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)
+
+Then from tests directory:
+
+`pytest -v`
+
+## Resources
+
+-   [Voicemeeter VBAN TEXT](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=19)
 
+-   [Voicemeeter RT Packet Service](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=27)
 
-setup(**setup_kwargs)
```

