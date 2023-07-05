# Comparing `tmp/unitpy-0.0.6.tar.gz` & `tmp/unitpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitpy-0.0.6.tar", last modified: Wed Jun 28 23:50:32 2023, max compression
+gzip compressed data, was "C:\Users\nicep\Desktop\Reseach_Post\python\unitpy\dist\.tmp-tw5ph_l4\unitpy-0.0.7.tar", last modified: Wed Jul  5 13:59:52 2023, max compression
```

## Comparing `unitpy-0.0.6.tar` & `unitpy-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.371806 unitpy-0.0.6/
--rw-rw-rw-   0        0        0     1497 2023-04-01 17:13:34.000000 unitpy-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4288 2023-06-28 23:50:32.371806 unitpy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2023-04-03 23:31:47.000000 unitpy-0.0.6/README.md
--rw-rw-rw-   0        0        0      307 2023-04-03 23:31:47.000000 unitpy-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      969 2023-06-28 23:50:32.375820 unitpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-04-01 17:13:34.000000 unitpy-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.320346 unitpy-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.327355 unitpy-0.0.6/src/unitpy/
--rw-rw-rw-   0        0        0      336 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/__init__.py
--rw-rw-rw-   0        0        0      451 2023-06-28 23:44:35.000000 unitpy-0.0.6/src/unitpy/config.py
--rw-rw-rw-   0        0        0    19293 2023-06-28 23:48:14.000000 unitpy-0.0.6/src/unitpy/core.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.345355 unitpy-0.0.6/src/unitpy/definitions/
--rw-rw-rw-   0        0        0        0 2023-04-01 17:13:34.000000 unitpy-0.0.6/src/unitpy/definitions/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-01 23:56:36.000000 unitpy-0.0.6/src/unitpy/definitions/constants.py
--rw-rw-rw-   0        0        0     7224 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/definitions/dimensions.py
--rw-rw-rw-   0        0        0     1511 2023-04-04 02:20:26.000000 unitpy-0.0.6/src/unitpy/definitions/entry.py
--rw-rw-rw-   0        0        0     5904 2023-04-04 02:21:19.000000 unitpy-0.0.6/src/unitpy/definitions/ledger.py
--rw-rw-rw-   0        0        0      797 2023-04-01 17:13:34.000000 unitpy-0.0.6/src/unitpy/definitions/metric.py
--rw-rw-rw-   0        0        0     1362 2023-04-02 20:54:32.000000 unitpy-0.0.6/src/unitpy/definitions/prefix.py
--rw-rw-rw-   0        0        0    16491 2023-04-04 02:20:26.000000 unitpy-0.0.6/src/unitpy/definitions/unit_NIST.py
--rw-rw-rw-   0        0        0     6166 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/definitions/unit_base.py
--rw-rw-rw-   0        0        0     3545 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/definitions/unit_derived.py
--rw-rw-rw-   0        0        0      925 2023-04-04 02:21:19.000000 unitpy-0.0.6/src/unitpy/definitions/unit_extra.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.348354 unitpy-0.0.6/src/unitpy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-01 17:13:34.000000 unitpy-0.0.6/src/unitpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1855 2023-06-28 23:44:35.000000 unitpy-0.0.6/src/unitpy/utils/equation_formating.py
--rw-rw-rw-   0        0        0     5005 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/utils/parsing.py
--rw-rw-rw-   0        0        0      356 2023-04-03 23:31:47.000000 unitpy-0.0.6/src/unitpy/utils/string_converter.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.338354 unitpy-0.0.6/src/unitpy.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-28 23:50:32.000000 unitpy-0.0.6/src/unitpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-06-28 23:50:32.000000 unitpy-0.0.6/src/unitpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 23:50:32.000000 unitpy-0.0.6/src/unitpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-01 23:51:15.000000 unitpy-0.0.6/src/unitpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-28 23:50:32.000000 unitpy-0.0.6/src/unitpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 23:50:32.371806 unitpy-0.0.6/tests/
--rw-rw-rw-   0        0        0      684 2023-04-03 23:31:47.000000 unitpy-0.0.6/tests/test_define_quantity.py
--rw-rw-rw-   0        0        0     1110 2023-04-03 23:31:47.000000 unitpy-0.0.6/tests/test_define_unit.py
--rw-rw-rw-   0        0        0     1340 2023-04-03 23:31:47.000000 unitpy-0.0.6/tests/test_dimensions.py
--rw-rw-rw-   0        0        0     1927 2023-04-02 17:23:10.000000 unitpy-0.0.6/tests/test_parsing_unit.py
--rw-rw-rw-   0        0        0     2965 2023-06-28 23:25:59.000000 unitpy-0.0.6/tests/test_quanitiy_math_operations.py
--rw-rw-rw-   0        0        0      756 2023-04-02 21:11:03.000000 unitpy-0.0.6/tests/test_unit_conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/
+-rw-rw-rw-   0        0        0     1497 2023-04-03 12:39:22.000000 unitpy-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     4288 2023-07-05 13:59:52.000000 unitpy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-03 20:27:46.000000 unitpy-0.0.7/README.md
+-rw-rw-rw-   0        0        0      307 2023-04-03 17:45:31.000000 unitpy-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      969 2023-07-05 13:59:52.000000 unitpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-04-03 12:39:22.000000 unitpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy/
+-rw-rw-rw-   0        0        0      336 2023-04-03 14:05:31.000000 unitpy-0.0.7/src/unitpy/__init__.py
+-rw-rw-rw-   0        0        0      451 2023-07-05 13:23:16.000000 unitpy-0.0.7/src/unitpy/config.py
+-rw-rw-rw-   0        0        0    19921 2023-07-05 13:57:41.000000 unitpy-0.0.7/src/unitpy/core.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy/definitions/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/constants.py
+-rw-rw-rw-   0        0        0     7224 2023-04-03 16:57:14.000000 unitpy-0.0.7/src/unitpy/definitions/dimensions.py
+-rw-rw-rw-   0        0        0     1511 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/entry.py
+-rw-rw-rw-   0        0        0     5904 2023-07-05 13:21:40.000000 unitpy-0.0.7/src/unitpy/definitions/ledger.py
+-rw-rw-rw-   0        0        0      797 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/metric.py
+-rw-rw-rw-   0        0        0     1362 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/prefix.py
+-rw-rw-rw-   0        0        0    16491 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/definitions/unit_NIST.py
+-rw-rw-rw-   0        0        0     6166 2023-04-03 14:27:27.000000 unitpy-0.0.7/src/unitpy/definitions/unit_base.py
+-rw-rw-rw-   0        0        0     3545 2023-04-03 16:16:53.000000 unitpy-0.0.7/src/unitpy/definitions/unit_derived.py
+-rw-rw-rw-   0        0        0      925 2023-07-05 13:21:40.000000 unitpy-0.0.7/src/unitpy/definitions/unit_extra.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.7/src/unitpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1855 2023-07-05 13:23:16.000000 unitpy-0.0.7/src/unitpy/utils/equation_formating.py
+-rw-rw-rw-   0        0        0     5005 2023-04-03 15:05:13.000000 unitpy-0.0.7/src/unitpy/utils/parsing.py
+-rw-rw-rw-   0        0        0      356 2023-04-03 13:51:24.000000 unitpy-0.0.7/src/unitpy/utils/string_converter.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-03 12:59:41.000000 unitpy-0.0.7/src/unitpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-05 13:59:52.000000 unitpy-0.0.7/src/unitpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 13:59:52.000000 unitpy-0.0.7/tests/
+-rw-rw-rw-   0        0        0      684 2023-04-03 17:57:48.000000 unitpy-0.0.7/tests/test_define_quantity.py
+-rw-rw-rw-   0        0        0     1110 2023-04-03 18:03:53.000000 unitpy-0.0.7/tests/test_define_unit.py
+-rw-rw-rw-   0        0        0     1340 2023-04-03 16:57:59.000000 unitpy-0.0.7/tests/test_dimensions.py
+-rw-rw-rw-   0        0        0     1927 2023-04-03 12:39:22.000000 unitpy-0.0.7/tests/test_parsing_unit.py
+-rw-rw-rw-   0        0        0      205 2023-07-05 13:26:28.000000 unitpy-0.0.7/tests/test_pickle.py
+-rw-rw-rw-   0        0        0     2965 2023-05-30 14:41:46.000000 unitpy-0.0.7/tests/test_quanitiy_math_operations.py
+-rw-rw-rw-   0        0        0      756 2023-04-03 12:39:22.000000 unitpy-0.0.7/tests/test_unit_conversion.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `unitpy-0.0.6/LICENSE.txt` & `unitpy-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/PKG-INFO` & `unitpy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.6/README.md` & `unitpy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/setup.cfg` & `unitpy-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7470 790d 0a76 6572 7369   = unitpy..versi
-00000020: 6f6e 203d 2030 2e30 2e36 0d0a 6465 7363  on = 0.0.6..desc
+00000020: 6f6e 203d 2030 2e30 2e37 0d0a 6465 7363  on = 0.0.7..desc
 00000030: 7269 7074 696f 6e20 3d20 576f 726b 696e  ription = Workin
 00000040: 6720 7769 7468 2073 6369 656e 7469 6669  g with scientifi
 00000050: 6320 756e 6974 7320 696e 2070 7974 686f  c units in pytho
 00000060: 6e2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  n...long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `unitpy-0.0.6/src/unitpy/core.py` & `unitpy-0.0.7/src/unitpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,19 +229,22 @@
         return value
 
 
 ## Quantity ## noqa
 #######################################################################################################################
 #######################################################################################################################
 class Quantity(typing.SupportsRound):
+    compact_pickle = True
+    # full pickle 624 bytes -> compact pickle 98 bytes
+    # full 0.20 -> compact 0.31 create time
     _ledger = ledger
 
     __slots__ = ("_unit", "_base_value")
 
-    def __new__(cls, value: str | int | float, unit: Unit | BaseSet | str = None):
+    def __new__(cls, value: str | int | float = None, unit: Unit | BaseSet | str = None):
         if isinstance(value, str):
             from unitpy.utils.parsing import parse_quantity
             return parse_quantity(value)
 
         return super().__new__(cls)
 
     def __init__(self, value: str | int | float, unit: Unit | BaseSet | str = None):
@@ -261,14 +264,29 @@
 
     def __hash__(self) -> int:
         if self.dimensionless:
             return hash(self.value)
         else:
             return hash((self._base_value, self._unit))
 
+    def __getstate__(self):
+        if self.compact_pickle:
+            return str(self)
+        return self._base_value, self._unit
+
+    def __setstate__(self, state):
+        if isinstance(state, str):
+            from unitpy.utils.parsing import parse_quantity
+            qant = parse_quantity(state)
+            self._base_value = qant._base_value
+            self._unit = qant._unit
+        else:
+            self._base_value = state[0]
+            self._unit = state[1]
+
     def __copy__(self) -> Quantity:
         return self.__class__(copy.copy(self._base_value), copy.copy(self._unit))
 
     def __deepcopy__(self, memo) -> Quantity:
         return self.__class__(copy.deepcopy(self._base_value), copy.deepcopy(self._unit))
 
     def _comparison_check(self, other: Quantity):
```

### Comparing `unitpy-0.0.6/src/unitpy/definitions/constants.py` & `unitpy-0.0.7/src/unitpy/definitions/constants.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/dimensions.py` & `unitpy-0.0.7/src/unitpy/definitions/dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/entry.py` & `unitpy-0.0.7/src/unitpy/definitions/entry.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/ledger.py` & `unitpy-0.0.7/src/unitpy/definitions/ledger.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/metric.py` & `unitpy-0.0.7/src/unitpy/definitions/metric.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/prefix.py` & `unitpy-0.0.7/src/unitpy/definitions/prefix.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/unit_NIST.py` & `unitpy-0.0.7/src/unitpy/definitions/unit_NIST.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/unit_base.py` & `unitpy-0.0.7/src/unitpy/definitions/unit_base.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/unit_derived.py` & `unitpy-0.0.7/src/unitpy/definitions/unit_derived.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/definitions/unit_extra.py` & `unitpy-0.0.7/src/unitpy/definitions/unit_extra.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/utils/equation_formating.py` & `unitpy-0.0.7/src/unitpy/utils/equation_formating.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy/utils/parsing.py` & `unitpy-0.0.7/src/unitpy/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/src/unitpy.egg-info/PKG-INFO` & `unitpy-0.0.7/src/unitpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.6/src/unitpy.egg-info/SOURCES.txt` & `unitpy-0.0.7/src/unitpy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 src/unitpy/utils/equation_formating.py
 src/unitpy/utils/parsing.py
 src/unitpy/utils/string_converter.py
 tests/test_define_quantity.py
 tests/test_define_unit.py
 tests/test_dimensions.py
 tests/test_parsing_unit.py
+tests/test_pickle.py
 tests/test_quanitiy_math_operations.py
 tests/test_unit_conversion.py
```

### Comparing `unitpy-0.0.6/tests/test_define_quantity.py` & `unitpy-0.0.7/tests/test_define_quantity.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/tests/test_define_unit.py` & `unitpy-0.0.7/tests/test_define_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/tests/test_dimensions.py` & `unitpy-0.0.7/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/tests/test_parsing_unit.py` & `unitpy-0.0.7/tests/test_parsing_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/tests/test_quanitiy_math_operations.py` & `unitpy-0.0.7/tests/test_quanitiy_math_operations.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.6/tests/test_unit_conversion.py` & `unitpy-0.0.7/tests/test_unit_conversion.py`

 * *Files identical despite different names*

