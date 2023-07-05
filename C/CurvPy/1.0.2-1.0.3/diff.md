# Comparing `tmp/CurvPy-1.0.2.tar.gz` & `tmp/CurvPy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CurvPy-1.0.2.tar", last modified: Tue Jul  4 08:10:00 2023, max compression
+gzip compressed data, was "CurvPy-1.0.3.tar", last modified: Wed Jul  5 19:16:25 2023, max compression
```

## Comparing `CurvPy-1.0.2.tar` & `CurvPy-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:10:00.066724 CurvPy-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:10:00.066724 CurvPy-1.0.2/CurvPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-04 08:10:00.000000 CurvPy-1.0.2/CurvPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-04 08:10:00.000000 CurvPy-1.0.2/CurvPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 08:10:00.000000 CurvPy-1.0.2/CurvPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-04 08:10:00.000000 CurvPy-1.0.2/CurvPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 08:10:00.000000 CurvPy-1.0.2/CurvPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-04 08:10:00.066724 CurvPy-1.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:10:00.066724 CurvPy-1.0.2/curvpy/
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-04 08:00:24.000000 CurvPy-1.0.2/curvpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6953 2023-07-03 22:35:53.000000 CurvPy-1.0.2/curvpy/curvpy.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 08:10:00.066724 CurvPy-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-04 08:07:12.000000 CurvPy-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:16:25.379822 CurvPy-1.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:16:25.379822 CurvPy-1.0.3/CurvPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-05 19:16:25.000000 CurvPy-1.0.3/CurvPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      193 2023-07-05 19:16:25.000000 CurvPy-1.0.3/CurvPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 19:16:25.000000 CurvPy-1.0.3/CurvPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-05 19:16:25.000000 CurvPy-1.0.3/CurvPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 19:16:25.000000 CurvPy-1.0.3/CurvPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-05 19:16:25.379822 CurvPy-1.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:16:25.379822 CurvPy-1.0.3/curvpy/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.3/curvpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-07-05 19:12:56.000000 CurvPy-1.0.3/curvpy/curvpy.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 19:16:25.379822 CurvPy-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 19:15:57.000000 CurvPy-1.0.3/setup.py
```

### Comparing `CurvPy-1.0.2/curvpy/curvpy.py` & `CurvPy-1.0.3/curvpy/curvpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -193,7 +193,37 @@
     plt.figure(figsize=(8, 6))
     plt.imshow(param_values, extent=[-1, 1, -1, 1], cmap='hot', aspect='auto')
     plt.colorbar()
     plt.xlabel('Parameter 1')
     plt.ylabel('Parameter 2')
     plt.title('Heatmap of Parameter Values')
     plt.show()
+
+
+def optifit_v2(func, initial_parameters, x, y):
+    def ask_user_input(prompt, default=None):
+        if default is not None:
+            prompt = f"{prompt} [{default}]: "
+        else:
+            prompt = f"{prompt}: "
+        value = input(prompt)
+        if value == '':
+            return default
+        if value == "-inf":
+            return -np.inf
+        if value == "inf":
+            return np.inf
+        return eval(value)
+    
+    lower_bounds_input = ask_user_input("Enter the lower bounds as a list (optional): ", default=None)
+    upper_bounds_input = ask_user_input("Enter the upper bounds as a list (optional): ", default=None)
+    maxfev = ask_user_input("Enter the maxfev (optional): ", default=None)
+    
+    lower_bounds = lower_bounds_input if lower_bounds_input is not None else -np.inf
+    upper_bounds = upper_bounds_input if upper_bounds_input is not None else np.inf
+    
+    if maxfev is None:
+        maxfev = 10000
+    
+    popt, pcov = curve_fit(func, x, y, p0=initial_parameters, bounds=(lower_bounds, upper_bounds), maxfev=maxfev)
+    
+    return popt
```

