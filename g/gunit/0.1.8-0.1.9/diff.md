# Comparing `tmp/gunit-0.1.8.tar.gz` & `tmp/gunit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gunit-0.1.8.tar", last modified: Tue Dec  8 11:36:27 2020, max compression
+gzip compressed data, was "dist/gunit-0.1.9.tar", last modified: Wed Jan 20 07:57:20 2021, max compression
```

## Comparing `gunit-0.1.8.tar` & `gunit-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2020-12-08 11:36:27.400035 gunit-0.1.8/
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       90 2020-09-22 10:35:29.000000 gunit-0.1.8/MANIFEST.in
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     1018 2020-12-08 11:36:27.400035 gunit-0.1.8/PKG-INFO
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      636 2020-12-08 11:24:14.000000 gunit-0.1.8/README.md
-drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2020-12-08 11:36:27.396036 gunit-0.1.8/bin/
--rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      674 2020-12-08 11:21:30.000000 gunit-0.1.8/bin/gunit-gdbserver
--rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      370 2020-12-08 11:35:00.000000 gunit-0.1.8/bin/gunit-header
--rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      785 2020-12-08 11:21:32.000000 gunit-0.1.8/bin/gunit-openocd
-drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2020-12-08 11:36:27.396036 gunit-0.1.8/gunit/
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     3307 2020-12-08 10:48:36.000000 gunit-0.1.8/gunit/GUnit.h
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     4548 2020-09-22 14:52:10.000000 gunit-0.1.8/gunit/GUnit.py
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       25 2020-09-22 14:48:19.000000 gunit-0.1.8/gunit/__init__.py
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      416 2020-09-22 09:34:26.000000 gunit-0.1.8/gunit/execute.gdb
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       92 2020-09-21 10:01:40.000000 gunit-0.1.8/gunit/setup.gdb
-drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2020-12-08 11:36:27.400035 gunit-0.1.8/gunit.egg-info/
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     1018 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/PKG-INFO
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      338 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/SOURCES.txt
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        1 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/dependency_links.txt
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        1 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/not-zip-safe
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       10 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/requires.txt
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        6 2020-12-08 11:36:27.000000 gunit-0.1.8/gunit.egg-info/top_level.txt
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       38 2020-12-08 11:36:27.400035 gunit-0.1.8/setup.cfg
--rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      616 2020-12-08 11:35:40.000000 gunit-0.1.8/setup.py
+drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2021-01-20 07:57:20.663429 gunit-0.1.9/
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       90 2020-09-22 10:35:29.000000 gunit-0.1.9/MANIFEST.in
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     1018 2021-01-20 07:57:20.663429 gunit-0.1.9/PKG-INFO
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      636 2020-12-08 11:24:14.000000 gunit-0.1.9/README.md
+drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2021-01-20 07:57:20.659430 gunit-0.1.9/bin/
+-rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      674 2020-12-08 11:21:30.000000 gunit-0.1.9/bin/gunit-gdbserver
+-rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      370 2020-12-08 11:35:00.000000 gunit-0.1.9/bin/gunit-header
+-rwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)      785 2020-12-08 11:21:32.000000 gunit-0.1.9/bin/gunit-openocd
+drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2021-01-20 07:57:20.663429 gunit-0.1.9/gunit/
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     3350 2021-01-20 07:56:34.000000 gunit-0.1.9/gunit/GUnit.h
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     4548 2020-09-22 14:52:10.000000 gunit-0.1.9/gunit/GUnit.py
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       25 2020-09-22 14:48:19.000000 gunit-0.1.9/gunit/__init__.py
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      416 2020-09-22 09:34:26.000000 gunit-0.1.9/gunit/execute.gdb
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       92 2020-09-21 10:01:40.000000 gunit-0.1.9/gunit/setup.gdb
+drwxrwxr-x   0 mathiasplans  (1000) mathiasplans  (1000)        0 2021-01-20 07:57:20.663429 gunit-0.1.9/gunit.egg-info/
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)     1018 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/PKG-INFO
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      338 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        1 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        1 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/not-zip-safe
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       10 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/requires.txt
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)        6 2021-01-20 07:57:20.000000 gunit-0.1.9/gunit.egg-info/top_level.txt
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)       38 2021-01-20 07:57:20.663429 gunit-0.1.9/setup.cfg
+-rw-rw-r--   0 mathiasplans  (1000) mathiasplans  (1000)      616 2021-01-20 07:56:47.000000 gunit-0.1.9/setup.py
```

### Comparing `gunit-0.1.8/PKG-INFO` & `gunit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: gunit
-Version: 0.1.8
+Version: 0.1.9
 Summary: App for unit testing with GDB
 Home-page: https://github.com/estcube/GUnit
 Author: Mathias Plans
 Author-email: mathiasplans15@gmail.com
 License: MIT
 Description: # GUnit
         App for executing unit tests using GDB.
```

### Comparing `gunit-0.1.8/README.md` & `gunit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gunit-0.1.8/bin/gunit-gdbserver` & `gunit-0.1.9/bin/gunit-gdbserver`

 * *Files identical despite different names*

### Comparing `gunit-0.1.8/bin/gunit-openocd` & `gunit-0.1.9/bin/gunit-openocd`

 * *Files identical despite different names*

### Comparing `gunit-0.1.8/gunit/GUnit.h` & `gunit-0.1.9/gunit/GUnit.h`

 * *Files 5% similar despite different names*

```diff
@@ -40,30 +40,31 @@
   return;
 }
 
 /**
  * Execute a test suite
  */
 __attribute__((optimize(0)))
-inline static void gunit_suite(gunit_function_t before, gunit_function_t after, gunit_function_t *tests, uintmax_t nr_of_tests) {
+inline static void gunit_suite(gunit_function_t before, gunit_function_t after, const gunit_function_t *tests,
+                               uintmax_t nr_of_tests) {
   for (uintmax_t i = 0; i < nr_of_tests; ++i) {
     if (before)
       (*before)();
 
     (*tests[i])();
 
     if (after)
       (*after)();
   }
 }
 
 /**
  * Execute given tests with before and after functions
  */
-#define GEXECUTE(before, after, ...)  {gunit_suite(before, after, (gunit_function_t[]){__VA_ARGS__}, \
+#define GEXECUTE(before, after, ...)  {gunit_suite(before, after, (const gunit_function_t[]){__VA_ARGS__}, \
     sizeof((gunit_function_t[]){__VA_ARGS__}) / sizeof(gunit_function_t));}
 
 /**
  * Exevute tests without before or after
  */
 #define GSIMPLE_EXECUTE(...) GEXECUTE(NULL, NULL, __VA_ARGS__)
```

### Comparing `gunit-0.1.8/gunit/GUnit.py` & `gunit-0.1.9/gunit/GUnit.py`

 * *Files identical despite different names*

### Comparing `gunit-0.1.8/gunit.egg-info/PKG-INFO` & `gunit-0.1.9/gunit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: gunit
-Version: 0.1.8
+Version: 0.1.9
 Summary: App for unit testing with GDB
 Home-page: https://github.com/estcube/GUnit
 Author: Mathias Plans
 Author-email: mathiasplans15@gmail.com
 License: MIT
 Description: # GUnit
         App for executing unit tests using GDB.
```

### Comparing `gunit-0.1.8/setup.py` & `gunit-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='gunit',
-        version = '0.1.8',
+        version = '0.1.9',
         description = 'App for unit testing with GDB',
         long_description = readme(),
         url = 'https://github.com/estcube/GUnit',
         author = 'Mathias Plans',
         author_email = 'mathiasplans15@gmail.com',
         license = 'MIT',
         packages = ['gunit'],
```

