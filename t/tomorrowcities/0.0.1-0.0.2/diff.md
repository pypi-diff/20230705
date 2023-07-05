# Comparing `tmp/tomorrowcities-0.0.1.tar.gz` & `tmp/tomorrowcities-0.0.2.tar.gz`

## Comparing `tomorrowcities-0.0.1.tar` & `tomorrowcities-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/src/tomorrowcities/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/src/tomorrowcities/datagenerator.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/LICENSE
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 tomorrowcities-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/src/tomorrowcities/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/src/tomorrowcities/core.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/LICENSE
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 tomorrowcities-0.0.2/PKG-INFO
```

### Comparing `tomorrowcities-0.0.1/LICENSE` & `tomorrowcities-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomorrowcities-0.0.1/pyproject.toml` & `tomorrowcities-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tomorrowcities"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Huseyin Kaya", email="hkayabilisim@gmail.com" },
   { name="Prashant Rawal", email="prashantrawal@nset.org.np" },
   { name="Erdem Ozer", email="ozerer@gmail.com" },
 ]
 description = "Tomorrow Cities' Python Library"
 readme = "README.md"
```

### Comparing `tomorrowcities-0.0.1/PKG-INFO` & `tomorrowcities-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomorrowcities
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tomorrow Cities' Python Library
 Project-URL: Homepage, https://github.com/TomorrowsCities
 Project-URL: Bug Tracker, https://github.com/TomorrowsCities
 Author-email: Huseyin Kaya <hkayabilisim@gmail.com>, Prashant Rawal <prashantrawal@nset.org.np>, Erdem Ozer <ozerer@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

