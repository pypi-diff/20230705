# Comparing `tmp/lnurl-0.3.5.tar.gz` & `tmp/lnurl-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lnurl-0.3.5.tar", last modified: Tue Aug 18 09:44:00 2020, max compression
+gzip compressed data, was "dist/lnurl-0.3.6.tar", last modified: Mon Apr 12 21:10:18 2021, max compression
```

## Comparing `lnurl-0.3.5.tar` & `lnurl-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2020-08-18 09:44:00.000000 lnurl-0.3.5/
--rw-r--r--   0 eillarra   (501) staff       (20)     7086 2020-08-18 09:44:00.000000 lnurl-0.3.5/PKG-INFO
--rwxr-xr-x   0 eillarra   (501) staff       (20)     5274 2020-05-06 15:42:41.000000 lnurl-0.3.5/README.md
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl/
--rw-r--r--   0 eillarra   (501) staff       (20)      336 2019-12-14 10:57:15.000000 lnurl-0.3.5/lnurl/__init__.py
--rw-r--r--   0 eillarra   (501) staff       (20)     1789 2020-08-18 09:38:18.000000 lnurl-0.3.5/lnurl/core.py
--rw-r--r--   0 eillarra   (501) staff       (20)      486 2019-12-14 10:57:15.000000 lnurl-0.3.5/lnurl/exceptions.py
--rw-r--r--   0 eillarra   (501) staff       (20)     1575 2020-05-06 20:11:13.000000 lnurl-0.3.5/lnurl/helpers.py
--rw-r--r--   0 eillarra   (501) staff       (20)     5199 2020-05-06 20:12:03.000000 lnurl-0.3.5/lnurl/models.py
--rw-r--r--   0 eillarra   (501) staff       (20)     7521 2020-08-04 15:57:51.000000 lnurl-0.3.5/lnurl/types.py
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/
--rw-r--r--   0 eillarra   (501) staff       (20)     7086 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/PKG-INFO
--rw-r--r--   0 eillarra   (501) staff       (20)      305 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/SOURCES.txt
--rw-r--r--   0 eillarra   (501) staff       (20)        1 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/dependency_links.txt
--rw-r--r--   0 eillarra   (501) staff       (20)        1 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/not-zip-safe
--rw-r--r--   0 eillarra   (501) staff       (20)       61 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/requires.txt
--rw-r--r--   0 eillarra   (501) staff       (20)        6 2020-08-18 09:44:00.000000 lnurl-0.3.5/lnurl.egg-info/top_level.txt
--rw-r--r--   0 eillarra   (501) staff       (20)       31 2019-12-20 11:30:21.000000 lnurl-0.3.5/pyproject.toml
--rw-r--r--   0 eillarra   (501) staff       (20)       38 2020-08-18 09:44:00.000000 lnurl-0.3.5/setup.cfg
--rw-r--r--   0 eillarra   (501) staff       (20)     1239 2020-08-18 09:43:40.000000 lnurl-0.3.5/setup.py
+drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2021-04-12 21:10:18.000000 lnurl-0.3.6/
+-rw-r--r--   0 eillarra   (501) staff       (20)     7361 2021-04-12 21:10:18.000000 lnurl-0.3.6/PKG-INFO
+-rwxr-xr-x   0 eillarra   (501) staff       (20)     5438 2021-04-12 13:31:15.000000 lnurl-0.3.6/README.md
+drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl/
+-rw-r--r--   0 eillarra   (501) staff       (20)      336 2019-12-14 10:57:15.000000 lnurl-0.3.6/lnurl/__init__.py
+-rw-r--r--   0 eillarra   (501) staff       (20)     1789 2021-04-12 20:58:46.000000 lnurl-0.3.6/lnurl/core.py
+-rw-r--r--   0 eillarra   (501) staff       (20)      486 2019-12-14 10:57:15.000000 lnurl-0.3.6/lnurl/exceptions.py
+-rw-r--r--   0 eillarra   (501) staff       (20)     1575 2020-05-06 20:11:13.000000 lnurl-0.3.6/lnurl/helpers.py
+-rw-r--r--   0 eillarra   (501) staff       (20)     5199 2020-05-06 20:12:03.000000 lnurl-0.3.6/lnurl/models.py
+-rw-r--r--   0 eillarra   (501) staff       (20)     7433 2021-04-12 15:33:38.000000 lnurl-0.3.6/lnurl/types.py
+drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/
+-rw-r--r--   0 eillarra   (501) staff       (20)     7361 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/PKG-INFO
+-rw-r--r--   0 eillarra   (501) staff       (20)      305 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/SOURCES.txt
+-rw-r--r--   0 eillarra   (501) staff       (20)        1 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/dependency_links.txt
+-rw-r--r--   0 eillarra   (501) staff       (20)        1 2020-08-18 09:44:00.000000 lnurl-0.3.6/lnurl.egg-info/not-zip-safe
+-rw-r--r--   0 eillarra   (501) staff       (20)       61 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/requires.txt
+-rw-r--r--   0 eillarra   (501) staff       (20)        6 2021-04-12 21:10:18.000000 lnurl-0.3.6/lnurl.egg-info/top_level.txt
+-rw-r--r--   0 eillarra   (501) staff       (20)       31 2019-12-20 11:30:21.000000 lnurl-0.3.6/pyproject.toml
+-rw-r--r--   0 eillarra   (501) staff       (20)       38 2021-04-12 21:10:18.000000 lnurl-0.3.6/setup.cfg
+-rw-r--r--   0 eillarra   (501) staff       (20)     1285 2021-04-12 20:58:46.000000 lnurl-0.3.6/setup.py
```

### Comparing `lnurl-0.3.5/PKG-INFO` & `lnurl-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lnurl
-Version: 0.3.5
+Version: 0.3.6
 Summary: LNURL implementation for Python.
-Home-page: https://github.com/python-ln/lnurl
+Home-page: https://github.com/lnbits/lnurl
 Author: jogco
 Author-email: jogco@lnsms.world
 Maintainer: eillarra
 Maintainer-email: eneko@illarra.com
 License: MIT
 Description: LNURL implementation for Python
         ===============================
@@ -17,14 +17,22 @@
         [![pypi-badge]][pypi]
         [![pypi-versions-badge]][pypi]
         [![license-badge]](LICENSE)
         
         
         A collection of helpers for building [LNURL][lnurl] support into wallets and services.
         
+        Configuration
+        -------------
+        
+        Developers can force strict RFC3986 validation for the URLs that the library encodes/decodes, using this env var:
+        
+        > LNURL_STRICT_RFC3986 = "0" by default (False)
+        
+        
         Basic usage
         -----------
         
         ```python
         >>> import lnurl
         >>> lnurl.encode('https://service.io/?q=3fc3645b439ce8e7')
         Lnurl('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', bech32=Bech32('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', hrp='lnurl', data=[13, 1, 26, 7, 8, 28, 3, 19, 7, 8, 23, 18, 30, 28, 27, 5, 14, 9, 27, 6, 18, 24, 27, 5, 5, 25, 20, 22, 30, 11, 25, 31, 14, 4, 30, 19, 6, 25, 19, 3, 6, 12, 27, 3, 8, 13, 11, 2, 6, 16, 25, 19, 18, 24, 27, 5, 7, 1, 18, 19, 14]), url=WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7'))
@@ -109,20 +117,20 @@
         You can also use camelCases when you parse the data, and it will be converted to snake_case to make your
         Python code nicer.
         
         If you want to export the data using :snake: snake_case (in your Python code, for example), you can change
         the `by_alias` parameter: `res.dict(by_alias=False)` (it is `True` by default).
         
         
-        [github-tests]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22tests%22
-        [github-tests-badge]: https://github.com/python-ln/lnurl/workflows/tests/badge.svg
-        [github-mypy]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22mypy%22
-        [github-mypy-badge]: https://github.com/python-ln/lnurl/workflows/mypy/badge.svg
-        [codecov]: https://codecov.io/gh/python-ln/lnurl
-        [codecov-badge]: https://codecov.io/gh/python-ln/lnurl/branch/master/graph/badge.svg
+        [github-tests]: https://github.com/lnbits/lnurl/actions?query=workflow%3Atests
+        [github-tests-badge]: https://github.com/lnbits/lnurl/workflows/tests/badge.svg
+        [github-mypy]: https://github.com/lnbits/lnurl/actions?query=workflow%3Amypy
+        [github-mypy-badge]: https://github.com/lnbits/lnurl/workflows/mypy/badge.svg
+        [codecov]: https://codecov.io/gh/lnbits/lnurl
+        [codecov-badge]: https://codecov.io/gh/lnbits/lnurl/branch/master/graph/badge.svg
         [pypi]: https://pypi.org/project/lnurl/
         [pypi-badge]: https://badge.fury.io/py/lnurl.svg
         [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/lnurl.svg
         [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
         
         [lnurl]: https://telegra.ph/lnurl-a-protocol-for-seamless-interaction-between-services-and-Lightning-wallets-08-19
         [lnurl-spec]: https://github.com/btcontract/lnurl-rfc/blob/master/spec.md
@@ -135,10 +143,11 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lnurl-0.3.5/README.md` & `lnurl-0.3.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 [![pypi-badge]][pypi]
 [![pypi-versions-badge]][pypi]
 [![license-badge]](LICENSE)
 
 
 A collection of helpers for building [LNURL][lnurl] support into wallets and services.
 
+Configuration
+-------------
+
+Developers can force strict RFC3986 validation for the URLs that the library encodes/decodes, using this env var:
+
+> LNURL_STRICT_RFC3986 = "0" by default (False)
+
+
 Basic usage
 -----------
 
 ```python
 >>> import lnurl
 >>> lnurl.encode('https://service.io/?q=3fc3645b439ce8e7')
 Lnurl('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', bech32=Bech32('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', hrp='lnurl', data=[13, 1, 26, 7, 8, 28, 3, 19, 7, 8, 23, 18, 30, 28, 27, 5, 14, 9, 27, 6, 18, 24, 27, 5, 5, 25, 20, 22, 30, 11, 25, 31, 14, 4, 30, 19, 6, 25, 19, 3, 6, 12, 27, 3, 8, 13, 11, 2, 6, 16, 25, 19, 18, 24, 27, 5, 7, 1, 18, 19, 14]), url=WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7'))
@@ -99,20 +107,20 @@
 You can also use camelCases when you parse the data, and it will be converted to snake_case to make your
 Python code nicer.
 
 If you want to export the data using :snake: snake_case (in your Python code, for example), you can change
 the `by_alias` parameter: `res.dict(by_alias=False)` (it is `True` by default).
 
 
-[github-tests]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22tests%22
-[github-tests-badge]: https://github.com/python-ln/lnurl/workflows/tests/badge.svg
-[github-mypy]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22mypy%22
-[github-mypy-badge]: https://github.com/python-ln/lnurl/workflows/mypy/badge.svg
-[codecov]: https://codecov.io/gh/python-ln/lnurl
-[codecov-badge]: https://codecov.io/gh/python-ln/lnurl/branch/master/graph/badge.svg
+[github-tests]: https://github.com/lnbits/lnurl/actions?query=workflow%3Atests
+[github-tests-badge]: https://github.com/lnbits/lnurl/workflows/tests/badge.svg
+[github-mypy]: https://github.com/lnbits/lnurl/actions?query=workflow%3Amypy
+[github-mypy-badge]: https://github.com/lnbits/lnurl/workflows/mypy/badge.svg
+[codecov]: https://codecov.io/gh/lnbits/lnurl
+[codecov-badge]: https://codecov.io/gh/lnbits/lnurl/branch/master/graph/badge.svg
 [pypi]: https://pypi.org/project/lnurl/
 [pypi-badge]: https://badge.fury.io/py/lnurl.svg
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/lnurl.svg
 [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
 
 [lnurl]: https://telegra.ph/lnurl-a-protocol-for-seamless-interaction-between-services-and-Lightning-wallets-08-19
 [lnurl-spec]: https://github.com/btcontract/lnurl-rfc/blob/master/spec.md
```

### Comparing `lnurl-0.3.5/lnurl/core.py` & `lnurl-0.3.6/lnurl/core.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.3.5/lnurl/helpers.py` & `lnurl-0.3.6/lnurl/helpers.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.3.5/lnurl/models.py` & `lnurl-0.3.6/lnurl/models.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.3.5/lnurl/types.py` & `lnurl-0.3.6/lnurl/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from urllib.parse import parse_qs
 from typing import Dict, List, Optional, Tuple, Union
 
 from .exceptions import InvalidLnurlPayMetadata
 from .helpers import _bech32_decode, _lnurl_clean, _lnurl_decode
 
 
-STRICT_RFC3986 = os.environ.get("LNURL_STRICT_RFC3986", "1") == "1"
-
-
 def ctrl_characters_validator(value: str) -> str:
     """Checks for control characters (unicode blocks C0 and C1, plus DEL)."""
     if re.compile(r"[\u0000-\u001f\u007f-\u009f]").search(value):
         raise ValueError
     return value
 
 
@@ -68,30 +65,30 @@
     """URL with extra validations over pydantic's `HttpUrl`."""
 
     max_length = 2047  # https://stackoverflow.com/questions/417142/
 
     @classmethod
     def __get_validators__(cls):
         yield ctrl_characters_validator
-        if STRICT_RFC3986:
+        if os.environ.get("LNURL_STRICT_RFC3986", "0") == "1":
             yield strict_rfc3986_validator
         yield cls.validate
 
     @property
     def base(self) -> str:
         hostport = f"{self.host}:{self.port}" if self.port else self.host
         return f"{self.scheme}://{hostport}{self.path}"
 
     @property
     def query_params(self) -> dict:
         return {k: v[0] for k, v in parse_qs(self.query).items()}
 
 
 class ClearnetUrl(Url):
-    """Web URL, secure by default; users can override the FORCE_SSL setting."""
+    """Secure web URL."""
 
     allowed_schemes = {"https"}
 
 
 class OnionUrl(Url):
     """Tor anonymous onion service."""
```

### Comparing `lnurl-0.3.5/lnurl.egg-info/PKG-INFO` & `lnurl-0.3.6/lnurl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lnurl
-Version: 0.3.5
+Version: 0.3.6
 Summary: LNURL implementation for Python.
-Home-page: https://github.com/python-ln/lnurl
+Home-page: https://github.com/lnbits/lnurl
 Author: jogco
 Author-email: jogco@lnsms.world
 Maintainer: eillarra
 Maintainer-email: eneko@illarra.com
 License: MIT
 Description: LNURL implementation for Python
         ===============================
@@ -17,14 +17,22 @@
         [![pypi-badge]][pypi]
         [![pypi-versions-badge]][pypi]
         [![license-badge]](LICENSE)
         
         
         A collection of helpers for building [LNURL][lnurl] support into wallets and services.
         
+        Configuration
+        -------------
+        
+        Developers can force strict RFC3986 validation for the URLs that the library encodes/decodes, using this env var:
+        
+        > LNURL_STRICT_RFC3986 = "0" by default (False)
+        
+        
         Basic usage
         -----------
         
         ```python
         >>> import lnurl
         >>> lnurl.encode('https://service.io/?q=3fc3645b439ce8e7')
         Lnurl('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', bech32=Bech32('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', hrp='lnurl', data=[13, 1, 26, 7, 8, 28, 3, 19, 7, 8, 23, 18, 30, 28, 27, 5, 14, 9, 27, 6, 18, 24, 27, 5, 5, 25, 20, 22, 30, 11, 25, 31, 14, 4, 30, 19, 6, 25, 19, 3, 6, 12, 27, 3, 8, 13, 11, 2, 6, 16, 25, 19, 18, 24, 27, 5, 7, 1, 18, 19, 14]), url=WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7'))
@@ -109,20 +117,20 @@
         You can also use camelCases when you parse the data, and it will be converted to snake_case to make your
         Python code nicer.
         
         If you want to export the data using :snake: snake_case (in your Python code, for example), you can change
         the `by_alias` parameter: `res.dict(by_alias=False)` (it is `True` by default).
         
         
-        [github-tests]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22tests%22
-        [github-tests-badge]: https://github.com/python-ln/lnurl/workflows/tests/badge.svg
-        [github-mypy]: https://github.com/python-ln/lnurl/actions?query=workflow%3A%22mypy%22
-        [github-mypy-badge]: https://github.com/python-ln/lnurl/workflows/mypy/badge.svg
-        [codecov]: https://codecov.io/gh/python-ln/lnurl
-        [codecov-badge]: https://codecov.io/gh/python-ln/lnurl/branch/master/graph/badge.svg
+        [github-tests]: https://github.com/lnbits/lnurl/actions?query=workflow%3Atests
+        [github-tests-badge]: https://github.com/lnbits/lnurl/workflows/tests/badge.svg
+        [github-mypy]: https://github.com/lnbits/lnurl/actions?query=workflow%3Amypy
+        [github-mypy-badge]: https://github.com/lnbits/lnurl/workflows/mypy/badge.svg
+        [codecov]: https://codecov.io/gh/lnbits/lnurl
+        [codecov-badge]: https://codecov.io/gh/lnbits/lnurl/branch/master/graph/badge.svg
         [pypi]: https://pypi.org/project/lnurl/
         [pypi-badge]: https://badge.fury.io/py/lnurl.svg
         [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/lnurl.svg
         [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
         
         [lnurl]: https://telegra.ph/lnurl-a-protocol-for-seamless-interaction-between-services-and-Lightning-wallets-08-19
         [lnurl-spec]: https://github.com/btcontract/lnurl-rfc/blob/master/spec.md
@@ -135,10 +143,11 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lnurl-0.3.5/setup.py` & `lnurl-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 with open(path.join(path.abspath(path.dirname(__file__)), "README.md")) as f:
     long_description = f.read()
 
 
 setup(
     name="lnurl",
-    version="0.3.5",
-    url="https://github.com/python-ln/lnurl",
+    version="0.3.6",
+    url="https://github.com/lnbits/lnurl",
     author="jogco",
     author_email="jogco@lnsms.world",
     maintainer="eillarra",
     maintainer_email="eneko@illarra.com",
     license="MIT",
     description="LNURL implementation for Python.",
     long_description=long_description,
@@ -25,14 +25,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Utilities",
     ],
     packages=["lnurl"],
     python_requires=">=3.6",
     install_requires=["bech32", "pydantic", "typing-extensions; python_version<'3.8'"],
     zip_safe=False,
 )
```

