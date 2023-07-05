# Comparing `tmp/pyiges-0.3.0.tar.gz` & `tmp/pyiges-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiges-0.3.0.tar", last modified: Tue Jun  6 18:46:03 2023, max compression
+gzip compressed data, was "pyiges-0.3.1.tar", last modified: Wed Jul  5 14:41:57 2023, max compression
```

## Comparing `pyiges-0.3.0.tar` & `pyiges-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-06 18:45:22.000000 pyiges-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-06 18:45:22.000000 pyiges-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 18:45:22.000000 pyiges-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-06 18:46:03.944400 pyiges-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 18:45:22.000000 pyiges-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.940400 pyiges-0.3.0/pyiges/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/check_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/pyiges/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4033498 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/impeller.igs
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/examples/sample.igs
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/faces.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyiges/iges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.940400 pyiges-0.3.0/pyiges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 18:46:03.000000 pyiges-0.3.0/pyiges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 18:45:22.000000 pyiges-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:46:03.944400 pyiges-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 18:45:22.000000 pyiges-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:46:03.944400 pyiges-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-06-06 18:45:22.000000 pyiges-0.3.0/tests/test_pyiges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:57.387570 pyiges-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-05 14:41:14.000000 pyiges-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 14:41:14.000000 pyiges-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-05 14:41:14.000000 pyiges-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-05 14:41:57.387570 pyiges-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-05 14:41:14.000000 pyiges-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:57.383571 pyiges-0.3.1/pyiges/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/check_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:57.387570 pyiges-0.3.1/pyiges/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4033498 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/examples/impeller.igs
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/examples/sample.igs
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/faces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyiges/iges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:57.383571 pyiges-0.3.1/pyiges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-05 14:41:57.000000 pyiges-0.3.1/pyiges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 14:41:57.000000 pyiges-0.3.1/pyiges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:41:57.000000 pyiges-0.3.1/pyiges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 14:41:57.000000 pyiges-0.3.1/pyiges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 14:41:57.000000 pyiges-0.3.1/pyiges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 14:41:14.000000 pyiges-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:41:57.387570 pyiges-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 14:41:14.000000 pyiges-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:57.387570 pyiges-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-05 14:41:14.000000 pyiges-0.3.1/tests/test_pyiges.py
```

### Comparing `pyiges-0.3.0/CONTRIBUTING.rst` & `pyiges-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/LICENSE` & `pyiges-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/PKG-INFO` & `pyiges-0.3.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pyiges
-Version: 0.3.0
-Summary: Pythonic IGES reader
-Home-page: https://github.com/pyvista/pyiges
-Author: PyVista Developers
-Author-email: info@pyvista.org
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
-Provides-Extra: full
-License-File: LICENSE
-
 pyIGES
 ======
 Python IGES reader with basic functionality to read an IGES file and
 convert some entities to a ``pyvista`` or ``vtk`` mesh.
 
 This module can read in and perform basic parsing of all entities and
 can perform additional parsing and geometry visualization of the
```

### Comparing `pyiges-0.3.0/pyiges/entity.py` & `pyiges-0.3.1/pyiges/entity.py`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/pyiges/examples/impeller.igs` & `pyiges-0.3.1/pyiges/examples/impeller.igs`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/pyiges/examples/sample.igs` & `pyiges-0.3.1/pyiges/examples/sample.igs`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/pyiges/geometry.py` & `pyiges-0.3.1/pyiges/geometry.py`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/pyiges/iges.py` & `pyiges-0.3.1/pyiges/iges.py`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/pyiges.egg-info/PKG-INFO` & `pyiges-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,117 @@
 Metadata-Version: 2.1
 Name: pyiges
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pythonic IGES reader
 Home-page: https://github.com/pyvista/pyiges
 Author: PyVista Developers
 Author-email: info@pyvista.org
 License: MIT
+Description: pyIGES
+        ======
+        Python IGES reader with basic functionality to read an IGES file and
+        convert some entities to a ``pyvista`` or ``vtk`` mesh.
+        
+        This module can read in and perform basic parsing of all entities and
+        can perform additional parsing and geometry visualization of the
+        following entities:
+        
+        - Vertex List (Type 502 Form 1)
+        - Edge List
+        - Loop (for specifying a bounded face for BREP geometries
+        - Face
+        - Circular arc
+        - Rational B-Spline Surface
+        - Rational B-Spline Curve
+        - Conic Arc (Type 104)
+        - Line
+        - Point
+        
+        
+        Installation
+        ------------
+        
+        ``pyiges`` is offered in a "full" variant including the conversion features
+        and a "pure" parsing module variant.
+        The pure variant has no conversion features, no dependencies to ``pyvista,geomdl``,
+        and can be installed by removing the ``[full]`` specificator from the following commands.
+        
+        Install with pip using:
+        
+        .. code::
+        
+           pip install pyiges[full]
+        
+        Otherwise, if you want the bleeding edge version, feel free to clone
+        this repo and install with:
+        
+        .. code:: bash
+        
+           git clone https://github.com/pyvista/pyiges
+           cd pyiges
+           pip install .[full]
+        
+        Note that the square brackets might need to be escaped or quoted when using ``zsh``.
+        
+        
+        Usage
+        -----
+        The ``pyiges`` module can read in many entities as raw text, but only
+        NURBS surfaces and bsplines can be converted to ``pyvista`` meshes.
+        
+        .. code:: python
+        
+            import pyiges
+            from pyiges import examples
+        
+            # load an example impeller
+            iges = pyiges.read(examples.impeller)
+        
+            # print an invidiual entity (boring)
+            print(iges[0])
+        
+            # convert all lines to a vtk mesh and plot it
+            lines = iges.to_vtk(bsplines=True, surfaces=False, merge=True)
+            lines.plot(color='w', line_width=2)
+        
+            # convert all surfaces to a vtk mesh and plot it
+            mesh = iges.to_vtk(bsplines=False, surfaces=True, merge=True, delta=0.05)
+            mesh.plot(color='w', smooth_shading=True)
+            # control resolution of the mesh by changing "delta"
+        
+            # save this surface to file
+            mesh.save('mesh.ply')  # as ply
+            mesh.save('mesh.stl')  # as stl
+            mesh.save('mesh.vtk')  # as vtk
+        
+        
+        Lines
+        ~~~~~
+        .. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_lines.png
+        
+        
+        Surfaces
+        ~~~~~~~~
+        .. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_surf.png
+        
+        
+        
+        Acknowledgments
+        ---------------
+        Substantial code was obtained from or inspired by https://github.com/cfinch/IGES-File-Reader
+        
+        IGES reference definitions were obtained from `Eclipse IGES Wiki <https://wiki.eclipse.org/IGES_file_Specification#Rational_B-Spline_Curve_.28Type_126.29>`_,
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: full
-License-File: LICENSE
-
-pyIGES
-======
-Python IGES reader with basic functionality to read an IGES file and
-convert some entities to a ``pyvista`` or ``vtk`` mesh.
-
-This module can read in and perform basic parsing of all entities and
-can perform additional parsing and geometry visualization of the
-following entities:
-
-- Vertex List (Type 502 Form 1)
-- Edge List
-- Loop (for specifying a bounded face for BREP geometries
-- Face
-- Circular arc
-- Rational B-Spline Surface
-- Rational B-Spline Curve
-- Conic Arc (Type 104)
-- Line
-- Point
-
-
-Installation
-------------
-
-``pyiges`` is offered in a "full" variant including the conversion features
-and a "pure" parsing module variant.
-The pure variant has no conversion features, no dependencies to ``pyvista,geomdl``,
-and can be installed by removing the ``[full]`` specificator from the following commands.
-
-Install with pip using:
-
-.. code::
-
-   pip install pyiges[full]
-
-Otherwise, if you want the bleeding edge version, feel free to clone
-this repo and install with:
-
-.. code:: bash
-
-   git clone https://github.com/pyvista/pyiges
-   cd pyiges
-   pip install .[full]
-
-Note that the square brackets might need to be escaped or quoted when using ``zsh``.
-
-
-Usage
------
-The ``pyiges`` module can read in many entities as raw text, but only
-NURBS surfaces and bsplines can be converted to ``pyvista`` meshes.
-
-.. code:: python
-
-    import pyiges
-    from pyiges import examples
-
-    # load an example impeller
-    iges = pyiges.read(examples.impeller)
-
-    # print an invidiual entity (boring)
-    print(iges[0])
-
-    # convert all lines to a vtk mesh and plot it
-    lines = iges.to_vtk(bsplines=True, surfaces=False, merge=True)
-    lines.plot(color='w', line_width=2)
-
-    # convert all surfaces to a vtk mesh and plot it
-    mesh = iges.to_vtk(bsplines=False, surfaces=True, merge=True, delta=0.05)
-    mesh.plot(color='w', smooth_shading=True)
-    # control resolution of the mesh by changing "delta"
-
-    # save this surface to file
-    mesh.save('mesh.ply')  # as ply
-    mesh.save('mesh.stl')  # as stl
-    mesh.save('mesh.vtk')  # as vtk
-
-
-Lines
-~~~~~
-.. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_lines.png
-
-
-Surfaces
-~~~~~~~~
-.. image:: https://github.com/pyvista/pyiges/raw/main/docs/images/impeller_surf.png
-
-
-
-Acknowledgments
----------------
-Substantial code was obtained from or inspired by https://github.com/cfinch/IGES-File-Reader
-
-IGES reference definitions were obtained from `Eclipse IGES Wiki <https://wiki.eclipse.org/IGES_file_Specification#Rational_B-Spline_Curve_.28Type_126.29>`_,
```

### Comparing `pyiges-0.3.0/pyproject.toml` & `pyiges-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/setup.py` & `pyiges-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyiges-0.3.0/tests/test_pyiges.py` & `pyiges-0.3.1/tests/test_pyiges.py`

 * *Files identical despite different names*

