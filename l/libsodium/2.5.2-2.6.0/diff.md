# Comparing `tmp/libsodium-2.5.2.tar.gz` & `tmp/libsodium-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsodium-2.5.2.tar", last modified: Sat Jul  1 21:50:17 2023, max compression
+gzip compressed data, was "libsodium-2.6.0.tar", last modified: Wed Jul  5 19:00:23 2023, max compression
```

## Comparing `libsodium-2.5.2.tar` & `libsodium-2.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 21:49:52.000000 libsodium-2.5.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 21:50:17.896142 libsodium-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-01 21:49:52.000000 libsodium-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 21:49:52.000000 libsodium-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-01 21:50:17.896142 libsodium-2.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.892142 libsodium-2.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.892142 libsodium-2.5.2/src/libsodium/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27113 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/src/libsodium/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/db/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/src/libsodium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.242575 libsodium-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:59:57.000000 libsodium-2.6.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-05 19:00:23.242575 libsodium-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 18:59:57.000000 libsodium-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 18:59:57.000000 libsodium-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 19:00:23.242575 libsodium-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/libsodium/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27113 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.242575 libsodium-2.6.0/src/libsodium/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/db/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/libsodium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/top_level.txt
```

### Comparing `libsodium-2.5.2/LICENCE` & `libsodium-2.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.2/PKG-INFO` & `libsodium-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.2
+Version: 2.6.0
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.52
+# Sodium v2.60
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
+
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
 pip3 install libsodium
 ```
 Windows:
```

### Comparing `libsodium-2.5.2/setup.cfg` & `libsodium-2.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libsodium
-version = 2.5.2
+version = 2.6.0
 author = Ahsan Ahmed
 author_email = ahsan.ahmed3246@gmail.com
 description = A simple web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://libsodium.readthedocs.io/en/latest/
 project_urls =
```

### Comparing `libsodium-2.5.2/src/libsodium/__main__.py` & `libsodium-2.6.0/src/libsodium/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             S:::::So::::o     o::::od:::::d     d:::::d  i::::i u:::::uuuu:::::u  m::::m   m::::m   m::::m
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 """
     print("\x1b[32m"+x+"\x1b[0m")
-    print("v2.52\nMade by ahsan")
+    print("v2.60\nMade by ahsan")
     exit()
 
 if args[0] == "init":
     print("\033[93m"+"Name for project(leave blank to use current directory):"+"\x1b[0m")
     project_name = input("\x1b[32m"+"> ")
     print("\033[93m"+"What is your interpreter(ex. python3, python, py)"+"\x1b[0m")
     interpreter = input("\x1b[32m"+"> ")
@@ -252,15 +252,15 @@
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 
     """
     print(F_Green+x+F_End)
-    print("v2.52")
+    print("v2.60")
     print(f"{getCurrentTime()} [{F_Magenta}INFO{F_End}] Creating Deamon... ")
     MainDeamon = Deamon()
 
     print(f"{getCurrentTime()} [{F_LightCyan}SocketIO{F_End}] Loading SocketIO app...")
     from src.websockets.app import sio
     from os import listdir
     from os.path import isfile
```

### Comparing `libsodium-2.5.2/src/libsodium/classes.py` & `libsodium-2.6.0/src/libsodium/classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             for i in routes:
                 self.Routes.append(i)
         except:
             raise Exception("Error while processing routes. Function 'addRoutes' requires data in format List[Route]. The format specified was not a list. You may have ment to use the Function 'addRoute' instead")
         self.onMount()
 
 """
-Blueprint API:
+Blueprint API(v1):
 Blueprints allow you to filter content that comes from the client. This
 allows you to allways expect your data in a format you define. For
 example, lets say you had a POST route under /signup. Instead of writing
 lots of checks to insure that the client has provided the required
 information to create an account. Lets say that the /signup route requires
 a username and password. Without blueprints you would have to write checks 
 to ensure that the client has provided a username and password. That would
@@ -84,22 +84,25 @@
 In the sinario above it doesn't save alot of time, but as your requests get
 bigger, the benifits of blueprinting become clear.
 """
 class Blueprint:
     def __init__(self, blueprint:list, **kwargs):
         for i in blueprint:
             if not isinstance(i, tuple) and not isinstance(i, list):
-                return "The blueprint provided had a rule that was not a tuple/array."
+                raise Exception("The blueprint provided had a rule that was not a tuple/array.")
             if len(i) > 3:
-                return "The blueprint provided contained a rule that had more than two elements."
+                print(i)
+                raise Exception("The blueprint provided contained a rule that had more than three elements.")
         self.blueprint = blueprint
-        regex = kwargs.get("regex")
-        if regex:
-            self.regex = regex
 
+class Rule:
+    def __init__(self, typ, regex=".", **kwargs) -> None:
+        self.regex = regex
+        self.typ = typ
+        
 
 def useBlueprint(b, mimetypes):
     def decorator(aclass):
         @wraps(aclass)
         def wrapper(*args,  **kwargs):
             def blueprint(self):
                 return b, mimetypes
```

### Comparing `libsodium-2.5.2/src/libsodium/wsgi.py` & `libsodium-2.6.0/src/libsodium/wsgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,20 +95,40 @@
                     rsp = controler.onRequest(request)
                 else:
                     rsp = Response('{"error":"Invalid Jwt"}', status=403)
                     rsp.headers['Content-Type'] = "application/json"
                     return rsp(environ, start_response)
 
             if hasattr(controler, "blueprint"):
+                from .classes import Blueprint
                 blueprint = controler.blueprint()
                 targetMimetypes = blueprint[1]
                 blueprint = blueprint[0]
+                #If reached, the blueprint was created using the class syntax
+                if not type(blueprint) == Blueprint:
+                    #Filter out everything but class varibles
+                    classattrs = dir(blueprint)
+                    names = []
+                    for i in classattrs:
+                        if not i.startswith("__"):
+                            names.append(i)
+                    #Get The Values
+                    values = []
+                    for i in names:
+                        values.append(eval(f"blueprint.{i}"))
+
+                    #Convert to a normal blueprint
+                    rules = []
+                    for name, value in zip(names, values):
+                        rules.append((name, value.typ, value.regex))
+                    blueprint = Blueprint(rules)
+
                 blueprint = blueprint.blueprint
                 if not request.mimetype in targetMimetypes:
-                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.52</p>")
+                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.60</p>")
                     rsp.headers['Content-Type'] = 'text/html' 
                     return rsp(environ, start_response)
                 if request.mimetype == "application/x-www-form-urlencoded":
                     target = request.form
                 elif request.mimetype == "multipart/form":
                         target = request.form
                 elif request.mimetype == "application/json":
```

### Comparing `libsodium-2.5.2/src/libsodium.egg-info/PKG-INFO` & `libsodium-2.6.0/src/libsodium.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.2
+Version: 2.6.0
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.52
+# Sodium v2.60
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
+
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
 pip3 install libsodium
 ```
 Windows:
```

