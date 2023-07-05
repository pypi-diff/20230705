# Comparing `tmp/RobotFramework-Examples-0.2.0.tar.gz` & `tmp/RobotFramework-Examples-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobotFramework-Examples-0.2.0.tar", last modified: Fri Dec 31 15:06:20 2021, max compression
+gzip compressed data, was "RobotFramework-Examples-1.0.0.tar", last modified: Wed Jul  5 13:07:59 2023, max compression
```

## Comparing `RobotFramework-Examples-0.2.0.tar` & `RobotFramework-Examples-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 15:06:20.563573 RobotFramework-Examples-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     9910 2021-12-31 15:05:56.000000 RobotFramework-Examples-0.2.0/Examples.py
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-31 15:05:56.000000 RobotFramework-Examples-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-12-31 15:06:20.563573 RobotFramework-Examples-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-12-31 15:05:56.000000 RobotFramework-Examples-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13752 2021-12-31 15:05:56.000000 RobotFramework-Examples-0.2.0/RoboPandas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 15:06:20.563573 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-12-31 15:06:20.000000 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-12-31 15:06:20.000000 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 15:06:20.000000 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-31 15:06:20.000000 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 15:06:20.000000 RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-31 15:06:20.563573 RobotFramework-Examples-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-12-31 15:05:56.000000 RobotFramework-Examples-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:07:59.764673 RobotFramework-Examples-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-07-05 13:07:28.000000 RobotFramework-Examples-1.0.0/Examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-05 13:07:28.000000 RobotFramework-Examples-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-05 13:07:59.764673 RobotFramework-Examples-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-05 13:07:28.000000 RobotFramework-Examples-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13752 2023-07-05 13:07:28.000000 RobotFramework-Examples-1.0.0/RoboPandas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:07:59.764673 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-05 13:07:59.000000 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-05 13:07:59.000000 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:07:59.000000 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-05 13:07:59.000000 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:07:59.000000 RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 13:07:59.764673 RobotFramework-Examples-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-07-05 13:07:28.000000 RobotFramework-Examples-1.0.0/setup.py
```

### Comparing `RobotFramework-Examples-0.2.0/Examples.py` & `RobotFramework-Examples-1.0.0/Examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         self.ROBOT_LIBRARY_LISTENER = self
         self.current_suite = None
         self.autoexpand = False if hasattr(autoexpand, 'lower') and autoexpand.lower() in ['false', 'no', 'off', 'f', '0'] else autoexpand
         self.max_examples = int(max_examples) if max_examples else max_examples
         self.random = random
 
-    def _start_suite(self, suite, result):
+    def start_suite(self, suite, result):
         # save current suite so that we can modify it later
         self.current_suite = suite
         if self.autoexpand:
             self.expand_test_examples()
 
     def _localise_scope(self):
         # Create a local scope for providing keyword arguments to user
@@ -177,20 +177,25 @@
 
     def _populate_example_to_body(self, body, target):
         for kw in body:
             self.kw = kw
             if kw.type == 'KEYWORD':
                 if kw.name.lower() == 'examples:':
                     continue
+                extra_args = {}
+                if hasattr(kw, "tags"):
+                    extra_args["tags"] = self.replace_list(kw.tags)
+                if hasattr(kw, "timeout"):
+                    extra_args["timeout"] = kw.timeout
+
                 target.create_keyword(self.variables.replace_scalar(kw.name, ignore_errors=True), 
                         args = self.replace_list(kw.args),
                         assign=kw.assign,
-                        tags=self.replace_list(kw.tags),
-                        timeout=kw.timeout,
-                        lineno=kw.lineno)
+                        lineno=kw.lineno,
+                        **extra_args)
             else:
                 new_kw = kw.deepcopy()
                 new_kw.body = None
                 if hasattr(new_kw, 'values'):
                     new_kw.values = self.replace_list(kw.values)
                 if hasattr(new_kw, 'condition'):
                     new_kw.condition = self.variables.replace_scalar(kw.condition, ignore_errors=True)
```

### Comparing `RobotFramework-Examples-0.2.0/LICENSE` & `RobotFramework-Examples-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RobotFramework-Examples-0.2.0/PKG-INFO` & `RobotFramework-Examples-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: RobotFramework-Examples
-Version: 0.2.0
+Version: 1.0.0
 Summary: Examples in Robot Framework. Expands example data to individual test cases
-Home-page: UNKNOWN
 Author: Vernon Crabtree
 Author-email: vernon.b.crabtree@gmail.com
 License: Apache License 2.0
 Project-URL: Examples, https://github.com/worldline/RobotFramework-Examples
 Keywords: robotframework testing testautomation bdd gwen examples
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,9 +44,7 @@
                 ...    Patsy     it's only a model!
 
 
 Keyword information can be found here: `Keywords`_
 
 
 .. _Keywords: https://worldline.github.io/RobotFramework-Examples
-
-
```

### Comparing `RobotFramework-Examples-0.2.0/README.rst` & `RobotFramework-Examples-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `RobotFramework-Examples-0.2.0/RoboPandas.py` & `RobotFramework-Examples-1.0.0/RoboPandas.py`

 * *Files identical despite different names*

### Comparing `RobotFramework-Examples-0.2.0/RobotFramework_Examples.egg-info/PKG-INFO` & `RobotFramework-Examples-1.0.0/RobotFramework_Examples.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: RobotFramework-Examples
-Version: 0.2.0
+Version: 1.0.0
 Summary: Examples in Robot Framework. Expands example data to individual test cases
-Home-page: UNKNOWN
 Author: Vernon Crabtree
 Author-email: vernon.b.crabtree@gmail.com
 License: Apache License 2.0
 Project-URL: Examples, https://github.com/worldline/RobotFramework-Examples
 Keywords: robotframework testing testautomation bdd gwen examples
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,9 +44,7 @@
                 ...    Patsy     it's only a model!
 
 
 Keyword information can be found here: `Keywords`_
 
 
 .. _Keywords: https://worldline.github.io/RobotFramework-Examples
-
-
```

### Comparing `RobotFramework-Examples-0.2.0/setup.py` & `RobotFramework-Examples-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Topic :: Software Development :: Testing
 Framework :: Robot Framework
 Framework :: Robot Framework :: Library
 '''.strip().splitlines()
 
 setup(
     name="RobotFramework-Examples",
-    version="0.2.0",
+    version="1.0.0",
     author="Vernon Crabtree",
     author_email="vernon.b.crabtree@gmail.com",
     description="Examples in Robot Framework. Expands example data to individual test cases",
     long_description=long_description,
     license='Apache License 2.0',
     keywords='robotframework testing testautomation bdd gwen examples',
     platforms='any',
```

