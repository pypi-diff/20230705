# Comparing `tmp/minecraftstatus-0.0.7.tar.gz` & `tmp/minecraftstatus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraftstatus-0.0.7.tar", max compression
+gzip compressed data, was "minecraftstatus-0.0.8.tar", max compression
```

## Comparing `minecraftstatus-0.0.7.tar` & `minecraftstatus-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1087 2022-02-24 06:09:15.254608 minecraftstatus-0.0.7/LICENSE
--rw-r--r--   0        0        0      281 2022-02-27 08:48:25.700639 minecraftstatus-0.0.7/minecraftstatus/__init__.py
--rw-r--r--   0        0        0     3814 2022-02-27 14:38:43.350799 minecraftstatus-0.0.7/minecraftstatus/client.py
--rw-r--r--   0        0        0      601 2022-02-27 08:48:25.708639 minecraftstatus-0.0.7/minecraftstatus/errors.py
--rw-r--r--   0        0        0      429 2022-02-27 08:48:25.729642 minecraftstatus-0.0.7/minecraftstatus/http.py
--rw-r--r--   0        0        0     3176 2022-02-27 08:48:25.753642 minecraftstatus-0.0.7/minecraftstatus/server_status.py
--rw-r--r--   0        0        0      472 2022-02-27 14:39:15.895352 minecraftstatus-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1022 2022-02-26 06:09:36.153211 minecraftstatus-0.0.7/README.md
--rw-r--r--   0        0        0     1709 2022-02-27 14:40:02.476575 minecraftstatus-0.0.7/setup.py
--rw-r--r--   0        0        0     1686 2022-02-27 14:40:02.476575 minecraftstatus-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/LICENSE
+-rw-r--r--   0        0        0      388 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/minecraftstatus/__init__.py
+-rw-r--r--   0        0        0     3224 2023-07-05 13:58:33.599966 minecraftstatus-0.0.8/minecraftstatus/client.py
+-rw-r--r--   0        0        0     1000 2022-03-15 12:48:24.000000 minecraftstatus-0.0.8/minecraftstatus/errors.py
+-rw-r--r--   0        0        0      429 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/minecraftstatus/http.py
+-rw-r--r--   0        0        0     3389 2023-07-05 14:21:25.086552 minecraftstatus-0.0.8/minecraftstatus/server_status.py
+-rw-r--r--   0        0        0      534 2023-07-04 13:54:18.974850 minecraftstatus-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1279 2023-07-04 13:51:09.785431 minecraftstatus-0.0.8/README.md
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 minecraftstatus-0.0.8/PKG-INFO
```

### Comparing `minecraftstatus-0.0.7/LICENSE` & `minecraftstatus-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraftstatus-0.0.7/minecraftstatus/client.py` & `minecraftstatus-0.0.8/minecraftstatus/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,86 @@
 from io import BytesIO
 
 from .server_status import ServerStatus
 from .http import HTTPClient
 from .errors import BadTextFormation, ServerNotFound
 
-__all__ = ("MCStatus",)
+__all__ = ("MCStatus", "ServerNotFound", "BadTextFormation")  # docs don't properly work without this
 base_url = "https://api.iapetus11.me/{}"
 
 
 class MCStatus(HTTPClient):
     """
     The main MCStatus class.
     """
 
     def __init__(self) -> None:
         HTTPClient.__init__(self)
 
     async def get_server(self, ip_address: str):
         """
-        Makes a request to the server status endpoint.
-
-        Parameters:
-        ----------
-        ip_address: :class:`str` IP address of the server.
-
-        Returns:
-        -------
-        ServerStatus class instance.
-
-        Attributes:
-        -----------
-        host: The host of the server.
-        port: The port of the server.
-        is_online: True if the server is online, False otherwise.
-        latency: The latency of the server.
-        max_players: The maximum players of the server.
-        online_players: The online players of the server.
-        motd: The message of the day of the server.
-        favicon: The base64 data of the favicon of the server.
-        game_map: The game map of the server.
-        game_mode: The game mode of the server.
-
-        Raises: :exc:`ServerNotFound` if the server is not found or is offline.
+        :param ip_address: IP address of the server
+        :type ip_address: :class:`str`
+        :raises ServerNotFound: server not found or is offline
+        :return: a :class:`ServerStatus` class instance
         """
 
-        resp = await self._request(
-            "GET", base_url.format(f"mc/server/status/{ip_address}")
-        )
+        resp = await self._request("GET", base_url.format(f"mc/server/status/{ip_address}"))
         data = await resp.json()
         if data["online"] is False:
             await self._close()
             raise ServerNotFound(ip_address)
+
         await self._close()
         return ServerStatus(data)
 
-    async def get_server_card(self, ip_address: str):
+    async def get_server_card(self, ip_address: str, custom_server_name: str = ""):
         """
-        Makes a request to the server-card endpoint.
-        Parameters:
-        ----------
-        ip_address: :class:`str` IP address of the server.
-
-        Returns:
-        -------
-        io.BytesIO object co-relating the server card.
-
-        Raises: :exc:`BadTextFormation` if the characters passed aren't between 1-30.
+        :param ip_address: IP address of the server
+        :param custom_server_name: A custom server name to be displayed on the server card
+        :type ip_address: :class:`str`
+        :type custom_server_name: :class:`str`
+        :raises `BadTextFormation`: text passed is not between 1-30 characters
+        :return: an :class:`io.BytesIO` object co-relating the server card image.
         """
+        if len(custom_server_name) == 0:
+            custom_server_name = ip_address
+
         if len(ip_address) > 30 and len(ip_address) < 1:
             raise BadTextFormation()
+
         res = await self._request(
-            "GET", base_url.format(f"mc/server/status/{ip_address}/image")
+            "GET", base_url.format(f"mc/server/status/{ip_address}/image?customName={custom_server_name}")
         )
         image = BytesIO(await res.read())
         await self._close()
         return image
 
     async def achievement(self, achievement: str):
         """
-        Makes a request to the achievement endpoint.
-        Parameters
-        ----------
-        achievement: :class:`str` name of the achievement to display.
-
-        Returns
-        -------
-        io.BytesIO object co-relating the achievement image.
-
-        Raises: :exc:`BadTextFormation` if the characters passed aren't between 1-30.
+        :param achievement: name of the achievement to display.
+        :type achievement: :class:`str`
+        :raises BadTextFormation: text passed is not between 1-30 characters
+        :return: an :class:`io.BytesIO` object co-relating the achievement image.
         """
         if len(achievement) > 30 and len(achievement) > 1:
             raise BadTextFormation()
-        res = await self._request(
-            "GET", base_url.format(f"mc/image/achievement/{achievement}")
-        )
+
+        res = await self._request("GET", base_url.format(f"mc/image/achievement/{achievement}"))
         image = BytesIO(await res.read())
         await self._close()
         return image
 
     async def splash_text(self, text: str):
         """
-        Makes a request to the splash text endpoint.
-        Parameters
-        ----------
-        text: :class:`str` text to display in the splash.
-
-        Returns
-        -------
-        io.BytesIO object co-relating the splash image.
-
-        Raises: :exc:`BadTextFormation` if the characters passed aren't between 1-30.
+        :param text: text to display in the splash.
+        :type text: :class:`str`
+        :raises BadTextFormation: text passed is not between 1-30 characters
+        :return: an :class:`io.BytesIO` object co-relating the splash text image.
         """
         if len(text) > 30 and len(text) < 1:
             raise BadTextFormation()
+
         res = await self._request("GET", base_url.format(f"mc/image/splash/{text}"))
         image = BytesIO(await res.read())
         await self._close()
         return image
```

### Comparing `minecraftstatus-0.0.7/README.md` & `minecraftstatus-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 
 
 An async API wrapper around [api.iapetus.me](https://github.com/Iapetus-11/api.iapetus11.me)
 
 
-### Get started
+[![CodeFactor](https://www.codefactor.io/repository/github/infernum1/minecraftstatus/badge/main)](https://www.codefactor.io/repository/github/infernum1/minecraftstatus/overview/main)
+
+### Get started || [Documentation](https://minecraftstatus.readthedocs.io/en/latest/)
 
 #### to get started, type this in your terminal
 ```
 pip install -U minecraftstatus
 ```
 
 #### or to install the main branch
 ```
 pip install -U git+https://github.com/Infernum1/minecraftstatus
 ```
-###### (make sure you have git installed)
+###### (make sure you have [git](https://gitforwindows.org) installed)
 ### Examples
 
 #### For examples, checkout the [examples directory](https://github.com/Infernum1/minecraftstatus/tree/main/examples)
 ##### If you plan to use the lib in a discord bot
 
 ```py
 import discord
@@ -32,8 +34,8 @@
   image = await client.achievement(achievement)
   file = discord.File(image, "achievement.png")
   await ctx.send(file=file)
 ```
 
 ###### these are just examples! it's upto you how you want to use this lib.
 
-### Join the [discord server](https://discord.gg/jJqJ3rjgqg) for support.
+### Add `Infernum#7041` on discord for help
```

