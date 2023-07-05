# Comparing `tmp/apache-airflow-providers-apache-kafka-1.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:21 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.2rc1.tar", last modified: Wed Jul  5 07:29:39 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1.tar` & `apache-airflow-providers-apache-kafka-1.1.2rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.234331 apache-airflow-providers-apache-kafka-1.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.234885 apache-airflow-providers-apache-kafka-1.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.137110 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.138409 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.139745 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.174605 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.188594 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.197120 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.202842 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.208920 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.232008 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1898 2023-06-20 11:41:21.236883 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.800284 apache-airflow-providers-apache-kafka-1.1.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-05 07:29:39.800932 apache-airflow-providers-apache-kafka-1.1.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.673005 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.674100 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.675729 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.724412 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.743020 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.753928 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.760817 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8219 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.767737 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2023-07-01 06:49:42.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.797219 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-05 07:29:39.803229 apache-airflow-providers-apache-kafka-1.1.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-kafka",
         "name": "Apache Kafka",
         "suspended": False,
         "description": "`Apache Kafka  <https://kafka.apache.org/>`__\n",
-        "versions": ["1.1.1", "1.1.0", "1.0.0"],
+        "versions": ["1.1.2", "1.1.1", "1.1.0", "1.0.0"],
         "dependencies": ["apache-airflow>=2.4.0", "asgiref", "confluent-kafka>=1.8.2"],
         "integrations": [
             {
                 "integration-name": "Apache Kafka",
                 "external-doc-url": "https://kafka.apache.org/",
                 "logo": "/integration-logos/apache/kafka.svg",
                 "tags": ["apache"],
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,16 @@
     def execute_complete(self, context, event=None):
         if self.xcom_push_key:
             self.xcom_push(context, key=self.xcom_push_key, value=event)
         return event
 
 
 class AwaitMessageTriggerFunctionSensor(BaseOperator):
-    """An Airflow sensor that defers until a specific message is published to
-    Kafka, then triggers a registered function, and goes back to waiting for
-    a message.
-
+    """
+    Defer until a specific message is published to Kafka, trigger a registered function, then resume waiting.
 
     The behavior of the consumer for this trigger is as follows:
     - poll the Kafka topics for a message
     - if no message returned, sleep
     - process the message with provided callable and commit the message offset
     - if callable returns any data, raise a TriggerEvent with the return data
     - else continue to next message
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,10 +109,11 @@
                 raise AirflowException(f"Error: {message.error()}")
             else:
 
                 rv = await async_message_process(message)
                 if rv:
                     await async_commit(asynchronous=False)
                     yield TriggerEvent(rv)
+                    break
                 else:
                     await async_commit(asynchronous=False)
                     await asyncio.sleep(self.poll_interval)
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.2rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.2rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py` & `apache-airflow-providers-apache-kafka-1.1.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-kafka package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.1.1"
+version = "1.1.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-kafka setup."""
     setup(
         version=version,
         extras_require={},
```

