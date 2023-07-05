# Comparing `tmp/linien-client-0.8.0rc6.tar.gz` & `tmp/linien-client-0.8.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-0.8.0rc6.tar", last modified: Mon Jul  3 14:23:17 2023, max compression
+gzip compressed data, was "linien-client-0.8.0rc8.tar", last modified: Wed Jul  5 09:24:09 2023, max compression
```

## Comparing `linien-client-0.8.0rc6.tar` & `linien-client-0.8.0rc8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:17.638093 linien-client-0.8.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 14:23:17.638093 linien-client-0.8.0rc6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:17.638093 linien-client-0.8.0rc6/linien_client/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:17.638093 linien-client-0.8.0rc6/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 14:23:17.000000 linien-client-0.8.0rc6/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 14:23:17.000000 linien-client-0.8.0rc6/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:23:17.000000 linien-client-0.8.0rc6/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 14:23:17.000000 linien-client-0.8.0rc6/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 14:23:17.000000 linien-client-0.8.0rc6/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:23:17.642093 linien-client-0.8.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 14:22:35.000000 linien-client-0.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/setup.py
```

### Comparing `linien-client-0.8.0rc6/PKG-INFO` & `linien-client-0.8.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc6/linien_client/communication.py` & `linien-client-0.8.0rc8/linien_client/communication.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc6/linien_client/connection.py` & `linien-client-0.8.0rc8/linien_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,28 +24,33 @@
 from typing import Callable, Optional
 
 import rpyc
 from linien_common.config import DEFAULT_SERVER_PORT
 
 from . import __version__
 from .communication import LinienControlService
-from .deploy import start_remote_server
+from .deploy import hash_username_and_password, start_remote_server
 from .exceptions import (
-    GeneralConnectionErrorException,
+    GeneralConnectionError,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotRunningException,
 )
 from .remote_parameters import RemoteParameters
 
 
-class RPYCServiceWithUUID(rpyc.Service):
-    def __init__(self, uuid: str):
+class ServiceWithAuth(rpyc.Service):
+    def __init__(self, uuid: str, user: str, password: str) -> None:
         super().__init__()
         self.exposed_uuid = uuid
+        self.auth_hash = hash_username_and_password(user, password).encode("utf-8")
+
+    def _connect(self, channel, config):
+        channel.stream.sock.send(self.auth_hash)  # send hash before rpyc takes over
+        return super()._connect(channel, config)
 
 
 class LinienClient:
     def __init__(
         self,
         host: str,
         user: str,
@@ -64,15 +69,15 @@
             # RP is configured such that "localhost" doesn't point to 127.0.0.1 in all
             # cases
             self.host = "127.0.0.1"
 
         self.uuid = "".join(random.choice(string.ascii_lowercase) for _ in range(10))
 
         # for exposing client's uuid to server
-        self.client_service = RPYCServiceWithUUID(self.uuid)
+        self.client_service = ServiceWithAuth(self.uuid, self.user, self.password)
 
     def connect(
         self,
         autostart_server: bool,
         use_parameter_cache: bool,
         call_on_error: Optional[Callable] = None,
     ) -> None:
@@ -124,15 +129,15 @@
                         print_exc()
                         print(
                             "Error: connection to the server could not be established"
                         )
                         break
 
         if self.connection is None:
-            raise GeneralConnectionErrorException()
+            raise GeneralConnectionError()
 
         # now check that the remote version is the same as ours
         remote_version = self.connection.root.exposed_get_server_version().split("+")[0]
         local_version = __version__.split("+")[0]
 
         if (remote_version != local_version) and not ("dev" in local_version):
             raise InvalidServerVersionException(local_version, remote_version)
```

### Comparing `linien-client-0.8.0rc6/linien_client/deploy.py` & `linien-client-0.8.0rc8/linien_client/deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import linien_client
 from fabric import Connection
 from linien_client.exceptions import (
     InvalidServerVersionException,
     ServerNotInstalledException,
 )
+from linien_common.communication import hash_username_and_password
 
 
 def read_remote_version(
     host: str, user: str, password: str, port: int = 22, out_stream=sys.stdout
 ) -> str:
     """Read the remote version of linien."""
 
@@ -68,14 +69,22 @@
         local_version = linien_client.__version__.split("+")[0]
         remote_version = read_remote_version(host, user, password, port).split("+")[0]
 
         if (local_version != remote_version) and not ("dev" in local_version):
             raise InvalidServerVersionException(local_version, remote_version)
 
         conn.run(
+            'python3 -c "from linien_common.communication import write_hash_to_file;'
+            f"write_hash_to_file('{hash_username_and_password(user, password)}')\"",
+            out_stream=out_stream,
+            err_stream=out_stream,
+            warn=True,
+        )
+
+        conn.run(
             "linien_start_server.sh",
             out_stream=out_stream,
             err_stream=out_stream,
             warn=True,
         )
```

### Comparing `linien-client-0.8.0rc6/linien_client/exceptions.py` & `linien-client-0.8.0rc8/linien_client/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,9 +44,9 @@
         )
 
 
 class ServerNotInstalledException(Exception):
     pass
 
 
-class GeneralConnectionErrorException(Exception):
+class GeneralConnectionError(Exception):
     pass
```

### Comparing `linien-client-0.8.0rc6/linien_client/remote_parameters.py` & `linien-client-0.8.0rc8/linien_client/remote_parameters.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc6/linien_client.egg-info/PKG-INFO` & `linien-client-0.8.0rc8/linien_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc6/setup.py` & `linien-client-0.8.0rc8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc6"
+version = "0.8.0rc8"
 
 setup(
     name="linien-client",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
```

