# Comparing `tmp/apache-airflow-providers-trino-5.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-trino-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-trino-5.1.1rc1.tar", last modified: Tue Jun 20 11:43:27 2023, max compression
+gzip compressed data, was "apache-airflow-providers-trino-5.2.0rc1.tar", last modified: Wed Jul  5 07:30:34 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.1.1rc1.tar` & `apache-airflow-providers-trino-5.2.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.095581 apache-airflow-providers-trino-5.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14638 2023-06-20 11:43:27.096913 apache-airflow-providers-trino-5.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13063 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.000669 apache-airflow-providers-trino-5.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.001882 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.041528 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.048823 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9387 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.055590 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.063905 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.092900 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14638 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-trino-5.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1904 2023-06-20 11:43:27.099356 apache-airflow-providers-trino-5.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:34.041403 apache-airflow-providers-trino-5.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-05 07:30:34.042484 apache-airflow-providers-trino-5.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.932620 apache-airflow-providers-trino-5.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.933834 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.970786 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-05 07:19:39.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.978141 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-06-25 14:35:06.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.986231 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.997483 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:34.037432 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-trino-5.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-05 07:30:34.045371 apache-airflow-providers-trino-5.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-trino-5.1.1rc1/LICENSE` & `apache-airflow-providers-trino-5.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/MANIFEST.in` & `apache-airflow-providers-trino-5.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.1.1"
+__version__ = "5.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-trino",
         "name": "Trino",
         "description": "`Trino <https://trino.io/>`__\n",
         "suspended": False,
         "versions": [
+            "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.0",
```

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/trino.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,20 @@
         auth = None
         user = db.login
         if db.password and extra.get("auth") in ("kerberos", "certs"):
             raise AirflowException(f"The {extra.get('auth')!r} authorization type doesn't support password.")
         elif db.password:
             auth = trino.auth.BasicAuthentication(db.login, db.password)  # type: ignore[attr-defined]
         elif extra.get("auth") == "jwt":
-            auth = trino.auth.JWTAuthentication(token=extra.get("jwt__token"))
+            if "jwt__file" in extra:
+                with open(extra.get("jwt__file")) as jwt_file:
+                    token = jwt_file.read()
+            else:
+                token = extra.get("jwt__token")
+            auth = trino.auth.JWTAuthentication(token=token)
         elif extra.get("auth") == "certs":
             auth = trino.auth.CertificateAuthentication(
                 extra.get("certs__client_cert_path"),
                 extra.get("certs__client_key_path"),
             )
         elif extra.get("auth") == "kerberos":
             auth = trino.auth.KerberosAuthentication(  # type: ignore[attr-defined]
```

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.1rc1/pyproject.toml` & `apache-airflow-providers-trino-5.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-trino-5.1.1rc1/setup.cfg` & `apache-airflow-providers-trino-5.2.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-trino-5.1.1rc1/setup.py` & `apache-airflow-providers-trino-5.2.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-trino package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.1"
+version = "5.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-trino setup."""
     setup(
         version=version,
         extras_require={
```

