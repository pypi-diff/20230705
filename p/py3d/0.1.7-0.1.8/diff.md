# Comparing `tmp/py3d-0.1.7.tar.gz` & `tmp/py3d-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.7.tar", last modified: Thu Jun 29 14:23:12 2023, max compression
+gzip compressed data, was "py3d-0.1.8.tar", last modified: Wed Jul  5 01:05:29 2023, max compression
```

## Comparing `py3d-0.1.7.tar` & `py3d-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-29 14:23:12.246305 py3d-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-29 14:22:49.000000 py3d-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29856 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 14:23:12.246305 py3d-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-29 14:21:54.000000 py3d-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.844173 py3d-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-05 01:05:29.844173 py3d-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-05 01:05:11.000000 py3d-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.840173 py3d-0.1.8/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29637 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.840173 py3d-0.1.8/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 01:05:29.844173 py3d-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-07-05 01:04:26.000000 py3d-0.1.8/setup.py
```

### Comparing `py3d-0.1.7/PKG-INFO` & `py3d-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.7
+Version: 0.1.8
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.7/README.md` & `py3d-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.7/py3d/core.py` & `py3d-0.1.8/py3d/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,25 +418,18 @@
         d: Vector = (self[..., numpy.newaxis, :] - pts).L
         d = d.reshape(*d.shape[:-2], -1)
         idx = d.argmin(d.ndim-1)
         spts = sum(pts.n)
         idx0 = idx//spts
         idx1 = idx % spts
         return idx0, idx1
-    
+
     def distance_to_points(self, points: Vector3) -> numpy.ndarray:
         return (self[..., None, :] - points).L.min(axis=-1).mean()
 
-    def as_scaling(self) -> Transform:
-        ret = Transform
-        ret[..., 0, 0] = self[..., 0]
-        ret[..., 1, 1] = self[..., 1]
-        ret[..., 2, 2] = self[..., 2]
-        return ret.view(Transform)
-
     def as_point(self) -> Point:
         entity = Point(*self.n)
         entity.xyz = self
         return entity
 
     def as_line(self) -> LineSegment:
         n = list(self.n)
@@ -712,15 +705,15 @@
 
     @property
     def scaling_vector(self) -> Vector3:
         return numpy.linalg.norm(self[..., 0:3, 0:3], axis=self.ndim-1).view(Vector3)
 
     @scaling_vector.setter
     def scaling_vector(self, v: Vector3):
-        self[:] = v.as_scaling() @ self.scaling.I @ self
+        self[:] = Transform.from_scaling(v) @ self.scaling.I @ self
 
     @property
     def translation(self) -> Transform:
         ret = Transform(*self.n)
         ret[..., 3, 0:3] = self.translation_vector
         return ret
 
@@ -785,15 +778,15 @@
         s0: Vector3 = self.scaling_vector[i-1]
         s1: Vector3 = self.scaling_vector[i]
         angle, axis = (r0.I@r1).as_angle_axis()
         rotation = Transform.from_angle_axis(d*angle, axis)
         translation = Transform.from_translation(
             d[..., numpy.newaxis] * (t1 - t0))
         scaling = Transform.from_scaling(
-            d[..., numpy.newaxis] * s1 / s0).as_scaling()
+            d[..., numpy.newaxis] * s1 / s0)
         return self[i-1]@scaling@rotation@translation
 
 
 class Color(Vector):
     BASE_SHAPE = 4,
 
     def __new__(cls, data: numpy.ndarray | list = [], r=0, g=0, b=0, a=1):
```

### Comparing `py3d-0.1.7/py3d/viewer.html` & `py3d-0.1.8/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.1.7/py3d.egg-info/PKG-INFO` & `py3d-0.1.8/py3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.7
+Version: 0.1.8
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.7/setup.py` & `py3d-0.1.8/setup.py`

 * *Files identical despite different names*

