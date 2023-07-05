# Comparing `tmp/inquestlabs-1.2.2.tar.gz` & `tmp/inquestlabs-1.2.3.tar.gz`

## Comparing `inquestlabs-1.2.2.tar` & `inquestlabs-1.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/.coveragerc
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/CONTRIBUTING.md
--rwxr-xr-x   0        0        0    58471 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/inquestlabs.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/requirements-testing.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/requirements.txt
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_api.py
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_attributes.py
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_details.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_download.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_list.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_search.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_sources.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_dfi_upload.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_iocdb_list.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_iocdb_search.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_iocdb_sources.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_repdb_list.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_repdb_search.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_repdb_sources.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_stats.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_yara_b64re.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_yara_hexcase.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_yara_uint.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/tests/test_yara_widere.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/LICENSE
--rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/README.md
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    38299 2020-02-02 00:00:00.000000 inquestlabs-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.coveragerc
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0    58471 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/inquestlabs.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/requirements-testing.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/requirements.txt
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_api.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_attributes.py
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_details.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_download.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_list.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_search.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_sources.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_dfi_upload.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_list.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_search.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_iocdb_sources.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_list.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_search.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_repdb_sources.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_stats.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_b64re.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_hexcase.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_uint.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/tests/test_yara_widere.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/LICENSE
+-rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/README.md
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    38299 2020-02-02 00:00:00.000000 inquestlabs-1.2.3/PKG-INFO
```

### Comparing `inquestlabs-1.2.2/inquestlabs.py` & `inquestlabs-1.2.3/inquestlabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 import sys
 import os
 import re
 # from importlib.metadata import version
 
 # extract version from installed package metadata
 __application_name__ = "inquestlabs"
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 # __version__ = version(__application_name__)
 __full_version__ = f"{__application_name__} {__version__}"
 
 VALID_CAT    = ["ext", "hash", "ioc"]
 VALID_EXT    = ["code", "context", "metadata", "ocr"]
 VALID_HASH   = ["md5", "sha1", "sha256", "sha512"]
 VALID_IOC    = ["domain", "email", "filename", "filepath", "ip", "registry", "url", "xmpid"]
```

### Comparing `inquestlabs-1.2.2/.github/workflows/workflow.yml` & `inquestlabs-1.2.3/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_api.py` & `inquestlabs-1.2.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_attributes.py` & `inquestlabs-1.2.3/tests/test_dfi_attributes.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_details.py` & `inquestlabs-1.2.3/tests/test_dfi_details.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_download.py` & `inquestlabs-1.2.3/tests/test_dfi_download.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_list.py` & `inquestlabs-1.2.3/tests/test_dfi_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_search.py` & `inquestlabs-1.2.3/tests/test_dfi_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_dfi_upload.py` & `inquestlabs-1.2.3/tests/test_dfi_upload.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_iocdb_list.py` & `inquestlabs-1.2.3/tests/test_iocdb_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_iocdb_search.py` & `inquestlabs-1.2.3/tests/test_iocdb_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_repdb_list.py` & `inquestlabs-1.2.3/tests/test_repdb_list.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_repdb_search.py` & `inquestlabs-1.2.3/tests/test_repdb_search.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_stats.py` & `inquestlabs-1.2.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_yara_b64re.py` & `inquestlabs-1.2.3/tests/test_yara_b64re.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_yara_hexcase.py` & `inquestlabs-1.2.3/tests/test_yara_hexcase.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_yara_uint.py` & `inquestlabs-1.2.3/tests/test_yara_uint.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/tests/test_yara_widere.py` & `inquestlabs-1.2.3/tests/test_yara_widere.py`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/.gitignore` & `inquestlabs-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/LICENSE` & `inquestlabs-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/README.md` & `inquestlabs-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `inquestlabs-1.2.2/pyproject.toml` & `inquestlabs-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling", "wheel"]
 build-backend = "hatchling.build"
 
 [project]
 name = "inquestlabs"
-version = "1.2.2"
+version = "1.2.3"
 license = {file = "LICENSE"}
 authors = [
 	{ name="InQuest", email="labs@inquest.net" },
 ]
 description = "A Pythonic interface and CLI tool for the InQuest Labs API"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.6"
 
 dependencies = [
     "attrs",
     "certifi",
     "charset-normalizer",
     "docopt",
     "idna",
```

### Comparing `inquestlabs-1.2.2/PKG-INFO` & `inquestlabs-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inquestlabs
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Pythonic interface and CLI tool for the InQuest Labs API
 Project-URL: Homepage, https://labs.inquest.net/
 Project-URL: Repository, https://github.com/InQuest/python-inquestlabs
 Project-URL: Bug Tracker, https://github.com/InQuest/python-inquestlabs/issues
 Author-email: InQuest <labs@inquest.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
@@ -345,15 +345,15 @@
         consider it more useful to permit linking proprietary applications with the
         library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Requires-Dist: attrs
 Requires-Dist: certifi
 Requires-Dist: charset-normalizer
 Requires-Dist: docopt
 Requires-Dist: idna
 Requires-Dist: iniconfig
 Requires-Dist: packaging
```

