# Comparing `tmp/apache-airflow-providers-hashicorp-3.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-hashicorp-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:16 2023, max compression
+gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.2rc1.tar", last modified: Wed Jul  5 07:30:12 2023, max compression
```

## Comparing `apache-airflow-providers-hashicorp-3.4.1rc1.tar` & `apache-airflow-providers-hashicorp-3.4.2rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.318517 apache-airflow-providers-hashicorp-3.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13211 2023-06-20 11:42:16.319613 apache-airflow-providers-hashicorp-3.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11651 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.231924 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.233137 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.272212 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.278286 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20545 2023-06-01 07:44:14.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.284373 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.291964 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11991 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.315683 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13211 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-hashicorp-3.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-20 11:42:16.321603 apache-airflow-providers-hashicorp-3.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:12.040607 apache-airflow-providers-hashicorp-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-05 07:30:12.041425 apache-airflow-providers-hashicorp-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.912613 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.915791 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.968515 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.978383 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21223 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.988449 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.998308 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:12.035782 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-hashicorp-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-05 07:30:12.043814 apache-airflow-providers-hashicorp-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/LICENSE` & `apache-airflow-providers-hashicorp-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/MANIFEST.in` & `apache-airflow-providers-hashicorp-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from __future__ import annotations
 
 from functools import cached_property
 
 import hvac
 from hvac.api.auth_methods import Kubernetes
 from hvac.exceptions import InvalidPath, VaultError
-from requests import Response
+from requests import Response, Session
+from requests.adapters import HTTPAdapter
+from urllib3.util import Retry
 
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 DEFAULT_KUBERNETES_JWT_PATH = "/var/run/secrets/kubernetes.io/serviceaccount/token"
 DEFAULT_KV_ENGINE_VERSION = 2
 
 
@@ -42,18 +44,20 @@
     "token",
     "userpass",
 ]
 
 
 class _VaultClient(LoggingMixin):
     """
-    Retrieves Authenticated client from Hashicorp Vault. This is purely internal class promoting
-    authentication code reuse between the Hook and the SecretBackend, it should not be used directly in
-    Airflow DAGs. Use VaultBackend for backend integration and Hook in case you want to communicate
-    with VaultHook using standard Airflow Connection definition.
+    Retrieves Authenticated client from Hashicorp Vault.
+
+    This is purely internal class promoting authentication code reuse between the Hook and the
+    SecretBackend, it should not be used directly in Airflow DAGs. Use VaultBackend for backend
+    integration and Hook in case you want to communicate with VaultHook using standard Airflow
+    Connection definition.
 
     :param url: Base URL for the Vault instance being addressed.
     :param auth_type: Authentication Type for Vault. Default is ``token``. Available values are in
         ('approle', 'aws_iam', 'azure', 'github', 'gcp', 'kubernetes', 'ldap', 'radius', 'token', 'userpass')
     :param auth_mount_point: It can be used to define mount_point for authentication chosen
           Default depends on the authentication method used.
     :param mount_point: The "path" the secret engine was mounted on. Default is "secret". Note that
@@ -166,20 +170,17 @@
         self.radius_host = radius_host
         self.radius_secret = radius_secret
         self.radius_port = radius_port
 
     @property
     def client(self):
         """
-        Authentication to Vault can expire. This wrapper function checks that
-        it is still authenticated to Vault, and invalidates the cache if this
-        is not the case.
+        Checks that it is still authenticated to Vault and invalidates the cache if this is not the case.
 
         :return: Vault Client
-
         """
         if not self._client.is_authenticated():
             # Invalidate the cache:
             # https://github.com/pydanny/cached-property#invalidating-the-cache
             self.__dict__.pop("_client", None)
         return self._client
 
@@ -187,14 +188,30 @@
     def _client(self) -> hvac.Client:
         """
         Return an authenticated Hashicorp Vault client.
 
         :return: Vault Client
 
         """
+        if "session" not in self.kwargs:
+            # If no session object provide one with retry as per hvac documentation:
+            # https://hvac.readthedocs.io/en/stable/advanced_usage.html#retrying-failed-requests
+            adapter = HTTPAdapter(
+                max_retries=Retry(
+                    total=3,
+                    backoff_factor=0.1,
+                    status_forcelist=[412, 500, 502, 503],
+                    raise_on_status=False,
+                )
+            )
+            session = Session()
+            session.mount("http://", adapter)
+            session.mount("https://", adapter)
+            self.kwargs["session"] = session
+
         _client = hvac.Client(url=self.url, **self.kwargs)
         if self.auth_type == "approle":
             self._auth_approle(_client)
         elif self.auth_type == "aws_iam":
             self._auth_aws_iam(_client)
         elif self.auth_type == "azure":
             self._auth_azure(_client)
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/get_provider_info.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-hashicorp",
         "name": "Hashicorp",
         "description": "Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.2",
             "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.1",
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/vault.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/vault.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,17 @@
     # Make sure connection is imported this way for type checking, otherwise when importing
     # the backend it will get a circular dependency and fail
     if TYPE_CHECKING:
         from airflow.models.connection import Connection
 
     def get_connection(self, conn_id: str) -> Connection | None:
         """
-        Get connection from Vault as secret. Prioritize conn_uri if exists,
-        if not fall back to normal Connection creation.
+        Get connection from Vault as secret.
+
+        Prioritize conn_uri if exists, if not fall back to normal Connection creation.
 
         :return: A Connection object constructed from Vault data
         """
         # The Connection needs to be locally imported because otherwise we get into cyclic import
         # problems when instantiating the backend during configuration
         from airflow.models.connection import Connection
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt` & `apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/pyproject.toml` & `apache-airflow-providers-hashicorp-3.4.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/setup.cfg` & `apache-airflow-providers-hashicorp-3.4.2rc1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1rc1/setup.py` & `apache-airflow-providers-hashicorp-3.4.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-hashicorp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.1"
+version = "3.4.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-hashicorp setup."""
     setup(
         version=version,
         extras_require={"google": ["apache-airflow-providers-google"]},
```

