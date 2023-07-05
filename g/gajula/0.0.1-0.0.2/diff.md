# Comparing `tmp/gajula-0.0.1.tar.gz` & `tmp/gajula-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gajula-0.0.1.tar", last modified: Wed Jul  5 07:32:34 2023, max compression
+gzip compressed data, was "gajula-0.0.2.tar", last modified: Wed Jul  5 07:55:11 2023, max compression
```

## Comparing `gajula-0.0.1.tar` & `gajula-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:32:34.898780 gajula-0.0.1/
--rw-rw-rw-   0        0        0     1096 2023-07-05 07:25:55.000000 gajula-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      412 2023-07-05 07:32:34.897781 gajula-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-05 07:32:34.835780 gajula-0.0.1/gajula/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:32:34.891781 gajula-0.0.1/gajula/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:32:34.882785 gajula-0.0.1/gajula/src/gajula.egg-info/
--rw-rw-rw-   0        0        0      412 2023-07-05 07:32:34.000000 gajula-0.0.1/gajula/src/gajula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-05 07:32:34.000000 gajula-0.0.1/gajula/src/gajula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:32:34.000000 gajula-0.0.1/gajula/src/gajula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-05 07:32:34.000000 gajula-0.0.1/gajula/src/gajula.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 07:32:34.000000 gajula-0.0.1/gajula/src/gajula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-07-05 07:28:11.000000 gajula-0.0.1/gajula/src/gajula.py
--rw-rw-rw-   0        0        0       42 2023-07-05 07:32:34.900786 gajula-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-07-05 07:29:45.000000 gajula-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:55:11.285651 gajula-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-07-05 07:25:55.000000 gajula-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      466 2023-07-05 07:55:11.284653 gajula-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 07:55:11.249651 gajula-0.0.2/gajula/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:55:11.279652 gajula-0.0.2/gajula/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:55:11.277646 gajula-0.0.2/gajula/src/gajula.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-07-05 07:55:11.000000 gajula-0.0.2/gajula/src/gajula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-05 07:55:11.000000 gajula-0.0.2/gajula/src/gajula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:55:11.000000 gajula-0.0.2/gajula/src/gajula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-05 07:55:11.000000 gajula-0.0.2/gajula/src/gajula.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 07:55:11.000000 gajula-0.0.2/gajula/src/gajula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      133 2023-07-05 07:50:50.000000 gajula-0.0.2/gajula/src/gajula.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:55:11.286647 gajula-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-07-05 07:54:05.000000 gajula-0.0.2/setup.py
```

### Comparing `gajula-0.0.1/LICENSE` & `gajula-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gajula-0.0.1/setup.py` & `gajula-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gajula",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The initial release version
     author="Jagadeesh Gajula",                     # Full name of the author
     description="This is demo package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

