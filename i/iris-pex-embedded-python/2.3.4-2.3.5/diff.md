# Comparing `tmp/iris_pex_embedded_python-2.3.4.tar.gz` & `tmp/iris_pex_embedded_python-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.4.tar", last modified: Fri Jun 16 16:07:39 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.5.tar", last modified: Wed Jul  5 11:46:47 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.4.tar` & `iris_pex_embedded_python-2.3.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:39.009221 iris_pex_embedded_python-2.3.4/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.4/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-16 16:07:39.008309 iris_pex_embedded_python-2.3.4/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.4/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.4/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-06-16 16:07:39.009491 iris_pex_embedded_python-2.3.4/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2322 2023-06-16 16:03:46.000000 iris_pex_embedded_python-2.3.4/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.923551 iris_pex_embedded_python-2.3.4/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.920246 iris_pex_embedded_python-2.3.4/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.959245 iris_pex_embedded_python-2.3.4/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-06-16 07:35:26.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112     5647 2023-06-16 15:49:29.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) 1252422112    15158 2023-06-15 13:47:53.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112    15066 2023-06-16 16:06:46.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.921263 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.982206 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/
--rw-r--r--   0 grongier (902446405) 1252422112      932 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessOperation.cls
--rw-r--r--   0 grongier (902446405) 1252422112     2633 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessProcess.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1039 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessService.cls
--rw-r--r--   0 grongier (902446405) 1252422112     3538 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Common.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1894 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Director.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.987563 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/
--rw-r--r--   0 grongier (902446405) 1252422112      543 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Operation.cls
--rw-r--r--   0 grongier (902446405) 1252422112     7103 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Process.cls
--rw-r--r--   0 grongier (902446405) 1252422112      179 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Service.cls
--rw-r--r--   0 grongier (902446405) 1252422112      628 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/InboundAdapter.cls
--rw-r--r--   0 grongier (902446405) 1252422112     8227 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Message.cls
--rw-r--r--   0 grongier (902446405) 1252422112      976 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/OutboundAdapter.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1691 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PickleMessage.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.989240 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/
--rw-r--r--   0 grongier (902446405) 1252422112     8065 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Duplex.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.996611 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/
--rw-r--r--   0 grongier (902446405) 1252422112      986 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls
--rw-r--r--   0 grongier (902446405) 1252422112      987 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls
--rw-r--r--   0 grongier (902446405) 1252422112      994 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1435 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Stop.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1622 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Test.cls
--rw-r--r--   0 grongier (902446405) 1252422112    13498 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Utils.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:39.006493 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112     1784 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       47 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/entry_points.txt
--rw-r--r--   0 grongier (902446405) 1252422112       43 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.376261 iris_pex_embedded_python-2.3.5/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.5/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-07-05 11:46:47.374787 iris_pex_embedded_python-2.3.5/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.5/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.5/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-07-05 11:46:47.376968 iris_pex_embedded_python-2.3.5/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2322 2023-07-05 11:46:31.000000 iris_pex_embedded_python-2.3.5/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.262765 iris_pex_embedded_python-2.3.5/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.259100 iris_pex_embedded_python-2.3.5/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.306510 iris_pex_embedded_python-2.3.5/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-06-19 12:50:33.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    12013 2023-06-26 12:55:30.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5647 2023-06-16 15:49:29.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15158 2023-06-20 09:39:24.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-06-19 10:23:02.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15325 2023-07-05 08:47:09.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.260396 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.337187 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/
+-rw-r--r--   0 grongier (902446405) 1252422112      932 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessOperation.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     2719 2023-06-26 12:48:53.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessProcess.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1039 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessService.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     3538 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Common.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1894 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Director.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.343351 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/
+-rw-r--r--   0 grongier (902446405) 1252422112      543 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/Operation.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     7103 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/Process.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      179 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/Service.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      628 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/InboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     8227 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Message.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      976 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/OutboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1691 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PickleMessage.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.346506 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/
+-rw-r--r--   0 grongier (902446405) 1252422112     8065 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Duplex.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.356735 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/
+-rw-r--r--   0 grongier (902446405) 1252422112      986 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      987 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      994 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1435 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Stop.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1622 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Test.cls
+-rw-r--r--   0 grongier (902446405) 1252422112    13498 2023-06-20 09:38:32.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Utils.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     2908 2023-06-21 15:28:25.000000 iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/WSGI.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-05 11:46:47.372239 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112     1819 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       47 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       43 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-07-05 11:46:47.000000 iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.4/LICENSE` & `iris_pex_embedded_python-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/PKG-INFO` & `iris_pex_embedded_python-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.4
+Version: 2.3.5
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.4/README.md` & `iris_pex_embedded_python-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/setup.py` & `iris_pex_embedded_python-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.4',
+        version='2.3.5',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     It can modify the message, convert it to a different format, or route it based on the message contents.
     The business process can route a message to a business operation or another business process.
     """
 
     DISPATCH = []
 
     PERSISTENT_PROPERTY_LIST=None
-    """ A list of the variable names of persistent properties."""        
+    """ A list of the variable names of persistent properties."""     
+
+    Context=None   
 
     def on_message(self, request):
         """ Called when the business operation receives a message from another production component.
         Typically, the operation will either send the message to the external system or forward it to a business process or another business operation.
         If the operation has an adapter, it uses the Adapter.invoke() method to call the method on the adapter that sends the message to the external system.
         If the operation is forwarding the message to another production component, it uses the SendRequestAsync() or the SendRequestSync() method
 
@@ -91,28 +93,32 @@
     def _set_iris_handles(self, handle_current, handle_partner):
         """ For internal use only. """
         self.iris_handle = handle_current
         return
 
     def _save_persistent_properties(self, host_object):
         """ For internal use only. """
+        if self.Context:
+            host_object.Context = self.Context
         if self.PERSISTENT_PROPERTY_LIST == None:
             return
         for prop in self.PERSISTENT_PROPERTY_LIST:
             val = getattr(self, prop, None)
             typ = val.__class__.__name__
             if (typ in ["str","int","float","bool","bytes"]):
                 try:
                     host_object.setPersistentProperty(prop, val)
                 except:
                     pass
         return
 
     def _restore_persistent_properties(self, host_object):
         """ For internal use only. """
+        if host_object.Context:
+            self.Context = host_object.Context
         if self.PERSISTENT_PROPERTY_LIST == None:
             return
         for prop in self.PERSISTENT_PROPERTY_LIST:
             try:
                 val = host_object.getPersistentProperty(prop)
                 setattr(self, prop, val)
             except:
```

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_cli.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,21 +186,30 @@
                 # check if the filename is absolute or relative
                 if os.path.isabs(filename):
                     path = os.path.dirname(filename)
                 else:
                     raise ValueError("The filename must be absolute")
                 # add the path to the system path
                 sys.path.append(path)
-                from settings import CLASSES, PRODUCTIONS
+            import settings
         except ImportError:
             # return an error if the settings file is not found
             # and explain how to create it
             raise ImportError("settings.py file not found. Please create it in the same directory as the main.py file. See the documentation for more information.")
-        _Utils.set_classes_settings(CLASSES)
-        _Utils.set_productions_settings(PRODUCTIONS)
+        try:
+            # set the classes settings
+            _Utils.set_classes_settings(settings.CLASSES)
+        except AttributeError:
+            print("No classes to register")
+        try:
+            # set the productions settings
+            _Utils.set_productions_settings(settings.PRODUCTIONS)
+        except AttributeError:
+            print("No productions to register")
+
 
 
     @staticmethod
     def set_classes_settings(class_items):
         """
         It takes a dictionary of classes and returns a dictionary of settings for each class
```

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessOperation.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessOperation.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessProcess.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessProcess.cls`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 Class Grongier.PEX.BusinessProcess Extends (Ens.BusinessProcess, Grongier.PEX.Common) [ Inheritance = right, ProcedureBlock, System = 4 ]
 {
 
 Parameter SETTINGS = "%classname:Python BusinessProcess,%module:Python BusinessProcess,%settings:Python BusinessProcess,%classpaths:Python BusinessProcess";
 
 Property persistentProperties As array Of %String(MAXLEN = "");
 
+Property Context As Ens.BP.Context;
+
 Method dispatchReply(response)
 {
 	set tSC = ..Reply(response)
 	if $$$ISERR(tSC) throw ##class(%Exception.StatusException).CreateFromStatus(tSC)
 	quit
 }
 
@@ -96,14 +98,17 @@
 </Value>
 <Value name="4">
 <Value>%settings</Value>
 </Value>
 <Value name="5">
 <Value>%class</Value>
 </Value>
+<Value name="6">
+<Value>Context</Value>
+</Value>
 </Data>
 <Data name="persistentProperties">
 <Attribute>persistentProperties</Attribute>
 <Structure>subnode</Structure>
 <Subscript>"Grongier.PEX.BusinessProcess.persistentProperties"</Subscript>
 </Data>
 <DefaultData>BusinessProcessDefaultData1</DefaultData>
```

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessService.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/BusinessService.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Common.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Common.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Director.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Director.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Operation.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/Operation.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Process.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Duplex/Process.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/InboundAdapter.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/InboundAdapter.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Message.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Message.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/OutboundAdapter.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/OutboundAdapter.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PickleMessage.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PickleMessage.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Duplex.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Duplex.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Stop.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/PrivateSession/Message/Stop.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Test.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Test.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Utils.cls` & `iris_pex_embedded_python-2.3.5/src/grongier/pex/data/PEX/Utils.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.4
+Version: 2.3.5
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.5/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/grongier/pex/data/PEX/Director.cls
 src/grongier/pex/data/PEX/InboundAdapter.cls
 src/grongier/pex/data/PEX/Message.cls
 src/grongier/pex/data/PEX/OutboundAdapter.cls
 src/grongier/pex/data/PEX/PickleMessage.cls
 src/grongier/pex/data/PEX/Test.cls
 src/grongier/pex/data/PEX/Utils.cls
+src/grongier/pex/data/PEX/WSGI.cls
 src/grongier/pex/data/PEX/Duplex/Operation.cls
 src/grongier/pex/data/PEX/Duplex/Process.cls
 src/grongier/pex/data/PEX/Duplex/Service.cls
 src/grongier/pex/data/PEX/PrivateSession/Duplex.cls
 src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls
 src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls
 src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls
```

