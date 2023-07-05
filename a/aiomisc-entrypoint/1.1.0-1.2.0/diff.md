# Comparing `tmp/aiomisc_entrypoint-1.1.0.tar.gz` & `tmp/aiomisc_entrypoint-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomisc_entrypoint-1.1.0.tar", max compression
+gzip compressed data, was "aiomisc_entrypoint-1.2.0.tar", max compression
```

## Comparing `aiomisc_entrypoint-1.1.0.tar` & `aiomisc_entrypoint-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1156 2023-01-17 09:01:46.923921 aiomisc_entrypoint-1.1.0/README.md
--rw-r--r--   0        0        0      606 2023-03-17 03:31:14.751369 aiomisc_entrypoint-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-01-16 14:51:58.126224 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/__init__.py
--rw-r--r--   0        0        0     1012 2023-03-17 03:31:14.751544 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/abstractions.py
--rw-r--r--   0        0        0     3109 2023-03-17 03:31:14.752156 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/entrypoint.py
--rw-r--r--   0        0        0      351 2023-03-17 03:31:14.754875 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/__init__.py
--rw-r--r--   0        0        0      898 2023-03-17 03:31:14.755918 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/change_user.py
--rw-r--r--   0        0        0      553 2023-03-17 03:31:14.756357 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/clear_environ.py
--rw-r--r--   0        0        0     2503 2023-03-17 03:31:14.756975 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/svc_dependency.py
--rw-r--r--   0        0        0     1344 2023-03-17 03:31:14.757465 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/svc_to_context.py
--rw-r--r--   0        0        0     1496 2023-03-17 03:31:14.757770 aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/sys_signals.py
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 aiomisc_entrypoint-1.1.0/setup.py
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 aiomisc_entrypoint-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1156 2023-01-17 09:01:46.923921 aiomisc_entrypoint-1.2.0/README.md
+-rw-r--r--   0        0        0      600 2023-07-05 08:20:04.055601 aiomisc_entrypoint-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-01-16 14:51:58.126224 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/__init__.py
+-rw-r--r--   0        0        0     1012 2023-03-17 03:31:14.751544 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/abstractions.py
+-rw-r--r--   0        0        0     3116 2023-07-05 08:20:04.055749 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/entrypoint.py
+-rw-r--r--   0        0        0      351 2023-03-17 03:31:14.754875 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/__init__.py
+-rw-r--r--   0        0        0      898 2023-03-17 03:31:14.755918 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/change_user.py
+-rw-r--r--   0        0        0      553 2023-03-17 03:31:14.756357 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/clear_environ.py
+-rw-r--r--   0        0        0     2503 2023-03-17 03:31:14.756975 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/svc_dependency.py
+-rw-r--r--   0        0        0     1344 2023-03-17 03:31:14.757465 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/svc_to_context.py
+-rw-r--r--   0        0        0     1496 2023-03-17 03:31:14.757770 aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/sys_signals.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 aiomisc_entrypoint-1.2.0/PKG-INFO
```

### Comparing `aiomisc_entrypoint-1.1.0/README.md` & `aiomisc_entrypoint-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/abstractions.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/abstractions.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/entrypoint.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self._entrypoint.post_start.connect(processor.post_start)
         self._entrypoint.pre_stop.connect(processor.pre_stop)
         self._entrypoint.post_stop.connect(processor.post_stop)
         processor.set_entrypoint_proxy(self)
 
     def run_until_complete(self, coro: t.Awaitable):
         with self._entrypoint as loop:
-            loop.run_until_complete(coro)
+            return loop.run_until_complete(coro)
 
     def run_forever(self):
         with self._entrypoint as loop:
             loop.run_forever()
 
     def system_signals_listener(self, *signals: int):
         processor = SysSignalListener(*signals)
```

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/change_user.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/change_user.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/clear_environ.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/clear_environ.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/svc_dependency.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/svc_dependency.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/svc_to_context.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/svc_to_context.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/src/aiomisc_entrypoint/processors/sys_signals.py` & `aiomisc_entrypoint-1.2.0/src/aiomisc_entrypoint/processors/sys_signals.py`

 * *Files identical despite different names*

### Comparing `aiomisc_entrypoint-1.1.0/setup.py` & `aiomisc_entrypoint-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,76 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aiomisc-entrypoint
+Version: 1.2.0
+Summary: 
+Home-page: https://github.com/anysoft-kz/aiomisc-entrypoint
+Author: Vladislav Vorobyov
+Author-email: vladislav.vorobyov@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiomisc (>=16.0.0,<17.0.0)
+Project-URL: Repository, https://github.com/anysoft-kz/aiomisc-entrypoint
+Description-Content-Type: text/markdown
+
+# Aiomisc Entrypoint
+
+Alternative way to run [aiomisc entrypoint](https://aiomisc.readthedocs.io/en/latest/entrypoint.html#entrypoint) with processors
+added behavior to start and stop events of entrypoint and custom query logger.
+
+
+## Basic usage
+```python
+from aiomisc_entrypoint import Entrypoint
+
+ep = Entrypoint()
+ep.clear_environ()
+ep.change_user()
+ep.system_signals_listener()
+ep.register_services_in_context()
+ep.first_start_last_stop()
+
+ep.run_forever()
+```
+
+
+## Extended usage
+
+```python
+from signal import SIGINT, SIGTERM, SIGKILL
+from aiomisc import Service
+from aiomisc_entrypoint import Entrypoint
+
+class TestService(Service):
+    
+    async def start(self):
+        ...
+
+    
+async def main():
+    ...
+
+
+services = (
+    TestService(context_name='svc1'),
+    TestService(context_name='svc2'),
+)
+    
+ep = Entrypoint(*services)
+ep.clear_environ(lambda x: x.startwith('APP_'))
+ep.change_user('user')
+ep.system_signals_listener(SIGINT, SIGTERM, SIGKILL)
+ep.register_services_in_context()
+ep.first_start_last_stop()
 
-package_dir = \
-{'': 'src'}
+ep.run_until_complete(main())
+```
 
-packages = \
-['aiomisc_entrypoint', 'aiomisc_entrypoint.processors']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiomisc>=16.0,<18.0']
-
-setup_kwargs = {
-    'name': 'aiomisc-entrypoint',
-    'version': '1.1.0',
-    'description': '',
-    'long_description': "# Aiomisc Entrypoint\n\nAlternative way to run [aiomisc entrypoint](https://aiomisc.readthedocs.io/en/latest/entrypoint.html#entrypoint) with processors\nadded behavior to start and stop events of entrypoint and custom query logger.\n\n\n## Basic usage\n```python\nfrom aiomisc_entrypoint import Entrypoint\n\nep = Entrypoint()\nep.clear_environ()\nep.change_user()\nep.system_signals_listener()\nep.register_services_in_context()\nep.first_start_last_stop()\n\nep.run_forever()\n```\n\n\n## Extended usage\n\n```python\nfrom signal import SIGINT, SIGTERM, SIGKILL\nfrom aiomisc import Service\nfrom aiomisc_entrypoint import Entrypoint\n\nclass TestService(Service):\n    \n    async def start(self):\n        ...\n\n    \nasync def main():\n    ...\n\n\nservices = (\n    TestService(context_name='svc1'),\n    TestService(context_name='svc2'),\n)\n    \nep = Entrypoint(*services)\nep.clear_environ(lambda x: x.startwith('APP_'))\nep.change_user('user')\nep.system_signals_listener(SIGINT, SIGTERM, SIGKILL)\nep.register_services_in_context()\nep.first_start_last_stop()\n\nep.run_until_complete(main())\n```\n\n\nRelease Notes:\n\nv1.0.1\n- fix error with set loop for `asyncio.Event` in `SysSignalListener`\n\n",
-    'author': 'Vladislav Vorobyov',
-    'author_email': 'vladislav.vorobyov@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/anysoft-kz/aiomisc-entrypoint',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+Release Notes:
+
+v1.0.1
+- fix error with set loop for `asyncio.Event` in `SysSignalListener`
 
 
-setup(**setup_kwargs)
```

