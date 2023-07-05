# Comparing `tmp/captain-4.4.0.tar.gz` & `tmp/captain-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captain-4.4.0.tar", last modified: Fri Mar  3 23:34:48 2023, max compression
+gzip compressed data, was "captain-4.5.0.tar", last modified: Wed Jul  5 18:02:48 2023, max compression
```

## Comparing `captain-4.4.0.tar` & `captain-4.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-03 23:34:48.888964 captain-4.4.0/
--rw-r--r--   0 jaymon     (501) staff       (20)     1083 2016-04-19 06:38:53.000000 captain-4.4.0/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     5420 2023-03-03 23:34:48.888821 captain-4.4.0/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     4818 2020-07-10 22:08:55.000000 captain-4.4.0/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-03 23:34:48.887741 captain-4.4.0/captain/
--rw-r--r--   0 jaymon     (501) staff       (20)      585 2023-03-03 22:10:13.000000 captain-4.4.0/captain/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)       97 2020-08-20 00:36:38.000000 captain-4.4.0/captain/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2290 2023-03-03 22:08:39.000000 captain-4.4.0/captain/decorators.py
--rw-r--r--   0 jaymon     (501) staff       (20)      346 2020-06-26 08:02:10.000000 captain-4.4.0/captain/environ.py
--rw-r--r--   0 jaymon     (501) staff       (20)      882 2020-06-27 07:47:48.000000 captain-4.4.0/captain/exception.py
--rw-r--r--   0 jaymon     (501) staff       (20)     8455 2023-03-03 22:08:59.000000 captain-4.4.0/captain/interface.py
--rw-r--r--   0 jaymon     (501) staff       (20)    26711 2022-12-21 02:35:25.000000 captain-4.4.0/captain/io.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3313 2022-12-21 02:36:09.000000 captain-4.4.0/captain/logging.py
--rw-r--r--   0 jaymon     (501) staff       (20)    18378 2022-12-21 23:51:53.000000 captain-4.4.0/captain/parse.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10352 2022-12-21 03:33:37.000000 captain-4.4.0/captain/reflection.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-03 23:34:48.888653 captain-4.4.0/captain.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     5420 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      411 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       54 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/entry_points.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        8 2023-03-03 23:34:48.000000 captain-4.4.0/captain.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-03-03 23:34:48.889007 captain-4.4.0/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1961 2023-03-03 22:09:18.000000 captain-4.4.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 18:02:48.946000 captain-4.5.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1083 2016-04-19 06:38:53.000000 captain-4.5.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     5400 2023-07-05 18:02:48.945847 captain-4.5.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     4818 2020-07-10 22:08:55.000000 captain-4.5.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 18:02:48.944162 captain-4.5.0/captain/
+-rw-r--r--   0 jaymon     (501) staff       (20)      585 2023-07-05 17:59:39.000000 captain-4.5.0/captain/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)       97 2020-08-20 00:36:38.000000 captain-4.5.0/captain/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2290 2023-03-03 22:08:39.000000 captain-4.5.0/captain/decorators.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      346 2020-06-26 08:02:10.000000 captain-4.5.0/captain/environ.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      882 2020-06-27 07:47:48.000000 captain-4.5.0/captain/exception.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     8455 2023-03-03 22:08:59.000000 captain-4.5.0/captain/interface.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    26711 2022-12-21 02:35:25.000000 captain-4.5.0/captain/io.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3313 2022-12-21 02:36:09.000000 captain-4.5.0/captain/logging.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    18452 2023-07-05 17:48:22.000000 captain-4.5.0/captain/parse.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    10352 2022-12-21 03:33:37.000000 captain-4.5.0/captain/reflection.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 18:02:48.945425 captain-4.5.0/captain.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     5400 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      411 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       53 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/entry_points.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        8 2023-07-05 18:02:48.000000 captain-4.5.0/captain.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-05 18:02:48.946048 captain-4.5.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1961 2023-03-03 22:09:18.000000 captain-4.5.0/setup.py
```

### Comparing `captain-4.4.0/LICENSE.txt` & `captain-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/PKG-INFO` & `captain-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: captain
-Version: 4.4.0
+Version: 4.5.0
 Summary: python cli scripts for humans
 Home-page: http://github.com/jaymon/captain
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: cli console
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -214,9 +213,7 @@
 
     $ pip install captain
 
 For latest and greatest:
 
     $ pip install -U "git+https://github.com/Jaymon/captain#egg=captain"
 
-
-
```

### Comparing `captain-4.4.0/README.md` & `captain-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/__init__.py` & `captain-4.5.0/captain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .interface import Captain
 from .interface import Command # extend this to create commands/subcommands in your scripts
 from .decorators import arg, args
 from . import exception
 from .exception import Stop, Error
 
 
-__version__ = "4.4.0"
+__version__ = "4.5.0"
 
 
 # get rid of "No handler found" warnings (cribbed from requests)
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 handle = Captain.get_instance().handle # invoke this at the end of your script
```

### Comparing `captain-4.4.0/captain/decorators.py` & `captain-4.5.0/captain/decorators.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/exception.py` & `captain-4.5.0/captain/exception.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/interface.py` & `captain-4.5.0/captain/interface.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/io.py` & `captain-4.5.0/captain/io.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/logging.py` & `captain-4.5.0/captain/logging.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain/parse.py` & `captain-4.5.0/captain/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,15 +366,18 @@
         # lots of them) but still support aliasing of the subcommands
         if argv and argv[0] in self.subcommand_aliases:
             argv[0] = self.subcommand_aliases[argv[0]]
 
         parsed, parsed_unknown = self.parse_known_args(argv)
 
         if parsed_unknown:
-            unknown_kwargs = UnknownParser(parsed_unknown)
+            unknown_kwargs = UnknownParser(
+                parsed_unknown,
+                hyphen_to_underscore=True,
+            )
             unknown_args = unknown_kwargs.pop("*", [])
             unknown_kwargs = unknown_kwargs.unwrap()
 
             if parsed._arg_count > 0:
 
                 if unknown_args and not parsed._has_handle_args:
                     # we parse again with the more restrictive parser to raise the error
```

### Comparing `captain-4.4.0/captain/reflection.py` & `captain-4.5.0/captain/reflection.py`

 * *Files identical despite different names*

### Comparing `captain-4.4.0/captain.egg-info/PKG-INFO` & `captain-4.5.0/captain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: captain
-Version: 4.4.0
+Version: 4.5.0
 Summary: python cli scripts for humans
 Home-page: http://github.com/jaymon/captain
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: cli console
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -214,9 +213,7 @@
 
     $ pip install captain
 
 For latest and greatest:
 
     $ pip install -U "git+https://github.com/Jaymon/captain#egg=captain"
 
-
-
```

### Comparing `captain-4.4.0/setup.py` & `captain-4.5.0/setup.py`

 * *Files identical despite different names*

