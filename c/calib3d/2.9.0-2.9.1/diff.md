# Comparing `tmp/calib3d-2.9.0.tar.gz` & `tmp/calib3d-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calib3d-2.9.0.tar", last modified: Mon Jan  9 08:55:33 2023, max compression
+gzip compressed data, was "dist/calib3d-2.9.1.tar", last modified: Tue Feb 14 09:39:29 2023, max compression
```

## Comparing `calib3d-2.9.0.tar` & `calib3d-2.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.601703 calib3d-2.9.0/
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.461704 calib3d-2.9.0/.github/
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.511703 calib3d-2.9.0/.github/workflows/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1299 2022-12-22 13:08:42.000000 calib3d-2.9.0/.github/workflows/python-package.yml
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1060 2022-12-22 13:08:42.000000 calib3d-2.9.0/.github/workflows/python-publish.yml
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       37 2022-12-20 08:50:01.000000 calib3d-2.9.0/.gitignore
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    35149 2022-12-20 08:50:01.000000 calib3d-2.9.0/LICENSE
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4402 2023-01-09 08:55:33.600703 calib3d-2.9.0/PKG-INFO
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     3248 2022-12-22 13:19:16.000000 calib3d-2.9.0/README.md
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.524703 calib3d-2.9.0/assets/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    46338 2022-12-22 13:08:42.000000 calib3d-2.9.0/assets/distortion_steps.png
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.549703 calib3d-2.9.0/calib3d/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      928 2022-12-22 13:08:42.000000 calib3d-2.9.0/calib3d/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    24930 2022-12-22 13:10:39.000000 calib3d-2.9.0/calib3d/calib.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5673 2023-01-09 08:53:06.000000 calib3d-2.9.0/calib3d/draw.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     7678 2022-12-22 13:08:42.000000 calib3d-2.9.0/calib3d/points.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.564703 calib3d-2.9.0/calib3d/pycuda/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       36 2022-12-22 13:08:42.000000 calib3d-2.9.0/calib3d/pycuda/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1846 2022-12-22 13:08:42.000000 calib3d-2.9.0/calib3d/pycuda/pycuda_calib.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.568703 calib3d-2.9.0/calib3d/tf1/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       53 2022-12-20 08:50:01.000000 calib3d-2.9.0/calib3d/tf1/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6923 2022-12-20 08:50:01.000000 calib3d-2.9.0/calib3d/tf1/tf1_calib.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.559703 calib3d-2.9.0/calib3d.egg-info/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4402 2023-01-09 08:55:32.000000 calib3d-2.9.0/calib3d.egg-info/PKG-INFO
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      795 2023-01-09 08:55:33.000000 calib3d-2.9.0/calib3d.egg-info/SOURCES.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        1 2023-01-09 08:55:32.000000 calib3d-2.9.0/calib3d.egg-info/dependency_links.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       20 2023-01-09 08:55:32.000000 calib3d-2.9.0/calib3d.egg-info/requires.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       14 2023-01-09 08:55:32.000000 calib3d-2.9.0/calib3d.egg-info/top_level.txt
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.574703 calib3d-2.9.0/docs/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       26 2022-12-22 13:08:42.000000 calib3d-2.9.0/docs/_config.yml
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.584703 calib3d-2.9.0/docs/calib3d/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    97326 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/calib.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    24731 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/draw.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     9570 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/index.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    41068 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/points.html
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.589703 calib3d-2.9.0/docs/calib3d/pycuda/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6902 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/pycuda/index.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    17905 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/pycuda/pycuda_calib.html
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.593703 calib3d-2.9.0/docs/calib3d/tf1/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6883 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/tf1/index.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    29770 2023-01-09 08:55:29.000000 calib3d-2.9.0/docs/calib3d/tf1/tf1_calib.html
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       59 2022-12-22 13:08:42.000000 calib3d-2.9.0/docs/index.html
--rwxr-x---   0 gvanzand (3002593) gvanzand (3002593)      478 2022-12-23 09:25:26.000000 calib3d-2.9.0/release.sh
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2022-12-22 13:08:42.000000 calib3d-2.9.0/requirements.txt
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2023-01-09 08:55:33.601703 calib3d-2.9.0/setup.cfg
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      904 2023-01-09 08:54:33.000000 calib3d-2.9.0/setup.py
-drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-01-09 08:55:33.597703 calib3d-2.9.0/tests/
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-12-22 13:08:42.000000 calib3d-2.9.0/tests/__init__.py
--rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5333 2022-12-22 13:08:48.000000 calib3d-2.9.0/tests/test_calib.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.606552 calib3d-2.9.1/
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.515552 calib3d-2.9.1/.github/
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.554552 calib3d-2.9.1/.github/workflows/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1299 2022-12-22 13:08:42.000000 calib3d-2.9.1/.github/workflows/python-package.yml
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1060 2022-12-22 13:08:42.000000 calib3d-2.9.1/.github/workflows/python-publish.yml
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       37 2022-12-20 08:50:01.000000 calib3d-2.9.1/.gitignore
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    35149 2022-12-20 08:50:01.000000 calib3d-2.9.1/LICENSE
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4402 2023-02-14 09:39:29.605552 calib3d-2.9.1/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     3248 2022-12-22 13:19:16.000000 calib3d-2.9.1/README.md
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.556552 calib3d-2.9.1/assets/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    46338 2022-12-22 13:08:42.000000 calib3d-2.9.1/assets/distortion_steps.png
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.564552 calib3d-2.9.1/calib3d/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      928 2022-12-22 13:08:42.000000 calib3d-2.9.1/calib3d/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    24930 2023-01-20 09:33:14.000000 calib3d-2.9.1/calib3d/calib.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5686 2023-02-03 10:00:24.000000 calib3d-2.9.1/calib3d/draw.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     7678 2022-12-22 13:08:42.000000 calib3d-2.9.1/calib3d/points.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.576552 calib3d-2.9.1/calib3d/pycuda/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       36 2022-12-22 13:08:42.000000 calib3d-2.9.1/calib3d/pycuda/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1846 2022-12-22 13:08:42.000000 calib3d-2.9.1/calib3d/pycuda/pycuda_calib.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.580552 calib3d-2.9.1/calib3d/tf1/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       53 2022-12-20 08:50:01.000000 calib3d-2.9.1/calib3d/tf1/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6923 2022-12-20 08:50:01.000000 calib3d-2.9.1/calib3d/tf1/tf1_calib.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.573552 calib3d-2.9.1/calib3d.egg-info/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     4402 2023-02-14 09:39:29.000000 calib3d-2.9.1/calib3d.egg-info/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      795 2023-02-14 09:39:29.000000 calib3d-2.9.1/calib3d.egg-info/SOURCES.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        1 2023-02-14 09:39:29.000000 calib3d-2.9.1/calib3d.egg-info/dependency_links.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       20 2023-02-14 09:39:29.000000 calib3d-2.9.1/calib3d.egg-info/requires.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       14 2023-02-14 09:39:29.000000 calib3d-2.9.1/calib3d.egg-info/top_level.txt
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.584552 calib3d-2.9.1/docs/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       26 2022-12-22 13:08:42.000000 calib3d-2.9.1/docs/_config.yml
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.592552 calib3d-2.9.1/docs/calib3d/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    97326 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/calib.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    24770 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/draw.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     9570 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/index.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    41068 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/points.html
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.596552 calib3d-2.9.1/docs/calib3d/pycuda/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6902 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/pycuda/index.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    17905 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/pycuda/pycuda_calib.html
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.600552 calib3d-2.9.1/docs/calib3d/tf1/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     6883 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/tf1/index.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)    29770 2023-02-14 09:39:26.000000 calib3d-2.9.1/docs/calib3d/tf1/tf1_calib.html
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       59 2022-12-22 13:08:42.000000 calib3d-2.9.1/docs/index.html
+-rwxr-x---   0 gvanzand (3002593) gvanzand (3002593)      478 2022-12-23 09:25:26.000000 calib3d-2.9.1/release.sh
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2022-12-22 13:08:42.000000 calib3d-2.9.1/requirements.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2023-02-14 09:39:29.607552 calib3d-2.9.1/setup.cfg
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      904 2023-02-14 09:38:42.000000 calib3d-2.9.1/setup.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-02-14 09:39:29.603552 calib3d-2.9.1/tests/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        0 2022-12-22 13:08:42.000000 calib3d-2.9.1/tests/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5333 2022-12-22 13:08:48.000000 calib3d-2.9.1/tests/test_calib.py
```

### Comparing `calib3d-2.9.0/.github/workflows/python-package.yml` & `calib3d-2.9.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/.github/workflows/python-publish.yml` & `calib3d-2.9.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/LICENSE` & `calib3d-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/PKG-INFO` & `calib3d-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calib3d
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python 3D calibration and homogenous coordinates computation library
 Home-page: https://github.com/ispgroupucl/calib3d
 Author: Gabriel Van Zandycke
 Author-email: gabriel.vanzandycke@hotmail.com
 License: LGPL
 Description: # Python camera calibration and projective geometry library
```

### Comparing `calib3d-2.9.0/README.md` & `calib3d-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/assets/distortion_steps.png` & `calib3d-2.9.1/assets/distortion_steps.png`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d/__init__.py` & `calib3d-2.9.1/calib3d/__init__.py`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d/calib.py` & `calib3d-2.9.1/calib3d/calib.py`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d/draw.py` & `calib3d-2.9.1/calib3d/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     canvas.add_patch(p)
                 except ImportError:
                     raise ImportError("The current implementation requires matplotlib")
             else:
                 canvas.plot(points.x, points.y, linewidth=thickness, color=np.array(color)/255, markersize=markersize, **kwargs)
 
     def polylines(self, canvas, points3D: Point3D, color=None, thickness: int=None, **kwargs):
-        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), thickness=thickness, **kwargs)
+        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), color=color, thickness=thickness, **kwargs)
         #for point3D1, point3D2 in zip(points3D, points3D.close()[:,1:]):
         #    self.draw_line(canvas, point3D1, point3D2, *args, **kwargs)
 
     def draw_line(self, canvas, point3D1: Point3D, point3D2: Point3D, color=None, thickness: int=None, only_visible=True, **kwargs):
         if only_visible:
             try:
                 point3D1, point3D2 = visible_segment(self.calib, point3D1, point3D2)
```

### Comparing `calib3d-2.9.0/calib3d/points.py` & `calib3d-2.9.1/calib3d/points.py`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d/pycuda/pycuda_calib.py` & `calib3d-2.9.1/calib3d/pycuda/pycuda_calib.py`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d/tf1/tf1_calib.py` & `calib3d-2.9.1/calib3d/tf1/tf1_calib.py`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/calib3d.egg-info/PKG-INFO` & `calib3d-2.9.1/calib3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calib3d
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python 3D calibration and homogenous coordinates computation library
 Home-page: https://github.com/ispgroupucl/calib3d
 Author: Gabriel Van Zandycke
 Author-email: gabriel.vanzandycke@hotmail.com
 License: LGPL
 Description: # Python camera calibration and projective geometry library
```

### Comparing `calib3d-2.9.0/calib3d.egg-info/SOURCES.txt` & `calib3d-2.9.1/calib3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/calib.html` & `calib3d-2.9.1/docs/calib3d/calib.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/draw.html` & `calib3d-2.9.1/docs/calib3d/draw.html`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                     canvas.add_patch(p)
                 except ImportError:
                     raise ImportError(&#34;The current implementation requires matplotlib&#34;)
             else:
                 canvas.plot(points.x, points.y, linewidth=thickness, color=np.array(color)/255, markersize=markersize, **kwargs)
 
     def polylines(self, canvas, points3D: Point3D, color=None, thickness: int=None, **kwargs):
-        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), thickness=thickness, **kwargs)
+        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), color=color, thickness=thickness, **kwargs)
         #for point3D1, point3D2 in zip(points3D, points3D.close()[:,1:]):
         #    self.draw_line(canvas, point3D1, point3D2, *args, **kwargs)
 
     def draw_line(self, canvas, point3D1: Point3D, point3D2: Point3D, color=None, thickness: int=None, only_visible=True, **kwargs):
         if only_visible:
             try:
                 point3D1, point3D2 = visible_segment(self.calib, point3D1, point3D2)
@@ -261,15 +261,15 @@
                     canvas.add_patch(p)
                 except ImportError:
                     raise ImportError(&#34;The current implementation requires matplotlib&#34;)
             else:
                 canvas.plot(points.x, points.y, linewidth=thickness, color=np.array(color)/255, markersize=markersize, **kwargs)
 
     def polylines(self, canvas, points3D: Point3D, color=None, thickness: int=None, **kwargs):
-        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), thickness=thickness, **kwargs)
+        self._polylines(canvas, self.calib.project_3D_to_2D(points3D), color=color, thickness=thickness, **kwargs)
         #for point3D1, point3D2 in zip(points3D, points3D.close()[:,1:]):
         #    self.draw_line(canvas, point3D1, point3D2, *args, **kwargs)
 
     def draw_line(self, canvas, point3D1: Point3D, point3D2: Point3D, color=None, thickness: int=None, only_visible=True, **kwargs):
         if only_visible:
             try:
                 point3D1, point3D2 = visible_segment(self.calib, point3D1, point3D2)
@@ -393,15 +393,15 @@
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def polylines(self, canvas, points3D: Point3D, color=None, thickness: int=None, **kwargs):
-    self._polylines(canvas, self.calib.project_3D_to_2D(points3D), thickness=thickness, **kwargs)</code></pre>
+    self._polylines(canvas, self.calib.project_3D_to_2D(points3D), color=color, thickness=thickness, **kwargs)</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
```

#### html2text {}

```diff
@@ -68,15 +68,15 @@
             else:
                 canvas.plot(points.x, points.y, linewidth=thickness,
 color=np.array(color)/255, markersize=markersize, **kwargs)
 
     def polylines(self, canvas, points3D: Point3D, color=None, thickness:
 int=None, **kwargs):
         self._polylines(canvas, self.calib.project_3D_to_2D(points3D),
-thickness=thickness, **kwargs)
+color=color, thickness=thickness, **kwargs)
         #for point3D1, point3D2 in zip(points3D, points3D.close()[:,1:]):
         #    self.draw_line(canvas, point3D1, point3D2, *args, **kwargs)
 
     def draw_line(self, canvas, point3D1: Point3D, point3D2: Point3D,
 color=None, thickness: int=None, only_visible=True, **kwargs):
         if only_visible:
             try:
@@ -248,15 +248,15 @@
                   else:
                       canvas.plot(points.x, points.y, linewidth=thickness,
       color=np.array(color)/255, markersize=markersize, **kwargs)
 
           def polylines(self, canvas, points3D: Point3D, color=None, thickness:
       int=None, **kwargs):
               self._polylines(canvas, self.calib.project_3D_to_2D(points3D),
-      thickness=thickness, **kwargs)
+      color=color, thickness=thickness, **kwargs)
               #for point3D1, point3D2 in zip(points3D, points3D.close()[:,1:]):
               #    self.draw_line(canvas, point3D1, point3D2, *args, **kwargs)
 
           def draw_line(self, canvas, point3D1: Point3D, point3D2: Point3D,
       color=None, thickness: int=None, only_visible=True, **kwargs):
               if only_visible:
                   try:
@@ -355,15 +355,15 @@
             thickness=-1)
         def polylines(self, canvas, points3D:Â Point3D, color=None, thickness:
         Â intÂ =Â None, **kwargs)
               Expand source code
             def polylines(self, canvas, points3D: Point3D, color=None,
             thickness: int=None, **kwargs):
                 self._polylines(canvas, self.calib.project_3D_to_2D(points3D),
-            thickness=thickness, **kwargs)
+            color=color, thickness=thickness, **kwargs)
 
 ****** Index ******
     * Projective_Drawing
     * **** Super-module ****
           o calib3d
     * **** Functions ****
           o visible_segment
```

### Comparing `calib3d-2.9.0/docs/calib3d/index.html` & `calib3d-2.9.1/docs/calib3d/index.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/points.html` & `calib3d-2.9.1/docs/calib3d/points.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/pycuda/index.html` & `calib3d-2.9.1/docs/calib3d/pycuda/index.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/pycuda/pycuda_calib.html` & `calib3d-2.9.1/docs/calib3d/pycuda/pycuda_calib.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/tf1/index.html` & `calib3d-2.9.1/docs/calib3d/tf1/index.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/docs/calib3d/tf1/tf1_calib.html` & `calib3d-2.9.1/docs/calib3d/tf1/tf1_calib.html`

 * *Files identical despite different names*

### Comparing `calib3d-2.9.0/setup.py` & `calib3d-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    version="2.9.0",
+    version="2.9.1",
     name='calib3d',
     author='Gabriel Van Zandycke',
     author_email="gabriel.vanzandycke@hotmail.com",
     url="https://github.com/ispgroupucl/calib3d",
     license="LGPL",
     python_requires='>=3.6',
     description="Python 3D calibration and homogenous coordinates computation library",
```

### Comparing `calib3d-2.9.0/tests/test_calib.py` & `calib3d-2.9.1/tests/test_calib.py`

 * *Files identical despite different names*

