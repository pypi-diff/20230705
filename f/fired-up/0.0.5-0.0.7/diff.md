# Comparing `tmp/fired-up-0.0.5.tar.gz` & `tmp/fired-up-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fired-up-0.0.5.tar", last modified: Sun Jun 25 07:09:45 2023, max compression
+gzip compressed data, was "fired-up-0.0.7.tar", last modified: Wed Jul  5 19:34:40 2023, max compression
```

## Comparing `fired-up-0.0.5.tar` & `fired-up-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474934 fired-up-0.0.5/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474027 fired-up-0.0.5/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     5171 2023-06-25 07:00:13.000000 fired-up-0.0.5/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.5/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.5/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     7174 2023-06-25 07:09:45.474818 fired-up-0.0.5/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474141 fired-up-0.0.5/fired_up/
--rw-r--r--   0 xtof       (501) staff       (20)     3039 2023-06-25 06:57:57.000000 fired-up-0.0.5/fired_up/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 07:09:45.474643 fired-up-0.0.5/fired_up.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     7174 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-25 07:09:45.000000 fired-up-0.0.5/fired_up.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-25 07:09:45.474975 fired-up-0.0.5/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.5/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-05 19:34:40.483506 fired-up-0.0.7/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-05 19:34:40.482164 fired-up-0.0.7/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     6628 2023-07-05 19:27:28.000000 fired-up-0.0.7/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.7/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.7/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     9231 2023-07-05 19:34:40.483344 fired-up-0.0.7/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-05 19:34:40.482280 fired-up-0.0.7/fired_up/
+-rw-r--r--   0 xtof       (501) staff       (20)     3340 2023-07-05 19:32:35.000000 fired-up-0.0.7/fired_up/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-05 19:34:40.482786 fired-up-0.0.7/fired_up.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     9231 2023-07-05 19:34:40.000000 fired-up-0.0.7/fired_up.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      318 2023-07-05 19:34:40.000000 fired-up-0.0.7/fired_up.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-05 19:34:40.000000 fired-up-0.0.7/fired_up.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       12 2023-07-05 19:34:40.000000 fired-up-0.0.7/fired_up.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       15 2023-07-05 19:34:40.000000 fired-up-0.0.7/fired_up.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-05 19:34:40.483543 fired-up-0.0.7/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1392 2023-06-25 19:48:26.000000 fired-up-0.0.7/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-05 19:34:40.483162 fired-up-0.0.7/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-06-25 19:36:30.000000 fired-up-0.0.7/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      405 2023-06-25 19:49:40.000000 fired-up-0.0.7/tests/conftest.py
+-rw-r--r--   0 xtof       (501) staff       (20)      373 2023-07-05 19:22:55.000000 fired-up-0.0.7/tests/test_function_commands.py
+-rw-r--r--   0 xtof       (501) staff       (20)      472 2023-07-05 19:28:37.000000 fired-up-0.0.7/tests/test_hello.py
```

### Comparing `fired-up-0.0.5/.github/README.md` & `fired-up-0.0.7/.github/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -128,23 +128,23 @@
 class Left(Group):
   def __init__(self, write, *args, **kwargs):
     super().__init__(*args, **kwargs)
     self._write = write
 
   def write(self):
     if self._write:
-      self.globals["message"] = "left was here"
+      self._globals["message"] = "left was here"
 
   def read(self):
-    print("left>", self.globals["message"])
+    print("left>", self._globals["message"])
 
 class Right(Group):
   def readwrite(self):
-    print("right>", self.globals["message"])
-    self.globals["message"] = "right was here too"
+    print("right>", self._globals["message"])
+    self._globals["message"] = "right was here too"
 
 FiredUp(left=(Left, { "write" : True }), right=Right)
 ```
 
 ```console
 % python examples/globals.py left write then right readwrite then left read
 right> left was here
@@ -186,7 +186,82 @@
 ```console
 % python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
 Commands> running...
 SubCommands> running...
 Commands> running...
 SubSubCommands> running...
 ```
+
+### Simple Commands
+
+Besides objects with commands and menus, you can also simply provide a function, which will be handled as a command:
+
+```python
+from fired_up import FiredUp, __version__
+
+def get_hello():
+  return "hello"
+
+def get_version():
+  return __version__
+  
+FiredUp(hello=get_hello, version=get_version)
+```
+
+```console
+% python examples/version.py --all hello then version
+hello
+0.0.7
+```
+
+### Public Functions and Output
+
+Since `FiredUp` makes all public functions chainable, public functions that return some value can't be used directly by other functions. To access the original return value one can use `.paste()` in a chaining way:
+
+```python
+from fired_up import FiredUp, Group
+
+class Test(Group):
+  def public1(self):
+    return "abc"                  # return value is "copied", self is returned
+
+  def public2(self):
+    print(self.public1().paste()) # returns the return value of public
+
+  def public3(self):
+    return self.public1()         # returns self, which is "pasted" as last result
+
+FiredUp(test=Test)
+```
+
+```console
+% python examples/public.py test public1
+abc
+% python examples/public.py test public2
+abc
+% python examples/public.py test public3
+NAME
+    public.py test public3
+
+SYNOPSIS
+    public.py test public3 GROUP | COMMAND
+
+GROUPS
+    GROUP is one of the following:
+
+     globals
+
+COMMANDS
+    COMMAND is one of the following:
+
+     copy
+
+     paste
+
+     public1
+
+     public2
+
+     public3
+
+     then
+```
```

### Comparing `fired-up-0.0.5/LICENSE.txt` & `fired-up-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fired-up-0.0.5/PKG-INFO` & `fired-up-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.5
+Version: 0.0.7
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -135,23 +135,23 @@
         class Left(Group):
           def __init__(self, write, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self._write = write
         
           def write(self):
             if self._write:
-              self.globals["message"] = "left was here"
+              self._globals["message"] = "left was here"
         
           def read(self):
-            print("left>", self.globals["message"])
+            print("left>", self._globals["message"])
         
         class Right(Group):
           def readwrite(self):
-            print("right>", self.globals["message"])
-            self.globals["message"] = "right was here too"
+            print("right>", self._globals["message"])
+            self._globals["message"] = "right was here too"
         
         FiredUp(left=(Left, { "write" : True }), right=Right)
         ```
         
         ```console
         % python examples/globals.py left write then right readwrite then left read
         right> left was here
@@ -194,13 +194,88 @@
         % python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
         Commands> running...
         SubCommands> running...
         Commands> running...
         SubSubCommands> running...
         ```
         
+        ### Simple Commands
+        
+        Besides objects with commands and menus, you can also simply provide a function, which will be handled as a command:
+        
+        ```python
+        from fired_up import FiredUp, __version__
+        
+        def get_hello():
+          return "hello"
+        
+        def get_version():
+          return __version__
+          
+        FiredUp(hello=get_hello, version=get_version)
+        ```
+        
+        ```console
+        % python examples/version.py --all hello then version
+        hello
+        0.0.7
+        ```
+        
+        ### Public Functions and Output
+        
+        Since `FiredUp` makes all public functions chainable, public functions that return some value can't be used directly by other functions. To access the original return value one can use `.paste()` in a chaining way:
+        
+        ```python
+        from fired_up import FiredUp, Group
+        
+        class Test(Group):
+          def public1(self):
+            return "abc"                  # return value is "copied", self is returned
+        
+          def public2(self):
+            print(self.public1().paste()) # returns the return value of public
+        
+          def public3(self):
+            return self.public1()         # returns self, which is "pasted" as last result
+        
+        FiredUp(test=Test)
+        ```
+        
+        ```console
+        % python examples/public.py test public1
+        abc
+        % python examples/public.py test public2
+        abc
+        % python examples/public.py test public3
+        NAME
+            public.py test public3
+        
+        SYNOPSIS
+            public.py test public3 GROUP | COMMAND
+        
+        GROUPS
+            GROUP is one of the following:
+        
+             globals
+        
+        COMMANDS
+            COMMAND is one of the following:
+        
+             copy
+        
+             paste
+        
+             public1
+        
+             public2
+        
+             public3
+        
+             then
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.5/fired_up/__init__.py` & `fired-up-0.0.7/fired_up/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 
   conventions and supporting tools for using Fire in a more natural-ish
   language style
 
 """
-__version__ = "0.0.5"
+__version__ = "0.0.7"
 
 import sys
 import functools
 
 import fire
 
 class Group():
@@ -17,40 +17,39 @@
   baseclass for command groups
   
   """
   def __init__(self, _parent=None):
     self._parent = _parent
 
   @property
-  def globals(self):
+  def _globals(self):
     return self._shared["globals"]
 
   @property
   def _shared(self):
     if self._parent:
       return self._parent._shared
     return None
 
   def then(self):
     return self._shared["exit"]
 
-  def copy(self, value, name="default"):
+  def copy(self, value, name="default", advance=False):
     self._shared["clipboard"][name] = value
+    if advance:
+      next(self._shared["clipboard"])
     return self
 
   def paste(self, name="default"):
     return self._shared["clipboard"][name]
 
 def keep(method):
   @functools.wraps(method)
   def wrapper(self, *args, **kwargs):
-    result = method(self, *args, **kwargs)
-    self.copy(result)
-    if result:
-      next(self._shared["clipboard"])
+    self.copy(method(self, *args, **kwargs), advance=True)
     return self
   return wrapper
 
 class Clipboards():
   """
   
   simple multi-clipboard support
@@ -72,67 +71,70 @@
     except:
       pass
     return None
 
   def __str__(self):
     return str(self._boards)
 
-if "--all" in sys.argv:
-  sys.argv.remove("--all")
-  def paste_result(obj):
-    return [board["default"] for board in obj._shared["clipboard"]._boards[:-1] ]
-else:
-  def paste_result(obj):
-    return obj.paste()
-
 class Menu(Group):
   """
   
   a menu is a set of groups or other menus
   
   """
   def __init__(self, **kwargs):
     super().__init__()
-
-    for group, clazz in kwargs.items():
-      # unpack tuple(clazz, arguments)
-      if type(clazz) is tuple:
-        clazz, args = clazz
+    for group, handler in kwargs.items():
+      # unpack optional tuple(handler, arguments)
+      if type(handler) is tuple:
+        handler, args = handler
       else:
         args = {}
-      # only handle classes, objects are used verbatim
-      if isinstance(clazz, type):
-        # make sure all public methods return self to allow for chaining
-        for attr in clazz.__dict__:
-          if callable(getattr(clazz, attr)) and attr[0] != "_":
-            setattr(clazz, attr, keep(getattr(clazz, attr)))
-        self.__dict__[group] = clazz(_parent=self, **args)
-      elif isinstance(clazz, Menu):
-        # handle "sub"menu's, which are already created and need a ref to the
-        # shared
-        self.__dict__[group] = clazz
-        clazz._parent = self
+
+      if isinstance(handler, type):
+        # make sure all "public" methods return self to allow for chaining
+        for attr in handler.__dict__:
+          if callable(getattr(handler, attr)) and attr[0] != "_":
+            setattr(handler, attr, keep(getattr(handler, attr)))
+        self.__dict__[group] = handler(_parent=self, **args)
+      elif isinstance(handler, Menu):
+        # handle "sub"menu's, which are already objects and need merely a ref
+        # to this parent, to allow for finding the top-level shared data
+        self.__dict__[group] = handler
+        handler._parent = self
+      elif callable(handler):
+        # simple functions
+        self.__dict__[group] = (lambda f: lambda: self.copy(f(), advance=True))(handler)
       else:
-        raise ValueError("classes or Menu's, nothing else please")
+        raise ValueError(f"Classes or other Menu'. Got '{type(handler)}'.")
 
 class FiredUp(Menu):
-  """
-  
-  the FiredUp class is the root-menu and holds the shared globals and clipboard
-  
-  """
-  
-  def __init__(self, name=None, **kwargs):
+
+  def __init__(self, name=None, command=None, all_results=False, **kwargs):
     self._actual_shared = {
       "clipboard" : Clipboards(),
       "globals"   : {},
       "exit"      : self
     }
+    if "--all" in sys.argv:
+      sys.argv.remove("--all")
+      all_results = True
+
+    if all_results:
+      def paste_result(obj):
+        return [board["default"] for board in obj._shared["clipboard"]._boards[:-1] ]
+    else:
+      def paste_result(obj):
+        try:
+          return obj.paste()
+        except AttributeError:
+          return obj
+    
     super().__init__(**kwargs)
     try:
-      fire.Fire(self, name=name, serialize=paste_result)
+      fire.Fire(self, name=name, command=command, serialize=paste_result)
     except KeyboardInterrupt:
       pass
 
   @property
   def _shared(self):
     return self._actual_shared
```

### Comparing `fired-up-0.0.5/fired_up.egg-info/PKG-INFO` & `fired-up-0.0.7/fired_up.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.5
+Version: 0.0.7
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -135,23 +135,23 @@
         class Left(Group):
           def __init__(self, write, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self._write = write
         
           def write(self):
             if self._write:
-              self.globals["message"] = "left was here"
+              self._globals["message"] = "left was here"
         
           def read(self):
-            print("left>", self.globals["message"])
+            print("left>", self._globals["message"])
         
         class Right(Group):
           def readwrite(self):
-            print("right>", self.globals["message"])
-            self.globals["message"] = "right was here too"
+            print("right>", self._globals["message"])
+            self._globals["message"] = "right was here too"
         
         FiredUp(left=(Left, { "write" : True }), right=Right)
         ```
         
         ```console
         % python examples/globals.py left write then right readwrite then left read
         right> left was here
@@ -194,13 +194,88 @@
         % python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
         Commands> running...
         SubCommands> running...
         Commands> running...
         SubSubCommands> running...
         ```
         
+        ### Simple Commands
+        
+        Besides objects with commands and menus, you can also simply provide a function, which will be handled as a command:
+        
+        ```python
+        from fired_up import FiredUp, __version__
+        
+        def get_hello():
+          return "hello"
+        
+        def get_version():
+          return __version__
+          
+        FiredUp(hello=get_hello, version=get_version)
+        ```
+        
+        ```console
+        % python examples/version.py --all hello then version
+        hello
+        0.0.7
+        ```
+        
+        ### Public Functions and Output
+        
+        Since `FiredUp` makes all public functions chainable, public functions that return some value can't be used directly by other functions. To access the original return value one can use `.paste()` in a chaining way:
+        
+        ```python
+        from fired_up import FiredUp, Group
+        
+        class Test(Group):
+          def public1(self):
+            return "abc"                  # return value is "copied", self is returned
+        
+          def public2(self):
+            print(self.public1().paste()) # returns the return value of public
+        
+          def public3(self):
+            return self.public1()         # returns self, which is "pasted" as last result
+        
+        FiredUp(test=Test)
+        ```
+        
+        ```console
+        % python examples/public.py test public1
+        abc
+        % python examples/public.py test public2
+        abc
+        % python examples/public.py test public3
+        NAME
+            public.py test public3
+        
+        SYNOPSIS
+            public.py test public3 GROUP | COMMAND
+        
+        GROUPS
+            GROUP is one of the following:
+        
+             globals
+        
+        COMMANDS
+            COMMAND is one of the following:
+        
+             copy
+        
+             paste
+        
+             public1
+        
+             public2
+        
+             public3
+        
+             then
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.5/setup.py` & `fired-up-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 CLASSIFIERS      = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
   
 ]
 INSTALL_REQUIRES = [
-  "fire",
+  "fire==0.5.0",
   
 ]
 ENTRY_POINTS = {
   
 }
 SCRIPTS = [
```

