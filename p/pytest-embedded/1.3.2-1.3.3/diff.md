# Comparing `tmp/pytest_embedded-1.3.2.tar.gz` & `tmp/pytest_embedded-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded-1.3.2.tar` & `pytest_embedded-1.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/LICENSE
--rw-r--r--   0        0        0      120 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/README.md
--rw-r--r--   0        0        0     2950 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/__init__.py
--rw-r--r--   0        0        0     1095 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/app.py
--rw-r--r--   0        0        0     6922 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/dut.py
--rw-r--r--   0        0        0     6886 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/log.py
--rw-r--r--   0        0        0    50859 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/plugin.py
--rw-r--r--   0        0        0    11199 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/unity.py
--rw-r--r--   0        0        0     9950 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/pytest_embedded/utils.py
--rw-r--r--   0        0        0    19868 2023-06-14 02:29:37.924594 pytest_embedded-1.3.2/tests/test_base.py
--rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_embedded-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/LICENSE
+-rw-r--r--   0        0        0      120 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/README.md
+-rw-r--r--   0        0        0     2950 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/pytest_embedded/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/pytest_embedded/app.py
+-rw-r--r--   0        0        0     6922 2023-07-05 01:18:10.855964 pytest_embedded-1.3.3/pytest_embedded/dut.py
+-rw-r--r--   0        0        0     6886 2023-07-05 01:18:10.859964 pytest_embedded-1.3.3/pytest_embedded/log.py
+-rw-r--r--   0        0        0    50859 2023-07-05 01:18:10.859964 pytest_embedded-1.3.3/pytest_embedded/plugin.py
+-rw-r--r--   0        0        0    11199 2023-07-05 01:18:10.859964 pytest_embedded-1.3.3/pytest_embedded/unity.py
+-rw-r--r--   0        0        0     9950 2023-07-05 01:18:10.859964 pytest_embedded-1.3.3/pytest_embedded/utils.py
+-rw-r--r--   0        0        0    19868 2023-07-05 01:18:10.859964 pytest_embedded-1.3.3/tests/test_base.py
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_embedded-1.3.3/PKG-INFO
```

### Comparing `pytest_embedded-1.3.2/LICENSE` & `pytest_embedded-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pyproject.toml` & `pytest_embedded-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/app.py` & `pytest_embedded-1.3.3/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/dut.py` & `pytest_embedded-1.3.3/pytest_embedded/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/log.py` & `pytest_embedded-1.3.3/pytest_embedded/log.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/plugin.py` & `pytest_embedded-1.3.3/pytest_embedded/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/unity.py` & `pytest_embedded-1.3.3/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/pytest_embedded/utils.py` & `pytest_embedded-1.3.3/pytest_embedded/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/tests/test_base.py` & `pytest_embedded-1.3.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.3.2/PKG-INFO` & `pytest_embedded-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pytest plugin that designed for embedded testing.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

