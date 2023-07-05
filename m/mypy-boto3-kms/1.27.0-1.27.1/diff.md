# Comparing `tmp/mypy-boto3-kms-1.27.0.tar.gz` & `tmp/mypy-boto3-kms-1.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.27.0.tar", last modified: Mon Jul  3 19:51:00 2023, max compression
+gzip compressed data, was "mypy-boto3-kms-1.27.1.tar", last modified: Wed Jul  5 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-kms-1.27.0.tar` & `mypy-boto3-kms-1.27.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:00.731544 mypy-boto3-kms-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-03 19:51:00.731544 mypy-boto3-kms-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:00.731544 mypy-boto3-kms-1.27.0/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40803 2023-07-03 19:40:31.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40739 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-03 19:40:32.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-03 19:40:32.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-03 19:40:31.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-03 19:40:31.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40380 2023-07-03 19:40:32.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40321 2023-07-03 19:40:32.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:00.731544 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:00.000000 mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:00.731544 mypy-boto3-kms-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:40:30.000000 mypy-boto3-kms-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-05 19:47:21.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-05 19:47:21.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-07-05 19:47:23.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40953 2023-07-05 19:47:22.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/setup.py
```

### Comparing `mypy-boto3-kms-1.27.0/LICENSE` & `mypy-boto3-kms-1.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/PKG-INFO` & `mypy-boto3-kms-1.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.27.0
-Summary: Type annotations for boto3.KMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.1
+Summary: Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.0/README.md` & `mypy-boto3-kms-1.27.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.KMS 1.27.1\nVersion:         1.27.1\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,40 +85,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KMSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
+    DryRunOperationException: Type[BotocoreClientError]
     ExpiredImportTokenException: Type[BotocoreClientError]
     IncorrectKeyException: Type[BotocoreClientError]
     IncorrectKeyMaterialException: Type[BotocoreClientError]
     IncorrectTrustAnchorException: Type[BotocoreClientError]
     InvalidAliasNameException: Type[BotocoreClientError]
     InvalidArnException: Type[BotocoreClientError]
     InvalidCiphertextException: Type[BotocoreClientError]
@@ -146,15 +144,14 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
-
 class KMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/)
     """
 
     meta: ClientMeta
@@ -163,57 +160,51 @@
     def exceptions(self) -> Exceptions:
         """
         KMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#can_paginate)
         """
-
     def cancel_key_deletion(self, *, KeyId: str) -> CancelKeyDeletionResponseTypeDef:
         """
         Cancels the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.cancel_key_deletion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#cancel_key_deletion)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#close)
         """
-
     def connect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Connects or reconnects a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ to its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.connect_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#connect_custom_key_store)
         """
-
     def create_alias(self, *, AliasName: str, TargetKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Creates a friendly name for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_alias)
         """
-
     def create_custom_key_store(
         self,
         *,
         CustomKeyStoreName: str,
         CloudHsmClusterId: str = ...,
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
@@ -228,33 +219,32 @@
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ backed by a key store that you own and manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_custom_key_store)
         """
-
     def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
         Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
-        Name: str = ...
+        Name: str = ...,
+        DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_grant)
         """
-
     def create_key(
         self,
         *,
         Policy: str = ...,
         Description: str = ...,
         KeyUsage: KeyUsageTypeType = ...,
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
@@ -270,61 +260,57 @@
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-
         keys)_ in your Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_key)
         """
-
     def decrypt(
         self,
         *,
         CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was enc...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.decrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#decrypt)
         """
-
     def delete_alias(self, *, AliasName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_alias)
         """
-
     def delete_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Deletes a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_custom_key_store)
         """
-
     def delete_imported_key_material(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes key material that was previously imported.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_imported_key_material)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_imported_key_material)
         """
-
     def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -333,238 +319,225 @@
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_custom_key_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#describe_custom_key_stores)
         """
-
     def describe_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> DescribeKeyResponseTypeDef:
         """
         Provides detailed information about a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#describe_key)
         """
-
     def disable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the state of a KMS key to disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disable_key)
         """
-
     def disable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Disables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disable_key_rotation)
         """
-
     def disconnect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Disconnects the [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ from its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disconnect_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disconnect_custom_key_store)
         """
-
     def enable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key)
         """
-
     def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
-
     def encrypt(
         self,
         *,
         KeyId: str,
         Plaintext: Union[str, bytes, IO[Any], StreamingBody],
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
+        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
+        DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#encrypt)
         """
-
     def generate_data_key(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key)
         """
-
     def generate_data_key_pair(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_pair)
         """
-
     def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_pair_without_plaintext)
         """
-
     def generate_data_key_without_plaintext(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_without_plaintext)
         """
-
     def generate_mac(
         self,
         *,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_mac)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_presigned_url)
         """
-
     def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_random)
         """
-
     def get_key_policy(self, *, KeyId: str, PolicyName: str) -> GetKeyPolicyResponseTypeDef:
         """
         Gets a key policy attached to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_policy)
         """
-
     def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
         Gets a Boolean value that indicates whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ is enabled for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_rotation_status)
         """
-
     def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
         WrappingKeySpec: WrappingKeySpecType
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_parameters_for_import)
         """
-
     def get_public_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> GetPublicKeyResponseTypeDef:
         """
         Returns the public key of an asymmetric KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_public_key)
         """
-
     def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: Union[str, bytes, IO[Any], StreamingBody],
         EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
         ValidTo: Union[datetime, str] = ...,
@@ -573,25 +546,23 @@
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#import_key_material)
         """
-
     def list_aliases(
         self, *, KeyId: str = ..., Limit: int = ..., Marker: str = ...
     ) -> ListAliasesResponseTypeDef:
         """
         Gets a list of aliases in the caller's Amazon Web Services account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_aliases)
         """
-
     def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
@@ -599,89 +570,83 @@
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_grants)
         """
-
     def list_key_policies(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListKeyPoliciesResponseTypeDef:
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_policies)
         """
-
     def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_keys)
         """
-
     def list_resource_tags(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListResourceTagsResponseTypeDef:
         """
         Returns all tags on the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_resource_tags)
         """
-
     def list_retirable_grants(
         self, *, RetiringPrincipal: str, Limit: int = ..., Marker: str = ...
     ) -> ListGrantsResponseTypeDef:
         """
         Returns information about all grants in the Amazon Web Services account and
         Region that have the specified retiring principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_retirable_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_retirable_grants)
         """
-
     def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
         BypassPolicyLockoutSafetyCheck: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#put_key_policy)
         """
-
     def re_encrypt(
         self,
         *,
         CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#re_encrypt)
         """
-
     def replicate_key(
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
@@ -690,91 +655,86 @@
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#replicate_key)
         """
-
     def retire_grant(
-        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ...
+        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ..., DryRun: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.retire_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#retire_grant)
         """
-
-    def revoke_grant(self, *, KeyId: str, GrantId: str) -> EmptyResponseMetadataTypeDef:
+    def revoke_grant(
+        self, *, KeyId: str, GrantId: str, DryRun: bool = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#revoke_grant)
         """
-
     def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#schedule_key_deletion)
         """
-
     def sign(
         self,
         *,
         KeyId: str,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
         signing KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.sign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#sign)
         """
-
     def tag_resource(
         self, *, KeyId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or edits tags on a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#tag_resource)
         """
-
     def untag_resource(self, *, KeyId: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#untag_resource)
         """
-
     def update_alias(self, *, AliasName: str, TargetKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Associates an existing KMS alias with a different KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_alias)
         """
-
     def update_custom_key_store(
         self,
         *,
         CustomKeyStoreId: str,
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
@@ -786,117 +746,108 @@
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_custom_key_store)
         """
-
     def update_key_description(
         self, *, KeyId: str, Description: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_key_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_key_description)
         """
-
     def update_primary_region(
         self, *, KeyId: str, PrimaryRegion: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the primary key of a multi-Region key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_primary_region)
         """
-
     def verify(
         self,
         *,
         KeyId: str,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         Signature: Union[str, bytes, IO[Any], StreamingBody],
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify)
         """
-
     def verify_mac(
         self,
         *,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: Union[str, bytes, IO[Any], StreamingBody],
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify_mac)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_key_stores"]
     ) -> DescribeCustomKeyStoresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_aliases"]) -> ListAliasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_grants"]) -> ListGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_policies"]
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_tags"]
     ) -> ListResourceTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_retirable_grants"]
     ) -> ListRetirableGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,37 +85,41 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("KMSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
+    DryRunOperationException: Type[BotocoreClientError]
     ExpiredImportTokenException: Type[BotocoreClientError]
     IncorrectKeyException: Type[BotocoreClientError]
     IncorrectKeyMaterialException: Type[BotocoreClientError]
     IncorrectTrustAnchorException: Type[BotocoreClientError]
     InvalidAliasNameException: Type[BotocoreClientError]
     InvalidArnException: Type[BotocoreClientError]
     InvalidCiphertextException: Type[BotocoreClientError]
@@ -143,14 +147,15 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
+
 class KMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/)
     """
 
     meta: ClientMeta
@@ -159,51 +164,57 @@
     def exceptions(self) -> Exceptions:
         """
         KMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#can_paginate)
         """
+
     def cancel_key_deletion(self, *, KeyId: str) -> CancelKeyDeletionResponseTypeDef:
         """
         Cancels the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.cancel_key_deletion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#cancel_key_deletion)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#close)
         """
+
     def connect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Connects or reconnects a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ to its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.connect_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#connect_custom_key_store)
         """
+
     def create_alias(self, *, AliasName: str, TargetKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Creates a friendly name for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_alias)
         """
+
     def create_custom_key_store(
         self,
         *,
         CustomKeyStoreName: str,
         CloudHsmClusterId: str = ...,
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
@@ -218,31 +229,34 @@
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ backed by a key store that you own and manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_custom_key_store)
         """
+
     def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
         Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
-        Name: str = ...
+        Name: str = ...,
+        DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_grant)
         """
+
     def create_key(
         self,
         *,
         Policy: str = ...,
         Description: str = ...,
         KeyUsage: KeyUsageTypeType = ...,
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
@@ -258,56 +272,62 @@
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-
         keys)_ in your Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_key)
         """
+
     def decrypt(
         self,
         *,
         CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was enc...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.decrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#decrypt)
         """
+
     def delete_alias(self, *, AliasName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_alias)
         """
+
     def delete_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Deletes a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_custom_key_store)
         """
+
     def delete_imported_key_material(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes key material that was previously imported.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_imported_key_material)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#delete_imported_key_material)
         """
+
     def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -316,219 +336,244 @@
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_custom_key_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#describe_custom_key_stores)
         """
+
     def describe_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> DescribeKeyResponseTypeDef:
         """
         Provides detailed information about a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#describe_key)
         """
+
     def disable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the state of a KMS key to disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disable_key)
         """
+
     def disable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Disables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disable_key_rotation)
         """
+
     def disconnect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Disconnects the [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ from its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disconnect_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#disconnect_custom_key_store)
         """
+
     def enable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key)
         """
+
     def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
+
     def encrypt(
         self,
         *,
         KeyId: str,
         Plaintext: Union[str, bytes, IO[Any], StreamingBody],
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
+        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
+        DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#encrypt)
         """
+
     def generate_data_key(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key)
         """
+
     def generate_data_key_pair(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_pair)
         """
+
     def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_pair_without_plaintext)
         """
+
     def generate_data_key_without_plaintext(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_without_plaintext)
         """
+
     def generate_mac(
         self,
         *,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_mac)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_presigned_url)
         """
+
     def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_random)
         """
+
     def get_key_policy(self, *, KeyId: str, PolicyName: str) -> GetKeyPolicyResponseTypeDef:
         """
         Gets a key policy attached to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_policy)
         """
+
     def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
         Gets a Boolean value that indicates whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ is enabled for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_rotation_status)
         """
+
     def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
         WrappingKeySpec: WrappingKeySpecType
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_parameters_for_import)
         """
+
     def get_public_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> GetPublicKeyResponseTypeDef:
         """
         Returns the public key of an asymmetric KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_public_key)
         """
+
     def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: Union[str, bytes, IO[Any], StreamingBody],
         EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
         ValidTo: Union[datetime, str] = ...,
@@ -537,23 +582,25 @@
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#import_key_material)
         """
+
     def list_aliases(
         self, *, KeyId: str = ..., Limit: int = ..., Marker: str = ...
     ) -> ListAliasesResponseTypeDef:
         """
         Gets a list of aliases in the caller's Amazon Web Services account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_aliases)
         """
+
     def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
@@ -561,82 +608,90 @@
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_grants)
         """
+
     def list_key_policies(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListKeyPoliciesResponseTypeDef:
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_policies)
         """
+
     def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_keys)
         """
+
     def list_resource_tags(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListResourceTagsResponseTypeDef:
         """
         Returns all tags on the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_resource_tags)
         """
+
     def list_retirable_grants(
         self, *, RetiringPrincipal: str, Limit: int = ..., Marker: str = ...
     ) -> ListGrantsResponseTypeDef:
         """
         Returns information about all grants in the Amazon Web Services account and
         Region that have the specified retiring principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_retirable_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_retirable_grants)
         """
+
     def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
         BypassPolicyLockoutSafetyCheck: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#put_key_policy)
         """
+
     def re_encrypt(
         self,
         *,
         CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#re_encrypt)
         """
+
     def replicate_key(
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
@@ -645,83 +700,94 @@
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#replicate_key)
         """
+
     def retire_grant(
-        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ...
+        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ..., DryRun: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.retire_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#retire_grant)
         """
-    def revoke_grant(self, *, KeyId: str, GrantId: str) -> EmptyResponseMetadataTypeDef:
+
+    def revoke_grant(
+        self, *, KeyId: str, GrantId: str, DryRun: bool = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#revoke_grant)
         """
+
     def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#schedule_key_deletion)
         """
+
     def sign(
         self,
         *,
         KeyId: str,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
         signing KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.sign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#sign)
         """
+
     def tag_resource(
         self, *, KeyId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or edits tags on a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#tag_resource)
         """
+
     def untag_resource(self, *, KeyId: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#untag_resource)
         """
+
     def update_alias(self, *, AliasName: str, TargetKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Associates an existing KMS alias with a different KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_alias)
         """
+
     def update_custom_key_store(
         self,
         *,
         CustomKeyStoreId: str,
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
@@ -733,106 +799,119 @@
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_custom_key_store)
         """
+
     def update_key_description(
         self, *, KeyId: str, Description: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_key_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_key_description)
         """
+
     def update_primary_region(
         self, *, KeyId: str, PrimaryRegion: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the primary key of a multi-Region key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_primary_region)
         """
+
     def verify(
         self,
         *,
         KeyId: str,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         Signature: Union[str, bytes, IO[Any], StreamingBody],
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify)
         """
+
     def verify_mac(
         self,
         *,
         Message: Union[str, bytes, IO[Any], StreamingBody],
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: Union[str, bytes, IO[Any], StreamingBody],
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify_mac)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_key_stores"]
     ) -> DescribeCustomKeyStoresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_aliases"]) -> ListAliasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_grants"]) -> ListGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_policies"]
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_tags"]
     ) -> ListResourceTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_retirable_grants"]
     ) -> ListRetirableGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,15 @@
 )
 _OptionalEncryptRequestRequestTypeDef = TypedDict(
     "_OptionalEncryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
@@ -432,14 +433,15 @@
     },
 )
 _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
@@ -479,14 +481,15 @@
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
@@ -512,14 +515,15 @@
         "MacAlgorithm": MacAlgorithmSpecType,
     },
 )
 _OptionalGenerateMacRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
@@ -954,14 +958,15 @@
     {
         "SourceEncryptionContext": Mapping[str, str],
         "SourceKeyId": str,
         "DestinationEncryptionContext": Mapping[str, str],
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
@@ -994,25 +999,40 @@
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
-RevokeGrantRequestRequestTypeDef = TypedDict(
-    "RevokeGrantRequestRequestTypeDef",
+_RequiredRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
     },
 )
+_OptionalRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeGrantRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class RevokeGrantRequestRequestTypeDef(
+    _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -1052,14 +1072,15 @@
     },
 )
 _OptionalSignRequestRequestTypeDef = TypedDict(
     "_OptionalSignRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
@@ -1118,14 +1139,15 @@
         "Mac": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
@@ -1153,14 +1175,15 @@
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
@@ -1258,14 +1281,15 @@
 _OptionalCreateGrantRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGrantRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
@@ -1376,14 +1400,15 @@
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
@@ -1400,14 +1425,15 @@
 )
 _OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
@@ -1426,14 +1452,15 @@
     "_OptionalGenerateDataKeyRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "NumberOfBytes": int,
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -383,14 +383,15 @@
 )
 _OptionalEncryptRequestRequestTypeDef = TypedDict(
     "_OptionalEncryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
@@ -427,14 +428,15 @@
     },
 )
 _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
@@ -472,14 +474,15 @@
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
@@ -503,14 +506,15 @@
         "MacAlgorithm": MacAlgorithmSpecType,
     },
 )
 _OptionalGenerateMacRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
@@ -921,14 +925,15 @@
     {
         "SourceEncryptionContext": Mapping[str, str],
         "SourceKeyId": str,
         "DestinationEncryptionContext": Mapping[str, str],
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
@@ -959,25 +964,38 @@
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
-RevokeGrantRequestRequestTypeDef = TypedDict(
-    "RevokeGrantRequestRequestTypeDef",
+_RequiredRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
     },
 )
+_OptionalRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeGrantRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class RevokeGrantRequestRequestTypeDef(
+    _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
+):
+    pass
 
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -1015,14 +1033,15 @@
     },
 )
 _OptionalSignRequestRequestTypeDef = TypedDict(
     "_OptionalSignRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
@@ -1079,14 +1098,15 @@
         "Mac": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
@@ -1112,14 +1132,15 @@
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
@@ -1211,14 +1232,15 @@
 _OptionalCreateGrantRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGrantRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
@@ -1325,14 +1347,15 @@
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
@@ -1347,14 +1370,15 @@
 )
 _OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
@@ -1371,14 +1395,15 @@
     "_OptionalGenerateDataKeyRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "NumberOfBytes": int,
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.27.0
-Summary: Type annotations for boto3.KMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.1
+Summary: Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.0/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.0/setup.py` & `mypy-boto3-kms-1.27.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.27.0",
+    version="1.27.1",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

