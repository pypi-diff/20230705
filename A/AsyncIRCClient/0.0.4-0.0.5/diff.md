# Comparing `tmp/AsyncIRCClient-0.0.4.tar.gz` & `tmp/AsyncIRCClient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncIRCClient-0.0.4.tar", last modified: Wed Jun 14 13:58:15 2023, max compression
+gzip compressed data, was "AsyncIRCClient-0.0.5.tar", last modified: Wed Jul  5 15:13:04 2023, max compression
```

## Comparing `AsyncIRCClient-0.0.4.tar` & `AsyncIRCClient-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.512573 AsyncIRCClient-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.510490 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/
--rw-rw-rw-   0        0        0     1339 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 13:58:15.000000 AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1339 2023-06-14 13:58:15.512573 AsyncIRCClient-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 13:58:15.511574 AsyncIRCClient-0.0.4/async_irc_client/
--rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.4/async_irc_client/__init__.py
--rw-rw-rw-   0        0        0    32657 2023-06-14 13:57:07.000000 AsyncIRCClient-0.0.4/async_irc_client/async_irc_client.py
--rw-rw-rw-   0        0        0       42 2023-06-14 13:58:15.513574 AsyncIRCClient-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      460 2023-06-14 13:57:29.000000 AsyncIRCClient-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:13:04.682341 AsyncIRCClient-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-05 15:13:04.678339 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/
+-rw-rw-rw-   0        0        0     1339 2023-07-05 15:13:04.000000 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-05 15:13:04.000000 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 15:13:04.000000 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 15:13:04.000000 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 15:13:04.000000 AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2023-07-05 15:13:04.681344 AsyncIRCClient-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 15:13:04.680341 AsyncIRCClient-0.0.5/async_irc_client/
+-rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.5/async_irc_client/__init__.py
+-rw-rw-rw-   0        0        0    34802 2023-07-05 15:11:15.000000 AsyncIRCClient-0.0.5/async_irc_client/async_irc_client.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 15:13:04.682341 AsyncIRCClient-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-07-05 15:13:01.000000 AsyncIRCClient-0.0.5/setup.py
```

### Comparing `AsyncIRCClient-0.0.4/AsyncIRCClient.egg-info/PKG-INFO` & `AsyncIRCClient-0.0.5/AsyncIRCClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.4/PKG-INFO` & `AsyncIRCClient-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.4/README.md` & `AsyncIRCClient-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `AsyncIRCClient-0.0.4/async_irc_client/async_irc_client.py` & `AsyncIRCClient-0.0.5/async_irc_client/async_irc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from asyncio import transports
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Union, Callable, Any, Coroutine
-
+import datetime
 from loguru import logger
 
 
 def is_event_loop_running() -> bool:
     """
     check if asyncio has loop running
     :return: bool
@@ -14,14 +14,47 @@
     try:
         loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
         return loop.is_running()
     except RuntimeError as _error:
         return False
 
 
+def get_time_difference(time_str: str) -> float:
+    """
+    get time difference
+    :param time_str:
+    :return:
+    """
+    now = datetime.datetime.now().time()
+
+    # Parse the target time from the input string
+    target_time = datetime.datetime.strptime(time_str, '%H:%M').time()
+
+    # Calculate the time difference between now and the target time
+    time_diff = datetime.datetime.combine(datetime.date.today(), target_time) - datetime.datetime.combine(
+        datetime.date.today(), now)
+
+    # If the target time has already passed today, calculate the time difference for tomorrow
+    if time_diff.total_seconds() < 0:
+        tomorrow = datetime.date.today() + datetime.timedelta(days=1)
+        time_diff = datetime.datetime.combine(tomorrow, target_time) - datetime.datetime.combine(
+            datetime.date.today(), now)
+
+    return time_diff.total_seconds()
+
+
+@dataclass
+class CommandCallback(object):
+    name: str
+    callback: Callable
+    mod_only: bool = False
+    aliases: list[str] = field(default_factory=lambda: [])
+    case_sensitive: bool = True
+
+
 @dataclass
 class Command(object):
     command: Union[None, str] = None
     channel: Union[None, str] = None
     channel_raw: Union[None, str] = None
     bot_command: Union[None, str] = None
     bot_command_params: Union[None, str] = None
@@ -571,15 +604,16 @@
     async def on_raid(self, message: Message) -> None:
         """called on raid event (msg-id == raid)"""
 
 
 class TwitchIRCBot(IRCClient, TwitchIRCBotInterfaceMixin):
     TWITCH_IRC_SERVER: str = "irc.chat.twitch.tv"
     TWITCH_IRC_PORT: int = 6667
-    command_callbacks: dict[str, tuple[bool, Callable]] = {}
+    command_callbacks: dict[str, CommandCallback] = {}
+    case_insensitive: list[str] = []
     tasks: list[Callable] = []
     _running_tasks: list[Callable] = []
 
     def __init__(self, oauth_token: str, nick_name: str, channel: str, timeout: int = 500, **kwargs):
         """
         constructor
         :param oauth_token: oauth token
@@ -600,22 +634,27 @@
         self._has_commands: bool = False
         self._has_tags: bool = False
         self._timeout: int = timeout
         self._disconnect_timer: Timer = Timer(self._timeout, self._on_disconnect_timer_timeout)
         self._pong_response_timer: Timer = Timer(20, self._on_pong_response_timer_timeout)
 
     @staticmethod
-    def command(name: str, mod_only: bool = False):
+    def command(name: str, mod_only: bool = False, aliases: list[str] = None, case_sensitive: bool = True):
         """
         registers function in command table
         :param name: name to register as
         :param mod_only: is command mod only
+        :param aliases: alternative names
+        :param case_sensitive: case-sensitive commands
         :return: decorator
         """
 
+        if aliases is None:
+            aliases = []
+
         def decorator(function):
             """
             Decorator function to wrap the original function and add it to the command table.
 
             :param function: The function to be wrapped.
             :return: The wrapper function.
             """
@@ -626,25 +665,35 @@
 
                 :param args: Positional arguments passed to the function.
                 :param kwargs: Keyword arguments passed to the function.
                 :return: The result of the original function.
                 """
                 return await function(*args, **kwargs)
 
-            TwitchIRCBot.command_callbacks[name] = (mod_only, wrapper)
+            command_callback: CommandCallback = CommandCallback(name, wrapper, mod_only, aliases, case_sensitive)
+
+            TwitchIRCBot.command_callbacks[name] = command_callback
+
+            if not case_sensitive:
+                TwitchIRCBot.case_insensitive.append(name.lower())
+
+            for alias in aliases:
+                TwitchIRCBot.command_callbacks[alias] = command_callback
+                TwitchIRCBot.case_insensitive.append(alias.lower())
 
             return wrapper
 
         return decorator
 
     @staticmethod
-    def loop(seconds: int):
+    def loop(seconds: int = 0, time: str = None):
         """
         repeat function in given intervals
         :param seconds: seconds
+        :param time: time to repeat function at (for example 12:00)
         :return: None
         """
 
         def decorator(function: Callable):
             """
             decorator
             :param function: functon to decorate
@@ -656,15 +705,19 @@
                 wrapper function
                 :param args: args
                 :param kwargs: kwargs
                 :return: None
                 """
                 while True:
                     await function(*args, **kwargs)
-                    await asyncio.sleep(seconds)
+
+                    if time is None:
+                        await asyncio.sleep(seconds)
+                    else:
+                        await asyncio.sleep(get_time_difference(time))
 
             TwitchIRCBot.tasks.append(wrapper)
 
             return wrapper
 
         return decorator
 
@@ -716,24 +769,28 @@
         # is not a command
         if not message.parameters.startswith("!"):
             return
 
         # split after '!'
         command_parts: list[str] = message.parameters[1:].split()
         command_name: str = command_parts[0]
-        command_data: tuple[bool, Callable] = TwitchIRCBot.command_callbacks.get(command_name)
 
-        if command_data is None:
+        if command_name.lower() in self.case_insensitive:
+            command_name = command_name.lower()
+
+        command_callback: CommandCallback = TwitchIRCBot.command_callbacks.get(command_name)
+
+        if command_callback is None:
             return logger.warning(f"No bound command found for: {command_parts}")
 
         # is mod only
-        if command_data[0] and not self.is_mod_or_broadcaster(message):
+        if command_callback.mod_only and not self.is_mod_or_broadcaster(message):
             return logger.debug(f"User {message.source.nick} tried to issue mod-only command: {message.parameters}")
 
-        self._loop.create_task(command_data[1](self, message))
+        self._loop.create_task(command_callback.callback(self, message))
 
     def _check_user_notice(self, message: Message) -> None:
         """
         check user notice for certain events
         :param message: message
         :return: None
         """
```

