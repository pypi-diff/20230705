# Comparing `tmp/lekko_client-0.1.2.tar.gz` & `tmp/lekko_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lekko_client-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lekko_client-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lekko_client-0.1.2.tar` & `lekko_client-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1194 2023-06-22 00:22:58.664693 lekko_client-0.1.2/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3078 2023-05-05 21:12:44.881820 lekko_client-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2023-05-05 21:12:44.881972 lekko_client-0.1.2/LICENSE
--rw-r--r--   0        0        0      644 2023-06-21 18:36:15.400750 lekko_client-0.1.2/Makefile
--rw-r--r--   0        0        0      147 2023-06-21 18:36:15.400875 lekko_client-0.1.2/README.md
--rw-r--r--   0        0        0      233 2023-05-05 21:12:44.882244 lekko_client-0.1.2/buf.gen.yaml
--rw-r--r--   0        0        0     2368 2023-06-09 21:08:10.443431 lekko_client-0.1.2/example.py
--rw-r--r--   0        0        0      245 2023-06-22 20:34:21.499893 lekko_client-0.1.2/lekko_client/__init__.py
--rw-r--r--   0        0        0     8129 2023-06-22 00:22:58.665259 lekko_client-0.1.2/lekko_client/client.py
--rw-r--r--   0        0        0      279 2023-05-05 21:12:44.882685 lekko_client-0.1.2/lekko_client/exceptions.py
--rw-r--r--   0        0        0    10136 2023-06-22 00:22:58.665633 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
--rw-r--r--   0        0        0    19270 2023-06-22 00:22:58.665913 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
--rw-r--r--   0        0        0    16283 2023-06-21 18:37:43.929549 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     1761 2023-06-09 21:40:27.116943 lekko_client-0.1.2/lekko_client/helpers.py
--rw-r--r--   0        0        0      753 2023-05-05 21:12:44.883532 lekko_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       61 2023-05-05 21:12:44.883614 lekko_client-0.1.2/requirements.txt
--rw-r--r--   0        0        0     3397 2023-06-21 18:36:15.401775 lekko_client-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     1888 2023-05-05 21:12:44.883843 lekko_client-0.1.2/tests/mock_server.py
--rw-r--r--   0        0        0       40 2023-05-05 21:12:44.883918 lekko_client-0.1.2/tests/requirements.txt
--rw-r--r--   0        0        0     8323 2023-06-22 00:22:58.666197 lekko_client-0.1.2/tests/test_client.py
--rw-r--r--   0        0        0     1546 2023-06-21 18:36:15.402106 lekko_client-0.1.2/tox.ini
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 lekko_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1194 2023-07-04 23:59:06.747388 lekko_client-0.1.4/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1536 2023-07-04 23:59:06.747388 lekko_client-0.1.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     3078 2023-07-04 23:59:06.747388 lekko_client-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-04 23:59:06.747388 lekko_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0      644 2023-07-04 23:59:06.747388 lekko_client-0.1.4/Makefile
+-rw-r--r--   0        0        0     2105 2023-07-04 23:59:06.747388 lekko_client-0.1.4/README.md
+-rw-r--r--   0        0        0      233 2023-07-04 23:59:06.747388 lekko_client-0.1.4/buf.gen.yaml
+-rw-r--r--   0        0        0     2368 2023-07-04 23:59:06.747388 lekko_client-0.1.4/example.py
+-rw-r--r--   0        0        0      245 2023-07-04 23:59:16.395477 lekko_client-0.1.4/lekko_client/__init__.py
+-rw-r--r--   0        0        0     8129 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/client.py
+-rw-r--r--   0        0        0      279 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/exceptions.py
+-rw-r--r--   0        0        0    10136 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
+-rw-r--r--   0        0        0    19270 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
+-rw-r--r--   0        0        0    16283 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1761 2023-07-04 23:59:06.747388 lekko_client-0.1.4/lekko_client/helpers.py
+-rw-r--r--   0        0        0      910 2023-07-04 23:59:16.395477 lekko_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-04 23:59:06.747388 lekko_client-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     3397 2023-07-04 23:59:06.747388 lekko_client-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     1888 2023-07-04 23:59:06.747388 lekko_client-0.1.4/tests/mock_server.py
+-rw-r--r--   0        0        0       40 2023-07-04 23:59:06.747388 lekko_client-0.1.4/tests/requirements.txt
+-rw-r--r--   0        0        0     8323 2023-07-04 23:59:06.747388 lekko_client-0.1.4/tests/test_client.py
+-rw-r--r--   0        0        0     1546 2023-07-04 23:59:06.747388 lekko_client-0.1.4/tox.ini
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 lekko_client-0.1.4/PKG-INFO
```

### Comparing `lekko_client-0.1.2/.github/workflows/ci.yaml` & `lekko_client-0.1.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/.gitignore` & `lekko_client-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/LICENSE` & `lekko_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/Makefile` & `lekko_client-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/example.py` & `lekko_client-0.1.4/example.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/lekko_client/client.py` & `lekko_client-0.1.4/lekko_client/client.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py` & `lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi` & `lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py` & `lekko_client-0.1.4/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/lekko_client/helpers.py` & `lekko_client-0.1.4/lekko_client/helpers.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/tests/conftest.py` & `lekko_client-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/tests/mock_server.py` & `lekko_client-0.1.4/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/tests/test_client.py` & `lekko_client-0.1.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.2/tox.ini` & `lekko_client-0.1.4/tox.ini`

 * *Files identical despite different names*

