# Comparing `tmp/mypy-boto3-mgn-1.27.0.tar.gz` & `tmp/mypy-boto3-mgn-1.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.27.1.tar", last modified: Wed Jul  5 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-mgn-1.27.0.tar` & `mypy-boto3-mgn-1.27.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21530 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.491685 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48373 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48291 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-03 19:42:21.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-03 19:42:20.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68618 2023-07-03 19:42:23.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68553 2023-07-03 19:42:22.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.836989 mypy-boto3-mgn-1.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-07-05 19:47:56.828989 mypy-boto3-mgn-1.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.816989 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51946 2023-07-05 19:47:25.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51859 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-05 19:47:26.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-07-05 19:47:25.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-05 19:47:25.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-05 19:47:25.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80103 2023-07-05 19:47:28.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79988 2023-07-05 19:47:27.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.828989 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 19:47:56.000000 mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:47:56.836989 mypy-boto3-mgn-1.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-05 19:47:24.000000 mypy-boto3-mgn-1.27.1/setup.py
```

### Comparing `mypy-boto3-mgn-1.27.0/LICENSE` & `mypy-boto3-mgn-1.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.27.0/PKG-INFO` & `mypy-boto3-mgn-1.27.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,20 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-mgn
-Version: 1.27.0
-Summary: Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mgn type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,14 +257,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 client: mgnClient = Session().client("mgn")
 
@@ -319,14 +288,17 @@
     "describe_vcenter_clients"
 )
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
 list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
 list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
 list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator(
+    "list_managed_accounts"
+)
 list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator(
     "list_source_server_actions"
 )
 list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator(
     "list_template_actions"
 )
 list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
@@ -368,14 +340,15 @@
     LaunchStatusType,
     LifeCycleStateType,
     ListApplicationsPaginatorName,
     ListExportErrorsPaginatorName,
     ListExportsPaginatorName,
     ListImportErrorsPaginatorName,
     ListImportsPaginatorName,
+    ListManagedAccountsPaginatorName,
     ListSourceServerActionsPaginatorName,
     ListTemplateActionsPaginatorName,
     ListWavesPaginatorName,
     PostLaunchActionExecutionStatusType,
     PostLaunchActionsDeploymentTypeType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
@@ -470,35 +443,41 @@
     ListApplicationsRequestFiltersTypeDef,
     ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
+    ListManagedAccountsRequestRequestTypeDef,
+    ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
     PaginatorConfigTypeDef,
+    PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
+    ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
+    StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
     UnarchiveApplicationRequestRequestTypeDef,
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -525,14 +504,15 @@
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
     ListSourceServerActionsRequestRequestTypeDef,
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
```

### Comparing `mypy-boto3-mgn-1.27.0/README.md` & `mypy-boto3-mgn-1.27.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,52 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-mgn
+Version: 1.27.1
+Summary: Type annotations for boto3.mgn 1.27.1 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 mgn type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -257,14 +289,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 client: mgnClient = Session().client("mgn")
 
@@ -287,14 +320,17 @@
     "describe_vcenter_clients"
 )
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
 list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
 list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
 list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator(
+    "list_managed_accounts"
+)
 list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator(
     "list_source_server_actions"
 )
 list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator(
     "list_template_actions"
 )
 list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
@@ -336,14 +372,15 @@
     LaunchStatusType,
     LifeCycleStateType,
     ListApplicationsPaginatorName,
     ListExportErrorsPaginatorName,
     ListExportsPaginatorName,
     ListImportErrorsPaginatorName,
     ListImportsPaginatorName,
+    ListManagedAccountsPaginatorName,
     ListSourceServerActionsPaginatorName,
     ListTemplateActionsPaginatorName,
     ListWavesPaginatorName,
     PostLaunchActionExecutionStatusType,
     PostLaunchActionsDeploymentTypeType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
@@ -438,35 +475,41 @@
     ListApplicationsRequestFiltersTypeDef,
     ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
+    ListManagedAccountsRequestRequestTypeDef,
+    ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
     PaginatorConfigTypeDef,
+    PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
+    ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
+    StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
     UnarchiveApplicationRequestRequestTypeDef,
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -493,14 +536,15 @@
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
     ListSourceServerActionsRequestRequestTypeDef,
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
         mgnClient,
     )
 
     session = Session()
@@ -34,14 +35,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from .client import mgnClient
 from .paginator import (
@@ -52,14 +54,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
@@ -73,12 +76,13 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
     "mgnClient",
 )
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
         mgnClient,
     )
 
     session = Session()
@@ -34,14 +35,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from .client import mgnClient
 from .paginator import (
@@ -52,14 +54,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
@@ -72,12 +75,13 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
     "mgnClient",
 )
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__main__.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mgn 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.mgn 1.27.1\nVersion:         1.27.1\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
     ApplicationResponseMetadataTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
@@ -64,14 +65,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
@@ -94,38 +96,34 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("mgnClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UninitializedAccountException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class mgnClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/)
     """
 
     meta: ClientMeta
@@ -134,91 +132,90 @@
     def exceptions(self) -> Exceptions:
         """
         mgnClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#exceptions)
         """
-
-    def archive_application(self, *, applicationID: str) -> ApplicationResponseMetadataTypeDef:
+    def archive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseMetadataTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_application)
         """
-
-    def archive_wave(self, *, waveID: str) -> WaveResponseMetadataTypeDef:
+    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_wave)
         """
-
     def associate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate applications to wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#associate_applications)
         """
-
     def associate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate source servers to application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#associate_source_servers)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#can_paginate)
         """
-
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
-        sourceServerID: str
+        sourceServerID: str,
+        accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#change_server_life_cycle_state)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#close)
         """
-
     def create_application(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> ApplicationResponseMetadataTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
-
     def create_launch_configuration_template(
         self,
         *,
         associatePublicIpAddress: bool = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
@@ -235,15 +232,14 @@
     ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
-
     def create_replication_configuration_template(
         self,
         *,
         associateDefaultSecurityGroup: bool,
         bandwidthThrottling: int,
         createPublicIP: bool,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,
@@ -251,118 +247,114 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
-
     def create_wave(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> WaveResponseMetadataTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
-
-    def delete_application(self, *, applicationID: str) -> Dict[str, Any]:
+    def delete_application(self, *, applicationID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_application)
         """
-
-    def delete_job(self, *, jobID: str) -> Dict[str, Any]:
+    def delete_job(self, *, jobID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_job)
         """
-
     def delete_launch_configuration_template(
         self, *, launchConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Deletes a single Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_launch_configuration_template)
         """
-
     def delete_replication_configuration_template(
         self, *, replicationConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_replication_configuration_template)
         """
-
-    def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
+    def delete_source_server(self, *, sourceServerID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single source server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_source_server)
         """
-
     def delete_vcenter_client(self, *, vcenterClientID: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a given vCenter client by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_vcenter_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_vcenter_client)
         """
-
-    def delete_wave(self, *, waveID: str) -> Dict[str, Any]:
+    def delete_wave(self, *, waveID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_wave)
         """
-
     def describe_job_log_items(
-        self, *, jobID: str, maxResults: int = ..., nextToken: str = ...
+        self, *, jobID: str, accountID: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobLogItemsResponseTypeDef:
         """
         Retrieves detailed job log items with paging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_job_log_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_job_log_items)
         """
-
     def describe_jobs(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_jobs)
         """
-
     def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
@@ -370,262 +362,269 @@
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_launch_configuration_templates)
         """
-
     def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         replicationConfigurationTemplateIDs: Sequence[str] = ...
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_replication_configuration_templates)
         """
-
     def describe_source_servers(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_source_servers)
         """
-
     def describe_vcenter_clients(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeVcenterClientsResponseTypeDef:
         """
         Returns a list of the installed vCenter clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_vcenter_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_vcenter_clients)
         """
-
     def disassociate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate applications from wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_applications)
         """
-
     def disassociate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate source servers from application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_source_servers)
         """
-
     def disconnect_from_service(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disconnect_from_service)
         """
-
-    def finalize_cutover(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+    def finalize_cutover(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#finalize_cutover)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#generate_presigned_url)
         """
-
-    def get_launch_configuration(self, *, sourceServerID: str) -> LaunchConfigurationTypeDef:
+    def get_launch_configuration(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> LaunchConfigurationTypeDef:
         """
         Lists all LaunchConfigurations available, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_launch_configuration)
         """
-
     def get_replication_configuration(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Lists all ReplicationConfigurations, filtered by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_replication_configuration)
         """
-
     def initialize_service(self) -> Dict[str, Any]:
         """
         Initialize Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.initialize_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#initialize_service)
         """
-
     def list_applications(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_applications)
         """
-
     def list_export_errors(
         self, *, exportID: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListExportErrorsResponseTypeDef:
         """
         List export errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_export_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_export_errors)
         """
-
     def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_exports)
         """
-
     def list_import_errors(
         self, *, importID: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListImportErrorsResponseTypeDef:
         """
         List import errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_import_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_import_errors)
         """
-
     def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_imports)
         """
+    def list_managed_accounts(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListManagedAccountsResponseTypeDef:
+        """
+        List Managed Accounts.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_managed_accounts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_managed_accounts)
+        """
     def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_source_server_actions)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List all tags for your Application Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_tags_for_resource)
         """
-
     def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_template_actions)
         """
-
     def list_waves(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
-
-    def mark_as_archived(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+    def mark_as_archived(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#mark_as_archived)
         """
+    def pause_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Pause Replication.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#pause_replication)
+        """
     def put_source_server_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         order: int,
         sourceServerID: str,
+        accountID: str = ...,
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
@@ -633,15 +632,14 @@
     ) -> SourceServerActionDocumentResponseMetadataTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
-
     def put_template_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         launchConfigurationTemplateID: str,
@@ -658,153 +656,165 @@
     ) -> TemplateActionDocumentResponseMetadataTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
-
-    def remove_source_server_action(self, *, actionID: str, sourceServerID: str) -> Dict[str, Any]:
+    def remove_source_server_action(
+        self, *, actionID: str, sourceServerID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Remove source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_source_server_action)
         """
-
     def remove_template_action(
         self, *, actionID: str, launchConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Remove template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_template_action)
         """
+    def resume_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Resume Replication.
 
-    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#resume_replication)
+        """
+    def retry_data_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#retry_data_replication)
         """
-
     def start_cutover(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartCutoverResponseTypeDef:
         """
         Launches a Cutover Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_cutover)
         """
-
     def start_export(
         self, *, s3Bucket: str, s3Key: str, s3BucketOwner: str = ...
     ) -> StartExportResponseTypeDef:
         """
         Start export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_export)
         """
-
     def start_import(
         self, *, s3BucketSource: S3BucketSourceTypeDef, clientToken: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Start import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_import)
         """
-
-    def start_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+    def start_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_replication)
         """
-
     def start_test(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartTestResponseTypeDef:
         """
         Launches a Test Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_test)
         """
+    def stop_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Stop Replication.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#stop_replication)
+        """
     def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Application
         Migration Service resource or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#tag_resource)
         """
-
     def terminate_target_instances(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> TerminateTargetInstancesResponseTypeDef:
         """
         Starts a job that terminates specific launched EC2 Test and Cutover instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#terminate_target_instances)
         """
-
-    def unarchive_application(self, *, applicationID: str) -> ApplicationResponseMetadataTypeDef:
+    def unarchive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseMetadataTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_application)
         """
-
-    def unarchive_wave(self, *, waveID: str) -> WaveResponseMetadataTypeDef:
+    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_wave)
         """
-
     def untag_resource(
         self, *, resourceArn: str, tagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified set of tags from the specified set of Application
         Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#untag_resource)
         """
-
     def update_application(
-        self, *, applicationID: str, description: str = ..., name: str = ...
+        self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> ApplicationResponseMetadataTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_application)
         """
-
     def update_launch_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
@@ -814,15 +824,14 @@
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
         """
-
     def update_launch_configuration_template(
         self,
         *,
         launchConfigurationTemplateID: str,
         associatePublicIpAddress: bool = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
@@ -839,41 +848,41 @@
     ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
-
     def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration)
         """
-
     def update_replication_configuration_template(
         self,
         *,
         replicationConfigurationTemplateID: str,
         arn: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
@@ -882,154 +891,147 @@
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
-
     def update_source_server_replication_type(
-        self, *, replicationType: ReplicationTypeType, sourceServerID: str
+        self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server_replication_type)
         """
-
     def update_wave(
-        self, *, waveID: str, description: str = ..., name: str = ...
+        self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> WaveResponseMetadataTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_wave)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_log_items"]
     ) -> DescribeJobLogItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["describe_jobs"]) -> DescribeJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_launch_configuration_templates"]
     ) -> DescribeLaunchConfigurationTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_replication_configuration_templates"]
     ) -> DescribeReplicationConfigurationTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_source_servers"]
     ) -> DescribeSourceServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_vcenter_clients"]
     ) -> DescribeVcenterClientsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_export_errors"]
     ) -> ListExportErrorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_exports"]) -> ListExportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_import_errors"]
     ) -> ListImportErrorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_imports"]) -> ListImportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_managed_accounts"]
+    ) -> ListManagedAccountsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_source_server_actions"]
     ) -> ListSourceServerActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_template_actions"]
     ) -> ListTemplateActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_waves"]) -> ListWavesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
     ApplicationResponseMetadataTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
@@ -64,14 +65,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
@@ -94,34 +96,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("mgnClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UninitializedAccountException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class mgnClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/)
     """
 
     meta: ClientMeta
@@ -130,82 +136,99 @@
     def exceptions(self) -> Exceptions:
         """
         mgnClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#exceptions)
         """
-    def archive_application(self, *, applicationID: str) -> ApplicationResponseMetadataTypeDef:
+
+    def archive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseMetadataTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_application)
         """
-    def archive_wave(self, *, waveID: str) -> WaveResponseMetadataTypeDef:
+
+    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_wave)
         """
+
     def associate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate applications to wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#associate_applications)
         """
+
     def associate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate source servers to application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#associate_source_servers)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#can_paginate)
         """
+
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
-        sourceServerID: str
+        sourceServerID: str,
+        accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#change_server_life_cycle_state)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#close)
         """
+
     def create_application(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> ApplicationResponseMetadataTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
+
     def create_launch_configuration_template(
         self,
         *,
         associatePublicIpAddress: bool = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
@@ -222,14 +245,15 @@
     ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
+
     def create_replication_configuration_template(
         self,
         *,
         associateDefaultSecurityGroup: bool,
         bandwidthThrottling: int,
         createPublicIP: bool,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType,
@@ -237,107 +261,125 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
+
     def create_wave(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> WaveResponseMetadataTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
-    def delete_application(self, *, applicationID: str) -> Dict[str, Any]:
+
+    def delete_application(self, *, applicationID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_application)
         """
-    def delete_job(self, *, jobID: str) -> Dict[str, Any]:
+
+    def delete_job(self, *, jobID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_job)
         """
+
     def delete_launch_configuration_template(
         self, *, launchConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Deletes a single Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_launch_configuration_template)
         """
+
     def delete_replication_configuration_template(
         self, *, replicationConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_replication_configuration_template)
         """
-    def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
+
+    def delete_source_server(self, *, sourceServerID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single source server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_source_server)
         """
+
     def delete_vcenter_client(self, *, vcenterClientID: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a given vCenter client by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_vcenter_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_vcenter_client)
         """
-    def delete_wave(self, *, waveID: str) -> Dict[str, Any]:
+
+    def delete_wave(self, *, waveID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#delete_wave)
         """
+
     def describe_job_log_items(
-        self, *, jobID: str, maxResults: int = ..., nextToken: str = ...
+        self, *, jobID: str, accountID: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobLogItemsResponseTypeDef:
         """
         Retrieves detailed job log items with paging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_job_log_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_job_log_items)
         """
+
     def describe_jobs(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_jobs)
         """
+
     def describe_launch_configuration_templates(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeLaunchConfigurationTemplatesResponseTypeDef:
@@ -345,240 +387,293 @@
         Lists all Launch Configuration Templates, filtered by Launch Configuration
         Template IDs See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DescribeLaunchConfigurationTemplates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_launch_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_launch_configuration_templates)
         """
+
     def describe_replication_configuration_templates(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         replicationConfigurationTemplateIDs: Sequence[str] = ...
     ) -> DescribeReplicationConfigurationTemplatesResponseTypeDef:
         """
         Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_replication_configuration_templates)
         """
+
     def describe_source_servers(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_source_servers)
         """
+
     def describe_vcenter_clients(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeVcenterClientsResponseTypeDef:
         """
         Returns a list of the installed vCenter clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_vcenter_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#describe_vcenter_clients)
         """
+
     def disassociate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate applications from wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_applications)
         """
+
     def disassociate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate source servers from application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_source_servers)
         """
+
     def disconnect_from_service(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disconnect_from_service)
         """
-    def finalize_cutover(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+
+    def finalize_cutover(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#finalize_cutover)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#generate_presigned_url)
         """
-    def get_launch_configuration(self, *, sourceServerID: str) -> LaunchConfigurationTypeDef:
+
+    def get_launch_configuration(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> LaunchConfigurationTypeDef:
         """
         Lists all LaunchConfigurations available, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_launch_configuration)
         """
+
     def get_replication_configuration(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Lists all ReplicationConfigurations, filtered by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_replication_configuration)
         """
+
     def initialize_service(self) -> Dict[str, Any]:
         """
         Initialize Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.initialize_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#initialize_service)
         """
+
     def list_applications(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_applications)
         """
+
     def list_export_errors(
         self, *, exportID: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListExportErrorsResponseTypeDef:
         """
         List export errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_export_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_export_errors)
         """
+
     def list_exports(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListExportsResponseTypeDef:
         """
         List exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_exports)
         """
+
     def list_import_errors(
         self, *, importID: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListImportErrorsResponseTypeDef:
         """
         List import errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_import_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_import_errors)
         """
+
     def list_imports(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_imports)
         """
+
+    def list_managed_accounts(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListManagedAccountsResponseTypeDef:
+        """
+        List Managed Accounts.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_managed_accounts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_managed_accounts)
+        """
+
     def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_source_server_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_source_server_actions)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List all tags for your Application Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_tags_for_resource)
         """
+
     def list_template_actions(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTemplateActionsResponseTypeDef:
         """
         List template post migration custom actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_template_actions)
         """
+
     def list_waves(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
-    def mark_as_archived(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+
+    def mark_as_archived(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#mark_as_archived)
         """
+
+    def pause_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Pause Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#pause_replication)
+        """
+
     def put_source_server_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         order: int,
         sourceServerID: str,
+        accountID: str = ...,
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
@@ -586,14 +681,15 @@
     ) -> SourceServerActionDocumentResponseMetadataTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
+
     def put_template_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         launchConfigurationTemplateID: str,
@@ -610,138 +706,182 @@
     ) -> TemplateActionDocumentResponseMetadataTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
-    def remove_source_server_action(self, *, actionID: str, sourceServerID: str) -> Dict[str, Any]:
+
+    def remove_source_server_action(
+        self, *, actionID: str, sourceServerID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Remove source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_source_server_action)
         """
+
     def remove_template_action(
         self, *, actionID: str, launchConfigurationTemplateID: str
     ) -> Dict[str, Any]:
         """
         Remove template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_template_action)
         """
-    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+
+    def resume_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Resume Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#resume_replication)
+        """
+
+    def retry_data_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#retry_data_replication)
         """
+
     def start_cutover(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartCutoverResponseTypeDef:
         """
         Launches a Cutover Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_cutover)
         """
+
     def start_export(
         self, *, s3Bucket: str, s3Key: str, s3BucketOwner: str = ...
     ) -> StartExportResponseTypeDef:
         """
         Start export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_export)
         """
+
     def start_import(
         self, *, s3BucketSource: S3BucketSourceTypeDef, clientToken: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Start import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_import)
         """
-    def start_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+
+    def start_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_replication)
         """
+
     def start_test(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartTestResponseTypeDef:
         """
         Launches a Test Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_test)
         """
+
+    def stop_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseMetadataTypeDef:
+        """
+        Stop Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#stop_replication)
+        """
+
     def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Application
         Migration Service resource or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#tag_resource)
         """
+
     def terminate_target_instances(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> TerminateTargetInstancesResponseTypeDef:
         """
         Starts a job that terminates specific launched EC2 Test and Cutover instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#terminate_target_instances)
         """
-    def unarchive_application(self, *, applicationID: str) -> ApplicationResponseMetadataTypeDef:
+
+    def unarchive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseMetadataTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_application)
         """
-    def unarchive_wave(self, *, waveID: str) -> WaveResponseMetadataTypeDef:
+
+    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_wave)
         """
+
     def untag_resource(
         self, *, resourceArn: str, tagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified set of tags from the specified set of Application
         Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#untag_resource)
         """
+
     def update_application(
-        self, *, applicationID: str, description: str = ..., name: str = ...
+        self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> ApplicationResponseMetadataTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_application)
         """
+
     def update_launch_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
@@ -751,14 +891,15 @@
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
         """
+
     def update_launch_configuration_template(
         self,
         *,
         launchConfigurationTemplateID: str,
         associatePublicIpAddress: bool = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
@@ -775,39 +916,43 @@
     ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
+
     def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration)
         """
+
     def update_replication_configuration_template(
         self,
         *,
         replicationConfigurationTemplateID: str,
         arn: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
@@ -816,138 +961,164 @@
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
+
     def update_source_server_replication_type(
-        self, *, replicationType: ReplicationTypeType, sourceServerID: str
+        self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseMetadataTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server_replication_type)
         """
+
     def update_wave(
-        self, *, waveID: str, description: str = ..., name: str = ...
+        self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> WaveResponseMetadataTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_wave)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_log_items"]
     ) -> DescribeJobLogItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["describe_jobs"]) -> DescribeJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_launch_configuration_templates"]
     ) -> DescribeLaunchConfigurationTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_replication_configuration_templates"]
     ) -> DescribeReplicationConfigurationTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_source_servers"]
     ) -> DescribeSourceServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_vcenter_clients"]
     ) -> DescribeVcenterClientsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_export_errors"]
     ) -> ListExportErrorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_exports"]) -> ListExportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_import_errors"]
     ) -> ListImportErrorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_imports"]) -> ListImportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_managed_accounts"]
+    ) -> ListManagedAccountsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_source_server_actions"]
     ) -> ListSourceServerActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_template_actions"]
     ) -> ListTemplateActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_waves"]) -> ListWavesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "LaunchStatusType",
     "LifeCycleStateType",
     "ListApplicationsPaginatorName",
     "ListExportErrorsPaginatorName",
     "ListExportsPaginatorName",
     "ListImportErrorsPaginatorName",
     "ListImportsPaginatorName",
+    "ListManagedAccountsPaginatorName",
     "ListSourceServerActionsPaginatorName",
     "ListTemplateActionsPaginatorName",
     "ListWavesPaginatorName",
     "PostLaunchActionExecutionStatusType",
     "PostLaunchActionsDeploymentTypeType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
@@ -191,14 +192,15 @@
     "TESTING",
 ]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListExportErrorsPaginatorName = Literal["list_export_errors"]
 ListExportsPaginatorName = Literal["list_exports"]
 ListImportErrorsPaginatorName = Literal["list_import_errors"]
 ListImportsPaginatorName = Literal["list_imports"]
+ListManagedAccountsPaginatorName = Literal["list_managed_accounts"]
 ListSourceServerActionsPaginatorName = Literal["list_source_server_actions"]
 ListTemplateActionsPaginatorName = Literal["list_template_actions"]
 ListWavesPaginatorName = Literal["list_waves"]
 PostLaunchActionExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 PostLaunchActionsDeploymentTypeType = Literal["CUTOVER_ONLY", "TEST_AND_CUTOVER", "TEST_ONLY"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["GP2", "GP3", "ST1"]
@@ -586,14 +588,15 @@
     "describe_source_servers",
     "describe_vcenter_clients",
     "list_applications",
     "list_export_errors",
     "list_exports",
     "list_import_errors",
     "list_imports",
+    "list_managed_accounts",
     "list_source_server_actions",
     "list_template_actions",
     "list_waves",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "LaunchStatusType",
     "LifeCycleStateType",
     "ListApplicationsPaginatorName",
     "ListExportErrorsPaginatorName",
     "ListExportsPaginatorName",
     "ListImportErrorsPaginatorName",
     "ListImportsPaginatorName",
+    "ListManagedAccountsPaginatorName",
     "ListSourceServerActionsPaginatorName",
     "ListTemplateActionsPaginatorName",
     "ListWavesPaginatorName",
     "PostLaunchActionExecutionStatusType",
     "PostLaunchActionsDeploymentTypeType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
@@ -189,14 +190,15 @@
     "TESTING",
 ]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListExportErrorsPaginatorName = Literal["list_export_errors"]
 ListExportsPaginatorName = Literal["list_exports"]
 ListImportErrorsPaginatorName = Literal["list_import_errors"]
 ListImportsPaginatorName = Literal["list_imports"]
+ListManagedAccountsPaginatorName = Literal["list_managed_accounts"]
 ListSourceServerActionsPaginatorName = Literal["list_source_server_actions"]
 ListTemplateActionsPaginatorName = Literal["list_template_actions"]
 ListWavesPaginatorName = Literal["list_waves"]
 PostLaunchActionExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 PostLaunchActionsDeploymentTypeType = Literal["CUTOVER_ONLY", "TEST_AND_CUTOVER", "TEST_ONLY"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["GP2", "GP3", "ST1"]
@@ -584,14 +586,15 @@
     "describe_source_servers",
     "describe_vcenter_clients",
     "list_applications",
     "list_export_errors",
     "list_exports",
     "list_import_errors",
     "list_imports",
+    "list_managed_accounts",
     "list_source_server_actions",
     "list_template_actions",
     "list_waves",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
     )
 
     session = Session()
     client: mgnClient = session.client("mgn")
@@ -36,14 +37,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
@@ -62,14 +64,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PaginatorConfigTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     TemplateActionsRequestFiltersTypeDef,
@@ -83,14 +86,15 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -106,15 +110,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -123,14 +127,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
@@ -177,14 +182,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
@@ -210,14 +216,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
@@ -285,24 +292,40 @@
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 
+class ListManagedAccountsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListManagedAccountsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
+        """
+
+
 class ListSourceServerActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
@@ -332,14 +355,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
     )
 
     session = Session()
     client: mgnClient = session.client("mgn")
@@ -36,14 +37,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
@@ -62,14 +64,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PaginatorConfigTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     TemplateActionsRequestFiltersTypeDef,
@@ -83,14 +86,15 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -103,15 +107,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(Paginator):
@@ -119,14 +123,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
@@ -170,14 +175,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
@@ -201,14 +207,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
@@ -271,24 +278,39 @@
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
+class ListManagedAccountsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListManagedAccountsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
+        """
+
 class ListSourceServerActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
@@ -316,14 +338,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,35 +121,41 @@
     "ListApplicationsRequestFiltersTypeDef",
     "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
     "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    "ListManagedAccountsRequestRequestTypeDef",
+    "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
     "PaginatorConfigTypeDef",
+    "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ResponseMetadataTypeDef",
+    "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
+    "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
     "UnarchiveApplicationRequestRequestTypeDef",
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
@@ -176,14 +182,15 @@
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListManagedAccountsResponseTypeDef",
     "ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     "ListSourceServerActionsRequestRequestTypeDef",
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
@@ -240,43 +247,102 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
     },
     total=False,
 )
 
-ArchiveApplicationRequestRequestTypeDef = TypedDict(
-    "ArchiveApplicationRequestRequestTypeDef",
+_RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ArchiveApplicationRequestRequestTypeDef(
+    _RequiredArchiveApplicationRequestRequestTypeDef,
+    _OptionalArchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
 
-ArchiveWaveRequestRequestTypeDef = TypedDict(
-    "ArchiveWaveRequestRequestTypeDef",
+_RequiredArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ArchiveWaveRequestRequestTypeDef(
+    _RequiredArchiveWaveRequestRequestTypeDef, _OptionalArchiveWaveRequestRequestTypeDef
+):
+    pass
 
-AssociateApplicationsRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationsRequestRequestTypeDef",
+
+_RequiredAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class AssociateApplicationsRequestRequestTypeDef(
+    _RequiredAssociateApplicationsRequestRequestTypeDef,
+    _OptionalAssociateApplicationsRequestRequestTypeDef,
+):
+    pass
 
-AssociateSourceServersRequestRequestTypeDef = TypedDict(
-    "AssociateSourceServersRequestRequestTypeDef",
+
+_RequiredAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class AssociateSourceServersRequestRequestTypeDef(
+    _RequiredAssociateSourceServersRequestRequestTypeDef,
+    _OptionalAssociateSourceServersRequestRequestTypeDef,
+):
+    pass
+
 
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
@@ -295,14 +361,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -347,14 +414,15 @@
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -368,14 +436,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -411,27 +480,55 @@
     {
         "name": DataReplicationInitiationStepNameType,
         "status": DataReplicationInitiationStepStatusType,
     },
     total=False,
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
+_RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
 
-DeleteJobRequestRequestTypeDef = TypedDict(
-    "DeleteJobRequestRequestTypeDef",
+class DeleteApplicationRequestRequestTypeDef(
+    _RequiredDeleteApplicationRequestRequestTypeDef, _OptionalDeleteApplicationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDeleteJobRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
+_OptionalDeleteJobRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteJobRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteJobRequestRequestTypeDef(
+    _RequiredDeleteJobRequestRequestTypeDef, _OptionalDeleteJobRequestRequestTypeDef
+):
+    pass
+
 
 DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
@@ -439,44 +536,74 @@
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
-DeleteSourceServerRequestRequestTypeDef = TypedDict(
-    "DeleteSourceServerRequestRequestTypeDef",
+_RequiredDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteSourceServerRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteSourceServerRequestRequestTypeDef(
+    _RequiredDeleteSourceServerRequestRequestTypeDef,
+    _OptionalDeleteSourceServerRequestRequestTypeDef,
+):
+    pass
+
 
 DeleteVcenterClientRequestRequestTypeDef = TypedDict(
     "DeleteVcenterClientRequestRequestTypeDef",
     {
         "vcenterClientID": str,
     },
 )
 
-DeleteWaveRequestRequestTypeDef = TypedDict(
-    "DeleteWaveRequestRequestTypeDef",
+_RequiredDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteWaveRequestRequestTypeDef(
+    _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
+        "accountID": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
@@ -491,14 +618,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestRequestTypeDef",
     {
+        "accountID": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 
@@ -576,14 +704,15 @@
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class ReplicationConfigurationTemplateTypeDef(
     _RequiredReplicationConfigurationTemplateTypeDef,
@@ -632,36 +761,81 @@
         "tags": Dict[str, str],
         "vcenterClientID": str,
         "vcenterUUID": str,
     },
     total=False,
 )
 
-DisassociateApplicationsRequestRequestTypeDef = TypedDict(
-    "DisassociateApplicationsRequestRequestTypeDef",
+_RequiredDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
 
-DisassociateSourceServersRequestRequestTypeDef = TypedDict(
-    "DisassociateSourceServersRequestRequestTypeDef",
+class DisassociateApplicationsRequestRequestTypeDef(
+    _RequiredDisassociateApplicationsRequestRequestTypeDef,
+    _OptionalDisassociateApplicationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DisconnectFromServiceRequestRequestTypeDef = TypedDict(
-    "DisconnectFromServiceRequestRequestTypeDef",
+
+class DisassociateSourceServersRequestRequestTypeDef(
+    _RequiredDisassociateSourceServersRequestRequestTypeDef,
+    _OptionalDisassociateSourceServersRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredDisconnectFromServiceRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalDisconnectFromServiceRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DisconnectFromServiceRequestRequestTypeDef(
+    _RequiredDisconnectFromServiceRequestRequestTypeDef,
+    _OptionalDisconnectFromServiceRequestRequestTypeDef,
+):
+    pass
+
 
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "bytes": int,
         "deviceName": str,
     },
@@ -689,34 +863,78 @@
         "applicationsCount": int,
         "serversCount": int,
         "wavesCount": int,
     },
     total=False,
 )
 
-FinalizeCutoverRequestRequestTypeDef = TypedDict(
-    "FinalizeCutoverRequestRequestTypeDef",
+_RequiredFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_RequiredFinalizeCutoverRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_OptionalFinalizeCutoverRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class FinalizeCutoverRequestRequestTypeDef(
+    _RequiredFinalizeCutoverRequestRequestTypeDef, _OptionalFinalizeCutoverRequestRequestTypeDef
+):
+    pass
 
-GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "GetLaunchConfigurationRequestRequestTypeDef",
+
+_RequiredGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class GetLaunchConfigurationRequestRequestTypeDef(
+    _RequiredGetLaunchConfigurationRequestRequestTypeDef,
+    _OptionalGetLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
-GetReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetReplicationConfigurationRequestRequestTypeDef",
+_RequiredGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class GetReplicationConfigurationRequestRequestTypeDef(
+    _RequiredGetReplicationConfigurationRequestRequestTypeDef,
+    _OptionalGetReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
 IdentificationHintsTypeDef = TypedDict(
     "IdentificationHintsTypeDef",
     {
         "awsInstanceID": str,
         "fqdn": str,
         "hostname": str,
@@ -725,14 +943,15 @@
     },
     total=False,
 )
 
 ImportErrorDataTypeDef = TypedDict(
     "ImportErrorDataTypeDef",
     {
+        "accountID": str,
         "applicationID": str,
         "ec2LaunchTemplateID": str,
         "rawError": str,
         "rowNumber": int,
         "sourceServerID": str,
         "waveID": str,
     },
@@ -967,14 +1186,39 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListManagedAccountsRequestRequestTypeDef = TypedDict(
+    "ListManagedAccountsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ManagedAccountTypeDef = TypedDict(
+    "ManagedAccountTypeDef",
+    {
+        "accountId": str,
+    },
+    total=False,
+)
+
 SourceServerActionsRequestFiltersTypeDef = TypedDict(
     "SourceServerActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -1007,20 +1251,34 @@
     {
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-MarkAsArchivedRequestRequestTypeDef = TypedDict(
-    "MarkAsArchivedRequestRequestTypeDef",
+_RequiredMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_RequiredMarkAsArchivedRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_OptionalMarkAsArchivedRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class MarkAsArchivedRequestRequestTypeDef(
+    _RequiredMarkAsArchivedRequestRequestTypeDef, _OptionalMarkAsArchivedRequestRequestTypeDef
+):
+    pass
+
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
@@ -1042,14 +1300,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredPauseReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalPauseReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class PauseReplicationRequestRequestTypeDef(
+    _RequiredPauseReplicationRequestRequestTypeDef, _OptionalPauseReplicationRequestRequestTypeDef
+):
+    pass
+
+
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -1058,21 +1337,36 @@
     "SsmParameterStoreParameterTypeDef",
     {
         "parameterName": str,
         "parameterType": Literal["STRING"],
     },
 )
 
-RemoveSourceServerActionRequestRequestTypeDef = TypedDict(
-    "RemoveSourceServerActionRequestRequestTypeDef",
+_RequiredRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_RequiredRemoveSourceServerActionRequestRequestTypeDef",
     {
         "actionID": str,
         "sourceServerID": str,
     },
 )
+_OptionalRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_OptionalRemoveSourceServerActionRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class RemoveSourceServerActionRequestRequestTypeDef(
+    _RequiredRemoveSourceServerActionRequestRequestTypeDef,
+    _OptionalRemoveSourceServerActionRequestRequestTypeDef,
+):
+    pass
+
 
 RemoveTemplateActionRequestRequestTypeDef = TypedDict(
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
@@ -1104,14 +1398,15 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -1119,30 +1414,67 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RetryDataReplicationRequestRequestTypeDef = TypedDict(
-    "RetryDataReplicationRequestRequestTypeDef",
+_RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredResumeReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalResumeReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ResumeReplicationRequestRequestTypeDef(
+    _RequiredResumeReplicationRequestRequestTypeDef, _OptionalResumeReplicationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredRetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalRetryDataReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class RetryDataReplicationRequestRequestTypeDef(
+    _RequiredRetryDataReplicationRequestRequestTypeDef,
+    _OptionalRetryDataReplicationRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
     "_OptionalStartCutoverRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class StartCutoverRequestRequestTypeDef(
@@ -1169,42 +1501,78 @@
 
 class StartExportRequestRequestTypeDef(
     _RequiredStartExportRequestRequestTypeDef, _OptionalStartExportRequestRequestTypeDef
 ):
     pass
 
 
-StartReplicationRequestRequestTypeDef = TypedDict(
-    "StartReplicationRequestRequestTypeDef",
+_RequiredStartReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalStartReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class StartReplicationRequestRequestTypeDef(
+    _RequiredStartReplicationRequestRequestTypeDef, _OptionalStartReplicationRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredStartTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartTestRequestRequestTypeDef = TypedDict(
     "_OptionalStartTestRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class StartTestRequestRequestTypeDef(
     _RequiredStartTestRequestRequestTypeDef, _OptionalStartTestRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredStopReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStopReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalStopReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStopReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class StopReplicationRequestRequestTypeDef(
+    _RequiredStopReplicationRequestRequestTypeDef, _OptionalStopReplicationRequestRequestTypeDef
+):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1214,40 +1582,70 @@
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalTerminateTargetInstancesRequestRequestTypeDef = TypedDict(
     "_OptionalTerminateTargetInstancesRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class TerminateTargetInstancesRequestRequestTypeDef(
     _RequiredTerminateTargetInstancesRequestRequestTypeDef,
     _OptionalTerminateTargetInstancesRequestRequestTypeDef,
 ):
     pass
 
 
-UnarchiveApplicationRequestRequestTypeDef = TypedDict(
-    "UnarchiveApplicationRequestRequestTypeDef",
+_RequiredUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-UnarchiveWaveRequestRequestTypeDef = TypedDict(
-    "UnarchiveWaveRequestRequestTypeDef",
+
+class UnarchiveApplicationRequestRequestTypeDef(
+    _RequiredUnarchiveApplicationRequestRequestTypeDef,
+    _OptionalUnarchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class UnarchiveWaveRequestRequestTypeDef(
+    _RequiredUnarchiveWaveRequestRequestTypeDef, _OptionalUnarchiveWaveRequestRequestTypeDef
+):
+    pass
+
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -1258,14 +1656,15 @@
     {
         "applicationID": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 
@@ -1293,43 +1692,60 @@
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
-    "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
+_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef",
     {
         "replicationType": ReplicationTypeType,
         "sourceServerID": str,
     },
 )
+_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class UpdateSourceServerReplicationTypeRequestRequestTypeDef(
+    _RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+    _OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredUpdateWaveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 _OptionalUpdateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 
@@ -1381,44 +1797,61 @@
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
     },
     total=False,
 )
 
-ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
-    "ChangeServerLifeCycleStateRequestRequestTypeDef",
+_RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
     },
 )
+_OptionalChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_OptionalChangeServerLifeCycleStateRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ChangeServerLifeCycleStateRequestRequestTypeDef(
+    _RequiredChangeServerLifeCycleStateRequestRequestTypeDef,
+    _OptionalChangeServerLifeCycleStateRequestRequestTypeDef,
+):
+    pass
+
 
 DataReplicationInitiationTypeDef = TypedDict(
     "DataReplicationInitiationTypeDef",
     {
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1430,23 +1863,25 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1554,23 +1989,25 @@
     },
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1608,23 +2045,33 @@
         "filters": ListImportsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListManagedAccountsResponseTypeDef = TypedDict(
+    "ListManagedAccountsResponseTypeDef",
+    {
+        "items": List[ManagedAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
@@ -1640,14 +2087,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestRequestTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1705,23 +2153,25 @@
 ):
     pass
 
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1749,14 +2199,15 @@
         "order": int,
         "sourceServerID": str,
     },
 )
 _OptionalPutSourceServerActionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSourceServerActionRequestRequestTypeDef",
     {
+        "accountID": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentVersion": str,
         "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
@@ -1921,41 +2372,44 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
         "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class UpdateReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
@@ -2313,14 +2767,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -120,35 +120,41 @@
     "ListApplicationsRequestFiltersTypeDef",
     "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
     "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    "ListManagedAccountsRequestRequestTypeDef",
+    "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
     "PaginatorConfigTypeDef",
+    "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ResponseMetadataTypeDef",
+    "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
+    "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
     "UnarchiveApplicationRequestRequestTypeDef",
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
@@ -175,14 +181,15 @@
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListManagedAccountsResponseTypeDef",
     "ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     "ListSourceServerActionsRequestRequestTypeDef",
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
@@ -239,43 +246,94 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
     },
     total=False,
 )
 
-ArchiveApplicationRequestRequestTypeDef = TypedDict(
-    "ArchiveApplicationRequestRequestTypeDef",
+_RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ArchiveApplicationRequestRequestTypeDef(
+    _RequiredArchiveApplicationRequestRequestTypeDef,
+    _OptionalArchiveApplicationRequestRequestTypeDef,
+):
+    pass
 
-ArchiveWaveRequestRequestTypeDef = TypedDict(
-    "ArchiveWaveRequestRequestTypeDef",
+_RequiredArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ArchiveWaveRequestRequestTypeDef(
+    _RequiredArchiveWaveRequestRequestTypeDef, _OptionalArchiveWaveRequestRequestTypeDef
+):
+    pass
 
-AssociateApplicationsRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationsRequestRequestTypeDef",
+_RequiredAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class AssociateApplicationsRequestRequestTypeDef(
+    _RequiredAssociateApplicationsRequestRequestTypeDef,
+    _OptionalAssociateApplicationsRequestRequestTypeDef,
+):
+    pass
 
-AssociateSourceServersRequestRequestTypeDef = TypedDict(
-    "AssociateSourceServersRequestRequestTypeDef",
+_RequiredAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class AssociateSourceServersRequestRequestTypeDef(
+    _RequiredAssociateSourceServersRequestRequestTypeDef,
+    _OptionalAssociateSourceServersRequestRequestTypeDef,
+):
+    pass
 
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
@@ -294,14 +352,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateApplicationRequestRequestTypeDef(
@@ -344,14 +403,15 @@
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -363,14 +423,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateWaveRequestRequestTypeDef(
@@ -404,27 +465,51 @@
     {
         "name": DataReplicationInitiationStepNameType,
         "status": DataReplicationInitiationStepStatusType,
     },
     total=False,
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
+_RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteApplicationRequestRequestTypeDef(
+    _RequiredDeleteApplicationRequestRequestTypeDef, _OptionalDeleteApplicationRequestRequestTypeDef
+):
+    pass
 
-DeleteJobRequestRequestTypeDef = TypedDict(
-    "DeleteJobRequestRequestTypeDef",
+_RequiredDeleteJobRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
+_OptionalDeleteJobRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteJobRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteJobRequestRequestTypeDef(
+    _RequiredDeleteJobRequestRequestTypeDef, _OptionalDeleteJobRequestRequestTypeDef
+):
+    pass
 
 DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
@@ -432,44 +517,70 @@
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
-DeleteSourceServerRequestRequestTypeDef = TypedDict(
-    "DeleteSourceServerRequestRequestTypeDef",
+_RequiredDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteSourceServerRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteSourceServerRequestRequestTypeDef(
+    _RequiredDeleteSourceServerRequestRequestTypeDef,
+    _OptionalDeleteSourceServerRequestRequestTypeDef,
+):
+    pass
 
 DeleteVcenterClientRequestRequestTypeDef = TypedDict(
     "DeleteVcenterClientRequestRequestTypeDef",
     {
         "vcenterClientID": str,
     },
 )
 
-DeleteWaveRequestRequestTypeDef = TypedDict(
-    "DeleteWaveRequestRequestTypeDef",
+_RequiredDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteWaveRequestRequestTypeDef(
+    _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
+):
+    pass
 
 _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
+        "accountID": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
     _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
@@ -482,14 +593,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestRequestTypeDef",
     {
+        "accountID": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 class DescribeJobLogItemsRequestRequestTypeDef(
@@ -565,14 +677,15 @@
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class ReplicationConfigurationTemplateTypeDef(
     _RequiredReplicationConfigurationTemplateTypeDef,
     _OptionalReplicationConfigurationTemplateTypeDef,
@@ -619,36 +732,75 @@
         "tags": Dict[str, str],
         "vcenterClientID": str,
         "vcenterUUID": str,
     },
     total=False,
 )
 
-DisassociateApplicationsRequestRequestTypeDef = TypedDict(
-    "DisassociateApplicationsRequestRequestTypeDef",
+_RequiredDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DisassociateApplicationsRequestRequestTypeDef(
+    _RequiredDisassociateApplicationsRequestRequestTypeDef,
+    _OptionalDisassociateApplicationsRequestRequestTypeDef,
+):
+    pass
 
-DisassociateSourceServersRequestRequestTypeDef = TypedDict(
-    "DisassociateSourceServersRequestRequestTypeDef",
+_RequiredDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DisassociateSourceServersRequestRequestTypeDef(
+    _RequiredDisassociateSourceServersRequestRequestTypeDef,
+    _OptionalDisassociateSourceServersRequestRequestTypeDef,
+):
+    pass
 
-DisconnectFromServiceRequestRequestTypeDef = TypedDict(
-    "DisconnectFromServiceRequestRequestTypeDef",
+_RequiredDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredDisconnectFromServiceRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalDisconnectFromServiceRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DisconnectFromServiceRequestRequestTypeDef(
+    _RequiredDisconnectFromServiceRequestRequestTypeDef,
+    _OptionalDisconnectFromServiceRequestRequestTypeDef,
+):
+    pass
 
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "bytes": int,
         "deviceName": str,
     },
@@ -676,34 +828,72 @@
         "applicationsCount": int,
         "serversCount": int,
         "wavesCount": int,
     },
     total=False,
 )
 
-FinalizeCutoverRequestRequestTypeDef = TypedDict(
-    "FinalizeCutoverRequestRequestTypeDef",
+_RequiredFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_RequiredFinalizeCutoverRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_OptionalFinalizeCutoverRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class FinalizeCutoverRequestRequestTypeDef(
+    _RequiredFinalizeCutoverRequestRequestTypeDef, _OptionalFinalizeCutoverRequestRequestTypeDef
+):
+    pass
 
-GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "GetLaunchConfigurationRequestRequestTypeDef",
+_RequiredGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class GetLaunchConfigurationRequestRequestTypeDef(
+    _RequiredGetLaunchConfigurationRequestRequestTypeDef,
+    _OptionalGetLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
 
-GetReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetReplicationConfigurationRequestRequestTypeDef",
+_RequiredGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class GetReplicationConfigurationRequestRequestTypeDef(
+    _RequiredGetReplicationConfigurationRequestRequestTypeDef,
+    _OptionalGetReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
 
 IdentificationHintsTypeDef = TypedDict(
     "IdentificationHintsTypeDef",
     {
         "awsInstanceID": str,
         "fqdn": str,
         "hostname": str,
@@ -712,14 +902,15 @@
     },
     total=False,
 )
 
 ImportErrorDataTypeDef = TypedDict(
     "ImportErrorDataTypeDef",
     {
+        "accountID": str,
         "applicationID": str,
         "ec2LaunchTemplateID": str,
         "rawError": str,
         "rowNumber": int,
         "sourceServerID": str,
         "waveID": str,
     },
@@ -944,14 +1135,39 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListManagedAccountsRequestRequestTypeDef = TypedDict(
+    "ListManagedAccountsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ManagedAccountTypeDef = TypedDict(
+    "ManagedAccountTypeDef",
+    {
+        "accountId": str,
+    },
+    total=False,
+)
+
 SourceServerActionsRequestFiltersTypeDef = TypedDict(
     "SourceServerActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -984,20 +1200,32 @@
     {
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-MarkAsArchivedRequestRequestTypeDef = TypedDict(
-    "MarkAsArchivedRequestRequestTypeDef",
+_RequiredMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_RequiredMarkAsArchivedRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_OptionalMarkAsArchivedRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class MarkAsArchivedRequestRequestTypeDef(
+    _RequiredMarkAsArchivedRequestRequestTypeDef, _OptionalMarkAsArchivedRequestRequestTypeDef
+):
+    pass
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
@@ -1019,14 +1247,33 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredPauseReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalPauseReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class PauseReplicationRequestRequestTypeDef(
+    _RequiredPauseReplicationRequestRequestTypeDef, _OptionalPauseReplicationRequestRequestTypeDef
+):
+    pass
+
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -1035,21 +1282,34 @@
     "SsmParameterStoreParameterTypeDef",
     {
         "parameterName": str,
         "parameterType": Literal["STRING"],
     },
 )
 
-RemoveSourceServerActionRequestRequestTypeDef = TypedDict(
-    "RemoveSourceServerActionRequestRequestTypeDef",
+_RequiredRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_RequiredRemoveSourceServerActionRequestRequestTypeDef",
     {
         "actionID": str,
         "sourceServerID": str,
     },
 )
+_OptionalRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_OptionalRemoveSourceServerActionRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class RemoveSourceServerActionRequestRequestTypeDef(
+    _RequiredRemoveSourceServerActionRequestRequestTypeDef,
+    _OptionalRemoveSourceServerActionRequestRequestTypeDef,
+):
+    pass
 
 RemoveTemplateActionRequestRequestTypeDef = TypedDict(
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
@@ -1081,14 +1341,15 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -1096,30 +1357,63 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RetryDataReplicationRequestRequestTypeDef = TypedDict(
-    "RetryDataReplicationRequestRequestTypeDef",
+_RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredResumeReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalResumeReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ResumeReplicationRequestRequestTypeDef(
+    _RequiredResumeReplicationRequestRequestTypeDef, _OptionalResumeReplicationRequestRequestTypeDef
+):
+    pass
+
+_RequiredRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredRetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalRetryDataReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class RetryDataReplicationRequestRequestTypeDef(
+    _RequiredRetryDataReplicationRequestRequestTypeDef,
+    _OptionalRetryDataReplicationRequestRequestTypeDef,
+):
+    pass
 
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
     "_OptionalStartCutoverRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartCutoverRequestRequestTypeDef(
     _RequiredStartCutoverRequestRequestTypeDef, _OptionalStartCutoverRequestRequestTypeDef
@@ -1142,40 +1436,72 @@
 )
 
 class StartExportRequestRequestTypeDef(
     _RequiredStartExportRequestRequestTypeDef, _OptionalStartExportRequestRequestTypeDef
 ):
     pass
 
-StartReplicationRequestRequestTypeDef = TypedDict(
-    "StartReplicationRequestRequestTypeDef",
+_RequiredStartReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalStartReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class StartReplicationRequestRequestTypeDef(
+    _RequiredStartReplicationRequestRequestTypeDef, _OptionalStartReplicationRequestRequestTypeDef
+):
+    pass
 
 _RequiredStartTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartTestRequestRequestTypeDef = TypedDict(
     "_OptionalStartTestRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartTestRequestRequestTypeDef(
     _RequiredStartTestRequestRequestTypeDef, _OptionalStartTestRequestRequestTypeDef
 ):
     pass
 
+_RequiredStopReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStopReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalStopReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStopReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class StopReplicationRequestRequestTypeDef(
+    _RequiredStopReplicationRequestRequestTypeDef, _OptionalStopReplicationRequestRequestTypeDef
+):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1185,38 +1511,64 @@
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalTerminateTargetInstancesRequestRequestTypeDef = TypedDict(
     "_OptionalTerminateTargetInstancesRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class TerminateTargetInstancesRequestRequestTypeDef(
     _RequiredTerminateTargetInstancesRequestRequestTypeDef,
     _OptionalTerminateTargetInstancesRequestRequestTypeDef,
 ):
     pass
 
-UnarchiveApplicationRequestRequestTypeDef = TypedDict(
-    "UnarchiveApplicationRequestRequestTypeDef",
+_RequiredUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-UnarchiveWaveRequestRequestTypeDef = TypedDict(
-    "UnarchiveWaveRequestRequestTypeDef",
+class UnarchiveApplicationRequestRequestTypeDef(
+    _RequiredUnarchiveApplicationRequestRequestTypeDef,
+    _OptionalUnarchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class UnarchiveWaveRequestRequestTypeDef(
+    _RequiredUnarchiveWaveRequestRequestTypeDef, _OptionalUnarchiveWaveRequestRequestTypeDef
+):
+    pass
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -1227,14 +1579,15 @@
     {
         "applicationID": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 class UpdateApplicationRequestRequestTypeDef(
@@ -1260,41 +1613,56 @@
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-UpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
-    "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
+_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef",
     {
         "replicationType": ReplicationTypeType,
         "sourceServerID": str,
     },
 )
+_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class UpdateSourceServerReplicationTypeRequestRequestTypeDef(
+    _RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+    _OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+):
+    pass
 
 _RequiredUpdateWaveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 _OptionalUpdateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 class UpdateWaveRequestRequestTypeDef(
@@ -1344,44 +1712,59 @@
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
     },
     total=False,
 )
 
-ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
-    "ChangeServerLifeCycleStateRequestRequestTypeDef",
+_RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
     },
 )
+_OptionalChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_OptionalChangeServerLifeCycleStateRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ChangeServerLifeCycleStateRequestRequestTypeDef(
+    _RequiredChangeServerLifeCycleStateRequestRequestTypeDef,
+    _OptionalChangeServerLifeCycleStateRequestRequestTypeDef,
+):
+    pass
 
 DataReplicationInitiationTypeDef = TypedDict(
     "DataReplicationInitiationTypeDef",
     {
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1393,23 +1776,25 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1515,23 +1900,25 @@
     },
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1569,23 +1956,33 @@
         "filters": ListImportsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListManagedAccountsResponseTypeDef = TypedDict(
+    "ListManagedAccountsResponseTypeDef",
+    {
+        "items": List[ManagedAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
@@ -1599,14 +1996,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestRequestTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1658,23 +2056,25 @@
     _OptionalListTemplateActionsRequestRequestTypeDef,
 ):
     pass
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1702,14 +2102,15 @@
         "order": int,
         "sourceServerID": str,
     },
 )
 _OptionalPutSourceServerActionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSourceServerActionRequestRequestTypeDef",
     {
+        "accountID": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentVersion": str,
         "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
@@ -1868,41 +2269,44 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
         "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class UpdateReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
@@ -2256,14 +2660,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.27.0
-Summary: Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.1
+Summary: Type annotations for boto3.mgn 1.27.1 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,14 +289,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 client: mgnClient = Session().client("mgn")
 
@@ -319,14 +320,17 @@
     "describe_vcenter_clients"
 )
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
 list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
 list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
 list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator(
+    "list_managed_accounts"
+)
 list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator(
     "list_source_server_actions"
 )
 list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator(
     "list_template_actions"
 )
 list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
@@ -368,14 +372,15 @@
     LaunchStatusType,
     LifeCycleStateType,
     ListApplicationsPaginatorName,
     ListExportErrorsPaginatorName,
     ListExportsPaginatorName,
     ListImportErrorsPaginatorName,
     ListImportsPaginatorName,
+    ListManagedAccountsPaginatorName,
     ListSourceServerActionsPaginatorName,
     ListTemplateActionsPaginatorName,
     ListWavesPaginatorName,
     PostLaunchActionExecutionStatusType,
     PostLaunchActionsDeploymentTypeType,
     ReplicationConfigurationDataPlaneRoutingType,
     ReplicationConfigurationDefaultLargeStagingDiskTypeType,
@@ -470,35 +475,41 @@
     ListApplicationsRequestFiltersTypeDef,
     ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
+    ListManagedAccountsRequestRequestTypeDef,
+    ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
     PaginatorConfigTypeDef,
+    PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
+    ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
+    StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
     UnarchiveApplicationRequestRequestTypeDef,
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -525,14 +536,15 @@
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
     ListSourceServerActionsRequestRequestTypeDef,
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
```

### Comparing `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.27.1/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.27.0/setup.py` & `mypy-boto3-mgn-1.27.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.27.0",
+    version="1.27.1",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.mgn 1.27.1 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

