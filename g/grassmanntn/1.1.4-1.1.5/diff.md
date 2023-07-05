# Comparing `tmp/grassmanntn-1.1.4.tar.gz` & `tmp/grassmanntn-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.4.tar", last modified: Wed Jul  5 08:49:17 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.5.tar", last modified: Wed Jul  5 09:18:35 2023, max compression
```

## Comparing `grassmanntn-1.1.4.tar` & `grassmanntn-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 08:49:17.055994 grassmanntn-1.1.4/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.4/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 08:49:17.055994 grassmanntn-1.1.4/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.4/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 08:49:17.055994 grassmanntn-1.1.4/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109545 2023-07-05 08:48:00.000000 grassmanntn-1.1.4/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.4/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.4/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.4/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 08:49:17.055994 grassmanntn-1.1.4/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 08:49:17.000000 grassmanntn-1.1.4/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-05 08:49:17.000000 grassmanntn-1.1.4/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-05 08:49:17.000000 grassmanntn-1.1.4/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-05 08:49:17.000000 grassmanntn-1.1.4/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-05 08:49:17.000000 grassmanntn-1.1.4/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-05 08:49:17.055994 grassmanntn-1.1.4/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-05 08:48:54.000000 grassmanntn-1.1.4/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.5/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.5/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109541 2023-07-05 09:17:07.000000 grassmanntn-1.1.5/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.5/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.5/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.5/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-05 09:18:09.000000 grassmanntn-1.1.5/setup.py
```

### Comparing `grassmanntn-1.1.4/LICENSE.txt` & `grassmanntn-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.4/PKG-INFO` & `grassmanntn-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.4
+Version: 1.1.5
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_114.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.4/README.md` & `grassmanntn-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.4/grassmanntn/__init__.py` & `grassmanntn-1.1.5/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: dense")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistics:",self.statistics)
+        print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
         iterator = np.nditer(self, flags=['multi_index'])
         for element in iterator:
@@ -340,15 +340,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: dense")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistics:",self.statistics)
+        print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print()
 
     def copy(self):
@@ -624,15 +624,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: sparse")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistics:",self.statistics)
+        print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
 
         C = self.coords
@@ -650,15 +650,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: sparse")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistics:",self.statistics)
+        print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print()
 
     def set_value(self,entry,value):
```

### Comparing `grassmanntn-1.1.4/grassmanntn/example.py` & `grassmanntn-1.1.5/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.4/grassmanntn/gauge2d.py` & `grassmanntn-1.1.5/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.4/grassmanntn/param.py` & `grassmanntn-1.1.5/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.4/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.5/grassmanntn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.4
+Version: 1.1.5
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_114.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.4/setup.py` & `grassmanntn-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.4',      # Start with a small number and increase it with every change you make
+  version = '1.1.5',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_114.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

