# Comparing `tmp/apache-airflow-providers-vertica-3.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-vertica-3.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-vertica-3.4.1rc1.tar", last modified: Tue Jun 20 11:43:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-vertica-3.5.0rc1.tar", last modified: Wed Jul  5 07:30:35 2023, max compression
```

## Comparing `apache-airflow-providers-vertica-3.4.1rc1.tar` & `apache-airflow-providers-vertica-3.5.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.961929 apache-airflow-providers-vertica-3.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:27.000000 apache-airflow-providers-vertica-3.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12246 2023-06-20 11:43:28.962920 apache-airflow-providers-vertica-3.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10688 2023-06-20 11:43:27.000000 apache-airflow-providers-vertica-3.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.890775 apache-airflow-providers-vertica-3.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.891897 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.923664 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-20 11:43:27.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.929756 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-02 11:31:21.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/hooks/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.935423 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/operators/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:28.959368 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12246 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      731 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:28.000000 apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-vertica-3.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1907 2023-06-20 11:43:28.964934 apache-airflow-providers-vertica-3.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-06-20 11:43:27.000000 apache-airflow-providers-vertica-3.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.940806 apache-airflow-providers-vertica-3.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-05 07:30:35.941670 apache-airflow-providers-vertica-3.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3983 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.854082 apache-airflow-providers-vertica-3.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.855783 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.894887 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 07:19:39.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.901863 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-30 08:49:17.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.908735 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.937335 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-vertica-3.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-05 07:30:35.944513 apache-airflow-providers-vertica-3.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/LICENSE` & `apache-airflow-providers-vertica-3.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/MANIFEST.in` & `apache-airflow-providers-vertica-3.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.1"
+__version__ = "3.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/get_provider_info.py` & `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-vertica",
         "name": "Vertica",
         "description": "`Vertica <https://www.vertica.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.5.0",
             "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
```

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/hooks/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/operators/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/airflow/providers/vertica/operators/vertica.py` & `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/vertica.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt` & `apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/pyproject.toml` & `apache-airflow-providers-vertica-3.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/setup.cfg` & `apache-airflow-providers-vertica-3.5.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-vertica-3.4.1rc1/setup.py` & `apache-airflow-providers-vertica-3.5.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-vertica package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.1"
+version = "3.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-vertica setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

