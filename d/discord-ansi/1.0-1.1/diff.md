# Comparing `tmp/discord-ansi-1.0.tar.gz` & `tmp/discord-ansi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ansi-1.0.tar", last modified: Mon Jul  3 12:09:25 2023, max compression
+gzip compressed data, was "discord-ansi-1.1.tar", last modified: Wed Jul  5 11:46:24 2023, max compression
```

## Comparing `discord-ansi-1.0.tar` & `discord-ansi-1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.807510 discord-ansi-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-03 12:09:25.807510 discord-ansi-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-03 12:09:10.000000 discord-ansi-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/discord_ansi/
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-03 12:09:10.000000 discord-ansi-1.0/discord_ansi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/discord_ansi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 12:09:10.000000 discord-ansi-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:09:25.807510 discord-ansi-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-03 12:09:10.000000 discord-ansi-1.0/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 11:46:14.000000 discord-ansi-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-05 11:46:24.667755 discord-ansi-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-05 11:46:14.000000 discord-ansi-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/discord_ansi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-05 11:46:14.000000 discord-ansi-1.1/discord_ansi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/discord_ansi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 11:46:14.000000 discord-ansi-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:46:24.667755 discord-ansi-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-05 11:46:14.000000 discord-ansi-1.1/tests/test1.py
```

### Comparing `discord-ansi-1.0/PKG-INFO` & `discord-ansi-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 1.0
+Version: 1.1
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This package is still in development, come back when it will be fully developed!
 ================================================================================
 
 Discord ANSI messages - allows you to create Discord messages with colour in it!
 Note: Some colors may be different on Discord light theme and dark theme. I adjusted it for dark theme since it's the most used one.
 # Features
@@ -83,23 +84,25 @@
 messageBuilder.addNewline()
 # Since we don't want to change anything (like the indent level), AND we have text **before** or **after**
 # the newline, we can safely put \n in addText().
 messageBuilder.addText("Arguments: none", background="orange")
 text = messageBuilder.getText()
 # Send the message using your library
 # The most popular one is Discord.py
+# bot.login("ODk2MjgzNjExMzYyMzY1NDYw.YW1C3A.rNvidfDBqKWxD5HhgNjH4d7UsfQ") (fake token)
 # interaction.response.send_message(text)
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2. ```py
+2. Use the code below:
+```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
```

### Comparing `discord-ansi-1.0/README.md` & `discord-ansi-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,30 +72,32 @@
 messageBuilder.addNewline()
 # Since we don't want to change anything (like the indent level), AND we have text **before** or **after**
 # the newline, we can safely put \n in addText().
 messageBuilder.addText("Arguments: none", background="orange")
 text = messageBuilder.getText()
 # Send the message using your library
 # The most popular one is Discord.py
+# bot.login("ODk2MjgzNjExMzYyMzY1NDYw.YW1C3A.rNvidfDBqKWxD5HhgNjH4d7UsfQ") (fake token)
 # interaction.response.send_message(text)
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2. ```py
+2. Use the code below:
+```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
 ```py
 messageBuilder.insertANSIText(output)
 ```
 If you want a completely new message, use the from_ansi_output() function:
 ```py
 discord_ansi.from_ansi_output(output)
-```
+```
```

### Comparing `discord-ansi-1.0/discord_ansi/__init__.py` & `discord-ansi-1.1/discord_ansi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional
+from typing import Optional, Union
+from ctypes import c_char
 
 import numpy
 
 def from_ansi_output(ansi_output: str):
     """
     Make a Discord coloured message from ANSI output.
     NOTE: This function is a bare bones minimum, which just formats the string as a code block.
@@ -149,33 +150,84 @@
         Parameters
         ----------
         x : int | required
             X position
         y : int | required
             Y position
         """
-        return self.data[x][y]
+        return self.data[x][y][0]
     
     def setPixel(self, x: int, y: int, color: str):
         """
-        Gets the color of a pixel.
+        Sets the color of a pixel.
         Please note that it starts counting from 0.
         
         Parameters
         ----------
         x : int | required
             X position
         y : int | required
             Y position
         color : str | required
             A valid color
         """
         if color not in background_colors:
             raise Exception("Invalid background color! (You can only use background colors, not foreground ones!)")
-        self.data[x][y] = color
+        self.data[x][y][0] = color
+    
+    def getPixelTextColor(self, x: int, y: int):
+        """
+        Gets the color of the text inside of a pixel.
+        Please note that it starts counting from 0.
+        
+        Parameters
+        ----------
+        x : int | required
+            X position
+        y : int | required
+            Y position
+        """
+        return self.data[x][y][1]
+    
+    def setPixelTextColor(self, x: int, y: int, color: str):
+        """
+        Sets the color of the text inside of a pixel.
+        Please note that it starts counting from 0.
+        
+        Parameters
+        ----------
+        x : int | required
+            X position
+        y : int | required
+            Y position
+        color : str | required
+            A valid color
+        """
+        if color not in background_colors:
+            raise Exception("Invalid foreground color! (You can only use foreground colors for character colors!)")
+        self.data[x][y][1] = color
+    
+    def setPixelChar(self, x: int, y: int, char: Union[str, c_char]):
+        """
+        Set a character to be inside the pixel.
+        
+        Parameters
+        ----------
+        x : int | required
+            X position
+        y : int | required
+            Y position
+        char : Union[str, c_char] | required
+            The character you want to put there
+        """
+        if type(char) == c_char:
+            char = chr(char.value[0])
+        if len(char) != 1:
+            raise Exception("Must be one character!")
+        self.data[x][y][2] = char
     
     def fillSquare(self, x1: int, y1: int, x2: int, y2: int, color: str):
         """
         Makes a square, from (x1, y1) to (x2, y2) inclusive!
         Please note that it starts counting from 0.
         
         Parameters
```

### Comparing `discord-ansi-1.0/discord_ansi.egg-info/PKG-INFO` & `discord-ansi-1.1/discord_ansi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 1.0
+Version: 1.1
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This package is still in development, come back when it will be fully developed!
 ================================================================================
 
 Discord ANSI messages - allows you to create Discord messages with colour in it!
 Note: Some colors may be different on Discord light theme and dark theme. I adjusted it for dark theme since it's the most used one.
 # Features
@@ -83,23 +84,25 @@
 messageBuilder.addNewline()
 # Since we don't want to change anything (like the indent level), AND we have text **before** or **after**
 # the newline, we can safely put \n in addText().
 messageBuilder.addText("Arguments: none", background="orange")
 text = messageBuilder.getText()
 # Send the message using your library
 # The most popular one is Discord.py
+# bot.login("ODk2MjgzNjExMzYyMzY1NDYw.YW1C3A.rNvidfDBqKWxD5HhgNjH4d7UsfQ") (fake token)
 # interaction.response.send_message(text)
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2. ```py
+2. Use the code below:
+```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
```

### Comparing `discord-ansi-1.0/tests/test1.py` & `discord-ansi-1.1/tests/test1.py`

 * *Files identical despite different names*

