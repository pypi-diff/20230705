# Comparing `tmp/textual-slider-0.1.0.tar.gz` & `tmp/textual-slider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-slider-0.1.0.tar", last modified: Thu Jun 29 21:47:14 2023, max compression
+gzip compressed data, was "textual-slider-0.1.1.tar", last modified: Wed Jul  5 19:39:39 2023, max compression
```

## Comparing `textual-slider-0.1.0.tar` & `textual-slider-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-29 21:47:14.432884 textual-slider-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)    35149 2023-06-06 19:46:23.000000 textual-slider-0.1.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-06-29 21:47:14.432884 textual-slider-0.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1517 2023-06-29 21:46:24.000000 textual-slider-0.1.0/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)       81 2023-06-25 07:42:02.000000 textual-slider-0.1.0/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)      719 2023-06-29 21:47:14.432884 textual-slider-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)       92 2023-06-06 19:58:44.000000 textual-slider-0.1.0/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-29 21:47:14.432884 textual-slider-0.1.0/src/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-29 21:47:14.432884 textual-slider-0.1.0/src/textual_slider/
--rw-r--r--   0 tom       (1000) tom       (1000)       87 2023-06-22 20:09:08.000000 textual-slider-0.1.0/src/textual_slider/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5385 2023-06-29 19:23:06.000000 textual-slider-0.1.0/src/textual_slider/_slider.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-29 21:47:14.432884 textual-slider-0.1.0/src/textual_slider.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-06-29 21:47:14.000000 textual-slider-0.1.0/src/textual_slider.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      321 2023-06-29 21:47:14.000000 textual-slider-0.1.0/src/textual_slider.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-29 21:47:14.000000 textual-slider-0.1.0/src/textual_slider.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       78 2023-06-29 21:47:14.000000 textual-slider-0.1.0/src/textual_slider.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       15 2023-06-29 21:47:14.000000 textual-slider-0.1.0/src/textual_slider.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 19:39:39.853636 textual-slider-0.1.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)    35149 2023-06-06 19:46:23.000000 textual-slider-0.1.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-07-05 19:39:39.853636 textual-slider-0.1.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1517 2023-06-29 21:46:24.000000 textual-slider-0.1.1/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)       81 2023-06-25 07:42:02.000000 textual-slider-0.1.1/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)      769 2023-07-05 19:39:39.853636 textual-slider-0.1.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)       92 2023-06-06 19:58:44.000000 textual-slider-0.1.1/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 19:39:39.853636 textual-slider-0.1.1/src/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 19:39:39.853636 textual-slider-0.1.1/src/textual_slider/
+-rw-r--r--   0 tom       (1000) tom       (1000)       87 2023-07-05 19:28:10.000000 textual-slider-0.1.1/src/textual_slider/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5385 2023-06-29 19:23:06.000000 textual-slider-0.1.1/src/textual_slider/_slider.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-06-06 19:58:44.000000 textual-slider-0.1.1/src/textual_slider/py.typed
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 19:39:39.853636 textual-slider-0.1.1/src/textual_slider.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-07-05 19:39:39.000000 textual-slider-0.1.1/src/textual_slider.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 2023-07-05 19:39:39.000000 textual-slider-0.1.1/src/textual_slider.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-05 19:39:39.000000 textual-slider-0.1.1/src/textual_slider.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       78 2023-07-05 19:39:39.000000 textual-slider-0.1.1/src/textual_slider.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       15 2023-07-05 19:39:39.000000 textual-slider-0.1.1/src/textual_slider.egg-info/top_level.txt
```

### Comparing `textual-slider-0.1.0/LICENSE` & `textual-slider-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual-slider-0.1.0/PKG-INFO` & `textual-slider-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-slider
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Textual widget for a simple slider
 Home-page: https://github.com/TomJGooding/textual-slider
 Author: TomJGooding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `textual-slider-0.1.0/README.md` & `textual-slider-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `textual-slider-0.1.0/setup.cfg` & `textual-slider-0.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 packages = find:
 install_requires = 
 	textual >= 0.24.0
 
 [options.packages.find]
 where = src
 
+[options.package_data]
+textual_slider = py.typed
+
 [options.extras_require]
 dev = 
 	black
 	flake8
 	isort
 	mypy
 	pytest
```

### Comparing `textual-slider-0.1.0/src/textual_slider/_slider.py` & `textual-slider-0.1.1/src/textual_slider/_slider.py`

 * *Files identical despite different names*

### Comparing `textual-slider-0.1.0/src/textual_slider.egg-info/PKG-INFO` & `textual-slider-0.1.1/src/textual_slider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-slider
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Textual widget for a simple slider
 Home-page: https://github.com/TomJGooding/textual-slider
 Author: TomJGooding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

