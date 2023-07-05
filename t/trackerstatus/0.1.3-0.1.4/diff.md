# Comparing `tmp/trackerstatus-0.1.3.tar.gz` & `tmp/trackerstatus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackerstatus-0.1.3.tar", max compression
+gzip compressed data, was "trackerstatus-0.1.4.tar", max compression
```

## Comparing `trackerstatus-0.1.3.tar` & `trackerstatus-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-10-04 14:19:57.810124 trackerstatus-0.1.3/LICENSE
--rw-r--r--   0        0        0     1010 2022-11-13 04:12:22.455567 trackerstatus-0.1.3/README.md
--rw-r--r--   0        0        0      425 2022-12-13 13:04:15.300711 trackerstatus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-03 03:40:05.750309 trackerstatus-0.1.3/trackerstatus/__init__.py
--rw-r--r--   0        0        0     3373 2022-10-18 13:39:34.992871 trackerstatus-0.1.3/trackerstatus/api.py
--rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 trackerstatus-0.1.3/setup.py
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 trackerstatus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-04 14:19:57.810124 trackerstatus-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1014 2023-02-07 14:40:53.465952 trackerstatus-0.1.4/README.md
+-rw-r--r--   0        0        0      425 2023-07-05 21:41:42.714932 trackerstatus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-03 03:40:05.750309 trackerstatus-0.1.4/trackerstatus/__init__.py
+-rw-r--r--   0        0        0     3776 2023-04-03 15:27:53.066316 trackerstatus-0.1.4/trackerstatus/api.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 trackerstatus-0.1.4/setup.py
+-rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 trackerstatus-0.1.4/PKG-INFO
```

### Comparing `trackerstatus-0.1.3/LICENSE` & `trackerstatus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trackerstatus-0.1.3/README.md` & `trackerstatus-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![CodeQL](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml)
 [![Pylint](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml)
 
 A python library for gathering data from the [https://trackerstatus.info](https://trackerstatus.info) website
 
 ## Install via Pip
 
-```
+```bash
 pip install trackerstatus
 ```
 
 ## Resources
 
 * Github repo: [https://github.com/mauvehed/trackerstatus/](https://github.com/mauvehed/trackerstatus/)
 * Pip package: [https://pypi.org/project/trackerstatus/](https://pypi.org/project/trackerstatus/)
```

### Comparing `trackerstatus-0.1.3/trackerstatus/api.py` & `trackerstatus-0.1.4/trackerstatus/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,40 @@
                 The API type to fetch data for
                 Must be one of 'status', 'latency', 'uptime', 'records', 'downtime' or 'all'
 
         Returns:
             dict: The data retrieved from the API
         """
         api_site_url = f'https://{self.site_name}.trackerstatus.info/api/{api_type}/'
-        response_is = requests.get(api_site_url,timeout=15)
-        if response_is.status_code == 200:
-            self.data = response_is.json()
-        return self.data
+        return self._extracted_from_get_sites_all_api(api_site_url)
+
 
     def get_sites_all_api(self):
         """Get the top level /api/list/ sites API data
 
         https://trackerstatus.info/api/list/
 
         Returns:
             dict: The data retrieved from the API
         """
-        response_is = requests.get(API_ALL_SITES_URL,timeout=15)
+        return self._extracted_from_get_sites_all_api(API_ALL_SITES_URL)
+
+    def _extracted_from_get_sites_all_api(self, api_site_url):
+        """Get the API data for the specific api_site_url
+        
+        Args:
+            api_site_url (str, optional):  Defaults to 'all'.
+        
+            The API type to fetch data for
+            Must be one of 'status', 'latency', 'uptime', 'records', 'downtime' or 'all'
+        
+        Returns:
+            dict: The data retrieved from the API
+        """
+        response_is = requests.get(api_site_url, timeout=15)
         if response_is.status_code == 200:
             self.data = response_is.json()
         return self.data
 
     def get_site_status(self):
         """Get the site status API data
```

### Comparing `trackerstatus-0.1.3/setup.py` & `trackerstatus-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'trackerstatus',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A python library for gathering data from the trackerstatus.info website',
-    'long_description': '# trackerstatus\n\n[![PyPI](https://img.shields.io/pypi/v/trackerstatus.svg)](https://pypi.org/project/trackerstatus/)\n[![Python Version](https://img.shields.io/pypi/pyversions/trackerstatus.svg)](https://github.com/mauvehed/yourIP/actions/workflows/main.yml)\n[![CodeQL](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml)\n[![Pylint](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml)\n\nA python library for gathering data from the [https://trackerstatus.info](https://trackerstatus.info) website\n\n## Install via Pip\n\n```\npip install trackerstatus\n```\n\n## Resources\n\n* Github repo: [https://github.com/mauvehed/trackerstatus/](https://github.com/mauvehed/trackerstatus/)\n* Pip package: [https://pypi.org/project/trackerstatus/](https://pypi.org/project/trackerstatus/)\n',
+    'long_description': '# trackerstatus\n\n[![PyPI](https://img.shields.io/pypi/v/trackerstatus.svg)](https://pypi.org/project/trackerstatus/)\n[![Python Version](https://img.shields.io/pypi/pyversions/trackerstatus.svg)](https://github.com/mauvehed/yourIP/actions/workflows/main.yml)\n[![CodeQL](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml)\n[![Pylint](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml)\n\nA python library for gathering data from the [https://trackerstatus.info](https://trackerstatus.info) website\n\n## Install via Pip\n\n```bash\npip install trackerstatus\n```\n\n## Resources\n\n* Github repo: [https://github.com/mauvehed/trackerstatus/](https://github.com/mauvehed/trackerstatus/)\n* Pip package: [https://pypi.org/project/trackerstatus/](https://pypi.org/project/trackerstatus/)\n',
     'author': 'mauvehed',
     'author_email': 'mh@mvh.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mauvehed/trackerstatus',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `trackerstatus-0.1.3/PKG-INFO` & `trackerstatus-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: trackerstatus
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python library for gathering data from the trackerstatus.info website
 Home-page: https://github.com/mauvehed/trackerstatus
 License: MIT
 Author: mauvehed
 Author-email: mh@mvh.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/mauvehed/trackerstatus
 Description-Content-Type: text/markdown
 
 # trackerstatus
 
 [![PyPI](https://img.shields.io/pypi/v/trackerstatus.svg)](https://pypi.org/project/trackerstatus/)
@@ -21,15 +22,15 @@
 [![CodeQL](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/codeql-analysis.yml)
 [![Pylint](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml/badge.svg)](https://github.com/mauvehed/trackerstatus/actions/workflows/pylint.yml)
 
 A python library for gathering data from the [https://trackerstatus.info](https://trackerstatus.info) website
 
 ## Install via Pip
 
-```
+```bash
 pip install trackerstatus
 ```
 
 ## Resources
 
 * Github repo: [https://github.com/mauvehed/trackerstatus/](https://github.com/mauvehed/trackerstatus/)
 * Pip package: [https://pypi.org/project/trackerstatus/](https://pypi.org/project/trackerstatus/)
```

