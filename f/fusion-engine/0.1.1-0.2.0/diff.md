# Comparing `tmp/fusion-engine-0.1.1.tar.gz` & `tmp/fusion-engine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.1.1.tar", last modified: Mon Jul  3 10:51:01 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.0.tar", last modified: Wed Jul  5 07:57:11 2023, max compression
```

## Comparing `fusion-engine-0.1.1.tar` & `fusion-engine-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:01.044057 fusion-engine-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/LICENCE.md
--rw-rw-rw-   0        0        0     4234 2023-07-03 10:51:01.035421 fusion-engine-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2964 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/README.md
--rw-rw-rw-   0        0        0     1688 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 10:51:01.045066 fusion-engine-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1055 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.801227 fusion-engine-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.956354 fusion-engine-0.1.1/src/fusion_engine.egg-info/
--rw-rw-rw-   0        0        0     4234 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 10:51:00.000000 fusion-engine-0.1.1/src/fusion_engine.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.961844 fusion-engine-0.1.1/src/fusionengine/
--rw-rw-rw-   0        0        0      871 2023-07-03 10:50:38.000000 fusion-engine-0.1.1/src/fusionengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:00.964840 fusion-engine-0.1.1/src/fusionengine/debugfiles/
--rw-rw-rw-   0        0        0     3326 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/debugfiles/test.png
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:01.033424 fusion-engine-0.1.1/src/fusionengine/files/
--rw-rw-rw-   0        0        0     2826 2023-07-03 09:35:35.000000 fusion-engine-0.1.1/src/fusionengine/files/body.py
--rw-rw-rw-   0        0        0      939 2023-07-03 09:39:18.000000 fusion-engine-0.1.1/src/fusionengine/files/color.py
--rw-rw-rw-   0        0        0      394 2023-07-03 09:40:19.000000 fusion-engine-0.1.1/src/fusionengine/files/data.py
--rw-rw-rw-   0        0        0     2442 2023-07-03 09:41:16.000000 fusion-engine-0.1.1/src/fusionengine/files/draw.py
--rw-rw-rw-   0        0        0      242 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/enums.py
--rw-rw-rw-   0        0        0    10951 2023-07-03 09:42:09.000000 fusion-engine-0.1.1/src/fusionengine/files/event.py
--rw-rw-rw-   0        0        0       96 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/exceptions.py
--rw-rw-rw-   0        0        0      928 2023-07-03 09:44:32.000000 fusion-engine-0.1.1/src/fusionengine/files/image.py
--rw-rw-rw-   0        0        0      481 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/imports.py
--rw-rw-rw-   0        0        0        0 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/physics.py
--rw-rw-rw-   0        0        0      552 2023-07-03 09:45:15.000000 fusion-engine-0.1.1/src/fusionengine/files/shape.py
--rw-rw-rw-   0        0        0     5708 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/storage.py
--rw-rw-rw-   0        0        0      788 2023-07-03 07:40:04.000000 fusion-engine-0.1.1/src/fusionengine/files/systems.py
--rw-rw-rw-   0        0        0     1759 2023-07-03 09:48:40.000000 fusion-engine-0.1.1/src/fusionengine/files/window.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.850639 fusion-engine-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/LICENCE.md
+-rw-rw-rw-   0        0        0     4234 2023-07-05 07:57:11.846676 fusion-engine-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2964 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1688 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-06-14 13:36:13.000000 fusion-engine-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:57:11.850639 fusion-engine-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1055 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.711274 fusion-engine-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.759055 fusion-engine-0.2.0/src/fusion_engine.egg-info/
+-rw-rw-rw-   0        0        0     4234 2023-07-05 07:57:11.000000 fusion-engine-0.2.0/src/fusion_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-05 07:57:11.000000 fusion-engine-0.2.0/src/fusion_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:57:11.000000 fusion-engine-0.2.0/src/fusion_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-05 07:57:11.000000 fusion-engine-0.2.0/src/fusion_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 07:57:11.000000 fusion-engine-0.2.0/src/fusion_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.761060 fusion-engine-0.2.0/src/fusionengine/
+-rw-rw-rw-   0        0        0      871 2023-07-05 07:53:19.000000 fusion-engine-0.2.0/src/fusionengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.767287 fusion-engine-0.2.0/src/fusionengine/debugfiles/
+-rw-rw-rw-   0        0        0     3326 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/debugfiles/test.png
+drwxrwxrwx   0        0        0        0 2023-07-05 07:57:11.843357 fusion-engine-0.2.0/src/fusionengine/files/
+-rw-rw-rw-   0        0        0     2835 2023-07-05 07:32:38.000000 fusion-engine-0.2.0/src/fusionengine/files/body.py
+-rw-rw-rw-   0        0        0     1452 2023-07-04 09:39:51.000000 fusion-engine-0.2.0/src/fusionengine/files/color.py
+-rw-rw-rw-   0        0        0      394 2023-07-03 10:59:50.000000 fusion-engine-0.2.0/src/fusionengine/files/data.py
+-rw-rw-rw-   0        0        0     2450 2023-07-05 07:34:19.000000 fusion-engine-0.2.0/src/fusionengine/files/draw.py
+-rw-rw-rw-   0        0        0      242 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/files/enums.py
+-rw-rw-rw-   0        0        0    10954 2023-07-05 07:33:12.000000 fusion-engine-0.2.0/src/fusionengine/files/event.py
+-rw-rw-rw-   0        0        0       96 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/files/exceptions.py
+-rw-rw-rw-   0        0        0      930 2023-07-05 07:32:53.000000 fusion-engine-0.2.0/src/fusionengine/files/image.py
+-rw-rw-rw-   0        0        0      481 2023-07-04 07:49:35.000000 fusion-engine-0.2.0/src/fusionengine/files/imports.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/files/physics.py
+-rw-rw-rw-   0        0        0      553 2023-07-05 07:29:47.000000 fusion-engine-0.2.0/src/fusionengine/files/shape.py
+-rw-rw-rw-   0        0        0     5708 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/files/storage.py
+-rw-rw-rw-   0        0        0      788 2023-07-03 07:40:04.000000 fusion-engine-0.2.0/src/fusionengine/files/systems.py
+-rw-rw-rw-   0        0        0     1904 2023-07-05 07:50:15.000000 fusion-engine-0.2.0/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.1.1/LICENCE.md` & `fusion-engine-0.2.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/PKG-INFO` & `fusion-engine-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.1.1
+Version: 0.2.0
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.1.1/README.md` & `fusion-engine-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/pyproject.toml` & `fusion-engine-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/setup.py` & `fusion-engine-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.0/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.1.1
+Version: 0.2.0
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python.
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.1.1/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.0/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENCE.md
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 src/fusion_engine.egg-info/PKG-INFO
 src/fusion_engine.egg-info/SOURCES.txt
 src/fusion_engine.egg-info/dependency_links.txt
 src/fusion_engine.egg-info/requires.txt
 src/fusion_engine.egg-info/top_level.txt
 src/fusionengine/__init__.py
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/__init__.py` & `fusion-engine-0.2.0/src/fusionengine/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Dimkauzh"
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 import fusionengine.files.data as data
 import fusionengine.files.systems as sysconfig
 
 from fusionengine.files.imports import *
 
 class Main:
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/debugfiles/test.png` & `fusion-engine-0.2.0/src/fusionengine/debugfiles/test.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/body.py` & `fusion-engine-0.2.0/src/fusionengine/files/body.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,37 +31,37 @@
         self.image = None
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.window = window
         self.gravity = 0
-        self._setBodyType(bodytype)
+        self._set_body_type(bodytype)
     
-    def openImage(self, window: window._CustomRenderer, image: image._CustomImage, x: int, y: int, width: int, height: int) -> None:
-        image.openImage(window, image, x, y, width, height)
+    def open_image(self, window: window._CustomRenderer, image: image._CustomImage, x: int, y: int, width: int, height: int) -> None:
+        image.open_image(window, image, x, y, width, height)
         self.image = image
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
 
-    def newRect(self, window: window._CustomRenderer, color: tuple) -> None:
-        data.drawRect(window,
+    def new_rect(self, window: window._CustomRenderer, color: tuple) -> None:
+        data.draw_rect(window,
                       self.x,
                       self.y,
                       self.width,
                       self.height,
                       color
                       )
-    def setGravity(self, gravity: int) -> None:
+    def set_gravity(self, gravity: int) -> None:
         self.gravity = gravity
     
-    def _setBodyType(self, bodytype: BodyType) -> None:
+    def _set_body_type(self, bodytype: BodyType) -> None:
         if bodytype == BodyType.RIGID_BODY:
             self.body = _RigidBody(self.window,
                                    self.x,
                                    self.y,
                                    self.width,
                                    self.height
                                    )
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/color.py` & `fusion-engine-0.2.0/src/fusionengine/files/color.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,7 +19,19 @@
         self.BRONZE = (205, 127, 50, 255)
         self.LIME = (0, 255, 0, 255)
         self.OLIVE = (128, 128, 0, 255)
         self.TEAL = (0, 128, 128, 255)
         self.NAVY = (0, 0, 128, 255)
         self.MAROON = (128, 0, 0, 255)
         self.INDIGO = (75, 0, 130, 255)
+        self.TURQUOISE = (64, 224, 208, 255)
+        self.VIOLET = (238, 130, 238, 255)
+        self.AQUA = (0, 255, 255, 255)
+        self.TAN = (210, 180, 140, 255)
+        self.BEIGE = (245, 245, 220, 255)
+        self.IVORY = (255, 255, 240, 255)
+        self.LAVENDER = (230, 230, 250, 255)
+        self.MINT = (189, 252, 201, 255)
+        self.SALMON = (250, 128, 114, 255)
+        self.SCARLET = (255, 36, 0, 255)
+        self.TEAL = (0, 128, 128, 255)
+        self.TOMATO = (255, 99, 71, 255)
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/draw.py` & `fusion-engine-0.2.0/src/fusionengine/files/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,53 +4,53 @@
 from fusionengine.files.imports import *
 import fusionengine.files.shape as shape
 
 class Draw:
     def __init__(self) -> None:
         self.rendereroptions = sysconfig.RendererOptions()
     
-    def drawLine(self, window: window._CustomRenderer, x1: int, y1: int, x2: int, y2: int, color: tuple) -> None:
+    def draw_line(self, window: window._CustomRenderer, x1: int, y1: int, x2: int, y2: int, color: tuple) -> None:
         SDL_SetRenderDrawColor(window.renderer,
                                color[0],
                                color[1],
                                color[2],
                                color[3]
                                )
 
         SDL_RenderDrawLine(window.renderer, x1, y1, x2, y2) 
                 
-    def drawLineRect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+    def draw_line_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
         rdr = window.renderer
         self.drawLine(rdr, x, y, x + width, y, color)
         self.drawLine(rdr, x, y + height, x + width, y + height, color)
         self.drawLine(rdr, x, y, x, y + height, color)
         self.drawLine(rdr, x + width, y, x + width, y + height, color)
         
-    def drawRect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+    def draw_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
         SDL_SetRenderDrawColor(window.renderer,
                                color[0],
                                color[1],
                                color[2],
                                color[3]
                                )
 
         rect = SDL_Rect(x, y, width, height)
         SDL_RenderFillRect(window.renderer, rect)
 
-    def drawOwnRect(self, window: window._CustomRenderer, rect: shape._CustomShape) -> None:
+    def draw_own_rect(self, window: window._CustomRenderer, rect: shape._CustomShape) -> None:
         SDL_SetRenderDrawColor(window.renderer,
                                rect.color[0],
                                rect.color[1],
                                rect.color[2],
                                rect.color[3]
                                )
 
         SDL_RenderFillRect(window.renderer, rect.rect)
     
-    def setBackgroundColor(self, window: window._CustomRenderer, color: tuple) -> None:
+    def set_background_color(self, window: window._CustomRenderer, color: tuple) -> None:
         SDL_SetRenderDrawColor(window.renderer,
                                color[0],
                                color[1],
                                color[2],
                                color[3]
                                )
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/event.py` & `fusion-engine-0.2.0/src/fusionengine/files/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fusionengine.files.imports import *
 import fusionengine.files.window as window
 
 class Event:
     def __init__(self) -> None:
         pass
 
-    def keyDown(self, key: int, window: window._CustomRenderer) -> bool:
+    def key_down(self, key: int, window: window._CustomRenderer) -> bool:
         event = window.event
         if event.type == sdl2.SDL_KEYDOWN:
             if event.key.keysym.sym == key:
                 return True
         return False
-    def keyDownOnce(self, key: int, window: window._CustomRenderer) -> bool:
+    def key_down_once(self, key: int, window: window._CustomRenderer) -> bool:
         pass
 
 
 class Keys:
     def __init__(self):
         self.KEY_UNKNOWN = sdl2.SDLK_UNKNOWN
         self.KEY_RETURN = sdl2.SDLK_RETURN
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/image.py` & `fusion-engine-0.2.0/src/fusionengine/files/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def __init__(self, window: window._CustomRenderer, texture, rect: shape._CustomShape) -> None:
         self.window = window
         self.renderer = window.renderer
         self.texture = texture
         self.rect = rect
 
 class Image: 
-    def openImage(self, window: window._CustomRenderer, image, x: int, y: int, width: int, height: int) -> _CustomImage:
+    def open_image(self, window: window._CustomRenderer, image, x: int, y: int, width: int, height: int) -> _CustomImage:
         image = sdl2.ext.load_image(image)
         texture = sdl2.SDL_CreateTextureFromSurface(window.renderer, image)
         rect = sdl2.SDL_Rect(x, y, width, height)
         return _CustomImage(window, texture, rect)
     
-    def drawImage(self, image: _CustomImage) -> None:
+    def draw_image(self, image: _CustomImage) -> None:
         sdl2.SDL_RenderClear(image.renderer)
         sdl2.SDL_RenderCopy(image.renderer, image.texture, None, image.rect)
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/shape.py` & `fusion-engine-0.2.0/src/fusionengine/files/shape.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,9 +9,9 @@
         self.color = color
         self.rect = SDL_Rect(x, y, width, height)
 
 class Shapes:
     def __init__(self) -> None:
         pass
     
-    def newRect(self, x: int, y: int, width: int, height: int, color: tuple) -> _CustomShape:
+    def new_rect(self, x: int, y: int, width: int, height: int, color: tuple) -> _CustomShape:
         return _CustomShape(x, y, width, height, color)
```

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/storage.py` & `fusion-engine-0.2.0/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/systems.py` & `fusion-engine-0.2.0/src/fusionengine/files/systems.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.1.1/src/fusionengine/files/window.py` & `fusion-engine-0.2.0/src/fusionengine/files/window.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,29 @@
     def __init__(self) -> None:
         self.window = None
         self._running = False
         self._NOW = SDL_GetPerformanceCounter();
         self._LAST = 0;
         self.DELTATIME = 0;   
     
-    def newWindow(self, title: str, width: int, height: int) -> _CustomRenderer:
+    def new_window(self, title: str, width: int, height: int) -> _CustomRenderer:
         encoded_title = title.encode('utf-8')
-        self.window = SDL_CreateWindow(encoded_title,
+        self.window_window = SDL_CreateWindow(encoded_title,
                                        SDL_WINDOWPOS_CENTERED,
                                        SDL_WINDOWPOS_CENTERED,
                                        width, height,
                                        SDL_WINDOW_SHOWN
                                        )
         self._running = True
-        return _CustomRenderer(self.window)
+        self.window = _CustomRenderer(self.window_window)
+        return self.window
+    
+    def loop(self, func):
+        while self.running(self.window):
+            func()
     
     def running(self, window:_CustomRenderer) -> bool:
         self._refresh(window)
         return self._running
     
     def _refresh(self, window: _CustomRenderer) -> None:
         SDL_UpdateWindowSurface(window.window)
```

