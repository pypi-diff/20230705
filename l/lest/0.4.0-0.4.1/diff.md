# Comparing `tmp/lest-0.4.0.tar.gz` & `tmp/lest-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lest-0.4.0.tar", last modified: Thu Jun 22 08:56:12 2023, max compression
+gzip compressed data, was "lest-0.4.1.tar", last modified: Wed Jul  5 07:01:31 2023, max compression
```

## Comparing `lest-0.4.0.tar` & `lest-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.390659 lest-0.4.0/
--rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1198 2023-06-22 08:56:12.389657 lest-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-06-22 08:48:11.000000 lest-0.4.0/README.md
--rw-rw-rw-   0        0        0      493 2023-06-22 08:54:20.000000 lest-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 08:56:12.390659 lest-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.300639 lest-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.367655 lest-0.4.0/src/lest/
--rw-rw-rw-   0        0        0      446 2023-06-22 08:44:53.000000 lest-0.4.0/src/lest/__init__.py
--rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.4.0/src/lest/assertions.py
--rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.4.0/src/lest/registerer.py
--rw-rw-rw-   0        0        0     2160 2023-06-22 08:50:50.000000 lest-0.4.0/src/lest/runner.py
--rw-rw-rw-   0        0        0      205 2023-06-22 08:40:08.000000 lest-0.4.0/src/lest/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:56:12.384658 lest-0.4.0/src/lest.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-22 08:56:12.000000 lest-0.4.0/src/lest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.253683 lest-0.4.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1238 2023-07-05 07:01:31.252682 lest-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-26 08:38:11.000000 lest-0.4.1/README.md
+-rw-rw-rw-   0        0        0      493 2023-07-05 06:59:57.000000 lest-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:01:31.253683 lest-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.220195 lest-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.242310 lest-0.4.1/src/lest/
+-rw-rw-rw-   0        0        0      446 2023-06-22 08:44:53.000000 lest-0.4.1/src/lest/__init__.py
+-rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.4.1/src/lest/assertions.py
+-rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.4.1/src/lest/registerer.py
+-rw-rw-rw-   0        0        0     2313 2023-07-05 06:48:27.000000 lest-0.4.1/src/lest/runner.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 08:40:08.000000 lest-0.4.1/src/lest/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.250679 lest-0.4.1/src/lest.egg-info/
+-rw-rw-rw-   0        0        0     1238 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/top_level.txt
```

### Comparing `lest-0.4.0/LICENSE` & `lest-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lest-0.4.0/PKG-INFO` & `lest-0.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.4.0
+Version: 0.4.1
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,15 @@
 
 # Lest
 
 ## Light Python library for testing
 
 ## Installing
 
-Just enter in command line:
-
-```shell
-pip install lest
-```
+See [installing](https://github.com/wchistow/lest/blob/master/docs/en/installing.md) in documentation.
 
 ## Usage
 
 ### Example:
 
 Code:
```

### Comparing `lest-0.4.0/src/lest/assertions.py` & `lest-0.4.1/src/lest/assertions.py`

 * *Files identical despite different names*

### Comparing `lest-0.4.0/src/lest/runner.py` & `lest-0.4.1/src/lest/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 
         result_table.add_column('Total tests', style='blue')
         result_table.add_column('Successful', style='green')
         result_table.add_column('Failed', style='red')
         result_table.add_column('Errors', style='red')
         result_table.add_column('Time elapsed', style='white')
 
-        result_table.add_row(str(self.successful + self.failed + self.errors),
+        total = self.successful + self.failed + self.errors
+        result_table.add_row(str(total),
                              str(self.successful),
                              str(self.failed),
                              str(self.errors),
                              '{:5.3f}'.format(self.elapsed))
 
         self.console.print(result_table)
+
+        if total != self.successful:  # some tests weren't successful
+            exit(1)
+        else:
+            exit(0)
```

### Comparing `lest-0.4.0/src/lest.egg-info/PKG-INFO` & `lest-0.4.1/src/lest.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.4.0
+Version: 0.4.1
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,15 @@
 
 # Lest
 
 ## Light Python library for testing
 
 ## Installing
 
-Just enter in command line:
-
-```shell
-pip install lest
-```
+See [installing](https://github.com/wchistow/lest/blob/master/docs/en/installing.md) in documentation.
 
 ## Usage
 
 ### Example:
 
 Code:
```

