# Comparing `tmp/chargemaster_parsers-0.0.3.tar.gz` & `tmp/chargemaster_parsers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chargemaster_parsers-0.0.3.tar", last modified: Sun Jun 25 19:47:45 2023, max compression
+gzip compressed data, was "chargemaster_parsers-0.0.4.tar", last modified: Tue Jul  4 22:11:23 2023, max compression
```

## Comparing `chargemaster_parsers-0.0.3.tar` & `chargemaster_parsers-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.567427 chargemaster_parsers-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-05-28 05:22:14.000000 chargemaster_parsers-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6837 2023-06-25 19:47:45.566926 chargemaster_parsers-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6343 2023-06-23 06:01:09.000000 chargemaster_parsers-0.0.3/README.md
--rw-rw-rw-   0        0        0      630 2023-06-25 19:46:31.000000 chargemaster_parsers-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 19:47:45.567427 chargemaster_parsers-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.542926 chargemaster_parsers-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.546926 chargemaster_parsers-0.0.3/src/chargemaster_parsers/
--rw-rw-rw-   0        0        0       39 2023-06-08 05:45:26.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.558426 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/
--rw-rw-rw-   0        0        0      493 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/__init__.py
--rw-rw-rw-   0        0        0     3627 2023-06-11 04:50:47.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/cedars_sinai.py
--rw-rw-rw-   0        0        0     4512 2023-06-11 04:49:06.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/kaiser.py
--rw-rw-rw-   0        0        0     3121 2023-06-11 04:57:40.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/parsers.py
--rw-rw-rw-   0        0        0      810 2023-06-11 04:48:59.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/rady.py
--rw-rw-rw-   0        0        0     7727 2023-06-23 06:11:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/scripps.py
--rw-rw-rw-   0        0        0    19082 2023-06-11 04:45:30.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/sharp.py
--rw-rw-rw-   0        0        0    12028 2023-06-25 05:34:46.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/stanford.py
--rw-rw-rw-   0        0        0     2641 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/uci.py
--rw-rw-rw-   0        0        0     8004 2023-06-19 06:39:14.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/ucsd.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.550927 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/
--rw-rw-rw-   0        0        0     6837 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.565927 chargemaster_parsers-0.0.3/tests/
--rw-rw-rw-   0        0        0     3638 2023-06-11 04:56:03.000000 chargemaster_parsers-0.0.3/tests/test_cedars_sinai.py
--rw-rw-rw-   0        0        0     3547 2023-06-11 04:55:34.000000 chargemaster_parsers-0.0.3/tests/test_kaiser.py
--rw-rw-rw-   0        0        0     2420 2023-06-08 06:21:40.000000 chargemaster_parsers-0.0.3/tests/test_parser.py
--rw-rw-rw-   0        0        0     1700 2023-06-11 04:55:08.000000 chargemaster_parsers-0.0.3/tests/test_rady.py
--rw-rw-rw-   0        0        0     6802 2023-06-23 06:16:44.000000 chargemaster_parsers-0.0.3/tests/test_scripps.py
--rw-rw-rw-   0        0        0     2094 2023-06-11 04:54:22.000000 chargemaster_parsers-0.0.3/tests/test_sharp.py
--rw-rw-rw-   0        0        0     4185 2023-06-25 05:38:02.000000 chargemaster_parsers-0.0.3/tests/test_stanford.py
--rw-rw-rw-   0        0        0     3804 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/tests/test_uci.py
--rw-rw-rw-   0        0        0    22776 2023-06-23 06:17:01.000000 chargemaster_parsers-0.0.3/tests/test_ucsd.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.862829 chargemaster_parsers-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-05-28 05:22:14.000000 chargemaster_parsers-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6837 2023-07-04 22:11:23.862829 chargemaster_parsers-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6343 2023-06-23 06:01:09.000000 chargemaster_parsers-0.0.4/README.md
+-rw-rw-rw-   0        0        0      630 2023-07-04 22:10:45.000000 chargemaster_parsers-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 22:11:23.862829 chargemaster_parsers-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.832046 chargemaster_parsers-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.836046 chargemaster_parsers-0.0.4/src/chargemaster_parsers/
+-rw-rw-rw-   0        0        0       39 2023-06-08 05:45:26.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.852328 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/
+-rw-rw-rw-   0        0        0      591 2023-07-03 02:28:25.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/__init__.py
+-rw-rw-rw-   0        0        0     3627 2023-06-11 04:50:47.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/cedars_sinai.py
+-rw-rw-rw-   0        0        0     4512 2023-06-11 04:49:06.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/kaiser.py
+-rw-rw-rw-   0        0        0     2128 2023-07-03 02:39:45.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/palomar.py
+-rw-rw-rw-   0        0        0     3144 2023-07-03 01:27:31.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/parsers.py
+-rw-rw-rw-   0        0        0      810 2023-06-11 04:48:59.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/rady.py
+-rw-rw-rw-   0        0        0     7727 2023-06-23 06:11:45.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/scripps.py
+-rw-rw-rw-   0        0        0    19082 2023-06-11 04:45:30.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/sharp.py
+-rw-rw-rw-   0        0        0     6762 2023-07-03 01:59:56.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/southwest.py
+-rw-rw-rw-   0        0        0    12028 2023-06-25 05:34:46.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/stanford.py
+-rw-rw-rw-   0        0        0     2641 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/uci.py
+-rw-rw-rw-   0        0        0     8004 2023-06-19 06:39:14.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/ucsd.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.839547 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/
+-rw-rw-rw-   0        0        0     6837 2023-07-04 22:11:23.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-04 22:11:23.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 22:11:23.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-04 22:11:23.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-04 22:11:23.000000 chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 22:11:23.861828 chargemaster_parsers-0.0.4/tests/
+-rw-rw-rw-   0        0        0     3638 2023-06-11 04:56:03.000000 chargemaster_parsers-0.0.4/tests/test_cedars_sinai.py
+-rw-rw-rw-   0        0        0     3547 2023-06-11 04:55:34.000000 chargemaster_parsers-0.0.4/tests/test_kaiser.py
+-rw-rw-rw-   0        0        0     1576 2023-07-03 02:33:56.000000 chargemaster_parsers-0.0.4/tests/test_palomar.py
+-rw-rw-rw-   0        0        0     2420 2023-06-08 06:21:40.000000 chargemaster_parsers-0.0.4/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1700 2023-06-11 04:55:08.000000 chargemaster_parsers-0.0.4/tests/test_rady.py
+-rw-rw-rw-   0        0        0     6802 2023-06-23 06:16:44.000000 chargemaster_parsers-0.0.4/tests/test_scripps.py
+-rw-rw-rw-   0        0        0     2094 2023-06-11 04:54:22.000000 chargemaster_parsers-0.0.4/tests/test_sharp.py
+-rw-rw-rw-   0        0        0    18949 2023-07-03 01:58:28.000000 chargemaster_parsers-0.0.4/tests/test_southwest.py
+-rw-rw-rw-   0        0        0     4185 2023-06-25 05:38:02.000000 chargemaster_parsers-0.0.4/tests/test_stanford.py
+-rw-rw-rw-   0        0        0     3804 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.4/tests/test_uci.py
+-rw-rw-rw-   0        0        0    22776 2023-06-23 06:17:01.000000 chargemaster_parsers-0.0.4/tests/test_ucsd.py
```

### Comparing `chargemaster_parsers-0.0.3/LICENSE` & `chargemaster_parsers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/PKG-INFO` & `chargemaster_parsers-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chargemaster_parsers
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for parsing machine readable healthcare chargemasters
 Author: Jacob Schaer, Yvonne Kaire
 Project-URL: Homepage, https://github.com/jacobschaer/chargemaster_parsers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chargemaster_parsers-0.0.3/README.md` & `chargemaster_parsers-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/pyproject.toml` & `chargemaster_parsers-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chargemaster_parsers"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jacob Schaer" },
   { name="Yvonne Kaire" }
 ]
 description = "A library for parsing machine readable healthcare chargemasters"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/cedars_sinai.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/cedars_sinai.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/kaiser.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/kaiser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/parsers.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "max_reimbursement",
         "min_reimbursement",
         "expected_reimbursement",
         "in_patient",
         "payer",
         "plan",
         "gross_charge",
+        "extra_data",
 
         # Unused
         "charge_code",
         "quantity",
         "in_patient_price"
     ])
```

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/rady.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/rady.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/scripps.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/scripps.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/sharp.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/sharp.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/stanford.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/stanford.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/uci.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/uci.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/ucsd.py` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers/parsers/ucsd.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/PKG-INFO` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chargemaster-parsers
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for parsing machine readable healthcare chargemasters
 Author: Jacob Schaer, Yvonne Kaire
 Project-URL: Homepage, https://github.com/jacobschaer/chargemaster_parsers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/SOURCES.txt` & `chargemaster_parsers-0.0.4/src/chargemaster_parsers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 src/chargemaster_parsers.egg-info/SOURCES.txt
 src/chargemaster_parsers.egg-info/dependency_links.txt
 src/chargemaster_parsers.egg-info/requires.txt
 src/chargemaster_parsers.egg-info/top_level.txt
 src/chargemaster_parsers/parsers/__init__.py
 src/chargemaster_parsers/parsers/cedars_sinai.py
 src/chargemaster_parsers/parsers/kaiser.py
+src/chargemaster_parsers/parsers/palomar.py
 src/chargemaster_parsers/parsers/parsers.py
 src/chargemaster_parsers/parsers/rady.py
 src/chargemaster_parsers/parsers/scripps.py
 src/chargemaster_parsers/parsers/sharp.py
+src/chargemaster_parsers/parsers/southwest.py
 src/chargemaster_parsers/parsers/stanford.py
 src/chargemaster_parsers/parsers/uci.py
 src/chargemaster_parsers/parsers/ucsd.py
 tests/test_cedars_sinai.py
 tests/test_kaiser.py
+tests/test_palomar.py
 tests/test_parser.py
 tests/test_rady.py
 tests/test_scripps.py
 tests/test_sharp.py
+tests/test_southwest.py
 tests/test_stanford.py
 tests/test_uci.py
 tests/test_ucsd.py
```

### Comparing `chargemaster_parsers-0.0.3/tests/test_cedars_sinai.py` & `chargemaster_parsers-0.0.4/tests/test_cedars_sinai.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_kaiser.py` & `chargemaster_parsers-0.0.4/tests/test_kaiser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_parser.py` & `chargemaster_parsers-0.0.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_rady.py` & `chargemaster_parsers-0.0.4/tests/test_rady.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_scripps.py` & `chargemaster_parsers-0.0.4/tests/test_scripps.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_sharp.py` & `chargemaster_parsers-0.0.4/tests/test_sharp.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_stanford.py` & `chargemaster_parsers-0.0.4/tests/test_stanford.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_uci.py` & `chargemaster_parsers-0.0.4/tests/test_uci.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.3/tests/test_ucsd.py` & `chargemaster_parsers-0.0.4/tests/test_ucsd.py`

 * *Files identical despite different names*

