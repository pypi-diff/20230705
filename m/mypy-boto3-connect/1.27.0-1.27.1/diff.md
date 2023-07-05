# Comparing `tmp/mypy-boto3-connect-1.27.0.tar.gz` & `tmp/mypy-boto3-connect-1.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.27.1.tar", last modified: Wed Jul  5 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-connect-1.27.0.tar` & `mypy-boto3-connect-1.27.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.227065 mypy-boto3-connect-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-03 19:50:36.227065 mypy-boto3-connect-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43814 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.227065 mypy-boto3-connect-1.27.0/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   150382 2023-07-03 19:34:57.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   150136 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-03 19:34:57.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-03 19:34:57.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-03 19:34:57.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-03 19:34:57.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   218168 2023-07-03 19:35:03.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   217837 2023-07-03 19:35:00.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:55.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.227065 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:36.000000 mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.227065 mypy-boto3-connect-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:34:54.000000 mypy-boto3-connect-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.840989 mypy-boto3-connect-1.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-05 19:47:56.840989 mypy-boto3-connect-1.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43814 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.836989 mypy-boto3-connect-1.27.1/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150407 2023-07-05 19:47:10.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150161 2023-07-05 19:47:09.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-05 19:47:12.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-05 19:47:11.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-05 19:47:11.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-05 19:47:11.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   218168 2023-07-05 19:47:19.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217837 2023-07-05 19:47:15.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.840989 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 19:47:56.000000 mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:47:56.840989 mypy-boto3-connect-1.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-05 19:47:08.000000 mypy-boto3-connect-1.27.1/setup.py
```

### Comparing `mypy-boto3-connect-1.27.0/LICENSE` & `mypy-boto3-connect-1.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/PKG-INFO` & `mypy-boto3-connect-1.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.27.0
-Summary: Type annotations for boto3.Connect 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.1
+Summary: Type annotations for boto3.Connect 1.27.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.27.0/README.md` & `mypy-boto3-connect-1.27.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Connect 1.27.1\nVersion:         1.27.1\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.27.0")
+    print("1.27.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1994,15 +1994,15 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
     ) -> SearchQueuesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
 
     def search_quick_connects(
         self,
@@ -2042,15 +2042,16 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches routing profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
 
     def search_security_profiles(
         self,
@@ -2058,15 +2059,16 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches security profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
 
     def search_users(
         self,
```

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1852,15 +1852,15 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
     ) -> SearchQueuesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
     def search_quick_connects(
         self,
         *,
@@ -1897,30 +1897,32 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches routing profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
     def search_security_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches security profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
     def search_users(
         self,
         *,
```

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.27.0
-Summary: Type annotations for boto3.Connect 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.1
+Summary: Type annotations for boto3.Connect 1.27.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.27.0/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.27.1/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.27.0/setup.py` & `mypy-boto3-connect-1.27.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.27.0",
+    version="1.27.1",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Connect 1.27.1 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

