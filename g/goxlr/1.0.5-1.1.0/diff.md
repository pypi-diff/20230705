# Comparing `tmp/goxlr-1.0.5.tar.gz` & `tmp/goxlr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.0.5.tar", last modified: Tue Jul  4 23:16:01 2023, max compression
+gzip compressed data, was "goxlr-1.1.0.tar", last modified: Wed Jul  5 12:38:56 2023, max compression
```

## Comparing `goxlr-1.0.5.tar` & `goxlr-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 23:16:01.003638 goxlr-1.0.5/
--rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.0.5/LICENSE-3RD-PARTY.txt
--rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2350 2023-07-04 23:16:01.003638 goxlr-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1994 2023-07-04 22:58:39.000000 goxlr-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 23:16:00.999641 goxlr-1.0.5/goxlr/
--rw-rw-rw-   0        0        0       61 2023-07-04 23:15:46.000000 goxlr-1.0.5/goxlr/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-04 22:59:52.000000 goxlr-1.0.5/goxlr/_version.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.5/goxlr/error.py
--rw-rw-rw-   0        0        0    27238 2023-07-04 21:56:29.000000 goxlr-1.0.5/goxlr/goxlr.py
--rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.5/goxlr/types.py
--rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.5/goxlr/ws.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:16:01.003139 goxlr-1.0.5/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2350 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-04 23:16:01.004640 goxlr-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.832906 goxlr-1.1.0/
+-rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.1.0/LICENSE-3RD-PARTY.txt
+-rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2503 2023-07-05 12:38:56.832906 goxlr-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2147 2023-07-05 12:32:01.000000 goxlr-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.824905 goxlr-1.1.0/goxlr/
+-rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.1.0/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-05 11:19:02.000000 goxlr-1.1.0/goxlr/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.831906 goxlr-1.1.0/goxlr/commands/
+-rw-rw-rw-   0        0        0      108 2023-07-05 11:52:15.000000 goxlr-1.1.0/goxlr/commands/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-07-05 12:17:31.000000 goxlr-1.1.0/goxlr/commands/daemon.py
+-rw-rw-rw-   0        0        0      237 2023-07-05 11:08:41.000000 goxlr-1.1.0/goxlr/commands/general.py
+-rw-rw-rw-   0        0        0    26136 2023-07-05 12:17:07.000000 goxlr-1.1.0/goxlr/commands/goxlr.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.1.0/goxlr/error.py
+-rw-rw-rw-   0        0        0     2482 2023-07-05 12:32:25.000000 goxlr-1.1.0/goxlr/socket.py
+-rw-rw-rw-   0        0        0    11533 2023-07-05 12:17:58.000000 goxlr-1.1.0/goxlr/types.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.828906 goxlr-1.1.0/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2503 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-05 12:38:56.833408 goxlr-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.1.0/setup.py
```

### Comparing `goxlr-1.0.5/LICENSE-3RD-PARTY.txt` & `goxlr-1.1.0/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.5/LICENSE.txt` & `goxlr-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.5/PKG-INFO` & `goxlr-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,43 +15,50 @@
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
 
 A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
 
 ## Features
 - Asynchronous connection to the GoXLR utility daemon
-- Almost all methods have been translated to Python
+- All methods have been translated to Python
 - Handy enumerators for everything
 - Very simple and easy to get started
 
 ## Installation
 ```shell
 pip install goxlr
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
+
 from goxlr import GoXLR
+from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
-        print(await xlr.ping())
+        await xlr.set_fader(Fader.A, Channel.Headphones)
+        await xlr.set_volume(Channel.Headphones, 0.5)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
+
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
 async def main():
     xlr = GoXLR()
-    xlr.connect()
-    print(await xlr.ping())
-    xlr.close()
+    await xlr.open()
+
+    ping = await xlr.ping()
+    print(ping)  # Ok
+
+    await xlr.close()
 ```
 
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
 
 ## Documentation
 Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.0.5/README.md` & `goxlr-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,43 +2,50 @@
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
 
 A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
 
 ## Features
 - Asynchronous connection to the GoXLR utility daemon
-- Almost all methods have been translated to Python
+- All methods have been translated to Python
 - Handy enumerators for everything
 - Very simple and easy to get started
 
 ## Installation
 ```shell
 pip install goxlr
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
+
 from goxlr import GoXLR
+from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
-        print(await xlr.ping())
+        await xlr.set_fader(Fader.A, Channel.Headphones)
+        await xlr.set_volume(Channel.Headphones, 0.5)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
+
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
 async def main():
     xlr = GoXLR()
-    xlr.connect()
-    print(await xlr.ping())
-    xlr.close()
+    await xlr.open()
+
+    ping = await xlr.ping()
+    print(ping)  # Ok
+
+    await xlr.close()
 ```
 
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
 
 ## Documentation
 Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.0.5/goxlr/goxlr.py` & `goxlr-1.1.0/goxlr/commands/goxlr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,70 @@
 import ctypes
-from .ws import Socket
-from .types import *
+from ..types import *
 
-# Based off of this file:
-# https://github.com/GoXLR-on-Linux/goxlr-utility/blob/f2a5c1b22080c7cfb2a096efde23913a149b657a/ipc/src/lib.rs
 
+class GoXLRCommands:
+    # GoXLR commands
 
-class GoXLR(Socket):
-    def __init__(self, host="localhost", port=14564):
-        super().__init__(host, port)
-
-    # General commands
+    async def __send_command(self, payload, serial=None):
+        payload = {"Command": [serial or self.serial, payload]}
+        return await self.send(payload)
 
-    async def ping(self):
+    async def set_shutdown_commands(self, *methods):
         """
-        Pings the GoXLR Utility daemon
+        Set the commands to be executed when the GoXLR is shutting down.
+        Commands are accepted as a list of lists, where the first item is
+        the method name and the remaining items are the arguments for that
+        method.
+
+        :param methods: A list of methods to be executed when the GoXLR is shutting down.
+        :type methods: list
+        :return: The response from the GoXLR.
+        :rtype: dict or str
+
+        :Example:
+
+        >>> await xlr.set_shutdown_commands(
+        ...     ["SetFader", FaderName.A, ChannelName.Headphones]
+        ... )
         """
-        return await self.send("Ping")
-
-    async def get_status(self):
-        return await self.send("GetStatus")
-
-    # Daemon commands
-
-    async def __send_daemon(self, payload):
-        payload = {"Daemon": payload}
-        return await self.send(payload)
 
-    async def open_ui(self):
-        return await self.__send_daemon("OpenUi")
+        # Initialize the command dictionary
+        command = {"SetShutdownCommands": []}
 
-    async def activate(self):
-        return await self.__send_daemon("Activate")
+        # Iterate over the provided methods
+        for method in methods:
+            if not isinstance(method, list):
+                raise TypeError("Methods must be provided as a list")
 
-    async def stop_daemon(self):
-        return await self.__send_daemon("StopDaemon")
+            # Extract the method name and arguments
+            method_name, *args = method
+            args = [arg.name if isinstance(arg, Enum) else arg for arg in args]
 
-    async def open_path(self, pathType: PathTypes):
-        return await self.__send_daemon({"OpenPath": pathType.name})
+            # Create a dictionary for the method and arguments
+            method_dict = {method_name: args}
 
-    async def set_log_level(self, logLevel: LogLevel):
-        return await self.__send_daemon({"SetLogLevel": logLevel.name})
+            # Append the method dictionary to the command
+            command["SetShutdownCommands"].append(method_dict)
 
-    async def set_show_tray_icon(self, enabled: bool):
-        return await self.__send_daemon({"SetShowTrayIcon": enabled})
-
-    async def set_tts_enabled(self, enabled: bool):
-        return await self.__send_daemon({"SetTTSEnabled": enabled})
-
-    async def set_auto_start_enabled(self, enabled: bool):
-        return await self.__send_daemon({"SetAutoStartEnabled": enabled})
-
-    async def set_allow_network_access(self, enabled: bool):
-        return await self.__send_daemon({"SetAllowNetworkAccess": enabled})
-
-    async def recover_defaults(self, pathType: PathTypes):
-        return await self.__send_daemon({"RecoverDefaults": pathType.name})
-
-    # GoXLR commands
-
-    async def __send_command(self, payload, serial=None):
-        payload = {"Command": [serial or self.serial, payload]}
-        return await self.send(payload)
-
-    async def set_shutdown_commands(self, *commands):
-        # I'm not sure how this works in the API, so I'm just going to leave it for now
-        # Plus I don't know how I'd make it work with the rest of my wrapper yet
-        pass
+        return await self.__send_command(command)
 
     async def set_sampler_pre_buffer_duration(self, duration: ctypes.c_uint16):
         return await self.__send_command({"SetSamplerPreBufferDuration": duration})
 
-    async def set_fader(self, fader_name: FaderName, channel_name: ChannelName):
-        return await self.__send_command(
-            {"SetFader": [fader_name.name, channel_name.name]}
-        )
+    async def set_fader(self, fader: Fader, channel: Channel):
+        return await self.__send_command({"SetFader": [fader.name, channel.name]})
 
-    async def set_fader_mute_function(
-        self, fader_name: FaderName, mute_function: MuteFunction
-    ):
+    async def set_fader_mute_function(self, fader: Fader, mute_function: MuteFunction):
         return await self.__send_command(
-            {"SetFaderMuteFunction": [fader_name.name, mute_function.name]}
+            {"SetFaderMuteFunction": [fader.name, mute_function.name]}
         )
 
-    async def set_volume(self, channel_name: ChannelName, volume: ctypes.c_uint8):
-        return await self.__send_command({"SetVolume": [channel_name.name, volume]})
+    async def set_volume(self, channel: Channel, volume: ctypes.c_uint8):
+        return await self.__send_command({"SetVolume": [channel.name, volume]})
 
     async def set_microphone_type(self, microphone_type: MicrophoneType):
         return await self.__send_command({"SetMicrophoneType": microphone_type.name})
 
     async def set_microphone_gain(
         self, microphone_type: MicrophoneType, gain: ctypes.c_uint16
     ):
@@ -112,48 +88,48 @@
 
     # Bleep Button
     async def set_swear_button_volume(self, volume: ctypes.c_int8):
         return await self.__send_command({"SetSwearButtonVolume": volume})
 
     # EQ Settings
     async def set_eq_mini_gain(
-        self, mini_eq_frequency: MiniEqFrequencies, gain: ctypes.c_int8
+        self, mini_eq_frequency: MiniEqFrequency, gain: ctypes.c_int8
     ):
         return await self.__send_command(
             {"SetEqMiniGain": [mini_eq_frequency.name, gain]}
         )
 
     async def set_eq_mini_frequency(
-        self, mini_eq_frequency: MiniEqFrequencies, frequency: ctypes.c_float
+        self, mini_eq_frequency: MiniEqFrequency, frequency: ctypes.c_float
     ):
         return await self.__send_command(
             {"SetEqMiniFrequency": [mini_eq_frequency.name, frequency]}
         )
 
-    async def set_eq_gain(self, eq_frequency: EqFrequencies, gain: ctypes.c_int8):
+    async def set_eq_gain(self, eq_frequency: EqFrequency, gain: ctypes.c_int8):
         return await self.__send_command({"SetEqGain": [eq_frequency.name, gain]})
 
     async def set_eq_frequency(
-        self, eq_frequency: EqFrequencies, frequency: ctypes.c_float
+        self, eq_frequency: EqFrequency, frequency: ctypes.c_float
     ):
         return await self.__send_command(
             {"SetEqFrequency": [eq_frequency.name, frequency]}
         )
 
     # Gate Settings
     async def set_gate_threshold(self, gate_threshold: ctypes.c_int8):
         return await self.__send_command({"SetGateThreshold": gate_threshold})
 
     async def set_gate_attenuation(self, gate_attenuation: ctypes.c_uint8):
         return await self.__send_command({"SetGateAttenuation": gate_attenuation})
 
-    async def set_gate_attack(self, gate_attack: GateTimes):
+    async def set_gate_attack(self, gate_attack: GateTime):
         return await self.__send_command({"SetGateAttack": gate_attack.name})
 
-    async def set_gate_release(self, gate_release: GateTimes):
+    async def set_gate_release(self, gate_release: GateTime):
         return await self.__send_command({"SetGateRelease": gate_release.name})
 
     async def set_gate_active(self, gate_active: bool):
         return await self.__send_command({"SetGateActive": gate_active})
 
     # Compressor Settings
     async def set_compressor_threshold(self, compressor_threshold: ctypes.c_int8):
@@ -179,18 +155,18 @@
     async def set_compressor_makeup_gain(self, compressor_makeup_gain: ctypes.c_int8):
         return await self.__send_command(
             {"SetCompressorMakeupGain": compressor_makeup_gain}
         )
 
     # Used to switch between display modes
     async def set_element_display_mode(
-        self, display_mode_components: DisplayModeComponents, display_mode: DisplayMode
+        self, display_mode_component: DisplayModeComponent, display_mode: DisplayMode
     ):
         return await self.__send_command(
-            {"SetElementDisplayMode": [display_mode_components.name, display_mode.name]}
+            {"SetElementDisplayMode": [display_mode_component.name, display_mode.name]}
         )
 
     # DeEss
     async def set_deeser(self, deesser: ctypes.c_uint8):
         return await self.__send_command({"SetDeesser": deesser})
 
     # Colour Related Settings
@@ -208,88 +184,82 @@
             {"SetAnimationWaterfall": waterfall_direction.name}
         )
 
     async def set_global_colour(self, colour: str):
         return await self.__send_command({"SetGlobalColour": colour})
 
     async def set_fader_display_style(
-        self, fader_name: FaderName, fader_display_style: FaderDisplayStyle
+        self, fader: Fader, fader_display_style: FaderDisplayStyle
     ):
         return await self.__send_command(
-            {"SetFaderDisplayStyle": [fader_name.name, fader_display_style.name]}
+            {"SetFaderDisplayStyle": [fader.name, fader_display_style.name]}
         )
 
-    async def set_fader_colours(
-        self, fader_name: FaderName, colour1: str, colour2: str
-    ):
+    async def set_fader_colours(self, fader: Fader, colour1: str, colour2: str):
         return await self.__send_command(
-            {"SetFaderColours": [fader_name.name, colour1, colour2]}
+            {"SetFaderColours": [fader.name, colour1, colour2]}
         )
 
     async def set_all_fader_colours(self, colour1: str, colour2: str):
         return await self.__send_command({"SetAllFaderColours": [colour1, colour2]})
 
     async def set_all_fader_display_style(self, fader_display_style: FaderDisplayStyle):
         return await self.__send_command(
             {"SetAllFaderDisplayStyle": fader_display_style.name}
         )
 
     async def set_button_colours(
-        self, button_name: Button, colour1: str, colour2: str = None
+        self, button: Button, colour1: str, colour2: str = None
     ):
         return await self.__send_command(
-            {"SetButtonColours": [button_name.name, colour1, colour2]}
+            {"SetButtonColours": [button.name, colour1, colour2]}
         )
 
     async def set_button_off_style(
-        self, button_name: Button, off_style: ButtonColourOffStyle
+        self, button: Button, off_style: ButtonColourOffStyle
     ):
         return await self.__send_command(
-            {"SetButtonOffStyle": [button_name.name, off_style.name]}
+            {"SetButtonOffStyle": [button.name, off_style.name]}
         )
 
     async def set_button_group_colours(
         self,
-        button_colour_groups: ButtonColourGroups,
+        button_colour_group: ButtonColourGroup,
         colour1: str,
         colour2: str = None,
     ):
         return await self.__send_command(
-            {"SetButtonGroupColours": [button_colour_groups.name, colour1, colour2]}
+            {"SetButtonGroupColours": [button_colour_group.name, colour1, colour2]}
         )
 
     async def set_button_group_off_style(
-        self, button_colour_groups: ButtonColourGroups, off_style: ButtonColourOffStyle
+        self, button_colour_group: ButtonColourGroup, off_style: ButtonColourOffStyle
     ):
         return await self.__send_command(
-            {"SetButtonGroupOffStyle": [button_colour_groups.name, off_style.name]}
+            {"SetButtonGroupOffStyle": [button_colour_group.name, off_style.name]}
         )
 
     async def set_simple_colour(
-        self, simple_colour_targets: SimpleColourTargets, colour: str
+        self, simple_colour_target: SimpleColourTarget, colour: str
     ):
         return await self.__send_command(
-            {"SetSimpleColour": [simple_colour_targets.name, colour]}
+            {"SetSimpleColour": [simple_colour_target.name, colour]}
         )
 
-    async def set_encoder_colour(self, encoder_name: EncoderColourTargets, colour: str):
-        return await self.__send_command(
-            {"SetEncoderColour": [encoder_name.name, colour]}
-        )
+    async def set_encoder_colour(self, encoder: EncoderColourTarget, colour: str):
+        return await self.__send_command({"SetEncoderColour": [encoder.name, colour]})
 
-    async def set_sample_colour(self, sample_name: SamplerColourTargets, colour: str):
-        return await self.__send_command(
-            {"SetSampleColour": [sample_name.name, colour]}
-        )
+    async def set_sample_colour(self, sample: SamplerColourTarget, colour: str):
+        return await self.__send_command({"SetSampleColour": [sample.name, colour]})
 
     async def set_sample_off_style(
-        self, sample_name: SamplerColourTargets, off_style: ButtonColourOffStyle
+        self, sample: SamplerColourTarget, off_style: ButtonColourOffStyle
     ):
         return await self.__send_command(
-            {"SetSampleOffStyle": [sample_name.name, off_style.name]}
+            {"SetSampleOffStyle": [sample.name, off_style.name]}
         )
 
     # Effect Related Settings
     async def load_effect(self, effect_name: str):
         return await self.__send_command({"LoadEffect": effect_name})
 
     async def rename_active_preset(self, new_name: str):
@@ -455,133 +425,133 @@
     # Sampler
     async def clear_sample_process_error(self):
         return await self.__send_command({"ClearSampleProcessError": []})
 
     async def set_sampler_function(
         self,
         sample_bank: SampleBank,
-        sample_buttons: SampleButtons,
+        sample_button: SampleButton,
         sample_playback_mode: SamplePlaybackMode,
     ):
         return await self.__send_command(
             {
                 "SetSamplerFunction": [
                     sample_bank.name,
-                    sample_buttons.name,
+                    sample_button.name,
                     sample_playback_mode.name,
                 ]
             }
         )
 
     async def set_sampler_order(
         self,
         sample_bank: SampleBank,
-        sample_buttons: SampleButtons,
+        sample_button: SampleButton,
         sample_play_order: SamplePlayOrder,
     ):
         return await self.__send_command(
             {
                 "SetSamplerOrder": [
                     sample_bank.name,
-                    sample_buttons.name,
+                    sample_button.name,
                     sample_play_order.name,
                 ]
             }
         )
 
     async def add_sample(
-        self, sample_bank: SampleBank, sample_buttons: SampleButtons, sample_name: str
+        self, sample_bank: SampleBank, sample_button: SampleButton, sample_name: str
     ):
         return await self.__send_command(
-            {"AddSample": [sample_bank.name, sample_buttons.name, sample_name]}
+            {"AddSample": [sample_bank.name, sample_button.name, sample_name]}
         )
 
     async def set_sample_start_percent(
         self,
         sample_bank: SampleBank,
-        sample_buttons: SampleButtons,
+        sample_button: SampleButton,
         index: int,
         sample_start_percent: ctypes.c_float,
     ):
         return await self.__send_command(
             {
                 "SetSampleStartPercent": [
                     sample_bank.name,
-                    sample_buttons.name,
+                    sample_button.name,
                     index,
                     sample_start_percent,
                 ]
             }
         )
 
     async def set_sample_stop_percent(
         self,
         sample_bank: SampleBank,
-        sample_buttons: SampleButtons,
+        sample_button: SampleButton,
         index: int,
         sample_stop_percent: ctypes.c_float,
     ):
         return await self.__send_command(
             {
                 "SetSampleStopPercent": [
                     sample_bank.name,
-                    sample_buttons.name,
+                    sample_button.name,
                     index,
                     sample_stop_percent,
                 ]
             }
         )
 
     async def remove_sample_by_index(
-        self, sample_bank: SampleBank, sample_buttons: SampleButtons, index: int
+        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
     ):
         return await self.__send_command(
-            {"RemoveSampleByIndex": [sample_bank.name, sample_buttons.name, index]}
+            {"RemoveSampleByIndex": [sample_bank.name, sample_button.name, index]}
         )
 
     async def play_sample_by_index(
-        self, sample_bank: SampleBank, sample_buttons: SampleButtons, index: int
+        self, sample_bank: SampleBank, sample_button: SampleButton, index: int
     ):
         return await self.__send_command(
-            {"PlaySampleByIndex": [sample_bank.name, sample_buttons.name, index]}
+            {"PlaySampleByIndex": [sample_bank.name, sample_button.name, index]}
         )
 
     async def play_next_sample(
-        self, sample_bank: SampleBank, sample_buttons: SampleButtons
+        self, sample_bank: SampleBank, sample_button: SampleButton
     ):
         return await self.__send_command(
-            {"PlayNextSample": [sample_bank.name, sample_buttons.name]}
+            {"PlayNextSample": [sample_bank.name, sample_button.name]}
         )
 
     async def stop_sample_playback(
-        self, sample_bank: SampleBank, sample_buttons: SampleButtons
+        self, sample_bank: SampleBank, sample_button: SampleButton
     ):
         return await self.__send_command(
-            {"StopSamplePlayback": [sample_bank.name, sample_buttons.name]}
+            {"StopSamplePlayback": [sample_bank.name, sample_button.name]}
         )
 
     # Scribbles
-    async def set_scribble_icon(self, fader_name: FaderName, scribble_icon: str = None):
+    async def set_scribble_icon(self, fader: Fader, scribble_icon: str = None):
         return await self.__send_command(
-            {"SetScribbleIcon": [fader_name.name, scribble_icon]}
+            {"SetScribbleIcon": [fader.name, scribble_icon]}
         )
 
-    async def set_scribble_text(self, fader_name: FaderName, scribble_text: str):
+    async def set_scribble_text(self, fader: Fader, scribble_text: str):
         return await self.__send_command(
-            {"SetScribbleText": [fader_name.name, scribble_text]}
+            {"SetScribbleText": [fader.name, scribble_text]}
         )
 
-    async def set_scribble_number(self, fader_name: FaderName, scribble_number: str):
+    async def set_scribble_number(self, fader: Fader, scribble_number: str):
         return await self.__send_command(
-            {"SetScribbleNumber": [fader_name.name, scribble_number]}
+            {"SetScribbleNumber": [fader.name, scribble_number]}
         )
 
-    async def set_scribble_invert(self, fader_name: FaderName, scribble_invert: bool):
+    async def set_scribble_invert(self, fader: Fader, scribble_invert: bool):
         return await self.__send_command(
-            {"SetScribbleInvert": [fader_name.name, scribble_invert]}
+            {"SetScribbleInvert": [fader.name, scribble_invert]}
         )
 
     # Profile Handling
     async def new_profile(self, profile_name: str):
         return await self.__send_command({"NewProfile": profile_name})
 
     async def load_profile(self, profile_name: str, save_changes: bool = False):
@@ -620,15 +590,15 @@
     async def set_mute_hold_duration(self, mute_hold_duration: ctypes.c_uint16):
         return await self.__send_command({"SetMuteHoldDuration": mute_hold_duration})
 
     async def set_vc_mute_also_mute_cm(self, vc_mute_also_mute_cm: bool):
         return await self.__send_command({"SetVCMuteAlsoMuteCM": vc_mute_also_mute_cm})
 
     # These control the current GoXLR state
-    async def set_active_effect_preset(self, active_effect_preset: EffectBankPresets):
+    async def set_active_effect_preset(self, active_effect_preset: EffectBankPreset):
         return await self.__send_command(
             {"SetActiveEffectPreset": active_effect_preset.name}
         )
 
     async def set_active_sampler_bank(self, active_sampler_bank: SampleBank):
         return await self.__send_command(
             {"SetActiveSamplerBank": active_sampler_bank.name}
@@ -642,37 +612,31 @@
 
     async def set_hardtune_enabled(self, hardtune_enabled: bool):
         return await self.__send_command({"SetHardTuneEnabled": hardtune_enabled})
 
     async def set_fx_enabled(self, fx_enabled: bool):
         return await self.__send_command({"SetFXEnabled": fx_enabled})
 
-    async def set_fader_mute_state(self, fader_name: FaderName, mute_state: MuteState):
+    async def set_fader_mute_state(self, fader: Fader, mute_state: MuteState):
         return await self.__send_command(
-            {"SetFaderMuteState": [fader_name.name, mute_state.name]}
+            {"SetFaderMuteState": [fader.name, mute_state.name]}
         )
 
     async def set_cough_mute_state(self, mute_state: MuteState):
         return await self.__send_command({"SetCoughMuteState": mute_state.name})
 
     # Submix commands
     async def set_submix_enabled(self, enabled: bool):
         return await self.__send_command({"SetSubMixEnabled": enabled})
 
-    async def set_submix_volume(
-        self, channel_name: ChannelName, volume: ctypes.c_uint8
-    ):
-        return await self.__send_command(
-            {"SetSubMixVolume": [channel_name.name, volume]}
-        )
+    async def set_submix_volume(self, channel: Channel, volume: ctypes.c_uint8):
+        return await self.__send_command({"SetSubMixVolume": [channel.name, volume]})
 
-    async def set_submix_linked(self, channel_name: ChannelName, linked: bool):
-        return await self.__send_command(
-            {"SetSubMixLinked": [channel_name.name, linked]}
-        )
+    async def set_submix_linked(self, channel: Channel, linked: bool):
+        return await self.__send_command({"SetSubMixLinked": [channel.name, linked]})
 
     async def set_submix_output_mix(self, output_device: OutputDevice, mix: Mix):
         return await self.__send_command(
             {"SetSubMixOutputMix": [output_device.name, mix.name]}
         )
 
     # Mix monitoring
```

### Comparing `goxlr-1.0.5/goxlr/types.py` & `goxlr-1.1.0/goxlr/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# Based off of this file:
-# https://github.com/GoXLR-on-Linux/goxlr-utility/blob/main/types/src/lib.rs
-
 from enum import Enum
 
 
-class PathTypes(Enum):
+class PathType(Enum):
     Profiles = 1
     MicProfiles = 2
     Presets = 3
     Samples = 4
     Icons = 5
     Logs = 6
 
@@ -18,15 +15,15 @@
     Error = 2
     Warn = 3
     Info = 4
     Debug = 5
     Trace = 6
 
 
-class ChannelName(Enum):
+class Channel(Enum):
     Mic = 1
     LineIn = 2
     Console = 3
     System = 4
     Game = 5
     Chat = 6
     Sample = 7
@@ -37,33 +34,33 @@
 
 
 class Mix(Enum):
     A = 1
     B = 2
 
 
-class SubMixChannelName(Enum):
+class SubMixChannel(Enum):
     Mic = 1
     LineIn = 2
     Console = 3
     System = 4
     Game = 5
     Chat = 6
     Sample = 7
     Music = 8
 
 
-class FaderName(Enum):
+class Fader(Enum):
     A = 1
     B = 2
     C = 3
     D = 4
 
 
-class EncoderName(Enum):
+class Encoder(Enum):
     Pitch = 1
     Gender = 2
     Reverb = 3
     Echo = 4
 
 
 class OutputDevice(Enum):
@@ -267,37 +264,37 @@
     SamplerTopLeft = 20
     SamplerTopRight = 21
     SamplerBottomLeft = 22
     SamplerBottomRight = 23
     SamplerClear = 24
 
 
-class SimpleColourTargets(Enum):
+class SimpleColourTarget(Enum):
     Global = 1
     Accent = 2
     Scribble1 = 3
     Scribble2 = 4
     Scribble3 = 5
     Scribble4 = 6
 
 
-class SamplerColourTargets(Enum):
+class SamplerColourTarget(Enum):
     SamplerSelectA = 1
     SamplerSelectB = 2
     SamplerSelectC = 3
 
 
-class EncoderColourTargets(Enum):
+class EncoderColourTarget(Enum):
     Reverb = 1
     Pitch = 2
     Echo = 3
     Gender = 4
 
 
-class ButtonColourGroups(Enum):
+class ButtonColourGroup(Enum):
     FaderMute = 1
     EffectSelector = 2
     EffectTypes = 3
 
 
 class ButtonColourOffStyle(Enum):
     Dimmed = 1
@@ -315,39 +312,39 @@
 
 class MicrophoneType(Enum):
     Dynamic = 1
     Condenser = 2
     Jack = 3
 
 
-class EffectBankPresets(Enum):
+class EffectBankPreset(Enum):
     Preset1 = 1
     Preset2 = 2
     Preset3 = 3
     Preset4 = 4
     Preset5 = 5
     Preset6 = 6
 
 
 class SampleBank(Enum):
     A = 1
     B = 2
     C = 3
 
 
-class MiniEqFrequencies(Enum):
+class MiniEqFrequency(Enum):
     Equalizer90Hz = 1
     Equalizer250Hz = 2
     Equalizer500Hz = 3
     Equalizer1KHz = 4
     Equalizer3KHz = 5
     Equalizer8KHz = 6
 
 
-class EqFrequencies(Enum):
+class EqFrequency(Enum):
     Equalizer31Hz = 1
     Equalizer63Hz = 2
     Equalizer125Hz = 3
     Equalizer250Hz = 4
     Equalizer500Hz = 5
     Equalizer1KHz = 6
     Equalizer2KHz = 7
@@ -370,15 +367,15 @@
     Ratio5_6 = 11
     Ratio8_0 = 12
     Ratio16_0 = 13
     Ratio32_0 = 14
     Ratio64_0 = 15
 
 
-class GateTimes(Enum):
+class GateTime(Enum):
     Gate10ms = 1
     Gate20ms = 2
     Gate30ms = 3
     Gate40ms = 4
     Gate50ms = 5
     Gate60ms = 6
     Gate70ms = 7
@@ -529,15 +526,15 @@
     All = 1
     Music = 2
     Game = 3
     LineIn = 4
     System = 5
 
 
-class SampleButtons(Enum):
+class SampleButton(Enum):
     TopLeft = 1
     TopRight = 2
     BottomLeft = 3
     BottomRight = 4
 
 
 class SamplePlaybackMode(Enum):
@@ -555,15 +552,15 @@
 
 
 class DisplayMode(Enum):
     Simple = 1
     Advanced = 2
 
 
-class DisplayModeComponents(Enum):
+class DisplayModeComponent(Enum):
     NoiseGate = 1
     Equaliser = 2
     Compressor = 3
     EqFineTune = 4
 
 
 class MuteState(Enum):
```

### Comparing `goxlr-1.0.5/goxlr/ws.py` & `goxlr-1.1.0/goxlr/socket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# connect to ws://localhost:14564/api/websocket
-# make sure to send a heartbeat every 5 seconds
-# make into a class
-
 import asyncio
 import websockets
 import json
 
+from .commands import *
+
 from .error import DaemonError
 
 
 class Socket:
     def __init__(self, host, port):
         self.host = host
         self.port = port
@@ -54,18 +52,31 @@
             if data.get("Error"):
                 raise DaemonError(data.get("Error"))
 
     async def receive(self):
         response = await self.socket.recv()
         return json.loads(response)
 
+    async def open(self):
+        return await self.connect()
+
     async def close(self):
         await self.socket.close()
         self.heartbeat_task.cancel()
         return self.socket.closed
 
     async def __aenter__(self):
         await self.connect()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
+
+
+class GoXLR(Socket, GeneralCommands, DaemonCommands, GoXLRCommands):
+    """
+    Bundles all functions across all command classes into one class. Inherits from Socket.
+    It is recommended to use this class instead of Socket.
+    """
+
+    def __init__(self, host="localhost", port=14564):
+        super().__init__(host, port)
```

### Comparing `goxlr-1.0.5/goxlr.egg-info/PKG-INFO` & `goxlr-1.1.0/goxlr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,43 +15,50 @@
 
  [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
 
 A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
 
 ## Features
 - Asynchronous connection to the GoXLR utility daemon
-- Almost all methods have been translated to Python
+- All methods have been translated to Python
 - Handy enumerators for everything
 - Very simple and easy to get started
 
 ## Installation
 ```shell
 pip install goxlr
 ```
 
 ## Getting Started
 Here's some sample code to get started with this package that pings the utility's daemon.
 ```py
 import asyncio
+
 from goxlr import GoXLR
+from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
-        print(await xlr.ping())
+        await xlr.set_fader(Fader.A, Channel.Headphones)
+        await xlr.set_volume(Channel.Headphones, 0.5)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
+
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
 async def main():
     xlr = GoXLR()
-    xlr.connect()
-    print(await xlr.ping())
-    xlr.close()
+    await xlr.open()
+
+    ping = await xlr.ping()
+    print(ping)  # Ok
+
+    await xlr.close()
 ```
 
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
 
 ## Documentation
 Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.0.5/setup.py` & `goxlr-1.1.0/setup.py`

 * *Files identical despite different names*

