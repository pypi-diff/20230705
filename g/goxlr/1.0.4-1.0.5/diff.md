# Comparing `tmp/goxlr-1.0.4.tar.gz` & `tmp/goxlr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.0.4.tar", last modified: Tue Jul  4 16:04:15 2023, max compression
+gzip compressed data, was "goxlr-1.0.5.tar", last modified: Tue Jul  4 23:16:01 2023, max compression
```

## Comparing `goxlr-1.0.4.tar` & `goxlr-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.638918 goxlr-1.0.4/
--rw-rw-rw-   0        0        0     1089 2023-07-04 11:05:46.000000 goxlr-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2218 2023-07-04 16:04:15.639419 goxlr-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1901 2023-07-04 16:00:21.000000 goxlr-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.633916 goxlr-1.0.4/goxlr/
--rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.4/goxlr/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.4/goxlr/error.py
--rw-rw-rw-   0        0        0    27172 2023-07-04 01:14:35.000000 goxlr-1.0.4/goxlr/goxlr.py
--rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.4/goxlr/types.py
--rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.4/goxlr/ws.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:04:15.637917 goxlr-1.0.4/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2218 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 16:04:15.000000 goxlr-1.0.4/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-04 16:04:15.639918 goxlr-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-07-04 15:59:27.000000 goxlr-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:16:01.003638 goxlr-1.0.5/
+-rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.0.5/LICENSE-3RD-PARTY.txt
+-rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2350 2023-07-04 23:16:01.003638 goxlr-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-07-04 22:58:39.000000 goxlr-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 23:16:00.999641 goxlr-1.0.5/goxlr/
+-rw-rw-rw-   0        0        0       61 2023-07-04 23:15:46.000000 goxlr-1.0.5/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-04 22:59:52.000000 goxlr-1.0.5/goxlr/_version.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.5/goxlr/error.py
+-rw-rw-rw-   0        0        0    27238 2023-07-04 21:56:29.000000 goxlr-1.0.5/goxlr/goxlr.py
+-rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.5/goxlr/types.py
+-rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.5/goxlr/ws.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:16:01.003139 goxlr-1.0.5/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2350 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 23:16:00.000000 goxlr-1.0.5/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-04 23:16:01.004640 goxlr-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.0.5/setup.py
```

### Comparing `goxlr-1.0.4/LICENSE.txt` & `goxlr-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.4/PKG-INFO` & `goxlr-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
- [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr)
+ [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
 
-A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio.
+A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
 
 ## Features
 - Asynchronous connection to the GoXLR utility daemon
 - Almost all methods have been translated to Python
 - Handy enumerators for everything
 - Very simple and easy to get started
 
@@ -45,12 +46,12 @@
 async def main():
     xlr = GoXLR()
     xlr.connect()
     print(await xlr.ping())
     xlr.close()
 ```
 
-## Documentation
-Coming soon. For now, please refer to [goxlr.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/goxlr.py) to see all of the daemon and GoXLR commands, and refer to [types.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/types.py) to see all of the enums. You may find it very useful to have an IntelliSense-style plugin in your IDE.
-
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
+
+## Documentation
+Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

### Comparing `goxlr-1.0.4/goxlr/goxlr.py` & `goxlr-1.0.5/goxlr/goxlr.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 class GoXLR(Socket):
     def __init__(self, host="localhost", port=14564):
         super().__init__(host, port)
 
     # General commands
 
     async def ping(self):
+        """
+        Pings the GoXLR Utility daemon
+        """
         return await self.send("Ping")
 
     async def get_status(self):
         return await self.send("GetStatus")
 
     # Daemon commands
```

### Comparing `goxlr-1.0.4/goxlr/types.py` & `goxlr-1.0.5/goxlr/types.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.4/goxlr/ws.py` & `goxlr-1.0.5/goxlr/ws.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.4/goxlr.egg-info/PKG-INFO` & `goxlr-1.0.5/goxlr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 
 # GoXLR Utility API Python Wrapper
 
- [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr)
+ [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/goxlr.svg)](https://badge.fury.io/py/goxlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/goxlr) ![GitHub issues](https://img.shields.io/github/issues/samcarsonx/goxlr) [![Documentation Status](https://readthedocs.org/projects/goxlr/badge/?version=latest)](https://goxlr.readthedocs.io/en/latest/?badge=latest)
 
-A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio.
+A python wrapper for the API of the open-source GoXLR software alternative, GoXLR Utility, that uses asyncio. Disclaimer: This project is not affiliated with the GoXLR brand or TC-Helicon in any way, shape, or form. This is a third-party package made for fun and educational purposes.
 
 ## Features
 - Asynchronous connection to the GoXLR utility daemon
 - Almost all methods have been translated to Python
 - Handy enumerators for everything
 - Very simple and easy to get started
 
@@ -45,12 +46,12 @@
 async def main():
     xlr = GoXLR()
     xlr.connect()
     print(await xlr.ping())
     xlr.close()
 ```
 
-## Documentation
-Coming soon. For now, please refer to [goxlr.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/goxlr.py) to see all of the daemon and GoXLR commands, and refer to [types.py](https://github.com/samcarsonx/goxlr/blob/main/goxlr/types.py) to see all of the enums. You may find it very useful to have an IntelliSense-style plugin in your IDE.
-
 ## Contributing
 Coming soon. As there isn't a CONTRIBUTING.md yet, please try to emulate the style of the rest of the code. Using snake_case and descriptive method argument names with type hints wherever possible.
+
+## Documentation
+Please visit the [documentation](https://goxlr.readthedocs.io/en/latest/) for more information on how to use this package.
```

