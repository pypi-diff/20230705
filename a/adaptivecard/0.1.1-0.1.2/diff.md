# Comparing `tmp/adaptivecard-0.1.1.tar.gz` & `tmp/adaptivecard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.1.1.tar", last modified: Wed Jul  5 09:04:13 2023, max compression
+gzip compressed data, was "dist/adaptivecard-0.1.2.tar", last modified: Wed Jul  5 19:46:52 2023, max compression
```

## Comparing `adaptivecard-0.1.1.tar` & `adaptivecard-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.154240 adaptivecard-0.1.1/
--rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/LICENSE.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 09:04:13.154018 adaptivecard-0.1.1/PKG-INFO
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.1/README.md
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.152575 adaptivecard-0.1.1/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.1/adaptivecard/__init__.py
--rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/_base_types.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3155 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/abstract_types.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1161 2023-07-05 08:59:57.000000 adaptivecard-0.1.1/adaptivecard/actions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3009 2023-07-05 09:00:13.000000 adaptivecard-0.1.1/adaptivecard/card_elements.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3545 2023-07-05 09:01:40.000000 adaptivecard-0.1.1/adaptivecard/cards.py
--rw-r--r--   0 cabutchei   (501) staff       (20)    14086 2023-07-05 08:59:30.000000 adaptivecard-0.1.1/adaptivecard/containers.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.1/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1611 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/mixin.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.153773 adaptivecard-0.1.1/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      445 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       37 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/requires.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 09:04:13.154294 adaptivecard-0.1.1/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)     1004 2023-07-05 09:02:46.000000 adaptivecard-0.1.1/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/PKG-INFO
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1628 2023-07-05 19:43:45.000000 adaptivecard-0.1.2/adaptivecard/mixin.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)    14086 2023-07-05 08:59:30.000000 adaptivecard-0.1.2/adaptivecard/containers.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3545 2023-07-05 09:01:40.000000 adaptivecard-0.1.2/adaptivecard/cards.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1161 2023-07-05 08:59:57.000000 adaptivecard-0.1.2/adaptivecard/actions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.2/adaptivecard/__init__.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.2/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3009 2023-07-05 09:00:13.000000 adaptivecard-0.1.2/adaptivecard/card_elements.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.2/adaptivecard/_base_types.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.2/README.md
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1004 2023-07-05 19:45:43.000000 adaptivecard-0.1.2/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      738 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      414 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       37 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 19:46:52.000000 adaptivecard-0.1.2/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.2/LICENSE.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `adaptivecard-0.1.1/LICENSE.txt` & `adaptivecard-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.1/PKG-INFO` & `adaptivecard-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microsoft Adaptive Cards
+Home-page: UNKNOWN
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
+License: UNKNOWN
 Keywords: python,adaptive,card,adaptive card,microsoft
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A package that helps you design adaptive cards in an object-oriented manner.
+
```

### Comparing `adaptivecard-0.1.1/adaptivecard/actions.py` & `adaptivecard-0.1.2/adaptivecard/actions.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.1/adaptivecard/card_elements.py` & `adaptivecard-0.1.2/adaptivecard/card_elements.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.1/adaptivecard/cards.py` & `adaptivecard-0.1.2/adaptivecard/cards.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.1/adaptivecard/containers.py` & `adaptivecard-0.1.2/adaptivecard/containers.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.1/adaptivecard/mixin.py` & `adaptivecard-0.1.2/adaptivecard/mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 
     def to_dict(self):
         """
         Returns a json/dictionary representative of the card element
         """
 
         def get_json_dic(obj):
-            return {key: value for key in obj.json_fields if hasattr(obj, key) and (value := getattr(obj, key)) is not None}
+            return {key: getattr(obj, key) for key in obj.json_fields if hasattr(obj, key) and getattr(obj, key) is not None}
 
         # possível problema de circular reference ao passar o mesmo objeto em dois lugares diferentes do card. Averiguar depois.
         dic = json.loads(json.dumps(self, default=lambda obj: get_json_dic(obj)))
         return dic
     
     def is_sequence(self, value):
         if isinstance(value, Sequence) and not isinstance(value, str):
             return True
         return False
 
     def __setattr__(self, __name: str, __value: Any) -> None:
-        if __name in (type_hints := get_type_hints(self.__init__)):
+        type_hints = get_type_hints(self.__init__)
+        if __name in type_hints:
                 check_type(__value, type_hints[__name])
         if __name in self.protected_attributes and hasattr(self, __name):
             raise AttributeError(f"Can't set '{__name}' attribute")
         super().__setattr__(__name, __value)
 
     def __delattr__(self, __name: str) -> None:
         if __name in self.protected_attributes or hasattr(self, 'json_fields') and __name in self.json_fields:
```

### Comparing `adaptivecard-0.1.1/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.1.2/adaptivecard.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microsoft Adaptive Cards
+Home-page: UNKNOWN
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
+License: UNKNOWN
 Keywords: python,adaptive,card,adaptive card,microsoft
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A package that helps you design adaptive cards in an object-oriented manner.
+
```

### Comparing `adaptivecard-0.1.1/setup.py` & `adaptivecard-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
```

