# Comparing `tmp/clingraph-1.1.0.tar.gz` & `tmp/clingraph-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clingraph-1.1.0.tar", last modified: Wed Jan  4 22:57:30 2023, max compression
+gzip compressed data, was "clingraph-1.1.1.tar", last modified: Wed Jul  5 20:57:49 2023, max compression
```

## Comparing `clingraph-1.1.0.tar` & `clingraph-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:57:30.864207 clingraph-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-04 22:57:15.000000 clingraph-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-01-04 22:57:30.864207 clingraph-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-01-04 22:57:15.000000 clingraph-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:57:30.864207 clingraph-1.1.0/clingraph/
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/clingo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/graphviz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/tex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-01-04 22:57:15.000000 clingraph-1.1.0/clingraph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:57:30.864207 clingraph-1.1.0/clingraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-04 22:57:30.000000 clingraph-1.1.0/clingraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-04 22:57:15.000000 clingraph-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-04 22:57:30.864207 clingraph-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-04 22:57:15.000000 clingraph-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:57:49.826002 clingraph-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 20:57:29.000000 clingraph-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-05 20:57:49.826002 clingraph-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-05 20:57:29.000000 clingraph-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:57:49.826002 clingraph-1.1.1/clingraph/
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/clingo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-05 20:57:29.000000 clingraph-1.1.1/clingraph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:57:49.826002 clingraph-1.1.1/clingraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 20:57:49.000000 clingraph-1.1.1/clingraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 20:57:29.000000 clingraph-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 20:57:49.826002 clingraph-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 20:57:29.000000 clingraph-1.1.1/setup.py
```

### Comparing `clingraph-1.1.0/LICENSE` & `clingraph-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/PKG-INFO` & `clingraph-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clingraph
-Version: 1.1.0
+Version: 1.1.1
 Summary: A visualizer for graphs defined as facts with special integration for clingo
 Home-page: https://github.com/potassco/clingraph
 Author: Susana Hahn
 Author-email: hahnmartinlu@uni-potsdam.de
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `clingraph-1.1.0/README.md` & `clingraph-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/__init__.py` & `clingraph-1.1.1/clingraph/__init__.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/clingo_utils.py` & `clingraph-1.1.1/clingraph/clingo_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,26 @@
         """
         val = str(s).strip('"')
         val = val.replace('_',' ')
         if capitalize:
             val = val[0].upper() + val[1:]
         return String(val)
 
+    def cluster(self, s):
+        """
+        Returns the cluster name for a graph
+        Args:
+            s: The identifier of the graph
+        Returns:
+            (clingo.Symbol.String) The string with the cluster name
+        """
+        val = str(s).strip('"')
+        return String("cluster_"+val)
+
+
     def html_escape(self, s):
         """
         Will escape the symbols of an HTML-Like label that provoque clashes: &, < and >
         Args:
             s (clingo.Symbol): The value that needs the symbols removed
         Returns:
             (clingo.Symbol.String) The string with the replacements
```

### Comparing `clingraph-1.1.0/clingraph/gif.py` & `clingraph-1.1.1/clingraph/gif.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 """
 
 import os
 import logging
 from .graphviz import render
 try:
     import imageio.v2 as imageio
+    import numpy
 except ImportError:
     raise RuntimeError("imageio module has to be installed to save gifs") from None
+try:
+    from PIL import Image
+except ImportError:
+    raise RuntimeError("pillow module has to be installed to save gifs") from None
 log = logging.getLogger('custom')
 
 def save_gif(graphs, directory='out', name_format="movie", engine="dot", fps=1, sort="asc-str"):
     """
     Generates a gif for the given graphs
 
     Args:
@@ -62,20 +67,32 @@
     paths = []
     for model_n,graph in enumerate(graphs):
         if graph is None:
             continue
         name = name_format.replace('{graph_name}','movie').replace('{model_number}',str(model_n))
         gif_path = os.path.join(directory, f'{name}.gif')
         images = []
+        max_x = 0
+        max_y = 0
         for k in all_keys[model_n]:
             img_path = img_name_format.replace('{graph_name}',k)
             img_path = img_path.replace('{model_number}',str(model_n))+".png"
-            images.append(imageio.imread(os.path.join(images_dir, img_path)))
+            img_arr = imageio.imread(os.path.join(images_dir, img_path),mode="RGBA")
+            x,y,_ = img_arr.shape
+            max_x = x if x>max_x else max_x
+            max_y = y if y>max_y else max_y
+            images.append(img_arr)
+        for idx,img in enumerate(images):
+            p_img= Image.fromarray(img).resize((max_y, max_x))
+            images[idx]=numpy.asarray(p_img)
+
+
         os.makedirs(os.path.dirname(gif_path), exist_ok=True)
 
+        duration = int(1000 * 1/fps)
         imageio.mimsave(gif_path,
-                        images, fps=fps)
+                        images, duration=duration)
         paths.append({'all':gif_path})
 
     if not is_multi:
         return paths[0]
     return paths
```

### Comparing `clingraph-1.1.0/clingraph/graphviz.py` & `clingraph-1.1.1/clingraph/graphviz.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/logger.py` & `clingraph-1.1.1/clingraph/logger.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/orm.py` & `clingraph-1.1.1/clingraph/orm.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/tex.py` & `clingraph-1.1.1/clingraph/tex.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph/utils.py` & `clingraph-1.1.1/clingraph/utils.py`

 * *Files identical despite different names*

### Comparing `clingraph-1.1.0/clingraph.egg-info/PKG-INFO` & `clingraph-1.1.1/clingraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clingraph
-Version: 1.1.0
+Version: 1.1.1
 Summary: A visualizer for graphs defined as facts with special integration for clingo
 Home-page: https://github.com/potassco/clingraph
 Author: Susana Hahn
 Author-email: hahnmartinlu@uni-potsdam.de
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `clingraph-1.1.0/setup.cfg` & `clingraph-1.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clingraph
-version = 1.1.0
+version = 1.1.1
 author = Susana Hahn
 author_email = hahnmartinlu@uni-potsdam.de
 description = A visualizer for graphs defined as facts with special integration for clingo
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/potassco/clingraph
@@ -28,15 +28,16 @@
 doc = 
 	nbsphinx
 	sphinx
 	sphinx_rtd_theme
 tex = 
 	dot2tex
 gif = 
-	imageio>=2.14
+	imageio==2.28
+	pillow
 
 [options.entry_points]
 console_scripts = 
 	clingraph = clingraph:main
 
 [egg_info]
 tag_build =
```

