# Comparing `tmp/pyfbsdk-stub-generator-1.0.0.tar.gz` & `tmp/pyfbsdk-stub-generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfbsdk-stub-generator-1.0.0.tar", last modified: Mon Apr 24 04:58:06 2023, max compression
+gzip compressed data, was "c:\Users\nils\Documents\GitHub\pyfbsdk-stub-generator\dist\.tmp-hiq8h2sm\pyfbsdk-stub-generator-1.0.1.tar", last modified: Wed Jul  5 19:44:26 2023, max compression
```

## Comparing `pyfbsdk-stub-generator-1.0.0.tar` & `pyfbsdk-stub-generator-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.897504 pyfbsdk-stub-generator-1.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       46 2023-04-15 19:55:38.000000 pyfbsdk-stub-generator-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2051 2023-04-24 04:58:06.898516 pyfbsdk-stub-generator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-04-15 19:07:58.000000 pyfbsdk-stub-generator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.838839 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/
--rw-rw-rw-   0        0        0      932 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.867663 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/base_content/
--rw-rw-rw-   0        0        0      330 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
--rw-rw-rw-   0        0        0     7750 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/module_types.py
--rw-rw-rw-   0        0        0     9220 2023-04-23 15:58:00.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/native_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.871672 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/
--rw-rw-rw-   0        0        0      568 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.874671 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
--rw-rw-rw-   0        0        0     1847 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.880675 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/
--rw-rw-rw-   0        0        0       57 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.883813 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
--rw-rw-rw-   0        0        0     4035 2023-04-24 04:50:45.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
--rw-rw-rw-   0        0        0     2978 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.887170 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/
--rw-rw-rw-   0        0        0       66 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.896489 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
--rw-rw-rw-   0        0        0      492 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
--rw-rw-rw-   0        0        0    12628 2023-04-22 08:47:04.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
--rw-rw-rw-   0        0        0     2593 2023-04-23 15:16:47.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
--rw-rw-rw-   0        0        0    17079 2023-04-24 04:54:07.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
--rw-rw-rw-   0        0        0     2704 2023-04-23 15:57:38.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/plugin.py
--rw-rw-rw-   0        0        0     6626 2023-04-24 04:47:13.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/stub_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.865340 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/
--rw-rw-rw-   0        0        0     2051 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1649 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-06-24 08:36:30.000000 pyfbsdk-stub-generator-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-24 04:58:06.900525 pyfbsdk-stub-generator-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/
+-rw-rw-rw-   0        0        0     1235 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2051 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/
+-rw-rw-rw-   0        0        0      932 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/base_content/
+-rw-rw-rw-   0        0        0      482 2023-07-05 19:01:00.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
+-rw-rw-rw-   0        0        0     7790 2023-07-05 18:42:11.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/module_types.py
+-rw-rw-rw-   0        0        0     9676 2023-07-05 19:01:59.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/native_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/
+-rw-rw-rw-   0        0        0      688 2023-07-03 19:50:19.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/dunder_methods/
+-rw-rw-rw-   0        0        0        0 2023-07-03 18:54:48.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/dunder_methods/__init__.py
+-rw-rw-rw-   0        0        0     2820 2023-07-05 19:40:20.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/fb_property/
+-rw-rw-rw-   0        0        0        0 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
+-rw-rw-rw-   0        0        0     1847 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/
+-rw-rw-rw-   0        0        0       57 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
+-rw-rw-rw-   0        0        0        0 2023-04-12 09:02:28.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
+-rw-rw-rw-   0        0        0     4035 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
+-rw-rw-rw-   0        0        0     2978 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/
+-rw-rw-rw-   0        0        0       66 2023-04-04 18:04:41.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
+-rw-rw-rw-   0        0        0        0 2023-04-04 18:04:41.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-04-04 18:04:41.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
+-rw-rw-rw-   0        0        0      492 2023-04-10 17:39:50.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
+-rw-rw-rw-   0        0        0    12984 2023-07-05 19:20:38.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
+-rw-rw-rw-   0        0        0     2593 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
+-rw-rw-rw-   0        0        0    17079 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
+-rw-rw-rw-   0        0        0     2704 2023-07-03 14:41:35.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/plugin.py
+-rw-rw-rw-   0        0        0     6626 2023-07-04 16:23:04.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/stub_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/
+-rw-rw-rw-   0        0        0     2051 2023-07-05 19:44:25.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-07-05 19:44:25.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 19:44:25.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 19:44:25.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-05 19:44:25.000000 pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-10 09:49:23.000000 pyfbsdk-stub-generator-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-07-05 19:44:26.000000 pyfbsdk-stub-generator-1.0.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyfbsdk-stub-generator-1.0.0/LICENSE` & `pyfbsdk-stub-generator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/PKG-INFO` & `pyfbsdk-stub-generator-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
 License: UNLICENSE
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyfbsdk-stub-generator-1.0.0/README.md` & `pyfbsdk-stub-generator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/__init__.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/module_types.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/module_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
         Get a list of variable/class names that needs to be declared before the current object
         """
         raise NotImplementedError("GetRequirements() has not yet been implemented")
 
 
 class StubFunction(StubBase):
-    def __init__(self, Ref, Name = "", Parameters = None, ReturnType = None):
+    def __init__(self, Ref, Name = "", Parameters: list[StubParameter] | None = None, ReturnType: str | None = None):
         super().__init__(Ref, Name = Name)
         self._Params: list[StubParameter] = Parameters if Parameters else []
         self.ReturnType = ReturnType
         self.bIsMethod = False
         self.bIsStatic = False
         self.bIsOverload = False
```

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/native_generator.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/native_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import inspect
+import types
 
 from types import ModuleType
 
 from .module_types import StubClass, StubFunction, StubParameter, StubProperty
 
 ENUMERATION_NAME = "Enumeration"
-
+ALLOWED_BUILTIN_OVERRIDES = {"__gt__", "__lt__", "__ge__", "__le__"}
 
 class FObjectType:
     Function = 'function'
     Class = 'class'
     Property = 'property'
     Enum = 'type'
 
@@ -67,15 +68,30 @@
         - Ignore {List[str]}: 
         - AlwaysAllow {List[str]}: Always allowed members named x, even if they exists in the parent class
 
     Returns: tuple("Name", Reference)
     """
     Members = inspect.getmembers(Class)
     ParentClass = GetClassParents(Class)[0]
-    UniqueMemebers = [x for x in Members if (not hasattr(ParentClass, x[0]) and x[0] not in Ignore) or x[0] in AllowedOverrides]  # and not x[0].startswith("__")
+
+    UniqueMemebers = []
+    for Name, Ref in Members:
+        if Name in Ignore:
+            continue
+
+        if hasattr(ParentClass, Name):
+            if ParentClass.__name__ == "instance":
+                if isinstance(Ref, (types.BuiltinFunctionType, types.BuiltinMethodType)) and Name in ALLOWED_BUILTIN_OVERRIDES:
+                    UniqueMemebers.append((Name, Ref))
+                    continue
+
+            if Name not in AllowedOverrides:
+                continue
+
+        UniqueMemebers.append((Name, Ref))
 
     return UniqueMemebers
 
 
 def GetClassParentNames(Class):
     ParentClassNames = []
     for Parent in GetClassParents(Class):
```

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from . import documentation_cache as cache
 
 reload(cache)
 reload(urls)
 
 PY2_TO_PY3_PRINT_PATTERN = re.compile(r"(?<!\w)print\s+(.*)\s*(?<!\\)(?:\n|$)")
 
+
 class ClassNames:
     Items = "memitem"
     ItemTitles = "memtitle"
     Doc = "memdoc"
     ItemName = "memname"
     ParameterName = "paramname"
     ParameterType = "paramtype"
@@ -96,15 +97,15 @@
     Items = Parser.find_all("div", class_ = ClassNames.Items)
     ItemTitles = Parser.find_all("h2", class_ = ClassNames.ItemTitles)
 
     # If the titles doesn't match, fallback to not using titles
     if len(Items) != len(ItemTitles):
         print(f"Warning: The number of items ({len(Items)}) and item titles ({len(ItemTitles)}) doesn't match for page '{PageName}'.")
         ItemTitles = [None] * len(Items)
-    
+
     for Item, Title in zip(Items, ItemTitles):
         ItemName = ""
         ItemType = ""
         ItemDocumentation = ""
         Url = ""
 
         if Title:
@@ -122,15 +123,15 @@
             if NameHtml:
                 ItemName: str = GetSafeText(NameHtml.get_text())
                 if " " in ItemName:
                     ItemType, _, ItemName = ItemName.rpartition(" ")
                     ItemName = ItemName.strip()
                     ItemType = ItemType.strip()
 
-                    # In 2024 `FBSystem::DesktopSize` type is broken and contains html code 
+                    # In 2024 `FBSystem::DesktopSize` type is broken and contains html code
                     if "</a>" in ItemType:
                         ItemType = ItemType.rpartition("</a>")[2].strip()
 
             # Find all parameters
             Parameters = []
             for Row in NameTable.find_all("tr"):
                 ParameterNameHtml = Row.find("td", class_ = ClassNames.ParameterName)
@@ -171,15 +172,22 @@
         self.UrlBase = UrlBase  # Base for any relative url's found
         self.bParamNiceName = bParamNiceName
 
     def ConvertDocString(self, DescriptionHtml: Tag | NavigableString):
         DocString = self.convert(str(DescriptionHtml))
 
         # There are some (what I guess is) broken <b> tags scattered around in the docstrings. Remove them.
-        DocString = DocString.replace("b>", " ").strip()
+        DocString = DocString.replace("b>", " ")
+
+        # Replace single backslashes followed by special characters with the character only
+        DocString = re.sub(r'(?<!\\)\\([*_])', r'\1', DocString)
+        # Replace single backslashes followed by letters/numbers with double backslashes
+        DocString = re.sub(r'(?<!\\)\\([a-zA-Z0-9\s])', r'\\\\\1', DocString)
+
+        DocString = DocString.strip()
 
         # Go through and patch up the generated docstring
         Lines = []
         bInCodeBlock = False
         bPreviousLineWasEmpty = False
         for Line in DocString.split("\n"):
             StrippedLine = Line.strip()
@@ -286,15 +294,15 @@
     def convert_div(self, el: Tag, text, convert_as_inline):
         """ Convert all <div> tags to a code block. """
         ElementClassNames = el.get("class")
         if ElementClassNames and ClassNames.CodeBlock in ElementClassNames:
             return self.convert_pre(el, text, convert_as_inline)
 
         return text
-    
+
     def convert_pre(self, el: Tag, text, convert_as_inline):
         # Exclude any <div> tags that have class names "ttc"
         for Child in el.find_all('div', class_='ttc'):
             Child.decompose()
 
         Code = GetSafeText(el.get_text()).strip("`")
         LanguageType = GetLanguageFromCode(Code)
```

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/plugin.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/stub_generator.py` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator/stub_generator.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
 License: UNLICENSE
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt` & `pyfbsdk-stub-generator-1.0.1/pyfbsdk_stub_generator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 pyfbsdk_stub_generator.egg-info/SOURCES.txt
 pyfbsdk_stub_generator.egg-info/dependency_links.txt
 pyfbsdk_stub_generator.egg-info/requires.txt
 pyfbsdk_stub_generator.egg-info/top_level.txt
 pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
 pyfbsdk_stub_generator/plugins/__init__.py
 pyfbsdk_stub_generator/plugins/plugin.py
+pyfbsdk_stub_generator/plugins/dunder_methods/__init__.py
+pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py
 pyfbsdk_stub_generator/plugins/fb_property/__init__.py
 pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
 pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
 pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
 pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
 pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
 pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
```

### Comparing `pyfbsdk-stub-generator-1.0.0/setup.cfg` & `pyfbsdk-stub-generator-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6273 646b 2d73 7475 622d   = pyfbsdk-stub-
 00000020: 6765 6e65 7261 746f 720d 0a76 6572 7369  generator..versi
-00000030: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
+00000030: 6f6e 203d 2031 2e30 2e31 0d0a 6175 7468  on = 1.0.1..auth
 00000040: 6f72 203d 204e 696c 7320 536f 6465 726d  or = Nils Soderm
 00000050: 616e 0d0a 6465 7363 7269 7074 696f 6e20  an..description 
 00000060: 3d20 4765 6e65 7261 7465 2070 7966 6273  = Generate pyfbs
 00000070: 646b 2073 7475 6220 6669 6c65 7320 666f  dk stub files fo
 00000080: 7220 6265 7474 6572 2069 6e74 656c 6c69  r better intelli
 00000090: 7365 6e73 6520 7768 656e 2077 6f72 6b69  sense when worki
 000000a0: 6e67 2077 6974 6820 4d6f 7469 6f6e 4275  ng with MotionBu
```

