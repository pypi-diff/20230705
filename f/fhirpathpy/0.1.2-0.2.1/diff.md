# Comparing `tmp/fhirpathpy-0.1.2.tar.gz` & `tmp/fhirpathpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirpathpy-0.1.2.tar", last modified: Tue Jan 10 22:36:53 2023, max compression
+gzip compressed data, was "fhirpathpy-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fhirpathpy-0.1.2.tar` & `fhirpathpy-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     2453 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/README.md
--rw-r--r--   0        0        0     2967 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/__init__.py
--rw-r--r--   0        0        0     4626 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/engine/__init__.py
--rw-r--r--   0        0        0     9043 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/engine/evaluators/__init__.py
--rw-r--r--   0        0        0     5746 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/__init__.py
--rw-r--r--   0        0        0      799 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/collections.py
--rw-r--r--   0        0        0      282 2023-01-10 22:36:45.038208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/combining.py
--rw-r--r--   0        0        0      587 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/constants.py
--rw-r--r--   0        0        0      932 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/datetime.py
--rw-r--r--   0        0        0     4686 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/equality.py
--rw-r--r--   0        0        0     2055 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/existence.py
--rw-r--r--   0        0        0     2165 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/filtering.py
--rw-r--r--   0        0        0     1223 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/logic.py
--rw-r--r--   0        0        0     3698 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/math.py
--rw-r--r--   0        0        0     2341 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/misc.py
--rw-r--r--   0        0        0     1450 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/navigation.py
--rw-r--r--   0        0        0     1526 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/strings.py
--rw-r--r--   0        0        0       94 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/invocations/subsetting.py
--rw-r--r--   0        0        0    11005 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/nodes.py
--rw-r--r--   0        0        0     1568 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/engine/util.py
--rw-r--r--   0        0        0     1280 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/ASTPathListener.py
--rw-r--r--   0        0        0     5507 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/FHIRPath.g4
--rw-r--r--   0        0        0      988 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/__init__.py
--rw-r--r--   0        0        0     5699 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPath.interp
--rw-r--r--   0        0        0     1029 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPath.tokens
--rw-r--r--   0        0        0    17301 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.interp
--rw-r--r--   0        0        0    20549 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.py
--rw-r--r--   0        0        0     1029 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.tokens
--rw-r--r--   0        0        0    12767 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathListener.py
--rw-r--r--   0        0        0    79435 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathParser.py
--rw-r--r--   0        0        0        0 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/fhirpathpy/parser/generated/__init__.py
--rw-r--r--   0        0        0     1786 2023-01-10 22:36:45.042208 fhirpathpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 fhirpathpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2453 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/README.md
+-rw-r--r--   0        0        0     2967 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/__init__.py
+-rw-r--r--   0        0        0     4626 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/__init__.py
+-rw-r--r--   0        0        0     9524 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/evaluators/__init__.py
+-rw-r--r--   0        0        0     5817 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/__init__.py
+-rw-r--r--   0        0        0      799 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/collections.py
+-rw-r--r--   0        0        0      282 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/combining.py
+-rw-r--r--   0        0        0      587 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/constants.py
+-rw-r--r--   0        0        0      932 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/datetime.py
+-rw-r--r--   0        0        0     4738 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/equality.py
+-rw-r--r--   0        0        0     2055 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/existence.py
+-rw-r--r--   0        0        0     2549 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/filtering.py
+-rw-r--r--   0        0        0     1223 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/logic.py
+-rw-r--r--   0        0        0     3698 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/math.py
+-rw-r--r--   0        0        0     2347 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/misc.py
+-rw-r--r--   0        0        0     1450 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/navigation.py
+-rw-r--r--   0        0        0     1526 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/strings.py
+-rw-r--r--   0        0        0       94 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/subsetting.py
+-rw-r--r--   0        0        0    11005 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/nodes.py
+-rw-r--r--   0        0        0     1568 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/util.py
+-rw-r--r--   0        0        0     1280 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/ASTPathListener.py
+-rw-r--r--   0        0        0     5507 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/FHIRPath.g4
+-rw-r--r--   0        0        0      988 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/__init__.py
+-rw-r--r--   0        0        0     5699 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.interp
+-rw-r--r--   0        0        0     1029 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.tokens
+-rw-r--r--   0        0        0    17301 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.interp
+-rw-r--r--   0        0        0    20549 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.py
+-rw-r--r--   0        0        0     1029 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.tokens
+-rw-r--r--   0        0        0    12767 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathListener.py
+-rw-r--r--   0        0        0    79435 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathParser.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/__init__.py
+-rw-r--r--   0        0        0     1786 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 fhirpathpy-0.2.1/PKG-INFO
```

### Comparing `fhirpathpy-0.1.2/LICENSE.md` & `fhirpathpy-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/README.md` & `fhirpathpy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/__init__.py` & `fhirpathpy-0.2.1/fhirpathpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from fhirpathpy.engine.invocations.constants import constants
 from fhirpathpy.parser import parse
 from fhirpathpy.engine import do_eval
 from fhirpathpy.engine.util import arraify, get_data, set_paths
 from fhirpathpy.engine.nodes import FP_Type
 
 __title__ = "fhirpathpy"
-__version__ = "0.1.2"
+__version__ = "0.2.1"
 __author__ = "beda.software"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 beda.software"
 
 # Version synonym
 VERSION = __version__
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/__init__.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/evaluators/__init__.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/evaluators/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,34 +178,45 @@
             model is not None
             and "choiceTypePaths" in model
             and childPath in model["choiceTypePaths"]
         ):
             actualTypes = model["choiceTypePaths"][childPath]
 
         toAdd = None
+        toAdd_ = None
 
         if isinstance(actualTypes, list):
             # Use actualTypes to find the field's value
             for actualType in actualTypes:
                 field = key + actualType
-                if isinstance(res.data, (dict, list)) and field in res.data:
-                    toAdd = res.data[field]
-                    childPath = actualType
-                    break
+                if isinstance(res.data, (dict, list)):
+                    toAdd = res.data.get(field)
+                    toAdd_ = res.data.get(f"_{field}")
+                    if toAdd is not None or toAdd_ is not None:
+                        childPath = actualType
+                        break
         else:
-            if isinstance(res.data, (dict, list)) and key in res.data:
-                toAdd = res.data[key]
+            if isinstance(res.data, (dict, list)):
+                toAdd = res.data.get(key)
+                toAdd_ = res.data.get(f"_{key}")
+                if key == 'extension':
+                    childPath = 'Extension'
 
         if util.is_some(toAdd):
             if isinstance(toAdd, list):
                 mapped = [nodes.ResourceNode.create_node(x, childPath) for x in toAdd]
                 acc = acc + mapped
             else:
                 acc.append(nodes.ResourceNode.create_node(toAdd, childPath))
-            return acc
+        if util.is_some(toAdd_):
+            if isinstance(toAdd_, list):
+                mapped = [nodes.ResourceNode.create_node(x, childPath) for x in toAdd_]
+                acc = acc + mapped
+            else:
+                acc.append(nodes.ResourceNode.create_node(toAdd_, childPath))
         return acc
 
     return func
 
 
 def member_invocation(ctx, parentData, node):
     key = engine.do_eval(ctx, parentData, node["children"][0])[0]
@@ -261,17 +272,15 @@
 
 
 def polarity_expression(ctx, parentData, node):
     sign = node["terminalNodeText"][0]
     rtn = engine.do_eval(ctx, parentData, node["children"][0])
 
     if len(rtn) != 1:  # not yet in spec, but per Bryn Rhodes
-        raise Exception(
-            "Unary " + sign + " can only be applied to an individual number."
-        )
+        raise Exception("Unary " + sign + " can only be applied to an individual number.")
 
     if not util.is_number(rtn[0]):
         raise Exception("Unary " + sign + " can only be applied to a number.")
 
     if sign == "-":
         rtn[0] = -rtn[0]
 
@@ -297,17 +306,15 @@
     # Invocations
     "ThisInvocation": this_invocation,
     "MemberInvocation": member_invocation,
     "FunctionInvocation": function_invocation,
     # expressions
     "PolarityExpression": polarity_expression,
     "IndexerExpression": indexer_expression,
-    "MembershipExpression": alias_op_expression(
-        {"contains": "containsOp", "in": "inOp"}
-    ),
+    "MembershipExpression": alias_op_expression({"contains": "containsOp", "in": "inOp"}),
     "TermExpression": term_expression,
     "UnionExpression": union_expression,
     "InvocationExpression": invocation_expression,
     "InequalityExpression": op_expression,
     "AdditiveExpression": op_expression,
     "MultiplicativeExpression": op_expression,
     "EqualityExpression": op_expression,
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/__init__.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "subsetOf": {"fn": existence.subset_of_fn, "arity": {1: ["AnyAtRoot"]}},
     "supersetOf": {"fn": existence.superset_of_fn, "arity": {1: ["AnyAtRoot"]}},
     "isDistinct": {"fn": existence.isdistinct_fn},
     "distinct": {"fn": existence.distinct_fn},
     "count": {"fn": existence.count_fn},
     "repeat": {"fn": filtering.repeat_macro, "arity": {1: ["Expr"]}},
     "where": {"fn": filtering.where_macro, "arity": {1: ["Expr"]}},
+    "extension": {"fn": filtering.extension, "arity": {1: ["String"]}},
     "select": {"fn": filtering.select_macro, "arity": {1: ["Expr"]}},
     "single": {"fn": filtering.single_fn},
     "first": {"fn": filtering.first_fn},
     "last": {"fn": filtering.last_fn},
     "ofType": {"fn": filtering.of_type_fn, "arity": {1: ["Identifier"]}},
     "tail": {"fn": filtering.tail_fn},
     "take": {"fn": filtering.take_fn, "arity": {1: ["Integer"]}},
@@ -38,16 +39,16 @@
     "intersect": {"fn": subsetting.intersect_fn, "arity": {1: ["AnyAtRoot"]}},
     "combine": {"fn": combining.combine_fn, "arity": {1: ["AnyAtRoot"]}},
     "iif": {"fn": misc.iif_macro, "arity": {3: ["Expr", "Expr", "Expr"]}},
     "trace": {"fn": misc.trace_fn, "arity": {0: [], 1: ["String"]}},
     "toInteger": {"fn": misc.to_integer},
     "toDecimal": {"fn": misc.to_decimal},
     "toString": {"fn": misc.to_string},
-    # toDateTime:   {fn: misc.toDateTime},
-    # toTime:       {fn: misc.toTime},
+    "toDateTime": {"fn": misc.to_date_time},
+    "toTime": {"fn": misc.to_time},
     "indexOf": {"fn": strings.index_of, "arity": {1: ["String"]}, "nullable_input": True},
     "substring": {
         "fn": strings.substring,
         "arity": {1: ["Integer"], 2: ["Integer", "Integer"]},
         "nullable_input": True,
     },
     "startsWith": {"fn": strings.starts_with, "arity": {1: ["String"]}, "nullable_input": True},
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/collections.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/collections.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/constants.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/constants.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/datetime.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/datetime.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/equality.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/equality.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,19 @@
     return x == y
 
 
 def datetime_equality(ctx, x, y):
     datetime_x = x[0]
     datetime_y = y[0]
     if type(datetime_x) not in DATETIME_NODES_LIST:
-        datetime_x = nodes.FP_DateTime(datetime_x) or nodes.FP_Time(datetime_x)
+        v_x = util.get_data(datetime_x)
+        datetime_x = nodes.FP_DateTime(v_x) or nodes.FP_Time(v_x)
     if type(datetime_y) not in DATETIME_NODES_LIST:
-        datetime_y = nodes.FP_DateTime(datetime_y) or nodes.FP_Time(datetime_y)
+        v_y = util.get_data(datetime_y)
+        datetime_y = nodes.FP_DateTime(v_y) or nodes.FP_Time(v_y)
     return datetime_x.equals(datetime_y)
 
 
 def equal(ctx, a, b):
     equality_result = equality(ctx, a, b)
     return util.arraify(equality_result)
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/existence.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/existence.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/filtering.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/filtering.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numbers
 import fhirpathpy.engine.util as util
+import fhirpathpy.engine.nodes as nodes
 
 # Contains the FHIRPath Filtering and Projection functions.
 # (Section 5.2 of the FHIRPath 1.0.0 specification).
 
 """
  Adds the filtering and projection functions to the given FHIRPath engine.
 """
@@ -111,7 +112,18 @@
         return True
 
     return False
 
 
 def of_type_fn(ctx, coll, tp):
     return list(filter(lambda x: check_fhir_type(ctx, util.get_data(x), tp), coll))
+
+
+def extension(ctx, data, url):
+    res = []
+    for d in data:
+        element = util.get_data(d)
+        if isinstance(element, dict):
+            exts = [e for e in element.get("extension", []) if e["url"] == url]
+            if len(exts) > 0:
+                res.append(nodes.ResourceNode.create_node(exts[0], "Extension"))
+    return res
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/logic.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/logic.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/math.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/math.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/misc.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     if ln == 1:
         value = util.get_data(coll[0])
 
         dateTimeObject = nodes.FP_DateTime(value)
 
         if dateTimeObject:
-            rtn[0] = dateTimeObject
+            rtn.append(dateTimeObject)
 
     return rtn
 
 
 def to_time(ctx, coll):
     ln = len(coll)
     rtn = []
@@ -109,10 +109,10 @@
 
     if ln == 1:
         value = util.get_data(coll[0])
 
         timeObject = nodes.FP_Time(value)
 
         if timeObject:
-            rtn[0] = timeObject
+            rtn.append(timeObject)
 
     return rtn
```

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/navigation.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/navigation.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/invocations/strings.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/strings.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/nodes.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/nodes.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/engine/util.py` & `fhirpathpy-0.2.1/fhirpathpy/engine/util.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/ASTPathListener.py` & `fhirpathpy-0.2.1/fhirpathpy/parser/ASTPathListener.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/FHIRPath.g4` & `fhirpathpy-0.2.1/fhirpathpy/parser/FHIRPath.g4`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/__init__.py` & `fhirpathpy-0.2.1/fhirpathpy/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPath.interp` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.interp`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPath.tokens` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.tokens`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.interp` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.interp`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.py` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathLexer.tokens` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.tokens`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathListener.py` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathListener.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/fhirpathpy/parser/generated/FHIRPathParser.py` & `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathParser.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/pyproject.toml` & `fhirpathpy-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.1.2/PKG-INFO` & `fhirpathpy-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirpathpy
-Version: 0.1.2
+Version: 0.2.1
 Summary: FHIRPath implementation in Python
 Keywords: fhir,fhirpath
 Author-email: "beda.software" <fhirpath@beda.software>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

