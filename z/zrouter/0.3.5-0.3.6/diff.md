# Comparing `tmp/zrouter-0.3.5.tar.gz` & `tmp/zrouter-0.3.6.tar.gz`

## Comparing `zrouter-0.3.5.tar` & `zrouter-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 zrouter-0.3.5/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.5/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.5/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.5/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.5/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 zrouter-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zrouter-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/decorator.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/exception.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.6/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.6/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 zrouter-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zrouter-0.3.6/PKG-INFO
```

### Comparing `zrouter-0.3.5/src/zrouter/__init__.py` & `zrouter-0.3.6/src/zrouter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 'files': request.files,
                 'params': request.form.to_dict()
             }
         else:
             try:
                 params = request.get_json()
                 return json_.to_lowcase(params)
-            except JSONDecodeError:
+            except:
                 return {
                     'data': request.get_data()
                 }
 
     @staticmethod
     def clean_params(params):
         """空值参数清理"""
```

### Comparing `zrouter-0.3.5/src/zrouter/decorator.py` & `zrouter-0.3.6/src/zrouter/decorator.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.5/LICENSE` & `zrouter-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.5/pyproject.toml` & `zrouter-0.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.3.5/PKG-INFO` & `zrouter-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.3.5
+Version: 0.3.6
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

