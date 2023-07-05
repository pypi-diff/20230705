# Comparing `tmp/scblender-0.0.4.tar.gz` & `tmp/scblender-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scblender-0.0.4.tar", last modified: Wed Jul  5 19:04:56 2023, max compression
+gzip compressed data, was "scblender-0.1.0.tar", last modified: Wed Jul  5 19:15:27 2023, max compression
```

## Comparing `scblender-0.0.4.tar` & `scblender-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:04:56.980084 scblender-0.0.4/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:04:56.979973 scblender-0.0.4/PKG-INFO
--rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.0.4/README.md
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:04:56.979308 scblender-0.0.4/scblender/
--rw-------   0 mackhughes   (501) staff       (20)      126 2023-07-05 18:47:04.000000 scblender-0.0.4/scblender/__init__.py
--rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.0.4/scblender/curve.py
--rw-------   0 mackhughes   (501) staff       (20)     5848 2023-07-05 18:51:21.000000 scblender-0.0.4/scblender/mesh.py
--rw-------   0 mackhughes   (501) staff       (20)     3822 2023-07-05 19:03:14.000000 scblender-0.0.4/scblender/particle.py
--rw-------   0 mackhughes   (501) staff       (20)     7980 2023-07-05 19:04:38.000000 scblender-0.0.4/scblender/setting.py
-drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:04:56.979806 scblender-0.0.4/scblender.egg-info/
--rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:04:56.000000 scblender-0.0.4/scblender.egg-info/PKG-INFO
--rw-r--r--   0 mackhughes   (501) staff       (20)      252 2023-07-05 19:04:56.000000 scblender-0.0.4/scblender.egg-info/SOURCES.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 19:04:56.000000 scblender-0.0.4/scblender.egg-info/dependency_links.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 19:04:56.000000 scblender-0.0.4/scblender.egg-info/top_level.txt
--rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 19:04:56.980135 scblender-0.0.4/setup.cfg
--rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 19:04:02.000000 scblender-0.0.4/setup.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.113554 scblender-0.1.0/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:15:27.113422 scblender-0.1.0/PKG-INFO
+-rw-------   0 mackhughes   (501) staff       (20)      497 2022-12-10 22:59:10.000000 scblender-0.1.0/README.md
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.112752 scblender-0.1.0/scblender/
+-rw-------   0 mackhughes   (501) staff       (20)      126 2023-07-05 18:47:04.000000 scblender-0.1.0/scblender/__init__.py
+-rw-------   0 mackhughes   (501) staff       (20)     1000 2023-01-07 18:53:12.000000 scblender-0.1.0/scblender/curve.py
+-rw-------   0 mackhughes   (501) staff       (20)     5899 2023-07-05 19:06:48.000000 scblender-0.1.0/scblender/mesh.py
+-rw-------   0 mackhughes   (501) staff       (20)     3818 2023-07-05 19:10:00.000000 scblender-0.1.0/scblender/particle.py
+-rw-------   0 mackhughes   (501) staff       (20)     7980 2023-07-05 19:04:38.000000 scblender-0.1.0/scblender/setting.py
+drwxr-xr-x   0 mackhughes   (501) staff       (20)        0 2023-07-05 19:15:27.113219 scblender-0.1.0/scblender.egg-info/
+-rw-r--r--   0 mackhughes   (501) staff       (20)     1072 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/PKG-INFO
+-rw-r--r--   0 mackhughes   (501) staff       (20)      252 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/SOURCES.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)        1 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/dependency_links.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       10 2023-07-05 19:15:27.000000 scblender-0.1.0/scblender.egg-info/top_level.txt
+-rw-r--r--   0 mackhughes   (501) staff       (20)       38 2023-07-05 19:15:27.113617 scblender-0.1.0/setup.cfg
+-rw-------   0 mackhughes   (501) staff       (20)     1033 2023-07-05 19:14:46.000000 scblender-0.1.0/setup.py
```

### Comparing `scblender-0.0.4/PKG-INFO` & `scblender-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.0.4
+Version: 0.1.0
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.0.4/scblender/curve.py` & `scblender-0.1.0/scblender/curve.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.4/scblender/mesh.py` & `scblender-0.1.0/scblender/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     set_keyframe_vertices("mesh", 1, 1)
     set_keyframe_vertices("mesh", 2, 1)
     
     
     
     #mesh.set_vertices((0,1,2), ((0,0,0), (1,0,0), (2,0,0)))
     
-    v
+    mesh.set_vertices({0:(0,0,0), 1:(1,0,0), 2:(2,0,0)})
     
     set_keyframe_vertices("mesh", 0, 10)
     set_keyframe_vertices("mesh", 1, 10)
     set_keyframe_vertices("mesh", 2, 10)
 
 # vertices = ((0,1,0),(1,0,0),(0,0,1),(-1,0,0))
 # edges = ([0,1],[1,2],[0,2],[0,3],[2,3])
```

### Comparing `scblender-0.0.4/scblender/particle.py` & `scblender-0.1.0/scblender/particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
             bpy.ops.object.editmode_toggle()
         bpy.ops.object.select_all(action="DESELECT")
         bpy.data.objects[self._name].select_set(True)
         for vertice_id in new_coordinate.keys(): 
             bpy.context.active_object.data.vertices[vertice_id].co = new_coordinate[vertice_id]
         return None
     
-    def set_keyframe_vertices(self.name, vertice_id, frame = setting.get_frame()) -> None:
-        bpy.data.objects[self.name].data.vertices[vertice_id].keyframe_insert("co", frame = frame)
+    def set_keyframe_vertices(self, vertice_id, frame = setting.get_frame()) -> None:
+        bpy.data.objects[self._name].data.vertices[vertice_id].keyframe_insert("co", frame = frame)
         return None
 
 
     @staticmethod
     def _checking_the_type_and_the_dimensionality(greatness) -> bool:
         if (len(greatness) == 3) and (
             isinstance(greatness, list) or isinstance(greatness, np.ndarray)
```

### Comparing `scblender-0.0.4/scblender/setting.py` & `scblender-0.1.0/scblender/setting.py`

 * *Files identical despite different names*

### Comparing `scblender-0.0.4/scblender.egg-info/PKG-INFO` & `scblender-0.1.0/scblender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scblender
-Version: 0.0.4
+Version: 0.1.0
 Summary: its purpose is to help and facilitate the commands
 Author: Mack Hughes (Allison Eduardo)
 Author-email: <mackhughes251@gmail.com
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scblender-0.0.4/setup.py` & `scblender-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.1.0'
 DESCRIPTION = 'its purpose is to help and facilitate the commands'
 
 # Setting up
 setup(
     name="scblender",
     version=VERSION,
     author="Mack Hughes (Allison Eduardo)",
```

