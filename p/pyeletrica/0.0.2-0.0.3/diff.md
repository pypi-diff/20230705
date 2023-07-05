# Comparing `tmp/pyeletrica-0.0.2.tar.gz` & `tmp/pyeletrica-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeletrica-0.0.2.tar", last modified: Sun Jun 25 18:40:51 2023, max compression
+gzip compressed data, was "pyeletrica-0.0.3.tar", last modified: Wed Jul  5 18:32:12 2023, max compression
```

## Comparing `pyeletrica-0.0.2.tar` & `pyeletrica-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.566014 pyeletrica-0.0.2/
--rw-rw-rw-   0        0        0     1106 2023-06-22 22:51:37.000000 pyeletrica-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3935 2023-06-25 18:40:51.557036 pyeletrica-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2147 2023-06-25 16:51:31.000000 pyeletrica-0.0.2/README.md
--rw-rw-rw-   0        0        0      749 2023-06-25 18:33:20.000000 pyeletrica-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 18:40:51.566014 pyeletrica-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.424393 pyeletrica-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.476254 pyeletrica-0.0.2/src/pyeletrica/
--rw-rw-rw-   0        0        0     8320 2023-06-25 18:33:10.000000 pyeletrica-0.0.2/src/pyeletrica/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:40:51.546066 pyeletrica-0.0.2/src/pyeletrica.egg-info/
--rw-rw-rw-   0        0        0     3935 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 18:40:51.000000 pyeletrica-0.0.2/src/pyeletrica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 18:32:12.962754 pyeletrica-0.0.3/
+-rw-rw-rw-   0        0        0     1106 2023-06-22 22:51:37.000000 pyeletrica-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3946 2023-07-05 18:32:12.951793 pyeletrica-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2158 2023-07-05 18:27:51.000000 pyeletrica-0.0.3/README.md
+-rw-rw-rw-   0        0        0      751 2023-06-26 00:06:52.000000 pyeletrica-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 18:32:12.963757 pyeletrica-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 18:32:12.751230 pyeletrica-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 18:32:12.813153 pyeletrica-0.0.3/src/pyeletrica/
+-rw-rw-rw-   0        0        0      243 2023-07-05 18:25:09.000000 pyeletrica-0.0.3/src/pyeletrica/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:32:12.926852 pyeletrica-0.0.3/src/pyeletrica/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 23:39:33.000000 pyeletrica-0.0.3/src/pyeletrica/core/__init__.py
+-rw-rw-rw-   0        0        0     9771 2023-07-05 18:24:37.000000 pyeletrica-0.0.3/src/pyeletrica/core/main.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:32:12.895933 pyeletrica-0.0.3/src/pyeletrica.egg-info/
+-rw-rw-rw-   0        0        0     3946 2023-07-05 18:32:12.000000 pyeletrica-0.0.3/src/pyeletrica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-05 18:32:12.000000 pyeletrica-0.0.3/src/pyeletrica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 18:32:12.000000 pyeletrica-0.0.3/src/pyeletrica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-05 18:32:12.000000 pyeletrica-0.0.3/src/pyeletrica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 18:32:12.000000 pyeletrica-0.0.3/src/pyeletrica.egg-info/top_level.txt
```

### Comparing `pyeletrica-0.0.2/LICENSE` & `pyeletrica-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeletrica-0.0.2/PKG-INFO` & `pyeletrica-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeletrica
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fundamental tools for electrical engineers.
 Author-email: Hugo Everaldo Salvador Bezerra <hugoesb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Everaldo Salvador Bezerra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,15 @@
 * tand
 * polar
 * rect
 * divI
 * ZIbase
 * Zparallel
 * plot3vectors
+* plotmho
 * to_linecomp
 * to_symcomp
 * overcurrent_time
 
 ## Help
 You can use the documentation to understand how the function works .
```

### Comparing `pyeletrica-0.0.2/README.md` & `pyeletrica-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 * tand
 * polar
 * rect
 * divI
 * ZIbase
 * Zparallel
 * plot3vectors
+* plotmho
 * to_linecomp
 * to_symcomp
 * overcurrent_time
 
 ## Help
 You can use the documentation to understand how the function works .
```

### Comparing `pyeletrica-0.0.2/pyproject.toml` & `pyeletrica-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["matplotlib", "numpy", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeletrica"
-version = "0.0.2"
+version = "0.0.3"
 description = "Fundamental tools for electrical engineers."
 readme = "README.md"
 authors = [{ name = "Hugo Everaldo Salvador Bezerra", email = "hugoesb@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -19,8 +19,8 @@
     "matplotlib",
     "numpy",
     'tomli; python_version < "3.12"',
 ]
 requires-python = ">=3.6"
 
 [project.urls]
-"Homepage" = "https://github.com/hugoesb/pyeletrica"
+"Homepage" = "https://github.com/hugoesb/pyeletrica"
```

### Comparing `pyeletrica-0.0.2/src/pyeletrica/__init__.py` & `pyeletrica-0.0.3/src/pyeletrica/core/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# Version of pyeletrica package
-__version__ = "0.0.2"
-
 import numpy as np
 import matplotlib.pyplot as plt
 
 def sind(angle):
     '''
     Compute sine of angle, where angle is in degrees.
 
@@ -72,26 +69,26 @@
 def ZIbase(S, V):
     '''
     Calculate base impedance in ohms and base current in ampere.
 
     Parameters
     ----------
     S: float
-        Power (watts).
+        Power (VA).
     V : float
         Voltage (volts).
     
     Returns
     -------
     out : array-like
         (base impedance (ohms), base current in (amps))
     '''
 
-    Zb = S / (np.sqrt(3) * V)
-    Ib = V**2 / S
+    Ib = S / (np.sqrt(3) * V)
+    Zb = V**2 / S
 
     return (Zb, Ib)
 
 def divI(I, z1, z2, ndigits = 3):
     '''
     Calculate currents in ampere passing in two impedances in parallel.
 
@@ -259,14 +256,61 @@
 
     plt.polar([0, np.deg2rad(V[0][1])], [0, V[0][0]], label=labels[0], marker='o')
     plt.polar([0, np.deg2rad(V[1][1])], [0, V[1][0]], label=labels[1], marker='o')
     plt.polar([0, np.deg2rad(V[2][1])], [0, V[2][0]], label=labels[2], marker='o')
     plt.legend()
     plt.show()
 
+def plotmho(Zline, reach=[0.8, 1.2], plotline=True, color='rb', label=['Zone 1', 'Zona 2'], ax=None):
+    '''
+    plot mho caracteristic.
+
+    Parameters
+    ----------
+    Zline : float
+        Line impedance.
+    reach: array-like
+        Array with reachs. The array must have the same length of 
+        color and label.
+    plotline: bool
+        if True plot Line impedance.
+    color: string or array-like
+        Colors of zones. The array must have the same length of 
+        reach and label.
+    label: array-like
+        Label of zones. The array must have the same length of 
+        reach as color.
+    ax: matplotlib.axes._axes.Axes
+        If None the function create in execution time.
+    '''
+    if not ax:
+        fig, ax = plt.subplots()
+    
+    Zline_rect = rect(Zline)
+    
+    for rc, c, l in zip(list(reach), list(color), list(label)):
+        Z = Zline_rect * rc        
+        offset0 = Z/2
+        ax.add_patch(plt.Circle([offset0.real, offset0.imag], 
+                            abs(Z)/2, color=c, fc='none', label=l))
+    if plotline:
+        ax.plot([0, Zline_rect.real], [0, Zline_rect.imag], label='Line')
+    ax.set_aspect('equal')
+    min,max = np.ceil(ax.get_xlim())
+    min -= 1
+    plt.xticks(range(int(min),int(max)))
+    min,max = np.ceil(ax.get_ylim())
+    min -= 1
+    plt.yticks(range(int(min),int(max)))
+    plt.axvline(0, color='k')
+    plt.axhline(0, color='k')
+    plt.grid()
+    plt.legend()
+    plt.show()
+
 def overcurrent_time(I, Is , TD, standard='iec', curva='si'):
     '''
     Tempo de atuação da função de sobrecorrente.
 
     Parâmetros
     ----------
     I: float
@@ -292,14 +336,15 @@
             'co8': US CO8 Inverse
             'co2': US CO2 Inverse short time
     Returns
     -------
     out: float
          Operating time (seconds).
     '''
+    
     Ir = I/Is
     if standard=='iec':
         if curva=='si':
             return TD * (0.14 / ((Ir**0.02) - 1)) # Inversa Padrão
         if curva=='vi':
             return TD * (13.5 / (Ir - 1)) # Muito Inversa
         if curva=='ei':
```

### Comparing `pyeletrica-0.0.2/src/pyeletrica.egg-info/PKG-INFO` & `pyeletrica-0.0.3/src/pyeletrica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeletrica
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fundamental tools for electrical engineers.
 Author-email: Hugo Everaldo Salvador Bezerra <hugoesb@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Everaldo Salvador Bezerra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,15 @@
 * tand
 * polar
 * rect
 * divI
 * ZIbase
 * Zparallel
 * plot3vectors
+* plotmho
 * to_linecomp
 * to_symcomp
 * overcurrent_time
 
 ## Help
 You can use the documentation to understand how the function works .
```

