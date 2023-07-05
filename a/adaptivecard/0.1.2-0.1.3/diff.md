# Comparing `tmp/adaptivecard-0.1.2.tar.gz` & `tmp/adaptivecard-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adaptivecard-0.1.2.tar", last modified: Wed Jul  5 19:46:52 2023, max compression
+gzip compressed data, was "dist/adaptivecard-0.1.3.tar", last modified: Wed Jul  5 20:12:12 2023, max compression
```

## Comparing `adaptivecard-0.1.2.tar` & `adaptivecard-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/
--rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/PKG-INFO
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)     1628 2023-07-05 19:43:45.000000 adaptivecard-0.1.2/adaptivecard/mixin.py
--rw-r--r--   0 cabutchei   (501) staff       (20)    14086 2023-07-05 08:59:30.000000 adaptivecard-0.1.2/adaptivecard/containers.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3545 2023-07-05 09:01:40.000000 adaptivecard-0.1.2/adaptivecard/cards.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1161 2023-07-05 08:59:57.000000 adaptivecard-0.1.2/adaptivecard/actions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.2/adaptivecard/__init__.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.2/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3009 2023-07-05 09:00:13.000000 adaptivecard-0.1.2/adaptivecard/card_elements.py
--rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.2/adaptivecard/_base_types.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.2/README.md
--rw-r--r--   0 cabutchei   (501) staff       (20)     1004 2023-07-05 19:45:43.000000 adaptivecard-0.1.2/setup.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      414 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       37 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/requires.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.2/LICENSE.txt
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/PKG-INFO
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1628 2023-07-05 19:43:45.000000 adaptivecard-0.1.3/adaptivecard/mixin.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)    14086 2023-07-05 08:59:30.000000 adaptivecard-0.1.3/adaptivecard/containers.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3545 2023-07-05 09:01:40.000000 adaptivecard-0.1.3/adaptivecard/cards.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1161 2023-07-05 08:59:57.000000 adaptivecard-0.1.3/adaptivecard/actions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.3/adaptivecard/__init__.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.3/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3009 2023-07-05 09:00:13.000000 adaptivecard-0.1.3/adaptivecard/card_elements.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.3/adaptivecard/_base_types.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.3/README.md
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1004 2023-07-05 20:12:03.000000 adaptivecard-0.1.3/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      414 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       37 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 20:12:12.000000 adaptivecard-0.1.3/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.3/LICENSE.txt
```

### Comparing `adaptivecard-0.1.2/PKG-INFO` & `adaptivecard-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.2
+Version: 0.1.3
 Summary: Microsoft Adaptive Cards
 Home-page: UNKNOWN
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 License: UNKNOWN
 Keywords: python,adaptive,card,adaptive card,microsoft
 Platform: UNKNOWN
```

### Comparing `adaptivecard-0.1.2/adaptivecard/mixin.py` & `adaptivecard-0.1.3/adaptivecard/mixin.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.2/adaptivecard/containers.py` & `adaptivecard-0.1.3/adaptivecard/containers.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.2/adaptivecard/cards.py` & `adaptivecard-0.1.3/adaptivecard/cards.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.2/adaptivecard/actions.py` & `adaptivecard-0.1.3/adaptivecard/actions.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.2/adaptivecard/card_elements.py` & `adaptivecard-0.1.3/adaptivecard/card_elements.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.2/setup.py` & `adaptivecard-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
```

### Comparing `adaptivecard-0.1.2/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.1.3/adaptivecard.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.2
+Version: 0.1.3
 Summary: Microsoft Adaptive Cards
 Home-page: UNKNOWN
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 License: UNKNOWN
 Keywords: python,adaptive,card,adaptive card,microsoft
 Platform: UNKNOWN
```

### Comparing `adaptivecard-0.1.2/LICENSE.txt` & `adaptivecard-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

