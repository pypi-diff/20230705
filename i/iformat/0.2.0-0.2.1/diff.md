# Comparing `tmp/iformat-0.2.0.tar.gz` & `tmp/iformat-0.2.1.tar.gz`

## Comparing `iformat-0.2.0.tar` & `iformat-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.2.0/setup.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 iformat-0.2.0/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.2.0/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.2.0/LICENSE
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 iformat-0.2.0/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 iformat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.2.1/setup.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 iformat-0.2.1/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.2.1/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 iformat-0.2.1/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 iformat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 iformat-0.2.1/PKG-INFO
```

### Comparing `iformat-0.2.0/src/iformat/__init__.py` & `iformat-0.2.1/src/iformat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,36 +19,40 @@
 
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # finne014@gmail.com
 
 # ----------- iPrint ---------- #
+from inspect import isfunction as _if, isbuiltin as _ib, ismethod as _im
 _iters = [dict, list, tuple, set]        # NOTE: 'dict' must be first, because it has special cases
 
 def _length(i):
     return (sum([_length(k) + _length(v) + (3 if len(i.keys()) <= 1 else (2 if len(i.keys()) <= 0 else 4)) for k, v in i.items()]) + 1) if type(i) == dict else (sum([_length(x) + 2 for x in i]) if type(i) in _iters else (len(i.__class__.__name__) + _length(i.__dict__) + len(i.__dict__.keys()) - 1 if hasattr(i, "__dict__") else len(str(i))))
 
 def _brackets(datatype, newline = False, indentAmount = 0):
     return [("[" if datatype == list else "(" if datatype == tuple else "{" if datatype in [set, dict] else "") + ("\n" if datatype in _iters and newline else "") + (" " * indentAmount), ("\n" if datatype in _iters and newline else "") + (" " * indentAmount) + ("]" if datatype == list else ")" if datatype == tuple else "}" if datatype in [set, dict] else "")]
 
 def _indent(indentLevel, indentDepth):
     return " " * (indentLevel * indentDepth)
 
+def _isfunctionish(i):
+    return _if(i) or _ib(i) or _im(i)
+
 def iformat(i, indentLevel = 0, indentDepth = 4, expansionThreshold = 0):
     il, id, et = indentLevel, indentDepth, expansionThreshold
     length = _length(i)
     if type(i) in _iters:
         return (_brackets(type(i), True if length > et else False, ((il + 1) * id) if length > et else False)[0]\
             + ((",\n" + _indent(il + 1, id)) if length > et else (", ")).join(\
                     [f"{iformat(k, il + 1, id, et)}: {iformat(v, il + 1, id, et)}" for k, v in i.items()]\
                 if type(i) == dict else\
                     [iformat(x, il + 1, id, et) for x in i])\
             + _brackets(type(i), True if length > et else False, (il * id) if length > et else 0)[-1])
-    elif type(i) == function:
+    elif _isfunctionish(i):
         return f"<function {i.__name__}>"
     else:
         if "iformat" in dir(i):
             return i.iformat(il, id, et)
         elif hasattr(i, "__dict__"):
             return (f"{i.__class__.__name__}({', '.join([f'{k} = {iformat(v, il, id, et)}' for k, v in i.__dict__.items()])})")
         else:
```

### Comparing `iformat-0.2.0/.gitignore` & `iformat-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.2.0/LICENSE` & `iformat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.2.0/README.md` & `iformat-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iformat
 
-iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting, and classes are otherwise printed with all their methods.
 
 ## Parameters:
 **`indentDepth`:** *(`iprint` and `iformat`)*\
 Specifies how many spaces should be inserted as one indent level. Default `4`.
 
 **`expansionThreshold`**: *(`iprint` and `iformat`)*\
 Specifies how long an object must be when printed before it is shown in a muilti-line format. Default `0`.\
```

### Comparing `iformat-0.2.0/PKG-INFO` & `iformat-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.2.0
-Summary: Provides a function that indents and pretty prints data structures
+Version: 0.2.1
+Summary: Indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # iformat
 
-iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting, and classes are otherwise printed with all their methods.
 
 ## Parameters:
 **`indentDepth`:** *(`iprint` and `iformat`)*\
 Specifies how many spaces should be inserted as one indent level. Default `4`.
 
 **`expansionThreshold`**: *(`iprint` and `iformat`)*\
 Specifies how long an object must be when printed before it is shown in a muilti-line format. Default `0`.\
```

