# Comparing `tmp/pytbai-1.1.tar.gz` & `tmp/pytbai-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.1.tar", last modified: Wed Jul  5 08:35:36 2023, max compression
+gzip compressed data, was "pytbai-1.1.1.tar", last modified: Wed Jul  5 08:51:02 2023, max compression
```

## Comparing `pytbai-1.1.tar` & `pytbai-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.746293 pytbai-1.1/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      145 2023-07-05 08:35:35.000000 pytbai-1.1/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-05 08:35:35.000000 pytbai-1.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-05 08:35:35.000000 pytbai-1.1/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      211 2023-07-05 08:35:35.000000 pytbai-1.1/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 08:35:35.000000 pytbai-1.1/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2846 2023-07-05 08:35:36.746293 pytbai-1.1/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1380 2023-07-05 08:35:35.000000 pytbai-1.1/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.742293 pytbai-1.1/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       42 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     8409 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2952 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.742293 pytbai-1.1/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.742293 pytbai-1.1/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.742293 pytbai-1.1/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.746293 pytbai-1.1/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.746293 pytbai-1.1/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      375 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4345 2023-07-05 08:35:35.000000 pytbai-1.1/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.742293 pytbai-1.1/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2846 2023-07-05 08:35:36.000000 pytbai-1.1/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      615 2023-07-05 08:35:36.000000 pytbai-1.1/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-05 08:35:36.000000 pytbai-1.1/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-05 08:35:36.000000 pytbai-1.1/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 08:35:35.000000 pytbai-1.1/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-05 08:35:36.746293 pytbai-1.1/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)      637 2023-07-05 08:35:35.000000 pytbai-1.1/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:36.746293 pytbai-1.1/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:35:35.000000 pytbai-1.1/tests/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-05 08:35:35.000000 pytbai-1.1/tests/context.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2461 2023-07-05 08:35:35.000000 pytbai-1.1/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      404 2023-07-05 08:51:00.000000 pytbai-1.1.1/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-05 08:51:00.000000 pytbai-1.1.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-05 08:51:00.000000 pytbai-1.1.1/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      211 2023-07-05 08:51:00.000000 pytbai-1.1.1/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 08:51:00.000000 pytbai-1.1.1/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3236 2023-07-05 08:51:02.394533 pytbai-1.1.1/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1380 2023-07-05 08:51:00.000000 pytbai-1.1.1/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.390533 pytbai-1.1.1/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       42 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     8409 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2952 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.390533 pytbai-1.1.1/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      375 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4345 2023-07-05 08:51:00.000000 pytbai-1.1.1/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3236 2023-07-05 08:51:02.000000 pytbai-1.1.1/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      615 2023-07-05 08:51:02.000000 pytbai-1.1.1/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-05 08:51:02.000000 pytbai-1.1.1/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-05 08:51:02.000000 pytbai-1.1.1/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 08:51:00.000000 pytbai-1.1.1/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-05 08:51:02.394533 pytbai-1.1.1/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1044 2023-07-05 08:51:00.000000 pytbai-1.1.1/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:02.394533 pytbai-1.1.1/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 08:51:00.000000 pytbai-1.1.1/tests/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-05 08:51:00.000000 pytbai-1.1.1/tests/context.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2461 2023-07-05 08:51:00.000000 pytbai-1.1.1/tests/test_basic.py
```

### Comparing `pytbai-1.1/LICENSE` & `pytbai-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/PKG-INFO` & `pytbai-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.1
+Version: 1.1.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `pytbai-1.1/README.md` & `pytbai-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/core.py` & `pytbai-1.1.1/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/definitions.py` & `pytbai-1.1.1/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.1.1/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.1.1/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.1.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.1.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/utils/pdf.py` & `pytbai-1.1.1/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai/utils/xml.py` & `pytbai-1.1.1/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/pytbai.egg-info/PKG-INFO` & `pytbai-1.1.1/pytbai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.1
+Version: 1.1.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `pytbai-1.1/pytbai.egg-info/SOURCES.txt` & `pytbai-1.1.1/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.1/tests/test_basic.py` & `pytbai-1.1.1/tests/test_basic.py`

 * *Files identical despite different names*

