# Comparing `tmp/beavers-0.0.2.tar.gz` & `tmp/beavers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beavers-0.0.2.tar", max compression
+gzip compressed data, was "beavers-0.0.3.tar", max compression
```

## Comparing `beavers-0.0.2.tar` & `beavers-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-30 10:34:01.950532 beavers-0.0.2/LICENSE
--rw-r--r--   0        0        0     2948 2023-06-30 10:34:01.950532 beavers-0.0.2/README.md
--rw-r--r--   0        0        0      116 2023-06-30 10:34:22.162736 beavers-0.0.2/beavers/__init__.py
--rw-r--r--   0        0        0    18570 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/engine.py
--rw-r--r--   0        0        0     9235 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/replay.py
--rw-r--r--   0        0        0     1657 2023-06-30 10:34:01.954532 beavers-0.0.2/beavers/testing.py
--rw-r--r--   0        0        0     1877 2023-06-30 10:34:22.162736 beavers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 beavers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 16:05:29.860944 beavers-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2949 2023-07-05 16:05:29.860944 beavers-0.0.3/README.md
+-rw-r--r--   0        0        0      116 2023-07-05 16:05:53.349254 beavers-0.0.3/beavers/__init__.py
+-rw-r--r--   0        0        0    18570 2023-07-05 16:05:29.860944 beavers-0.0.3/beavers/engine.py
+-rw-r--r--   0        0        0    23172 2023-07-05 16:05:29.860944 beavers-0.0.3/beavers/kafka.py
+-rw-r--r--   0        0        0     9235 2023-07-05 16:05:29.860944 beavers-0.0.3/beavers/replay.py
+-rw-r--r--   0        0        0     1657 2023-07-05 16:05:29.860944 beavers-0.0.3/beavers/testing.py
+-rw-r--r--   0        0        0     1916 2023-07-05 16:05:53.349254 beavers-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 beavers-0.0.3/PKG-INFO
```

### Comparing `beavers-0.0.2/LICENSE` & `beavers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beavers-0.0.2/README.md` & `beavers-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,30 @@
 [![Documentation][doc-image]][doc-url]
 [![License][license-image]][license-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
 
 # Beavers
-_____
 
 **Beavers** is a python library for stream processing, optimized for analytics. 
 
-
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to calculate analytics and serve model predictions,
 in both realtime and batch jobs.
 
 # Key Features
 
 
 * Works in **real time** (eg: reading from kafka) and **replay mode** (eg: reading from parquet)
 * Optimized for analytics, it uses micro-batching (instead of processing records one by one)
 * Similar to [incremental](https://github.com/janestreet/incremental), it  updates nodes in a dag incrementally
 * Taking inspiration from [kafka streams](https://www.confluent.io/blog/kafka-streams-tables-part-1-event-streaming/), there are two types of nodes in the dag:
-  * Stream: ephemeral micro-batches of events (cleared after every cycle)
-  * State: durable state derived from streams
+  * **Stream:** ephemeral micro-batches of events (cleared after every cycle)
+  * **State:** durable state derived from streams
 * Clear separation between the business logic and the IO. 
   So the same dag can be used in real time mode, replay mode or can be easily tested.
 * functional interface (no inheritance required)
 
 [pypi-image]: https://img.shields.io/pypi/v/beavers
 [pypi-url]: https://pypi.org/project/beavers/
 [build-image]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml/badge.svg
```

### Comparing `beavers-0.0.2/beavers/engine.py` & `beavers-0.0.3/beavers/engine.py`

 * *Files identical despite different names*

### Comparing `beavers-0.0.2/beavers/replay.py` & `beavers-0.0.3/beavers/replay.py`

 * *Files identical despite different names*

### Comparing `beavers-0.0.2/beavers/testing.py` & `beavers-0.0.3/beavers/testing.py`

 * *Files identical despite different names*

### Comparing `beavers-0.0.2/pyproject.toml` & `beavers-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "beavers"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python stream processing"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "beavers" }
 ]
 readme = "README.md"
@@ -19,28 +19,30 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = ["apache-arrow", "streaming", "data"]
 
 [tool.poetry.dependencies]
 pandas = ">1.4.0"
+confluent_kafka = ">=2.1.1"
 python = ">=3.10,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 coverage = ">=6.5.0"
 flake8 = ">=5.0.4"
 isort = ">=5.10.1"
 mkdocs = ">=1.4.2"
 pip-tools = "^6.12.1"
 pre-commit = ">=2.20.0"
 pylint = ">=2.15.0"
 pytest = ">=7.2.0"
 mkdocs-material = ">=9.0.3"
 mkdocstrings = { version = ">=0.21.2", extras = ['python'] }
+mock = "*"
 
 [tool.poetry.group.docs.dependencies]
 markdown-include = "*"
 mkdocs = "*"
 mkdocs-material = "*"
 mkdocs-material-extensions = "*"
 mkdocstrings = {version = "*", extras = ['python']}
```

### Comparing `beavers-0.0.2/PKG-INFO` & `beavers-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beavers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python stream processing
 Home-page: https://github.com/tradewelltech/beavers
 License: Apache-2.0
 Keywords: apache-arrow,streaming,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
@@ -12,14 +12,15 @@
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: confluent_kafka (>=2.1.1)
 Requires-Dist: pandas (>1.4.0)
 Project-URL: Documentation, https://beavers.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tradewelltech/beavers
 Description-Content-Type: text/markdown
 
 
 [![PyPI Version][pypi-image]][pypi-url]
@@ -30,32 +31,30 @@
 [![Documentation][doc-image]][doc-url]
 [![License][license-image]][license-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Downloads][downloads-month-image]][downloads-month-url]
 [![Code style: black][codestyle-image]][codestyle-url]
 
 # Beavers
-_____
 
 **Beavers** is a python library for stream processing, optimized for analytics. 
 
-
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
 to calculate analytics and serve model predictions,
 in both realtime and batch jobs.
 
 # Key Features
 
 
 * Works in **real time** (eg: reading from kafka) and **replay mode** (eg: reading from parquet)
 * Optimized for analytics, it uses micro-batching (instead of processing records one by one)
 * Similar to [incremental](https://github.com/janestreet/incremental), it  updates nodes in a dag incrementally
 * Taking inspiration from [kafka streams](https://www.confluent.io/blog/kafka-streams-tables-part-1-event-streaming/), there are two types of nodes in the dag:
-  * Stream: ephemeral micro-batches of events (cleared after every cycle)
-  * State: durable state derived from streams
+  * **Stream:** ephemeral micro-batches of events (cleared after every cycle)
+  * **State:** durable state derived from streams
 * Clear separation between the business logic and the IO. 
   So the same dag can be used in real time mode, replay mode or can be easily tested.
 * functional interface (no inheritance required)
 
 [pypi-image]: https://img.shields.io/pypi/v/beavers
 [pypi-url]: https://pypi.org/project/beavers/
 [build-image]: https://github.com/tradewelltech/beavers/actions/workflows/ci.yaml/badge.svg
```

