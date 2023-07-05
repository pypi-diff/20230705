# Comparing `tmp/pytest_embedded_arduino-1.3.2.tar.gz` & `tmp/pytest_embedded_arduino-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_arduino-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_arduino-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_arduino-1.3.2.tar` & `pytest_embedded_arduino-1.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/LICENSE
--rw-r--r--   0        0        0      516 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/README.md
--rw-r--r--   0        0        0     3047 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      193 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/__init__.py
--rw-r--r--   0        0        0     1879 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/app.py
--rw-r--r--   0        0        0     1870 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/serial.py
--rw-r--r--   0        0        0      747 2023-06-14 02:29:37.920594 pytest_embedded_arduino-1.3.2/tests/test_arduino.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/LICENSE
+-rw-r--r--   0        0        0      516 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/README.md
+-rw-r--r--   0        0        0     3047 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0        0        0     1965 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/pytest_embedded_arduino/app.py
+-rw-r--r--   0        0        0     1870 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/pytest_embedded_arduino/serial.py
+-rw-r--r--   0        0        0      747 2023-07-05 01:18:10.855964 pytest_embedded_arduino-1.3.3/tests/test_arduino.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.3.3/PKG-INFO
```

### Comparing `pytest_embedded_arduino-1.3.2/LICENSE` & `pytest_embedded_arduino-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.3.2/README.md` & `pytest_embedded_arduino-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.3.2/pyproject.toml` & `pytest_embedded_arduino-1.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.3.2",
+    "pytest-embedded~=1.3.3",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.3.2"
+    "pytest-embedded-serial-esp~=1.3.3"
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
```

### Comparing `pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/app.py` & `pytest_embedded_arduino-1.3.3/pytest_embedded_arduino/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     #: dict of binaries' offset.
     binary_offsets = {
         'esp32': [0x1000, 0x8000, 0x10000],
         'esp32s2': [0x1000, 0x8000, 0x10000],
         'esp32c3': [0x0, 0x8000, 0x10000],
         'esp32s3': [0x0, 0x8000, 0x10000],
+        'esp32c6': [0x0, 0x8000, 0x10000],
+        'esp32h2': [0x0, 0x8000, 0x10000],
     }
 
     def __init__(
         self,
         **kwargs,
     ):
         super().__init__(**kwargs)
```

### Comparing `pytest_embedded_arduino-1.3.2/pytest_embedded_arduino/serial.py` & `pytest_embedded_arduino-1.3.3/pytest_embedded_arduino/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.3.2/tests/test_arduino.py` & `pytest_embedded_arduino-1.3.3/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.3.2/PKG-INFO` & `pytest_embedded_arduino-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.3.2
+Version: 1.3.3
 Summary: Make pytest-embedded plugin work with Arduino.
 Author-email: Abdelatif Guettouche <abdelatif.guettouche@espressif.com>, Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.3.2
-Requires-Dist: pytest-embedded-serial-esp~=1.3.2 ; extra == "serial"
+Requires-Dist: pytest-embedded~=1.3.3
+Requires-Dist: pytest-embedded-serial-esp~=1.3.3 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
 
 ### pytest-embedded-arduino
```

