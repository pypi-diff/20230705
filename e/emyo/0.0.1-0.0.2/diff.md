# Comparing `tmp/emyo-0.0.1.tar.gz` & `tmp/emyo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emyo-0.0.1.tar", last modified: Wed Jul  5 12:46:52 2023, max compression
+gzip compressed data, was "emyo-0.0.2.tar", last modified: Wed Jul  5 15:59:05 2023, max compression
```

## Comparing `emyo-0.0.1.tar` & `emyo-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:46:52.416880 emyo-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-07-05 12:41:34.000000 emyo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-05 12:41:34.000000 emyo-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1081 2023-07-05 12:46:52.416880 emyo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-05 12:41:34.000000 emyo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 12:46:52.393880 emyo-0.0.1/emyo/
--rw-rw-rw-   0        0        0      127 2023-07-05 12:41:34.000000 emyo-0.0.1/emyo/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-05 12:41:34.000000 emyo-0.0.1/emyo/common.py
--rw-rw-rw-   0        0        0       20 2023-07-05 12:41:34.000000 emyo-0.0.1/emyo/emyo.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:46:52.410910 emyo-0.0.1/emyo.egg-info/
--rw-rw-rw-   0        0        0     1081 2023-07-05 12:46:52.000000 emyo-0.0.1/emyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-05 12:46:52.000000 emyo-0.0.1/emyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:46:52.000000 emyo-0.0.1/emyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-05 12:46:52.000000 emyo-0.0.1/emyo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-07-05 12:46:52.000000 emyo-0.0.1/emyo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-05 12:41:34.000000 emyo-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      412 2023-07-05 12:46:52.418910 emyo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1724 2023-07-05 12:41:34.000000 emyo-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:46:52.415913 emyo-0.0.1/tests/
--rw-rw-rw-   0        0        0      393 2023-07-05 12:41:34.000000 emyo-0.0.1/tests/test_emyo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:59:05.378885 emyo-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 15:58:50.000000 emyo-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 15:58:50.000000 emyo-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-05 15:59:05.382885 emyo-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 15:58:50.000000 emyo-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:59:05.378885 emyo-0.0.2/emyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 15:58:50.000000 emyo-0.0.2/emyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 15:58:50.000000 emyo-0.0.2/emyo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 15:58:50.000000 emyo-0.0.2/emyo/emyo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:59:05.378885 emyo-0.0.2/emyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-05 15:59:05.000000 emyo-0.0.2/emyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 15:59:05.000000 emyo-0.0.2/emyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:59:05.000000 emyo-0.0.2/emyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:59:05.000000 emyo-0.0.2/emyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 15:59:05.000000 emyo-0.0.2/emyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:50.000000 emyo-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 15:59:05.382885 emyo-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-05 15:58:50.000000 emyo-0.0.2/setup.py
```

### Comparing `emyo-0.0.1/LICENSE` & `emyo-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Edmar Tabamo
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Edmar Tabamo
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `emyo-0.0.1/PKG-INFO` & `emyo-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: emyo
-Version: 0.0.1
-Summary: An interactive map for children
-Home-page: https://github.com/geofixit/emyo
-Author: Edmar Tabamo
-Author-email: geoed316@gmail.com
-License: MIT license
-Keywords: emyo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# emyo
-
-
-[![image](https://img.shields.io/pypi/v/emyo.svg)](https://pypi.python.org/pypi/emyo)
-[![image](https://img.shields.io/conda/vn/conda-forge/emyo.svg)](https://anaconda.org/conda-forge/emyo)
-
-
-**An interactive map for children**
-
-
--   Free software: MIT license
--   Documentation: https://geofixit.github.io/emyo
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: emyo
+Version: 0.0.2
+Summary: An interactive map for children
+Home-page: https://github.com/geofixit/emyo
+Author: Edmar Tabamo
+Author-email: geoed316@gmail.com
+License: MIT license
+Keywords: emyo
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# emyo
+
+
+[![image](https://img.shields.io/pypi/v/emyo.svg)](https://pypi.python.org/pypi/emyo)
+[![image](https://img.shields.io/conda/vn/conda-forge/emyo.svg)](https://anaconda.org/conda-forge/emyo)
+
+
+**An interactive map for children**
+
+
+-   Free software: MIT license
+-   Documentation: https://geofixit.github.io/emyo
+    
+
+## Features
+
+-   TODO
```

### Comparing `emyo-0.0.1/emyo.egg-info/PKG-INFO` & `emyo-0.0.2/emyo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: emyo
-Version: 0.0.1
-Summary: An interactive map for children
-Home-page: https://github.com/geofixit/emyo
-Author: Edmar Tabamo
-Author-email: geoed316@gmail.com
-License: MIT license
-Keywords: emyo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# emyo
-
-
-[![image](https://img.shields.io/pypi/v/emyo.svg)](https://pypi.python.org/pypi/emyo)
-[![image](https://img.shields.io/conda/vn/conda-forge/emyo.svg)](https://anaconda.org/conda-forge/emyo)
-
-
-**An interactive map for children**
-
-
--   Free software: MIT license
--   Documentation: https://geofixit.github.io/emyo
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: emyo
+Version: 0.0.2
+Summary: An interactive map for children
+Home-page: https://github.com/geofixit/emyo
+Author: Edmar Tabamo
+Author-email: geoed316@gmail.com
+License: MIT license
+Keywords: emyo
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# emyo
+
+
+[![image](https://img.shields.io/pypi/v/emyo.svg)](https://pypi.python.org/pypi/emyo)
+[![image](https://img.shields.io/conda/vn/conda-forge/emyo.svg)](https://anaconda.org/conda-forge/emyo)
+
+
+**An interactive map for children**
+
+
+-   Free software: MIT license
+-   Documentation: https://geofixit.github.io/emyo
+    
+
+## Features
+
+-   TODO
```

