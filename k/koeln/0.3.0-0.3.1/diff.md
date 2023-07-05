# Comparing `tmp/koeln-0.3.0.tar.gz` & `tmp/koeln-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koeln-0.3.0.tar", max compression
+gzip compressed data, was "koeln-0.3.1.tar", max compression
```

## Comparing `koeln-0.3.0.tar` & `koeln-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-07 22:37:43.406683 koeln-0.3.0/LICENSE
--rw-r--r--   0        0        0     7478 2023-03-07 22:37:43.406683 koeln-0.3.0/README.md
--rw-r--r--   0        0        0      339 2023-03-07 22:37:43.406683 koeln-0.3.0/koeln/__init__.py
--rw-r--r--   0        0        0      266 2023-03-07 22:37:43.406683 koeln-0.3.0/koeln/exceptions.py
--rw-r--r--   0        0        0     7634 2023-03-07 22:37:43.406683 koeln-0.3.0/koeln/koeln.py
--rw-r--r--   0        0        0     1063 2023-03-07 22:37:43.406683 koeln-0.3.0/koeln/models.py
--rw-r--r--   0        0        0        0 2023-03-07 22:37:43.406683 koeln-0.3.0/koeln/py.typed
--rw-r--r--   0        0        0     3804 2023-03-07 22:38:03.006935 koeln-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9009 1970-01-01 00:00:00.000000 koeln-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-05 10:30:26.916844 koeln-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7478 2023-07-05 10:30:26.916844 koeln-0.3.1/README.md
+-rw-r--r--   0        0        0     3733 2023-07-05 10:30:41.240870 koeln-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-07-05 10:30:26.916844 koeln-0.3.1/src/koeln/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-05 10:30:26.916844 koeln-0.3.1/src/koeln/exceptions.py
+-rw-r--r--   0        0        0     7546 2023-07-05 10:30:26.916844 koeln-0.3.1/src/koeln/koeln.py
+-rw-r--r--   0        0        0     1063 2023-07-05 10:30:26.916844 koeln-0.3.1/src/koeln/models.py
+-rw-r--r--   0        0        0        0 2023-07-05 10:30:26.916844 koeln-0.3.1/src/koeln/py.typed
+-rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 koeln-0.3.1/PKG-INFO
```

### Comparing `koeln-0.3.0/LICENSE` & `koeln-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koeln-0.3.0/README.md` & `koeln-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 pip install koeln
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- [Disabled parking spaces / Behindertenparkplätze][disabled_parkings] (425 locations)
+- [Disabled parking spaces / Behindertenparkplätze][disabled_parkings] (441 locations)
 
 <details>
     <summary>Click here to get more details</summary>
 
 ### Disabled parking spaces
 
 | Variable | Type | Description |
```

### Comparing `koeln-0.3.0/koeln/koeln.py` & `koeln-0.3.1/src/koeln/koeln.py`

 * *Files 10% similar despite different names*

```diff
@@ -209,28 +209,24 @@
     async def disabled_parkings(self) -> list[DisabledParking]:
         """Get list of disabled parking spaces.
 
         Returns
         -------
             A list of DisabledParking objects.
         """
-        results: list[DisabledParking] = []
         locations = await self._request(
             "basiskarten/stadtplanthemen/MapServer/0/query",
             params={
                 "where": "objectid is not null",
                 "outFields": "*",
                 "outSR": "4326",
                 "f": "json",
             },
         )
-
-        for item in locations["features"]:
-            results.append(DisabledParking.from_dict(item))
-        return results
+        return [DisabledParking.from_dict(item) for item in locations["features"]]
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> StadtKoeln:
```

### Comparing `koeln-0.3.0/koeln/models.py` & `koeln-0.3.1/src/koeln/models.py`

 * *Files identical despite different names*

### Comparing `koeln-0.3.0/pyproject.toml` & `koeln-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,133 @@
 [tool.poetry]
 name = "koeln"
-version = "0.3.0"
+version = "0.3.1"
 description = "Asynchronous Python client providing Open Data information of Köln"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-koeln"
 repository = "https://github.com/klaasnicolaas/python-koeln"
 documentation = "https://github.com/klaasnicolaas/python-koeln"
 keywords = ["open", "data", "platform", "Köln", "cologne", "parking", "api", "async", "client"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "koeln" }
+  { include = "koeln", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-koeln/issues"
 Changelog = "https://github.com/klaasnicolaas/python-koeln/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.255"
-aresponses = "^2.1.6"
-black = ">=22.10,<24.0"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.2"
-coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = "^1.1"
-pre-commit = "^3.0.3"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.16.1"
-pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.3.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["koeln"]
+ruff = "0.0.277"
+aresponses = "2.1.6"
+black = "23.3.0"
+blacken-docs = "1.14.0"
+codespell = "2.2.5"
+coverage = {version = "7.2.7", extras = ["toml"]}
+mypy = "1.4.1"
+pre-commit = "3.3.3"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.1.0"
+yamllint = "1.32.0"
+covdefaults = "2.3.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["koeln"]
 
+[tool.coverage.report]
+fail_under = 90
+show_missing = true
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "vw",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes=20
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 20
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -153,9 +147,9 @@
 [tool.ruff.isort]
 known-first-party = ["koeln"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `koeln-0.3.0/PKG-INFO` & `koeln-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koeln
-Version: 0.3.0
+Version: 0.3.1
 Summary: Asynchronous Python client providing Open Data information of Köln
 Home-page: https://github.com/klaasnicolaas/python-koeln
 License: MIT
 Keywords: open,data,platform,Köln,cologne,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -15,18 +15,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-koeln/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-koeln/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-koeln
 Project-URL: Repository, https://github.com/klaasnicolaas/python-koeln
@@ -67,15 +63,15 @@
 pip install koeln
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- [Disabled parking spaces / Behindertenparkplätze][disabled_parkings] (425 locations)
+- [Disabled parking spaces / Behindertenparkplätze][disabled_parkings] (441 locations)
 
 <details>
     <summary>Click here to get more details</summary>
 
 ### Disabled parking spaces
 
 | Variable | Type | Description |
```

