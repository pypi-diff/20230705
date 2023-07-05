# Comparing `tmp/adaptivecard-0.1.0.tar.gz` & `tmp/adaptivecard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.1.0.tar", last modified: Wed Jul  5 05:00:51 2023, max compression
+gzip compressed data, was "adaptivecard-0.1.1.tar", last modified: Wed Jul  5 09:04:13 2023, max compression
```

## Comparing `adaptivecard-0.1.0.tar` & `adaptivecard-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.990020 adaptivecard-0.1.0/
--rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/LICENSE.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 05:00:51.989762 adaptivecard-0.1.0/PKG-INFO
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.0/README.md
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.988551 adaptivecard-0.1.0/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.0/adaptivecard/__init__.py
--rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/_base_types.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3155 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/abstract_types.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1132 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/actions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     2980 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/card_elements.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     3516 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/cards.py
--rw-r--r--   0 cabutchei   (501) staff       (20)    13967 2023-07-05 04:51:20.000000 adaptivecard-0.1.0/adaptivecard/containers.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.0/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1611 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/mixin.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.989418 adaptivecard-0.1.0/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      445 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       19 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/requires.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 05:00:51.990082 adaptivecard-0.1.0/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)      975 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.154240 adaptivecard-0.1.1/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/LICENSE.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 09:04:13.154018 adaptivecard-0.1.1/PKG-INFO
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.1/README.md
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.152575 adaptivecard-0.1.1/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.1/adaptivecard/__init__.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/_base_types.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3155 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/abstract_types.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1161 2023-07-05 08:59:57.000000 adaptivecard-0.1.1/adaptivecard/actions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3009 2023-07-05 09:00:13.000000 adaptivecard-0.1.1/adaptivecard/card_elements.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3545 2023-07-05 09:01:40.000000 adaptivecard-0.1.1/adaptivecard/cards.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)    14086 2023-07-05 08:59:30.000000 adaptivecard-0.1.1/adaptivecard/containers.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.1/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1611 2023-07-05 04:12:51.000000 adaptivecard-0.1.1/adaptivecard/mixin.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 09:04:13.153773 adaptivecard-0.1.1/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      445 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       37 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 09:04:13.000000 adaptivecard-0.1.1/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 09:04:13.154294 adaptivecard-0.1.1/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1004 2023-07-05 09:02:46.000000 adaptivecard-0.1.1/setup.py
```

### Comparing `adaptivecard-0.1.0/LICENSE.txt` & `adaptivecard-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.0/PKG-INFO` & `adaptivecard-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.0
+Version: 0.1.1
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.1.0/adaptivecard/abstract_types.py` & `adaptivecard-0.1.1/adaptivecard/abstract_types.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.0/adaptivecard/actions.py` & `adaptivecard-0.1.1/adaptivecard/actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Literal
+from typing import Optional
+from typing_extensions import Literal
 from adaptivecard.cards import AdaptiveCard
 from adaptivecard.mixin import Mixin
 from adaptivecard._base_types import Action
 
 
 class ShowCard(Mixin, Action):
     def __init__(self,
```

### Comparing `adaptivecard-0.1.0/adaptivecard/card_elements.py` & `adaptivecard-0.1.1/adaptivecard/card_elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Optional, Union, Literal
+from typing import Any, Optional, Union
+from typing_extensions import Literal
 from adaptivecard._base_types import Element
 from adaptivecard.mixin import Mixin
 
 
 
 class TextBlock(Mixin, Element):
     """Elemento de texto"""
```

### Comparing `adaptivecard-0.1.0/adaptivecard/cards.py` & `adaptivecard-0.1.1/adaptivecard/cards.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Optional, Union, Sequence, Literal
+from typing import Any, Optional, Union, Sequence
+from typing_extensions import Literal
 from adaptivecard.mixin import Mixin
 from adaptivecard._base_types import Element, Action
 
 
 
 
 class Content:
```

### Comparing `adaptivecard-0.1.0/adaptivecard/containers.py` & `adaptivecard-0.1.1/adaptivecard/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Optional, Union, Literal, Sequence, List, get_type_hints
+from typing import Any, Optional, Union, Sequence, List, get_type_hints
+from typing_extensions import Literal
 from adaptivecard._base_types import Element, Action, ISelectAction
 from adaptivecard.mixin import Mixin
 from tabulate import tabulate
 from typeguard import check_type
 from adaptivecard.card_elements import TextBlock
 
 
@@ -193,14 +194,16 @@
         self.json_fields = ("type", "cells", "style")
     def __getitem__(self, __i):
         if isinstance(__i, slice):
             return self.__class__(cells=self.cells[__i])
         return self.cells.__getitem__(__i)
     def __setitem__(self, __key, __value):
         self.cells.__setitem__(__key, TableCell(__value))
+    def __add__(self, __value):
+        return self.__class__(self.cells + __value.cells)
     def __len__(self):
         return len(self.cells)
     def __repr__(self):
         return f"{self.__class__.__name__}({str(self.cells)})"
     def __str__(self):
         return "[" + ", ".join([str(cell) for cell in self.cells]) + "]"
```

### Comparing `adaptivecard-0.1.0/adaptivecard/mixin.py` & `adaptivecard-0.1.1/adaptivecard/mixin.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.1.0/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.1.1/adaptivecard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.1.0
+Version: 0.1.1
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.1.0/setup.py` & `adaptivecard-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
     author_email="<luropa_paz@hotmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         'typeguard',
-        'tabulate'
+        'tabulate',
+        'typing_extensions'
     ],
     keywords=['python', 'adaptive', 'card', 'adaptive card', 'microsoft'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License", 
         "Programming Language :: Python :: 3",
```

