# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar", last modified: Tue Jun 20 11:41:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar", last modified: Wed Jul  5 07:29:50 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.350021 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    35763 2023-06-20 11:41:43.351420 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34208 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.184249 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.185461 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.186767 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.245870 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.251883 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.257997 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.263989 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.281363 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    39267 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.287253 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.296090 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10368 2023-06-18 13:29:11.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.314088 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5209 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)    23192 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.347126 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    35763 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1893 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-20 11:41:43.353536 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.958422 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-05 07:29:50.959046 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.816293 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.817531 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.818692 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.865239 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.871145 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.877032 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.882992 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.898742 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    40772 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.910348 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.919973 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11941 2023-06-30 08:49:17.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.931804 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)    24797 2023-07-01 06:49:42.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.955701 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-05 07:29:50.960978 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.1.0"
+__version__ = "7.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "7.2.0",
             "7.1.0",
             "7.0.0",
             "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,16 @@
             extras = connection.extra_dejson
         else:
             extras = {}
         return extras
 
     def _get_field(self, field_name):
         """
+        Handles backcompat for extra fields.
+
         Prior to Airflow 2.3, in order to make use of UI customizations for extra fields,
         we needed to store them with the prefix ``extra__kubernetes__``. This method
         handles the backcompat, i.e. if the extra dict contains prefixed fields.
         """
         if field_name.startswith("extra__"):
             raise ValueError(
                 f"Got prefixed name {field_name}; please remove the 'extra__kubernetes__' prefix "
@@ -425,18 +427,15 @@
             label_selector=label_selector,
             _preload_content=False,
             **kwargs,
         )
 
 
 def _get_bool(val) -> bool | None:
-    """
-    Converts val to bool if can be done with certainty.
-    If we cannot infer intention we return None.
-    """
+    """Converts val to bool if can be done with certainty; if we cannot infer intention we return None."""
     if isinstance(val, bool):
         return val
     elif isinstance(val, str):
         if val.strip().lower() == "true":
             return True
         elif val.strip().lower() == "false":
             return False
@@ -565,17 +564,20 @@
             except async_client.ApiException as e:
                 # If the pod is already deleted
                 if e.status != 404:
                     raise
 
     async def read_logs(self, name: str, namespace: str):
         """
-        Reads logs inside the pod while starting containers inside. All the logs will be outputted with its
-        timestamp to track the logs after the execution of the pod is completed. The method is used for async
-        output of the logs only in the pod failed it execution or the task was cancelled by the user.
+        Reads logs inside the pod while starting containers inside.
+
+        All the logs will be outputted with its timestamp to track
+        the logs after the execution of the pod is completed. The
+        method is used for async output of the logs only in the pod
+        failed it execution or the task was cancelled by the user.
 
         :param name: Name of the pod.
         :param namespace: Name of the pod's namespace.
         """
         async with self.get_conn() as connection:
             try:
                 v1_api = async_client.CoreV1Api(connection)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 from __future__ import annotations
 
 import json
 import logging
 import re
 import secrets
 import string
+import warnings
 from collections.abc import Container
 from contextlib import AbstractContextManager
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
-from airflow.exceptions import AirflowException, AirflowSkipException
+from airflow.configuration import conf
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
 from airflow.kubernetes import pod_generator
 from airflow.kubernetes.pod_generator import PodGenerator
 from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
     convert_configmap,
@@ -48,14 +50,15 @@
     convert_volume,
     convert_volume_mount,
 )
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook
 from airflow.providers.cncf.kubernetes.triggers.pod import KubernetesPodTrigger
 from airflow.providers.cncf.kubernetes.utils import xcom_sidecar  # type: ignore[attr-defined]
 from airflow.providers.cncf.kubernetes.utils.pod_manager import (
+    OnFinishAction,
     PodLaunchFailedException,
     PodManager,
     PodOperatorHookProtocol,
     PodPhase,
     get_container_termination_message,
 )
 from airflow.settings import pod_mutation_hook
@@ -184,17 +187,14 @@
     :param config_file: The path to the Kubernetes config file. (templated)
         If not specified, default value is ``~/.kube/config``
     :param node_selector: A dict containing a group of scheduling rules.
     :param image_pull_secrets: Any image pull secrets to be given to the pod.
         If more than one secret is required, provide a
         comma separated list: secret_a,secret_b
     :param service_account_name: Name of the service account
-    :param is_delete_operator_pod: What to do when the pod reaches its final
-        state, or the execution is interrupted. If True (default), delete the
-        pod; if False, leave the pod.
     :param hostnetwork: If True enable host networking on the pod.
     :param tolerations: A list of kubernetes tolerations.
     :param security_context: security options the pod should run with (PodSecurityContext).
     :param container_security_context: security options the container should run with.
     :param dnspolicy: dnspolicy for the pod.
     :param dns_config: dns configuration (ip addresses, searches, options) for the pod.
     :param hostname: hostname for the pod.
@@ -222,14 +222,21 @@
     :param base_container_name: The name of the base container in the pod. This container's logs
         will appear as part of this task's logs if get_logs is True. Defaults to None. If None,
         will consult the class variable BASE_CONTAINER_NAME (which defaults to "base") for the base
         container name to use.
     :param deferrable: Run operator in the deferrable mode.
     :param poll_interval: Polling period in seconds to check for the status. Used only in deferrable mode.
     :param log_pod_spec_on_failure: Log the pod's specification if a failure occurs
+    :param on_finish_action: What to do when the pod reaches its final state, or the execution is interrupted.
+        If "delete_pod", the pod will be deleted regardless it's state; if "delete_succeeded_pod",
+        only succeeded pod will be deleted. You can set to "keep_pod" to keep the pod.
+    :param is_delete_operator_pod: What to do when the pod reaches its final
+        state, or the execution is interrupted. If True (default), delete the
+        pod; if False, leave the pod.
+        Deprecated - use `on_finish_action` instead.
     """
 
     # This field can be overloaded at the instance level via base_container_name
     BASE_CONTAINER_NAME = "base"
 
     POD_CHECKED_KEY = "already_checked"
     POST_TERMINATION_TIMEOUT = 120
@@ -275,15 +282,14 @@
         annotations: dict | None = None,
         container_resources: k8s.V1ResourceRequirements | None = None,
         affinity: k8s.V1Affinity | None = None,
         config_file: str | None = None,
         node_selector: dict | None = None,
         image_pull_secrets: list[k8s.V1LocalObjectReference] | None = None,
         service_account_name: str | None = None,
-        is_delete_operator_pod: bool = True,
         hostnetwork: bool = False,
         tolerations: list[k8s.V1Toleration] | None = None,
         security_context: dict | None = None,
         container_security_context: dict | None = None,
         dnspolicy: str | None = None,
         dns_config: k8s.V1PodDNSConfig | None = None,
         hostname: str | None = None,
@@ -296,17 +302,19 @@
         pod_template_file: str | None = None,
         priority_class_name: str | None = None,
         pod_runtime_info_envs: list[k8s.V1EnvVar] | None = None,
         termination_grace_period: int | None = None,
         configmaps: list[str] | None = None,
         skip_on_exit_code: int | Container[int] | None = None,
         base_container_name: str | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: float = 2,
         log_pod_spec_on_failure: bool = True,
+        on_finish_action: str = "delete_pod",
+        is_delete_operator_pod: None | bool = None,
         **kwargs,
     ) -> None:
         # TODO: remove in provider 6.0.0 release. This is a mitigate step to advise users to switch to the
         # container_resources parameter.
         if isinstance(kwargs.get("resources"), k8s.V1ResourceRequirements):
             raise AirflowException(
                 "Specifying resources for the launched pod with 'resources' is deprecated. "
@@ -346,15 +354,14 @@
         self.node_selector = node_selector or {}
         self.annotations = annotations or {}
         self.affinity = convert_affinity(affinity) if affinity else {}
         self.container_resources = container_resources
         self.config_file = config_file
         self.image_pull_secrets = convert_image_pull_secrets(image_pull_secrets) if image_pull_secrets else []
         self.service_account_name = service_account_name
-        self.is_delete_operator_pod = is_delete_operator_pod
         self.hostnetwork = hostnetwork
         self.tolerations = (
             [convert_toleration(toleration) for toleration in tolerations] if tolerations else []
         )
         self.security_context = security_context or {}
         self.container_security_context = container_security_context
         self.dnspolicy = dnspolicy
@@ -380,14 +387,28 @@
             else []
         )
         self.base_container_name = base_container_name or self.BASE_CONTAINER_NAME
         self.deferrable = deferrable
         self.poll_interval = poll_interval
         self.remote_pod: k8s.V1Pod | None = None
         self.log_pod_spec_on_failure = log_pod_spec_on_failure
+        if is_delete_operator_pod is not None:
+            warnings.warn(
+                "`is_delete_operator_pod` parameter is deprecated, please use `on_finish_action`",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            self.on_finish_action = (
+                OnFinishAction.DELETE_POD if is_delete_operator_pod else OnFinishAction.KEEP_POD
+            )
+            self.is_delete_operator_pod = is_delete_operator_pod
+        else:
+            self.on_finish_action = OnFinishAction(on_finish_action)
+            self.is_delete_operator_pod = self.on_finish_action == OnFinishAction.DELETE_POD
+
         self._config_dict: dict | None = None  # TODO: remove it when removing convert_config_file_to_dict
 
     @cached_property
     def _incluster_namespace(self):
         from pathlib import Path
 
         path = Path("/var/run/secrets/kubernetes.io/serviceaccount/namespace")
@@ -591,18 +612,18 @@
                 pod_namespace=self.pod.metadata.namespace,
                 trigger_start_time=trigger_start_time,
                 kubernetes_conn_id=self.kubernetes_conn_id,
                 cluster_context=self.cluster_context,
                 config_file=self.config_file,
                 in_cluster=self.in_cluster,
                 poll_interval=self.poll_interval,
-                should_delete_pod=self.is_delete_operator_pod,
                 get_logs=self.get_logs,
                 startup_timeout=self.startup_timeout_seconds,
                 base_container_name=self.base_container_name,
+                on_finish_action=self.on_finish_action.value,
             ),
             method_name="execute_complete",
         )
 
     def execute_complete(self, context: Context, event: dict, **kwargs):
         pod = None
         remote_pod = None
@@ -665,15 +686,16 @@
             pod=pod,
             remote_pod=remote_pod,
         )
 
     def cleanup(self, pod: k8s.V1Pod, remote_pod: k8s.V1Pod):
         pod_phase = remote_pod.status.phase if hasattr(remote_pod, "status") else None
 
-        if pod_phase != PodPhase.SUCCEEDED or not self.is_delete_operator_pod:
+        # if the pod fails or success, but we don't want to delete it
+        if pod_phase != PodPhase.SUCCEEDED or self.on_finish_action == OnFinishAction.KEEP_POD:
             self.patch_already_checked(remote_pod, reraise=False)
 
         if pod_phase != PodPhase.SUCCEEDED:
             if self.log_events_on_failure:
                 self._read_pod_events(pod, reraise=False)
 
             self.process_pod_deletion(remote_pod, reraise=False)
@@ -718,15 +740,19 @@
         with _optionally_suppress(reraise=reraise):
             for event in self.pod_manager.read_pod_events(pod).items:
                 self.log.error("Pod Event: %s - %s", event.reason, event.message)
 
     def process_pod_deletion(self, pod: k8s.V1Pod, *, reraise=True):
         with _optionally_suppress(reraise=reraise):
             if pod is not None:
-                if self.is_delete_operator_pod:
+                should_delete_pod = (self.on_finish_action == OnFinishAction.DELETE_POD) or (
+                    self.on_finish_action == OnFinishAction.DELETE_SUCCEEDED_POD
+                    and pod.status.phase == PodPhase.SUCCEEDED
+                )
+                if should_delete_pod:
                     self.log.info("Deleting pod: %s", pod.metadata.name)
                     self.pod_manager.delete_pod(pod)
                 else:
                     self.log.info("Skipping deleting pod: %s", pod.metadata.name)
 
     def _build_find_pod_label_selector(self, context: Context | None = None, *, exclude_checked=True) -> str:
         labels = self._get_ti_pod_labels(context, include_try_number=False)
@@ -863,14 +889,15 @@
         )
         pod_mutation_hook(pod)
         return pod
 
     def dry_run(self) -> None:
         """
         Prints out the pod definition that would be created by this operator.
+
         Does not include labels specific to the task instance (since there isn't
         one in a dry_run) and excludes all empty elements.
         """
         pod = self.build_pod_request_obj()
         print(yaml.dump(prune_dict(pod.to_dict(), mode="strict")))
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import datetime
 from typing import TYPE_CHECKING, Sequence
 
 from kubernetes.watch import Watch
 
+from airflow import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook, _load_body_to_dict
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -39,14 +41,15 @@
     :param application_file: Defines Kubernetes 'custom_resource_definition' of 'sparkApplication' as either a
         path to a '.yaml' file, '.json' file, YAML string or JSON string.
     :param namespace: kubernetes namespace to put sparkApplication
     :param kubernetes_conn_id: The :ref:`kubernetes connection id <howto/connection:kubernetes>`
         for the to Kubernetes cluster.
     :param api_group: kubernetes api group of sparkApplication
     :param api_version: kubernetes api version of sparkApplication
+    :param watch: whether to watch the job status and logs or not
     """
 
     template_fields: Sequence[str] = ("application_file", "namespace")
     template_ext: Sequence[str] = (".yaml", ".yml", ".json")
     ui_color = "#f4a460"
 
     def __init__(
@@ -56,67 +59,101 @@
         namespace: str | None = None,
         kubernetes_conn_id: str = "kubernetes_default",
         api_group: str = "sparkoperator.k8s.io",
         api_version: str = "v1beta2",
         in_cluster: bool | None = None,
         cluster_context: str | None = None,
         config_file: str | None = None,
+        watch: bool = False,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.namespace = namespace
         self.kubernetes_conn_id = kubernetes_conn_id
         self.api_group = api_group
         self.api_version = api_version
         self.plural = "sparkapplications"
         self.application_file = application_file
         self.in_cluster = in_cluster
         self.cluster_context = cluster_context
         self.config_file = config_file
+        self.watch = watch
 
         self.hook = KubernetesHook(
             conn_id=self.kubernetes_conn_id,
             in_cluster=self.in_cluster,
             config_file=self.config_file,
             cluster_context=self.cluster_context,
         )
 
     def execute(self, context: Context):
         body = _load_body_to_dict(self.application_file)
         name = body["metadata"]["name"]
         namespace = self.namespace or self.hook.get_namespace()
-        namespace_event_stream = Watch().stream(
-            self.hook.core_v1_client.list_namespaced_pod,
-            namespace=namespace,
-            _preload_content=False,
-            watch=True,
-            label_selector=f"sparkoperator.k8s.io/app-name={name},spark-role=driver",
-            field_selector="status.phase=Running",
-        )
 
-        self.hook.create_custom_object(
-            group=self.api_group,
-            version=self.api_version,
-            plural=self.plural,
-            body=body,
-            namespace=namespace,
-        )
-        for event in namespace_event_stream:
-            if event["type"] == "ADDED":
-                pod_log_stream = Watch().stream(
-                    self.hook.core_v1_client.read_namespaced_pod_log,
-                    name=f"{name}-driver",
+        response = None
+        is_job_created = False
+        if self.watch:
+            try:
+                namespace_event_stream = Watch().stream(
+                    self.hook.core_v1_client.list_namespaced_event,
                     namespace=namespace,
-                    _preload_content=False,
-                    timestamps=True,
+                    watch=True,
+                    field_selector=f"involvedObject.kind=SparkApplication,involvedObject.name={name}",
                 )
-                for line in pod_log_stream:
-                    self.log.info(line)
-            else:
-                break
+
+                response = self.hook.create_custom_object(
+                    group=self.api_group,
+                    version=self.api_version,
+                    plural=self.plural,
+                    body=body,
+                    namespace=namespace,
+                )
+                is_job_created = True
+                for event in namespace_event_stream:
+                    obj = event["object"]
+                    if event["object"].last_timestamp >= datetime.datetime.strptime(
+                        response["metadata"]["creationTimestamp"], "%Y-%m-%dT%H:%M:%S%z"
+                    ):
+                        self.log.info(obj.message)
+                        if obj.reason == "SparkDriverRunning":
+                            pod_log_stream = Watch().stream(
+                                self.hook.core_v1_client.read_namespaced_pod_log,
+                                name=f"{name}-driver",
+                                namespace=namespace,
+                                timestamps=True,
+                            )
+                            for line in pod_log_stream:
+                                self.log.info(line)
+                        elif obj.reason in [
+                            "SparkApplicationSubmissionFailed",
+                            "SparkApplicationFailed",
+                            "SparkApplicationDeleted",
+                        ]:
+                            is_job_created = False
+                            raise AirflowException(obj.message)
+                        elif obj.reason == "SparkApplicationCompleted":
+                            break
+                        else:
+                            continue
+            except Exception:
+                if is_job_created:
+                    self.on_kill()
+                raise
+
+        else:
+            response = self.hook.create_custom_object(
+                group=self.api_group,
+                version=self.api_version,
+                plural=self.plural,
+                body=body,
+                namespace=namespace,
+            )
+
+        return response
 
     def on_kill(self) -> None:
         body = _load_body_to_dict(self.application_file)
         name = body["metadata"]["name"]
         namespace = self.namespace or self.hook.get_namespace()
         self.hook.delete_custom_object(
             group=self.api_group,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,30 +13,33 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import asyncio
+import warnings
 from asyncio import CancelledError
 from datetime import datetime
 from enum import Enum
 from typing import Any, AsyncIterator
 
 import pytz
 from kubernetes_asyncio.client.models import V1Pod
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import AsyncKubernetesHook
-from airflow.providers.cncf.kubernetes.utils.pod_manager import PodPhase
+from airflow.providers.cncf.kubernetes.utils.pod_manager import OnFinishAction, PodPhase
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class ContainerState(str, Enum):
     """
-    Possible container states
+    Possible container states.
+
     See https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/#pod-phase.
     """
 
     WAITING = "waiting"
     RUNNING = "running"
     TERMINATED = "terminated"
     FAILED = "failed"
@@ -52,50 +55,67 @@
     :param kubernetes_conn_id: The :ref:`kubernetes connection id <howto/connection:kubernetes>`
         for the Kubernetes cluster.
     :param cluster_context: Context that points to kubernetes cluster.
     :param config_file: Path to kubeconfig file.
     :param poll_interval: Polling period in seconds to check for the status.
     :param trigger_start_time: time in Datetime format when the trigger was started
     :param in_cluster: run kubernetes client with in_cluster configuration.
+    :param get_logs: get the stdout of the container as logs of the tasks.
+    :param startup_timeout: timeout in seconds to start up the pod.
+    :param on_finish_action: What to do when the pod reaches its final state, or the execution is interrupted.
+        If "delete_pod", the pod will be deleted regardless it's state; if "delete_succeeded_pod",
+        only succeeded pod will be deleted. You can set to "keep_pod" to keep the pod.
     :param should_delete_pod: What to do when the pod reaches its final
         state, or the execution is interrupted. If True (default), delete the
         pod; if False, leave the pod.
-    :param get_logs: get the stdout of the container as logs of the tasks.
-    :param startup_timeout: timeout in seconds to start up the pod.
+        Deprecated - use `on_finish_action` instead.
     """
 
     def __init__(
         self,
         pod_name: str,
         pod_namespace: str,
         trigger_start_time: datetime,
         base_container_name: str,
         kubernetes_conn_id: str | None = None,
         poll_interval: float = 2,
         cluster_context: str | None = None,
         config_file: str | None = None,
         in_cluster: bool | None = None,
-        should_delete_pod: bool = True,
         get_logs: bool = True,
         startup_timeout: int = 120,
+        on_finish_action: str = "delete_pod",
+        should_delete_pod: bool | None = None,
     ):
         super().__init__()
         self.pod_name = pod_name
         self.pod_namespace = pod_namespace
         self.trigger_start_time = trigger_start_time
         self.base_container_name = base_container_name
         self.kubernetes_conn_id = kubernetes_conn_id
         self.poll_interval = poll_interval
         self.cluster_context = cluster_context
         self.config_file = config_file
         self.in_cluster = in_cluster
-        self.should_delete_pod = should_delete_pod
         self.get_logs = get_logs
         self.startup_timeout = startup_timeout
 
+        if should_delete_pod is not None:
+            warnings.warn(
+                "`should_delete_pod` parameter is deprecated, please use `on_finish_action`",
+                AirflowProviderDeprecationWarning,
+            )
+            self.on_finish_action = (
+                OnFinishAction.DELETE_POD if should_delete_pod else OnFinishAction.KEEP_POD
+            )
+            self.should_delete_pod = should_delete_pod
+        else:
+            self.on_finish_action = OnFinishAction(on_finish_action)
+            self.should_delete_pod = self.on_finish_action == OnFinishAction.DELETE_POD
+
         self._hook: AsyncKubernetesHook | None = None
         self._since_time = None
 
     def serialize(self) -> tuple[str, dict[str, Any]]:
         """Serializes KubernetesCreatePodTrigger arguments and classpath."""
         return (
             "airflow.providers.cncf.kubernetes.triggers.pod.KubernetesPodTrigger",
@@ -104,18 +124,19 @@
                 "pod_namespace": self.pod_namespace,
                 "base_container_name": self.base_container_name,
                 "kubernetes_conn_id": self.kubernetes_conn_id,
                 "poll_interval": self.poll_interval,
                 "cluster_context": self.cluster_context,
                 "config_file": self.config_file,
                 "in_cluster": self.in_cluster,
-                "should_delete_pod": self.should_delete_pod,
                 "get_logs": self.get_logs,
                 "startup_timeout": self.startup_timeout,
                 "trigger_start_time": self.trigger_start_time,
+                "should_delete_pod": self.should_delete_pod,
+                "on_finish_action": self.on_finish_action.value,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:  # type: ignore[override]
         """Gets current pod status and yields a TriggerEvent."""
         hook = self._get_async_hook()
         self.log.info("Checking pod %r in namespace %r.", self.pod_name, self.pod_namespace)
@@ -129,23 +150,31 @@
                 pod_status = pod.status.phase
                 self.log.debug("Pod %s status: %s", self.pod_name, pod_status)
 
                 container_state = self.define_container_state(pod)
                 self.log.debug("Container %s status: %s", self.base_container_name, container_state)
 
                 if container_state == ContainerState.TERMINATED:
-                    yield TriggerEvent(
-                        {
-                            "name": self.pod_name,
-                            "namespace": self.pod_namespace,
-                            "status": "success",
-                            "message": "All containers inside pod have started successfully.",
-                        }
-                    )
-                    return
+                    if pod_status not in PodPhase.terminal_states:
+                        self.log.info(
+                            "Pod %s is still running. Sleeping for %s seconds.",
+                            self.pod_name,
+                            self.poll_interval,
+                        )
+                        await asyncio.sleep(self.poll_interval)
+                    else:
+                        yield TriggerEvent(
+                            {
+                                "name": self.pod_name,
+                                "namespace": self.pod_namespace,
+                                "status": "success",
+                                "message": "All containers inside pod have started successfully.",
+                            }
+                        )
+                        return
                 elif self.should_wait(pod_phase=pod_status, container_state=container_state):
                     self.log.info("Container is not completed and still working.")
 
                     if pod_status == PodPhase.PENDING and container_state == ContainerState.UNDEFINED:
                         delta = datetime.now(tz=pytz.UTC) - self.trigger_start_time
                         if delta.total_seconds() >= self.startup_timeout:
                             message = (
@@ -178,15 +207,15 @@
                 # That means that task was marked as failed
                 if self.get_logs:
                     self.log.info("Outputting container logs...")
                     await self._get_async_hook().read_logs(
                         name=self.pod_name,
                         namespace=self.pod_namespace,
                     )
-                if self.should_delete_pod:
+                if self.on_finish_action == OnFinishAction.DELETE_POD:
                     self.log.info("Deleting pod...")
                     await self._get_async_hook().delete_pod(
                         name=self.pod_name,
                         namespace=self.pod_namespace,
                     )
                 yield TriggerEvent(
                     {
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,18 +138,15 @@
         resp = getattr(k8s_api, f"delete_{kind}")(name=name, body=body, **kwargs)
     if verbose:
         print(f"{kind} deleted. status='{str(resp.status)}'")
     return resp
 
 
 class FailToDeleteError(Exception):
-    """
-    An exception class for handling error if an error occurred when
-    handling a yaml file during deletion of the resource.
-    """
+    """For handling error if an error occurred when handling a yaml file during deletion of the resource."""
 
     def __init__(self, api_exceptions: list):
         self.api_exceptions = api_exceptions
 
     def __str__(self):
         msg = ""
         for api_exception in self.api_exceptions:
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Launches PODs."""
 from __future__ import annotations
 
+import enum
 import json
 import logging
 import math
 import time
 import warnings
 from contextlib import closing, suppress
 from dataclasses import dataclass
@@ -59,15 +60,16 @@
     if isinstance(exception, ApiException):
         return exception.status == 409
     return False
 
 
 class PodPhase:
     """
-    Possible pod phases
+    Possible pod phases.
+
     See https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/#pod-phase.
     """
 
     PENDING = "Pending"
     RUNNING = "Running"
     FAILED = "Failed"
     SUCCEEDED = "Succeeded"
@@ -110,25 +112,27 @@
         return next((x for x in container_statuses if x.name == container_name), None)
     return None
 
 
 def container_is_running(pod: V1Pod, container_name: str) -> bool:
     """
     Examines V1Pod ``pod`` to determine whether ``container_name`` is running.
+
     If that container is present and running, returns True.  Returns False otherwise.
     """
     container_status = get_container_status(pod, container_name)
     if not container_status:
         return False
     return container_status.state.running is not None
 
 
 def container_is_terminated(pod: V1Pod, container_name: str) -> bool:
     """
     Examines V1Pod ``pod`` to determine whether ``container_name`` is terminated.
+
     If that container is present and terminated, returns True.  Returns False otherwise.
     """
     container_statuses = pod.status.container_statuses if pod and pod.status else None
     if not container_statuses:
         return False
     container_status = next((x for x in container_statuses if x.name == container_name), None)
     if not container_status:
@@ -141,16 +145,15 @@
         container_statuses = pod.status.container_statuses
         container_status = next((x for x in container_statuses if x.name == container_name), None)
         return container_status.state.terminated.message if container_status else None
 
 
 class PodLogsConsumer:
     """
-    PodLogsConsumer is responsible for pulling pod logs from a stream with checking a container status before
-    reading data.
+    Responsible for pulling pod logs from a stream with checking a container status before reading data.
 
     This class is a workaround for the issue https://github.com/apache/airflow/issues/23497.
 
     :param response: HTTP response with logs
     :param pod: Pod instance from Kubernetes client
     :param pod_manager: Pod manager instance
     :param container_name: Name of the container that we're reading logs from
@@ -235,18 +238,15 @@
     """Used for returning the status of the pod and last log time when exiting from `fetch_container_logs`."""
 
     running: bool
     last_log_time: DateTime | None
 
 
 class PodManager(LoggingMixin):
-    """
-    Helper class for creating, monitoring, and otherwise interacting with Kubernetes pods
-    for use with the KubernetesPodOperator.
-    """
+    """Create, monitor, and otherwise interact with Kubernetes pods for use with the KubernetesPodOperator."""
 
     def __init__(
         self,
         kube_client: client.CoreV1Api,
     ):
         """
         Creates the launcher.
@@ -354,14 +354,15 @@
             before=before_log(self.log, logging.INFO),
         )
         def consume_logs(
             *, since_time: DateTime | None = None, follow: bool = True, termination_timeout: int = 120
         ) -> DateTime | None:
             """
             Tries to follow container logs until container completes.
+
             For a long-running container, sometimes the log read may be interrupted
             Such errors of this kind are suppressed.
 
             Returns the last timestamp observed in logs.
             """
             timestamp = None
             try:
@@ -540,14 +541,27 @@
             if not warned:
                 self.log.warning("The xcom sidecar container is not yet started.")
                 warned = True
             time.sleep(1)
 
     def extract_xcom(self, pod: V1Pod) -> str:
         """Retrieves XCom value and kills xcom sidecar container."""
+        try:
+            result = self.extract_xcom_json(pod)
+            return result
+        finally:
+            self.extract_xcom_kill(pod)
+
+    @tenacity.retry(
+        stop=tenacity.stop_after_attempt(5),
+        wait=tenacity.wait_exponential(multiplier=1, min=4, max=10),
+        reraise=True,
+    )
+    def extract_xcom_json(self, pod: V1Pod) -> str:
+        """Retrieves XCom value and also checks if xcom json is valid."""
         with closing(
             kubernetes_stream(
                 self._client.connect_get_namespaced_pod_exec,
                 pod.metadata.name,
                 pod.metadata.namespace,
                 container=PodDefaults.SIDECAR_CONTAINER_NAME,
                 command=["/bin/sh"],
@@ -558,19 +572,46 @@
                 _preload_content=False,
             )
         ) as resp:
             result = self._exec_pod_command(
                 resp,
                 f"if [ -s {PodDefaults.XCOM_MOUNT_PATH}/return.json ]; then cat {PodDefaults.XCOM_MOUNT_PATH}/return.json; else echo __airflow_xcom_result_empty__; fi",  # noqa
             )
-            self._exec_pod_command(resp, "kill -s SIGINT 1")
+            if result and result.rstrip() != "__airflow_xcom_result_empty__":
+                # Note: result string is parsed to check if its valid json.
+                # This function still returns a string which is converted into json in the calling method.
+                json.loads(result)
+
         if result is None:
             raise AirflowException(f"Failed to extract xcom from pod: {pod.metadata.name}")
         return result
 
+    @tenacity.retry(
+        stop=tenacity.stop_after_attempt(5),
+        wait=tenacity.wait_exponential(multiplier=1, min=4, max=10),
+        reraise=True,
+    )
+    def extract_xcom_kill(self, pod: V1Pod):
+        """Kills xcom sidecar container."""
+        with closing(
+            kubernetes_stream(
+                self._client.connect_get_namespaced_pod_exec,
+                pod.metadata.name,
+                pod.metadata.namespace,
+                container=PodDefaults.SIDECAR_CONTAINER_NAME,
+                command=["/bin/sh"],
+                stdin=True,
+                stdout=True,
+                stderr=True,
+                tty=False,
+                _preload_content=False,
+            )
+        ) as resp:
+            self._exec_pod_command(resp, "kill -s SIGINT 1")
+
     def _exec_pod_command(self, resp, command: str) -> str | None:
         res = None
         if resp.is_open():
             self.log.info("Running command... %s\n", command)
             resp.write_stdin(command + "\n")
             while resp.is_open():
                 resp.update(timeout=1)
@@ -581,7 +622,15 @@
                     error_res = error_res + resp.read_stderr() if error_res else resp.read_stderr()
                 if error_res:
                     self.log.info("stderr from command: %s", error_res)
                     break
                 if res:
                     return res
         return res
+
+
+class OnFinishAction(enum.Enum):
+    """Action to take when the pod finishes."""
+
+    KEEP_POD = "keep_pod"
+    DELETE_POD = "delete_pod"
+    DELETE_SUCCEEDED_POD = "delete_succeeded_pod"
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""
-This module handles all xcom functionality for the KubernetesPodOperator
-by attaching a sidecar container that blocks the pod from completing until
-Airflow has pulled result data into the worker for xcom serialization.
-"""
+"""Attach a sidecar container that blocks the pod from completing until Airflow pulls result data."""
 from __future__ import annotations
 
 import copy
 
 from kubernetes.client import models as k8s
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.1.0"
+version = "7.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

