# Comparing `tmp/flake8-json-21.7.0.tar.gz` & `tmp/flake8_json-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-json-21.7.0.tar", last modified: Mon Jul 26 22:06:51 2021, max compression
+gzip compressed data, was "flake8_json-23.7.0.tar", last modified: Tue Jul  4 21:57:08 2023, max compression
```

## Comparing `flake8-json-21.7.0.tar` & `flake8_json-23.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-26 22:06:51.642839 flake8-json-21.7.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1113 2021-07-26 22:05:29.000000 flake8-json-21.7.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1751 2021-07-26 22:06:51.642839 flake8-json-21.7.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      800 2021-07-26 22:05:29.000000 flake8-json-21.7.0/README.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1132 2021-07-26 22:06:51.642839 flake8-json-21.7.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)      462 2021-07-26 22:05:29.000000 flake8-json-21.7.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-26 22:06:51.642839 flake8-json-21.7.0/src/
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-26 22:06:51.642839 flake8-json-21.7.0/src/flake8_json.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1751 2021-07-26 22:06:51.000000 flake8-json-21.7.0/src/flake8_json.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      310 2021-07-26 22:06:51.000000 flake8-json-21.7.0/src/flake8_json.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-07-26 22:06:51.000000 flake8-json-21.7.0/src/flake8_json.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      128 2021-07-26 22:06:51.000000 flake8-json-21.7.0/src/flake8_json.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       21 2021-07-26 22:06:51.000000 flake8-json-21.7.0/src/flake8_json.egg-info/top_level.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-26 22:06:51.642839 flake8-json-21.7.0/src/flake8_json_reporter/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       58 2021-07-26 22:05:56.000000 flake8-json-21.7.0/src/flake8_json_reporter/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5090 2021-07-26 22:05:29.000000 flake8-json-21.7.0/src/flake8_json_reporter/reporters.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1113 2023-07-04 21:37:55.000000 flake8_json-23.7.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2023-07-04 21:57:08.323271 flake8_json-23.7.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      879 2023-07-04 21:55:26.000000 flake8_json-23.7.0/README.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2023-07-04 21:57:08.323271 flake8_json-23.7.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      167 2023-07-04 21:37:55.000000 flake8_json-23.7.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.319271 flake8_json-23.7.0/src/
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/src/flake8_json.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      310 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      186 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       21 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/src/flake8_json_reporter/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       58 2023-07-04 21:55:56.000000 flake8_json-23.7.0/src/flake8_json_reporter/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6287 2023-07-04 21:55:26.000000 flake8_json-23.7.0/src/flake8_json_reporter/reporters.py
```

### Comparing `flake8-json-21.7.0/LICENSE` & `flake8_json-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-json-21.7.0/PKG-INFO` & `flake8_json-23.7.0/src/flake8_json.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: flake8-json
-Version: 21.7.0
+Version: 23.7.0
 Summary: JSON Formatting Reporter plugin for Flake8
-Home-page: https://gitlab.com/pycqa/flake8-json
+Home-page: https://github.com/pycqa/flake8-json
 Author: Ian Stapleton Cordasco
 Author-email: graffatcolmingov@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,>=2.7
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Flake8-JSON
 ===========
 
-This is a plugin for Flake8 that will format the output as JSON. By default,
-the output is **not** pretty-printed. We would love to add that as a separate
-formatter option, though.
+This is a plugin for Flake8 that will format the output as JSON. The output of
+the default JSON formatter is not pretty-printed. If you'd like the output to
+be pretty-printed, use json-pretty instead.
 
 CodeClimate support is also offered through this plugin as of v20.12.0
 
 
 Installation
 ------------
 
@@ -46,14 +43,18 @@
 
 .. code-block:: bash
 
     flake8 --format=json ...
 
 .. code-block:: bash
 
+    flake8 --format=json-pretty ...
+
+.. code-block:: bash
+
     flake8 --format=codeclimate ...
 
 
 Competitors
 -----------
 
 None that I could find on PyPI
@@ -64,9 +65,7 @@
 
 This project is seeking maintainers. Please open an issue if you're interested
 and ensure that you've read the PyCQA's `Code of Conduct`_.
 
 
 .. _Code of Conduct:
     http://meta.pycqa.org/en/latest/code-of-conduct.html
-
-
```

### Comparing `flake8-json-21.7.0/README.rst` & `flake8_json-23.7.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Flake8-JSON
 ===========
 
-This is a plugin for Flake8 that will format the output as JSON. By default,
-the output is **not** pretty-printed. We would love to add that as a separate
-formatter option, though.
+This is a plugin for Flake8 that will format the output as JSON. The output of
+the default JSON formatter is not pretty-printed. If you'd like the output to
+be pretty-printed, use json-pretty instead.
 
 CodeClimate support is also offered through this plugin as of v20.12.0
 
 
 Installation
 ------------
 
@@ -21,14 +21,18 @@
 
 .. code-block:: bash
 
     flake8 --format=json ...
 
 .. code-block:: bash
 
+    flake8 --format=json-pretty ...
+
+.. code-block:: bash
+
     flake8 --format=codeclimate ...
 
 
 Competitors
 -----------
 
 None that I could find on PyPI
```

### Comparing `flake8-json-21.7.0/src/flake8_json.egg-info/PKG-INFO` & `flake8_json-23.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
-Name: flake8-json
-Version: 21.7.0
+Name: flake8_json
+Version: 23.7.0
 Summary: JSON Formatting Reporter plugin for Flake8
-Home-page: https://gitlab.com/pycqa/flake8-json
+Home-page: https://github.com/pycqa/flake8-json
 Author: Ian Stapleton Cordasco
 Author-email: graffatcolmingov@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,>=2.7
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Flake8-JSON
 ===========
 
-This is a plugin for Flake8 that will format the output as JSON. By default,
-the output is **not** pretty-printed. We would love to add that as a separate
-formatter option, though.
+This is a plugin for Flake8 that will format the output as JSON. The output of
+the default JSON formatter is not pretty-printed. If you'd like the output to
+be pretty-printed, use json-pretty instead.
 
 CodeClimate support is also offered through this plugin as of v20.12.0
 
 
 Installation
 ------------
 
@@ -46,14 +43,18 @@
 
 .. code-block:: bash
 
     flake8 --format=json ...
 
 .. code-block:: bash
 
+    flake8 --format=json-pretty ...
+
+.. code-block:: bash
+
     flake8 --format=codeclimate ...
 
 
 Competitors
 -----------
 
 None that I could find on PyPI
@@ -64,9 +65,7 @@
 
 This project is seeking maintainers. Please open an issue if you're interested
 and ensure that you've read the PyCQA's `Code of Conduct`_.
 
 
 .. _Code of Conduct:
     http://meta.pycqa.org/en/latest/code-of-conduct.html
-
-
```

### Comparing `flake8-json-21.7.0/src/flake8_json_reporter/reporters.py` & `flake8_json-23.7.0/src/flake8_json_reporter/reporters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module containing all of the JSON reporters for Flake8."""
-from __future__ import print_function, unicode_literals
-
 import hashlib
 import json
+import textwrap
 
 from flake8.formatting import base
 
 
 class DefaultJSON(base.BaseFormatter):
     """The non-pretty-printing JSON formatter."""
 
@@ -22,29 +21,29 @@
 
     def write_line(self, line):
         """Override write for convenience."""
         self.write(line, None)
 
     def start(self):
         """Override the default to start printing JSON."""
-        super(DefaultJSON, self).start()
+        super().start()
         self.write_line("{")
         self.files_reported_count = 0
 
     def stop(self):
         """Override the default to finish printing JSON."""
         self.write_line("}")
 
     def beginning(self, filename):
         """We're starting a new file."""
         json_filename = json.dumps(filename)
         if self.files_reported_count > 0:
-            self.write_line(", {}: [".format(json_filename))
+            self.write_line(f", {json_filename}: [")
         else:
-            self.write_line("{}: [".format(json_filename))
+            self.write_line(f"{json_filename}: [")
         self.reported_errors_count = 0
 
     def finished(self, filename):
         """We've finished processing a file."""
         self.files_reported_count += 1
         self.write_line("]")
 
@@ -62,20 +61,62 @@
             ]
         }
 
     def format(self, violation):
         """Format a violation."""
         formatted = json.dumps(self.dictionary_from(violation))
         if self.reported_errors_count > 0:
-            self.write_line(", {}".format(formatted))
+            self.write_line(f", {formatted}")
         else:
             self.write_line(formatted)
         self.reported_errors_count += 1
 
 
+def _indent(text, indent):
+    return textwrap.indent(text, " " * indent)
+
+
+class FormattedJSON(DefaultJSON):
+    """Pretty-printing JSON formatter."""
+
+    def stop(self):
+        """Override the default to finish printing JSON."""
+        if self.files_reported_count > 0:
+            self.write_line("\n")
+        self.write_line("}\n")
+
+    def beginning(self, filename):
+        """We're starting a new file."""
+        if self.files_reported_count > 0:
+            self.write_line(",\n")
+            self.write_line(f"  {json.dumps(filename)}: [")
+        else:
+            self.write_line(f"\n  {json.dumps(filename)}: [")
+        self.reported_errors_count = 0
+
+    def finished(self, filename):
+        """We've finished processing a file."""
+        self.files_reported_count += 1
+        if self.reported_errors_count > 0:
+            self.write_line("\n")
+            self.write_line("  ]")
+        else:
+            self.write_line("]")
+
+    def format(self, violation):
+        """Format a violation."""
+        formatted = json.dumps(self.dictionary_from(violation), indent=2)
+        formatted = _indent(formatted, indent=4)
+        if self.reported_errors_count > 0:
+            self.write_line(",")
+        self.write_line("\n")
+        self.write_line(formatted)
+        self.reported_errors_count += 1
+
+
 class CodeClimateJSON(base.BaseFormatter):
     """Formatter for CodeClimate JSON."""
 
     def after_init(self):
         """Force newline to be empty."""
         self.newline = ""
 
@@ -87,29 +128,29 @@
 
     def write_line(self, line):
         """Override write for convenience."""
         self.write(line, None)
 
     def start(self):
         """Override the default to start printing JSON."""
-        super(CodeClimateJSON, self).start()
+        super().start()
         self.write_line("{")
         self.files_reported_count = 0
 
     def stop(self):
         """Override the default to finish printing JSON."""
         self.write_line("}")
 
     def beginning(self, filename):
         """We're starting a new file."""
         json_filename = json.dumps(filename)
         if self.files_reported_count > 0:
-            self.write_line(", {}: [".format(json_filename))
+            self.write_line(f", {json_filename}: [")
         else:
-            self.write_line("{}: [".format(json_filename))
+            self.write_line(f"{json_filename}: [")
         self.reported_errors_count = 0
 
     def finished(self, filename):
         """We've finished processing a file."""
         self.files_reported_count += 1
         self.write_line("]")
 
@@ -149,11 +190,11 @@
             "fingerprint": self._fingerprint(violation),
         }
 
     def format(self, violation):
         """Format a violation."""
         formatted = json.dumps(self.dictionary_from(violation))
         if self.reported_errors_count > 0:
-            self.write_line(", {}".format(formatted))
+            self.write_line(f", {formatted}")
         else:
             self.write_line(formatted)
         self.reported_errors_count += 1
```

