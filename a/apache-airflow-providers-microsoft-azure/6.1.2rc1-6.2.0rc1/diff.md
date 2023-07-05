# Comparing `tmp/apache-airflow-providers-microsoft-azure-6.1.2rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.1.2rc1.tar", last modified: Tue Jun 20 11:42:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.2.0rc1.tar", last modified: Wed Jul  5 07:30:17 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1.tar` & `apache-airflow-providers-microsoft-azure-6.2.0rc1.tar`

### file list

```diff
@@ -1,72 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.164695 apache-airflow-providers-microsoft-azure-6.1.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:26.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    27768 2023-06-20 11:42:28.166059 apache-airflow-providers-microsoft-azure-6.1.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26146 2023-06-20 11:42:26.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:27.942233 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:27.943200 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:27.944155 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:27.987735 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17113 2023-06-20 11:42:26.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.036584 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8732 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14227 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    43009 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    21409 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    12987 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    27574 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.043732 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10057 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.081036 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29309 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    12432 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.088665 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7890 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.102565 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.123538 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-06-17 16:45:00.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4536 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.133412 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:28.161387 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)    27768 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2944 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:27.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2360 2023-06-20 11:42:28.168438 apache-airflow-providers-microsoft-azure-6.1.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-20 11:42:26.000000 apache-airflow-providers-microsoft-azure-6.1.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.280108 apache-airflow-providers-microsoft-azure-6.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:15.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-05 07:30:17.281063 apache-airflow-providers-microsoft-azure-6.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4854 2023-07-05 07:30:15.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.049700 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.050969 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.052126 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.099536 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.108881 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/example_dag/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/example_dag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
+-rw-r--r--   0 root         (0) root         (0)    17240 2023-07-05 07:30:15.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.161343 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8759 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    44145 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-06-28 06:26:40.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    13004 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    29041 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.168943 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.205070 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29255 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.211162 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.223106 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8065 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.241688 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-06-17 16:45:00.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.250932 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11197 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7382 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:17.275731 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-07-05 07:30:17.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:16.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-05 07:30:17.284495 apache-airflow-providers-microsoft-azure-6.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-05 07:30:15.000000 apache-airflow-providers-microsoft-azure-6.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/LICENSE` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.1.2"
+__version__ = "6.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
         "suspended": False,
         "versions": [
+            "6.2.0",
             "6.1.2",
             "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.3.1",
             "5.3.0",
             "5.2.1",
@@ -287,37 +288,38 @@
                 "python-modules": ["airflow.providers.microsoft.azure.triggers.wasb"],
             },
         ],
         "transfers": [
             {
                 "source-integration-name": "Local",
                 "target-integration-name": "Microsoft Azure Data Lake Storage",
-                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/operators/local_to_adls.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/local_to_adls.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.local_to_adls",
             },
             {
                 "source-integration-name": "Oracle",
                 "target-integration-name": "Microsoft Azure Data Lake Storage",
                 "python-module": "airflow.providers.microsoft.azure.transfers.oracle_to_azure_data_lake",
             },
             {
                 "source-integration-name": "Local",
                 "target-integration-name": "Microsoft Azure Blob Storage",
+                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/local_to_wasb.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.local_to_wasb",
             },
             {
                 "source-integration-name": "Microsoft Azure Blob Storage",
                 "target-integration-name": "Google Cloud Storage (GCS)",
-                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/operators/azure_blob_to_gcs.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/azure_blob_to_gcs.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.azure_blob_to_gcs",
             },
             {
                 "source-integration-name": "SSH File Transfer Protocol (SFTP)",
                 "target-integration-name": "Microsoft Azure Blob Storage",
-                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/operators/sftp_to_wasb.rst",
+                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/sftp_to_wasb.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.sftp_to_wasb",
             },
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.microsoft.azure.hooks.base_azure.AzureBaseHook",
                 "connection-type": "azure",
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,17 @@
         else:
             raise AirflowException(f"Unknown authentication method: {auth_method}")
 
         return KustoClient(kcsb)
 
     def run_query(self, query: str, database: str, options: dict | None = None) -> KustoResponseDataSetV2:
         """
-        Run KQL query using provided configuration, and return
-        `azure.kusto.data.response.KustoResponseDataSet` instance.
+        Run KQL query using provided configuration, and return KustoResponseDataSet instance.
+
+        See: `azure.kusto.data.response.KustoResponseDataSet`
         If query is unsuccessful AirflowException is raised.
 
         :param query: KQL query to run
         :param database: Database to run the query on.
         :param options: Optional query options. See:
            https://docs.microsoft.com/en-us/azure/kusto/api/netfx/request-properties#list-of-clientrequestproperties
         :return: dict
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 
 
 class AzureBaseHook(BaseHook):
     """
-    This hook acts as a base hook for azure services. It offers several authentication mechanisms to
-    authenticate the client library used for upstream azure hooks.
+    This hook acts as a base hook for azure services.
+
+    It offers several authentication mechanisms to authenticate
+    the client library used for upstream azure hooks.
 
     :param sdk_client: The SDKClient to use.
     :param conn_id: The :ref:`Azure connection id<howto/connection:azure>`
         which refers to the information to connect to the service.
     """
 
     conn_name_attr = "azure_conn_id"
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,18 +233,15 @@
             raise AirflowBadRequest("Collection name cannot be None.")
 
         self.get_conn().get_database_client(self.__get_database_name(database_name)).delete_container(
             collection_name
         )
 
     def upsert_document(self, document, database_name=None, collection_name=None, document_id=None):
-        """
-        Inserts a new document (or updates an existing one) into an existing
-        collection in the CosmosDB database.
-        """
+        """Insert or update a document into an existing collection in the CosmosDB database."""
         # Assign unique ID if one isn't provided
         if document_id is None:
             document_id = str(uuid.uuid4())
 
         if document is None:
             raise AirflowBadRequest("You cannot insert a None document")
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 import inspect
 import time
 from functools import wraps
 from typing import Any, Callable, TypeVar, Union, cast
 
 from asgiref.sync import sync_to_async
+from azure.core.exceptions import ServiceRequestError
 from azure.core.polling import LROPoller
 from azure.identity import ClientSecretCredential, DefaultAzureCredential
 from azure.identity.aio import (
     ClientSecretCredential as AsyncClientSecretCredential,
     DefaultAzureCredential as AsyncDefaultAzureCredential,
 )
 from azure.mgmt.datafactory import DataFactoryManagementClient
@@ -210,14 +211,18 @@
             )
         else:
             credential = DefaultAzureCredential()
         self._conn = self._create_client(credential, subscription_id)
 
         return self._conn
 
+    def refresh_conn(self) -> DataFactoryManagementClient:
+        self._conn = None
+        return self.get_conn()
+
     @provide_targeted_factory
     def get_factory(
         self, resource_group_name: str | None = None, factory_name: str | None = None, **config: Any
     ) -> Factory:
         """
         Get the factory.
 
@@ -808,14 +813,15 @@
         """
         pipeline_run_info = PipelineRunInfo(
             run_id=run_id,
             factory_name=factory_name,
             resource_group_name=resource_group_name,
         )
         pipeline_run_status = self.get_pipeline_run_status(**pipeline_run_info)
+        executed_after_token_refresh = True
 
         start_time = time.monotonic()
 
         while (
             pipeline_run_status not in AzureDataFactoryPipelineRunStatus.TERMINAL_STATUSES
             and pipeline_run_status not in expected_statuses
         ):
@@ -824,15 +830,22 @@
                 raise AzureDataFactoryPipelineRunException(
                     f"Pipeline run {run_id} has not reached a terminal status after {timeout} seconds."
                 )
 
             # Wait to check the status of the pipeline run based on the ``check_interval`` configured.
             time.sleep(check_interval)
 
-            pipeline_run_status = self.get_pipeline_run_status(**pipeline_run_info)
+            try:
+                pipeline_run_status = self.get_pipeline_run_status(**pipeline_run_info)
+                executed_after_token_refresh = True
+            except ServiceRequestError:
+                if executed_after_token_refresh:
+                    self.refresh_conn()
+                    continue
+                raise
 
         return pipeline_run_status in expected_statuses
 
     @provide_targeted_factory
     def cancel_pipeline_run(
         self,
         run_id: str,
@@ -1128,14 +1141,18 @@
         self._async_conn = AsyncDataFactoryManagementClient(
             credential=credential,
             subscription_id=subscription_id,
         )
 
         return self._async_conn
 
+    async def refresh_conn(self) -> AsyncDataFactoryManagementClient:
+        self._conn = None
+        return await self.get_async_conn()
+
     @provide_targeted_factory_async
     async def get_pipeline_run(
         self,
         run_id: str,
         resource_group_name: str | None = None,
         factory_name: str | None = None,
         **config: Any,
@@ -1145,33 +1162,49 @@
 
         :param run_id: The pipeline run identifier.
         :param resource_group_name: The resource group name.
         :param factory_name: The factory name.
         :param config: Extra parameters for the ADF client.
         """
         client = await self.get_async_conn()
-        try:
-            pipeline_run = await client.pipeline_runs.get(resource_group_name, factory_name, run_id)
-            return pipeline_run
-        except Exception as e:
-            raise AirflowException(e)
+        pipeline_run = await client.pipeline_runs.get(resource_group_name, factory_name, run_id)
+        return pipeline_run
 
     async def get_adf_pipeline_run_status(
         self, run_id: str, resource_group_name: str | None = None, factory_name: str | None = None
     ) -> str:
         """
         Connect to Azure Data Factory asynchronously and get the pipeline status by run_id.
 
         :param run_id: The pipeline run identifier.
         :param resource_group_name: The resource group name.
         :param factory_name: The factory name.
         """
+        pipeline_run = await self.get_pipeline_run(
+            run_id=run_id,
+            factory_name=factory_name,
+            resource_group_name=resource_group_name,
+        )
+        status: str = pipeline_run.status
+        return status
+
+    @provide_targeted_factory_async
+    async def cancel_pipeline_run(
+        self,
+        run_id: str,
+        resource_group_name: str | None = None,
+        factory_name: str | None = None,
+        **config: Any,
+    ) -> None:
+        """
+        Cancel the pipeline run.
+
+        :param run_id: The pipeline run identifier.
+        :param resource_group_name: The resource group name.
+        :param factory_name: The factory name.
+        :param config: Extra parameters for the ADF client.
+        """
+        client = await self.get_async_conn()
         try:
-            pipeline_run = await self.get_pipeline_run(
-                run_id=run_id,
-                factory_name=factory_name,
-                resource_group_name=resource_group_name,
-            )
-            status: str = pipeline_run.status
-            return status
+            await client.pipeline_runs.cancel(resource_group_name, factory_name, run_id)
         except Exception as e:
             raise AirflowException(e)
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files 2% similar despite different names*

```diff
@@ -505,7 +505,20 @@
         """Delete the specified directory in a file system.
 
         :param file_system_name: Name of the file system or instance of FileSystemProperties.
         :param directory_name: Name of the directory.
         """
         directory_client = self.get_directory_client(file_system_name, directory_name)
         directory_client.delete_directory()
+
+    def test_connection(self):
+        """Test ADLS Gen2 Storage connection."""
+        try:
+            # Attempts to list file systems in ADLS Gen2 Storage and retrieves the first
+            # file_system from the returned iterator. The Azure DataLake Storage allows creation
+            # of DataLakeServiceClient even if the credentials are incorrect but will fail properly
+            # if we try to fetch the file_system. We need to _actually_ try to retrieve a
+            # file_system to properly test the connection
+            next(self.get_conn().list_file_systems(), None)
+            return True, "Successfully connected to ADLS Gen2 Storage."
+        except Exception as e:
+            return False, str(e)
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from azure.storage.file import File, FileService
 
 from airflow.hooks.base import BaseHook
 
 
 def _ensure_prefixes(conn_type):
     """
+    Deprecated.
+
     Remove when provider min airflow version >= 2.5.0 since this is handled by
     provider manager from that version.
     """
 
     def dec(func):
         @wraps(func)
         def inner():
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 from airflow.hooks.base import BaseHook
 
 AsyncCredentials = Union[AsyncClientSecretCredential, AsyncDefaultAzureCredential]
 
 
 def _ensure_prefixes(conn_type):
     """
+    Deprecated.
+
     Remove when provider min airflow version >= 2.5.0 since this is handled by
     provider manager from that version.
     """
 
     def dec(func):
         @wraps(func)
         def inner():
@@ -122,28 +124,29 @@
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="wasb")
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour."""
         return {
-            "hidden_fields": ["schema", "port", "extra"],
+            "hidden_fields": ["schema", "port"],
             "relabeling": {
                 "login": "Blob Storage Login (optional)",
                 "password": "Blob Storage Key (optional)",
                 "host": "Account Name (Active Directory Auth)",
             },
             "placeholders": {
                 "login": "account name",
                 "password": "secret",
                 "host": "account url",
                 "connection_string": "connection string auth",
                 "tenant_id": "tenant",
                 "shared_access_key": "shared access key",
                 "sas_token": "account url or token",
+                "extra": "additional options for use with ClientSecretCredential or DefaultAzureCredential",
             },
         }
 
     def __init__(
         self,
         wasb_conn_id: str = default_conn_name,
         public_read: bool = False,
@@ -170,55 +173,56 @@
             return extra_dict[field_name] or None
         return extra_dict.get(f"{prefix}{field_name}") or None
 
     def get_conn(self) -> BlobServiceClient:
         """Return the BlobServiceClient object."""
         conn = self.get_connection(self.conn_id)
         extra = conn.extra_dejson or {}
-
-        if self.public_read:
-            # Here we use anonymous public read
-            # more info
-            # https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources
-            return BlobServiceClient(account_url=conn.host, **extra)
+        client_secret_auth_config = extra.pop("client_secret_auth_config", {})
 
         connection_string = self._get_field(extra, "connection_string")
         if connection_string:
             # connection_string auth takes priority
             return BlobServiceClient.from_connection_string(connection_string, **extra)
 
-        shared_access_key = self._get_field(extra, "shared_access_key")
-        if shared_access_key:
-            # using shared access key
-            return BlobServiceClient(account_url=conn.host, credential=shared_access_key, **extra)
-
         tenant = self._get_field(extra, "tenant_id")
         if tenant:
             # use Active Directory auth
             app_id = conn.login
             app_secret = conn.password
-            token_credential = ClientSecretCredential(tenant, app_id, app_secret)
+            token_credential = ClientSecretCredential(tenant, app_id, app_secret, **client_secret_auth_config)
             return BlobServiceClient(account_url=conn.host, credential=token_credential, **extra)
 
+        account_url = conn.host if conn.host else f"https://{conn.login}.blob.core.windows.net/"
+
+        if self.public_read:
+            # Here we use anonymous public read
+            # more info
+            # https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources
+            return BlobServiceClient(account_url=account_url, **extra)
+
+        shared_access_key = self._get_field(extra, "shared_access_key")
+        if shared_access_key:
+            # using shared access key
+            return BlobServiceClient(account_url=account_url, credential=shared_access_key, **extra)
+
         sas_token = self._get_field(extra, "sas_token")
         if sas_token:
             if sas_token.startswith("https"):
                 return BlobServiceClient(account_url=sas_token, **extra)
             else:
-                return BlobServiceClient(
-                    account_url=f"https://{conn.login}.blob.core.windows.net/{sas_token}", **extra
-                )
+                return BlobServiceClient(account_url=f"{account_url}/{sas_token}", **extra)
 
         # Fall back to old auth (password) or use managed identity if not provided.
         credential = conn.password
         if not credential:
             credential = DefaultAzureCredential()
             self.log.info("Using DefaultAzureCredential as credential")
         return BlobServiceClient(
-            account_url=f"https://{conn.login}.blob.core.windows.net/",
+            account_url=account_url,
             credential=credential,
             **extra,
         )
 
     def _get_container_client(self, container_name: str) -> ContainerClient:
         """
         Instantiates a container client.
@@ -286,14 +290,41 @@
         container = self._get_container_client(container_name)
         blob_list = []
         blobs = container.walk_blobs(name_starts_with=prefix, include=include, delimiter=delimiter, **kwargs)
         for blob in blobs:
             blob_list.append(blob.name)
         return blob_list
 
+    def get_blobs_list_recursive(
+        self,
+        container_name: str,
+        prefix: str | None = None,
+        include: list[str] | None = None,
+        endswith: str = "",
+        **kwargs,
+    ) -> list:
+        """
+        List blobs in a given container.
+
+        :param container_name: The name of the container
+        :param prefix: Filters the results to return only blobs whose names
+            begin with the specified prefix.
+        :param include: Specifies one or more additional datasets to include in the
+            response. Options include: ``snapshots``, ``metadata``, ``uncommittedblobs``,
+            ``copy`, ``deleted``.
+        :param delimiter: filters objects based on the delimiter (for e.g '.csv')
+        """
+        container = self._get_container_client(container_name)
+        blob_list = []
+        blobs = container.list_blobs(name_starts_with=prefix, include=include, **kwargs)
+        for blob in blobs:
+            if blob.name.endswith(endswith):
+                blob_list.append(blob.name)
+        return blob_list
+
     def load_file(
         self,
         file_path: str,
         container_name: str,
         blob_name: str,
         create_container: bool = False,
         **kwargs,
@@ -538,66 +569,71 @@
     async def get_async_conn(self) -> AsyncBlobServiceClient:
         """Return the Async BlobServiceClient object."""
         if self.blob_service_client is not None:
             return self.blob_service_client
 
         conn = await sync_to_async(self.get_connection)(self.conn_id)
         extra = conn.extra_dejson or {}
-
-        if self.public_read:
-            # Here we use anonymous public read
-            # more info
-            # https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources
-            self.blob_service_client = AsyncBlobServiceClient(account_url=conn.host, **extra)
-            return self.blob_service_client
+        client_secret_auth_config = extra.pop("client_secret_auth_config", {})
 
         connection_string = self._get_field(extra, "connection_string")
         if connection_string:
             # connection_string auth takes priority
             self.blob_service_client = AsyncBlobServiceClient.from_connection_string(
                 connection_string, **extra
             )
             return self.blob_service_client
 
-        shared_access_key = self._get_field(extra, "shared_access_key")
-        if shared_access_key:
-            # using shared access key
-            self.blob_service_client = AsyncBlobServiceClient(
-                account_url=conn.host, credential=shared_access_key, **extra
-            )
-            return self.blob_service_client
-
         tenant = self._get_field(extra, "tenant_id")
         if tenant:
             # use Active Directory auth
             app_id = conn.login
             app_secret = conn.password
-            token_credential = AsyncClientSecretCredential(tenant, app_id, app_secret)
+            token_credential = AsyncClientSecretCredential(
+                tenant, app_id, app_secret, **client_secret_auth_config
+            )
             self.blob_service_client = AsyncBlobServiceClient(
                 account_url=conn.host, credential=token_credential, **extra  # type:ignore[arg-type]
             )
             return self.blob_service_client
 
+        account_url = conn.host if conn.host else f"https://{conn.login}.blob.core.windows.net/"
+
+        if self.public_read:
+            # Here we use anonymous public read
+            # more info
+            # https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources
+            self.blob_service_client = AsyncBlobServiceClient(account_url=account_url, **extra)
+            return self.blob_service_client
+
+        shared_access_key = self._get_field(extra, "shared_access_key")
+        if shared_access_key:
+            # using shared access key
+            self.blob_service_client = AsyncBlobServiceClient(
+                account_url=account_url, credential=shared_access_key, **extra
+            )
+            return self.blob_service_client
+
         sas_token = self._get_field(extra, "sas_token")
         if sas_token:
             if sas_token.startswith("https"):
                 self.blob_service_client = AsyncBlobServiceClient(account_url=sas_token, **extra)
             else:
                 self.blob_service_client = AsyncBlobServiceClient(
-                    account_url=f"https://{conn.login}.blob.core.windows.net/{sas_token}", **extra
+                    account_url=f"{account_url}/{sas_token}", **extra
                 )
             return self.blob_service_client
 
         # Fall back to old auth (password) or use managed identity if not provided.
         credential = conn.password
         if not credential:
             credential = AsyncDefaultAzureCredential()
             self.log.info("Using DefaultAzureCredential as credential")
         self.blob_service_client = AsyncBlobServiceClient(
-            account_url=f"https://{conn.login}.blob.core.windows.net/",
+            account_url=account_url,
             credential=credential,
             **extra,
         )
 
         return self.blob_service_client
 
     def _get_blob_client(self, container_name: str, blob_name: str) -> AsyncBlobClient:
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/example_dag/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     if Version(version) < Version("2.6"):
         return False
     return conf.getboolean("logging", "delete_local_logs")
 
 
 class WasbTaskHandler(FileTaskHandler, LoggingMixin):
     """
-    WasbTaskHandler is a python log handler that handles and reads
-    task instance logs. It extends airflow FileTaskHandler and
-    uploads to and reads from Wasb remote storage.
+    WasbTaskHandler is a python log handler that handles and reads task instance logs.
+
+    It extends airflow FileTaskHandler and uploads to and reads from Wasb remote storage.
     """
 
     trigger_should_wrap = True
 
     def __init__(
         self,
         base_log_folder: str,
@@ -167,14 +167,15 @@
         return messages, logs
 
     def _read(
         self, ti, try_number: int, metadata: dict[str, Any] | None = None
     ) -> tuple[str, dict[str, bool]]:
         """
         Read logs of given task instance and try_number from Wasb remote storage.
+
         If failed, read the log from task instance host machine.
 
         todo: when min airflow version >= 2.6, remove this method
 
         :param ti: task instance object
         :param try_number: task instance try_number to read logs from
         :param metadata: log metadata,
@@ -203,16 +204,15 @@
 
         except Exception as e:
             self.log.debug('Exception when trying to check remote location: "%s"', e)
         return False
 
     def wasb_read(self, remote_log_location: str, return_error: bool = False):
         """
-        Returns the log found at the remote_log_location. Returns '' if no
-        logs are found or there is an error.
+        Return the log found at the remote_log_location. Returns '' if no logs are found or there is an error.
 
         :param remote_log_location: the log's location in remote storage
         :param return_error: if True, returns a string error message if an
             error occurs. Otherwise returns '' when an error occurs.
         """
         try:
             return self.hook.read_file(self.wasb_container, remote_log_location)
@@ -222,16 +222,15 @@
             # return error if needed
             if return_error:
                 return msg
             return ""
 
     def wasb_write(self, log: str, remote_log_location: str, append: bool = True) -> bool:
         """
-        Writes the log to the remote_log_location. Fails silently if no hook
-        was created.
+        Writes the log to the remote_log_location. Fails silently if no hook was created.
 
         :param log: the log to write to the remote_log_location
         :param remote_log_location: the log's location in remote storage
         :param append: if False, any existing log file is overwritten. If True,
             the new log is appended to any existing logs.
         """
         if append and self.wasb_log_exists(remote_log_location):
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,18 +151,15 @@
         super().__init__(**kwargs)
         self.queue_name = queue_name
         self.azure_service_bus_conn_id = azure_service_bus_conn_id
         self.max_message_count = max_message_count
         self.max_wait_time = max_wait_time
 
     def execute(self, context: Context) -> None:
-        """
-        Receive Message in specific queue in Service Bus namespace,
-        by connecting to Service Bus client.
-        """
+        """Receive Message in specific queue in Service Bus namespace by connecting to Service Bus client."""
         # Create the hook
         hook = MessageHook(azure_service_bus_conn_id=self.azure_service_bus_conn_id)
 
         # Receive message
         hook.receive_message(
             self.queue_name, max_message_count=self.max_message_count, max_wait_time=self.max_wait_time
         )
@@ -523,18 +520,15 @@
         self.topic_name = topic_name
         self.subscription_name = subscription_name
         self.max_message_count = max_message_count
         self.max_wait_time = max_wait_time
         self.azure_service_bus_conn_id = azure_service_bus_conn_id
 
     def execute(self, context: Context) -> None:
-        """
-        Receive Message in specific queue in Service Bus namespace,
-        by connecting to Service Bus client.
-        """
+        """Receive Message in specific queue in Service Bus namespace by connecting to Service Bus client."""
         # Create the hook
         hook = MessageHook(azure_service_bus_conn_id=self.azure_service_bus_conn_id)
 
         # Receive message
         hook.receive_subscription_message(
             self.topic_name, self.subscription_name, self.max_message_count, self.max_wait_time
         )
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import time
 import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.microsoft.azure.hooks.data_factory import (
     AzureDataFactoryHook,
     AzureDataFactoryPipelineRunException,
     AzureDataFactoryPipelineRunStatus,
@@ -136,15 +137,15 @@
         reference_pipeline_run_id: str | None = None,
         is_recovery: bool | None = None,
         start_activity_name: str | None = None,
         start_from_failure: bool | None = None,
         parameters: dict[str, Any] | None = None,
         timeout: int = 60 * 60 * 24 * 7,
         check_interval: int = 60,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.azure_data_factory_conn_id = azure_data_factory_conn_id
         self.pipeline_name = pipeline_name
         self.wait_for_termination = wait_for_termination
         self.resource_group_name = resource_group_name
@@ -228,16 +229,16 @@
                     "Argument `wait_for_termination` is False and `deferrable` is True , hence "
                     "`deferrable` parameter doesn't have any effect",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event:
             if event["status"] == "error":
                 raise AirflowException(event["message"])
             self.log.info(event["message"])
 
     def on_kill(self) -> None:
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 
         return self._get_secret(self.config_prefix, key)
 
     @staticmethod
     def build_path(path_prefix: str, secret_id: str, sep: str = "-") -> str:
         """
         Given a path_prefix and secret_id, build a valid secret name for the Azure Key Vault Backend.
+
         Also replaces underscore in the path with dashes to support easy switching between
         environment variables, so ``connection_default`` becomes ``connection-default``.
 
         :param path_prefix: The path prefix of the secret to retrieve
         :param secret_id: Name of the secret
         :param sep: Separator used to concatenate path_prefix and secret_id
         """
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.microsoft.azure.hooks.data_factory import (
     AzureDataFactoryHook,
     AzureDataFactoryPipelineRunException,
     AzureDataFactoryPipelineRunStatus,
 )
 from airflow.providers.microsoft.azure.triggers.data_factory import ADFPipelineRunStatusSensorTrigger
@@ -56,15 +57,15 @@
     def __init__(
         self,
         *,
         run_id: str,
         azure_data_factory_conn_id: str = AzureDataFactoryHook.default_conn_name,
         resource_group_name: str | None = None,
         factory_name: str | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.azure_data_factory_conn_id = azure_data_factory_conn_id
         self.run_id = run_id
         self.resource_group_name = resource_group_name
         self.factory_name = factory_name
@@ -108,16 +109,16 @@
                     ),
                     method_name="execute_complete",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event:
             if event["status"] == "error":
                 raise AirflowException(event["message"])
             self.log.info(event["message"])
         return None
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # under the License.
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
 from airflow.providers.microsoft.azure.triggers.wasb import WasbBlobSensorTrigger, WasbPrefixSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -49,15 +50,15 @@
         self,
         *,
         container_name: str,
         blob_name: str,
         wasb_conn_id: str = "wasb_default",
         check_options: dict | None = None,
         public_read: bool = False,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if check_options is None:
             check_options = {}
         self.wasb_conn_id = wasb_conn_id
         self.container_name = container_name
@@ -92,16 +93,16 @@
                     ),
                     method_name="execute_complete",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event:
             if event["status"] == "error":
                 raise AirflowException(event["message"])
             self.log.info(event["message"])
         else:
             raise AirflowException("Did not receive valid event from the triggerer")
@@ -147,15 +148,15 @@
     def __init__(
         self,
         *,
         container_name: str,
         prefix: str,
         wasb_conn_id: str = "wasb_default",
         check_options: dict | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if check_options is None:
             check_options = {}
         self.wasb_conn_id = wasb_conn_id
         self.container_name = container_name
@@ -188,16 +189,16 @@
                     ),
                     method_name="execute_complete",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event:
             if event["status"] == "error":
                 raise AirflowException(event["message"])
             self.log.info(event["message"])
         else:
             raise AirflowException("Did not receive valid event from the triggerer")
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             **self.extra_upload_options,
         )
 
 
 class LocalToAzureDataLakeStorageOperator(LocalFilesystemToADLSOperator):
     """
     This class is deprecated.
+
     Please use `airflow.providers.microsoft.azure.transfers.local_to_adls.LocalFilesystemToADLSOperator`.
     """
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             """This class is deprecated.
             Please use
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class OracleToAzureDataLakeOperator(BaseOperator):
     """
-    Moves data from Oracle to Azure Data Lake. The operator runs the query against
-    Oracle and stores the file locally before loading it into Azure Data Lake.
-
+    Runs the query against Oracle and stores the file locally before loading it into Azure Data Lake.
 
     :param filename: file name to be used by the csv file.
     :param azure_data_lake_conn_id: destination azure data lake connection.
     :param azure_data_lake_path: destination path in azure data lake to put the file.
     :param oracle_conn_id: :ref:`Source Oracle connection <howto/connection:oracle>`.
     :param sql: SQL query to execute against the Oracle database. (templated)
     :param sql_params: Parameters to use in sql query. (templated)
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # under the License.
 from __future__ import annotations
 
 import asyncio
 import time
 from typing import Any, AsyncIterator
 
+from azure.core.exceptions import ServiceRequestError
+
 from airflow.providers.microsoft.azure.hooks.data_factory import (
     AzureDataFactoryAsyncHook,
     AzureDataFactoryPipelineRunStatus,
 )
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
@@ -64,32 +66,49 @@
                 "poke_interval": self.poke_interval,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:
         """Make async connection to Azure Data Factory, polls for the pipeline run status."""
         hook = AzureDataFactoryAsyncHook(azure_data_factory_conn_id=self.azure_data_factory_conn_id)
+        executed_after_token_refresh = False
         try:
             while True:
-                pipeline_status = await hook.get_adf_pipeline_run_status(
-                    run_id=self.run_id,
-                    resource_group_name=self.resource_group_name,
-                    factory_name=self.factory_name,
-                )
-                if pipeline_status == AzureDataFactoryPipelineRunStatus.FAILED:
-                    yield TriggerEvent(
-                        {"status": "error", "message": f"Pipeline run {self.run_id} has Failed."}
+                try:
+                    pipeline_status = await hook.get_adf_pipeline_run_status(
+                        run_id=self.run_id,
+                        resource_group_name=self.resource_group_name,
+                        factory_name=self.factory_name,
                     )
-                elif pipeline_status == AzureDataFactoryPipelineRunStatus.CANCELLED:
-                    msg = f"Pipeline run {self.run_id} has been Cancelled."
-                    yield TriggerEvent({"status": "error", "message": msg})
-                elif pipeline_status == AzureDataFactoryPipelineRunStatus.SUCCEEDED:
-                    msg = f"Pipeline run {self.run_id} has been Succeeded."
-                    yield TriggerEvent({"status": "success", "message": msg})
-                await asyncio.sleep(self.poke_interval)
+                    executed_after_token_refresh = False
+                    if pipeline_status == AzureDataFactoryPipelineRunStatus.FAILED:
+                        yield TriggerEvent(
+                            {"status": "error", "message": f"Pipeline run {self.run_id} has Failed."}
+                        )
+                        return
+                    elif pipeline_status == AzureDataFactoryPipelineRunStatus.CANCELLED:
+                        msg = f"Pipeline run {self.run_id} has been Cancelled."
+                        yield TriggerEvent({"status": "error", "message": msg})
+                        return
+                    elif pipeline_status == AzureDataFactoryPipelineRunStatus.SUCCEEDED:
+                        msg = f"Pipeline run {self.run_id} has been Succeeded."
+                        yield TriggerEvent({"status": "success", "message": msg})
+                        return
+                    await asyncio.sleep(self.poke_interval)
+                except ServiceRequestError:
+                    # conn might expire during long running pipeline.
+                    # If expcetion is caught, it tries to refresh connection once.
+                    # If it still doesn't fix the issue,
+                    # than the execute_after_token_refresh would still be False
+                    # and an exception will be raised
+                    if executed_after_token_refresh:
+                        await hook.refresh_conn()
+                        executed_after_token_refresh = False
+                        continue
+                    raise
         except Exception as e:
             yield TriggerEvent({"status": "error", "message": str(e)})
 
 
 class AzureDataFactoryTrigger(BaseTrigger):
     """Trigger when the Azure data factory pipeline job finishes.
 
@@ -143,41 +162,57 @@
         hook = AzureDataFactoryAsyncHook(azure_data_factory_conn_id=self.azure_data_factory_conn_id)
         try:
             pipeline_status = await hook.get_adf_pipeline_run_status(
                 run_id=self.run_id,
                 resource_group_name=self.resource_group_name,
                 factory_name=self.factory_name,
             )
+            executed_after_token_refresh = True
             if self.wait_for_termination:
                 while self.end_time > time.time():
-                    pipeline_status = await hook.get_adf_pipeline_run_status(
-                        run_id=self.run_id,
-                        resource_group_name=self.resource_group_name,
-                        factory_name=self.factory_name,
-                    )
-                    if pipeline_status in AzureDataFactoryPipelineRunStatus.FAILURE_STATES:
-                        yield TriggerEvent(
-                            {
-                                "status": "error",
-                                "message": f"The pipeline run {self.run_id} has {pipeline_status}.",
-                                "run_id": self.run_id,
-                            }
+                    try:
+                        pipeline_status = await hook.get_adf_pipeline_run_status(
+                            run_id=self.run_id,
+                            resource_group_name=self.resource_group_name,
+                            factory_name=self.factory_name,
                         )
-                    elif pipeline_status == AzureDataFactoryPipelineRunStatus.SUCCEEDED:
-                        yield TriggerEvent(
-                            {
-                                "status": "success",
-                                "message": f"The pipeline run {self.run_id} has {pipeline_status}.",
-                                "run_id": self.run_id,
-                            }
+                        executed_after_token_refresh = True
+                        if pipeline_status in AzureDataFactoryPipelineRunStatus.FAILURE_STATES:
+                            yield TriggerEvent(
+                                {
+                                    "status": "error",
+                                    "message": f"The pipeline run {self.run_id} has {pipeline_status}.",
+                                    "run_id": self.run_id,
+                                }
+                            )
+                            return
+                        elif pipeline_status == AzureDataFactoryPipelineRunStatus.SUCCEEDED:
+                            yield TriggerEvent(
+                                {
+                                    "status": "success",
+                                    "message": f"The pipeline run {self.run_id} has {pipeline_status}.",
+                                    "run_id": self.run_id,
+                                }
+                            )
+                            return
+                        self.log.info(
+                            "Sleeping for %s. The pipeline state is %s.", self.check_interval, pipeline_status
                         )
-                    self.log.info(
-                        "Sleeping for %s. The pipeline state is %s.", self.check_interval, pipeline_status
-                    )
-                    await asyncio.sleep(self.check_interval)
+                        await asyncio.sleep(self.check_interval)
+                    except ServiceRequestError:
+                        # conn might expire during long running pipeline.
+                        # If expcetion is caught, it tries to refresh connection once.
+                        # If it still doesn't fix the issue,
+                        # than the execute_after_token_refresh would still be False
+                        # and an exception will be raised
+                        if executed_after_token_refresh:
+                            await hook.refresh_conn()
+                            executed_after_token_refresh = False
+                            continue
+                        raise
 
                 yield TriggerEvent(
                     {
                         "status": "error",
                         "message": f"Timeout: The pipeline run {self.run_id} has {pipeline_status}.",
                         "run_id": self.run_id,
                     }
@@ -187,8 +222,18 @@
                     {
                         "status": "success",
                         "message": f"The pipeline run {self.run_id} has {pipeline_status} status.",
                         "run_id": self.run_id,
                     }
                 )
         except Exception as e:
+            if self.run_id:
+                try:
+                    await hook.cancel_pipeline_run(
+                        run_id=self.run_id,
+                        resource_group_name=self.resource_group_name,
+                        factory_name=self.factory_name,
+                    )
+                    self.log.info("Unexpected error %s caught. Cancel pipeline run %s", str(e), self.run_id)
+                except Exception as err:
+                    yield TriggerEvent({"status": "error", "message": str(err), "run_id": self.run_id})
             yield TriggerEvent({"status": "error", "message": str(e), "run_id": self.run_id})
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 
 from airflow.providers.microsoft.azure.hooks.wasb import WasbAsyncHook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class WasbBlobSensorTrigger(BaseTrigger):
     """
-    WasbBlobSensorTrigger is fired as deferred class with params to run the task in
-    trigger worker to check for existence of the given blob in the provided container.
+    Checks for existence of the given blob in the provided container.
+
+    WasbBlobSensorTrigger is fired as deferred class with params to run the task in trigger worker.
 
     :param container_name: name of the container in which the blob should be searched for
     :param blob_name: name of the blob to check existence for
     :param wasb_conn_id: the connection identifier for connecting to Azure WASB
     :param poke_interval:  polling period in seconds to check for the status
     :param public_read: whether an anonymous public read access should be used. Default is False
     """
@@ -86,16 +87,17 @@
                         await asyncio.sleep(self.poke_interval)
         except Exception as e:
             yield TriggerEvent({"status": "error", "message": str(e)})
 
 
 class WasbPrefixSensorTrigger(BaseTrigger):
     """
+    Checks for the existence of a blob with the given prefix in the provided container.
+
     WasbPrefixSensorTrigger is fired as a deferred class with params to run the task in trigger.
-    It checks for the existence of a blob with the given prefix in the provided container.
 
     :param container_name: name of the container in which the blob should be searched for
     :param prefix: prefix of the blob to check existence for
     :param include: specifies one or more additional datasets to include in the
             response. Options include: ``snapshots``, ``metadata``, ``uncommittedblobs``,
             ``copy``, ``deleted``
     :param delimiter: filters objects based on the delimiter (for e.g '.csv')
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 import warnings
 from functools import wraps
 
 
 def _ensure_prefixes(conn_type):
     """
+    Deprecated.
+
     Remove when provider min airflow version >= 2.5.0 since this is handled by
     provider manager from that version.
     """
 
     def dec(func):
         @wraps(func)
         def inner():
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/microsoft/azure/__init__.py
 airflow/providers/microsoft/azure/get_provider_info.py
 airflow/providers/microsoft/azure/utils.py
+airflow/providers/microsoft/azure/example_dag/__init__.py
+airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
+airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
 airflow/providers/microsoft/azure/hooks/__init__.py
 airflow/providers/microsoft/azure/hooks/adx.py
 airflow/providers/microsoft/azure/hooks/asb.py
 airflow/providers/microsoft/azure/hooks/base_azure.py
 airflow/providers/microsoft/azure/hooks/batch.py
 airflow/providers/microsoft/azure/hooks/container_instance.py
 airflow/providers/microsoft/azure/hooks/container_registry.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.2rc1/setup.py` & `apache-airflow-providers-microsoft-azure-6.2.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.2"
+version = "6.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
```

