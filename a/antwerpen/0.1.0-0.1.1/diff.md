# Comparing `tmp/antwerpen-0.1.0.tar.gz` & `tmp/antwerpen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antwerpen-0.1.0.tar", max compression
+gzip compressed data, was "antwerpen-0.1.1.tar", max compression
```

## Comparing `antwerpen-0.1.0.tar` & `antwerpen-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-04-28 14:18:12.460880 antwerpen-0.1.0/LICENSE
--rw-r--r--   0        0        0     8265 2023-04-28 14:18:12.460880 antwerpen-0.1.0/README.md
--rw-r--r--   0        0        0      341 2023-04-28 14:18:12.460880 antwerpen-0.1.0/antwerpen/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-28 14:18:12.460880 antwerpen-0.1.0/antwerpen/antwerpen.py
--rw-r--r--   0        0        0      290 2023-04-28 14:18:12.460880 antwerpen-0.1.0/antwerpen/exceptions.py
--rw-r--r--   0        0        0     1854 2023-04-28 14:18:12.460880 antwerpen-0.1.0/antwerpen/models.py
--rw-r--r--   0        0        0        0 2023-04-28 14:18:12.460880 antwerpen-0.1.0/antwerpen/py.typed
--rw-r--r--   0        0        0     3841 2023-04-28 14:18:34.417031 antwerpen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9803 1970-01-01 00:00:00.000000 antwerpen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-05 08:54:14.072629 antwerpen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8265 2023-07-05 08:54:14.072629 antwerpen-0.1.1/README.md
+-rw-r--r--   0        0        0     3760 2023-07-05 08:54:30.205539 antwerpen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-07-05 08:54:14.072629 antwerpen-0.1.1/src/antwerpen/__init__.py
+-rw-r--r--   0        0        0     4350 2023-07-05 08:54:14.072629 antwerpen-0.1.1/src/antwerpen/antwerpen.py
+-rw-r--r--   0        0        0      290 2023-07-05 08:54:14.072629 antwerpen-0.1.1/src/antwerpen/exceptions.py
+-rw-r--r--   0        0        0     1854 2023-07-05 08:54:14.072629 antwerpen-0.1.1/src/antwerpen/models.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:54:14.072629 antwerpen-0.1.1/src/antwerpen/py.typed
+-rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 antwerpen-0.1.1/PKG-INFO
```

### Comparing `antwerpen-0.1.0/LICENSE` & `antwerpen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antwerpen-0.1.0/README.md` & `antwerpen-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `antwerpen-0.1.0/antwerpen/antwerpen.py` & `antwerpen-0.1.1/src/antwerpen/antwerpen.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,28 +102,24 @@
         ----
             limit: Number of items to return.
 
         Returns:
         -------
             A list of DisabledParking objects.
         """
-        results: list[DisabledParking] = []
         locations = await self._request(
             "portal_publiek6/MapServer/585/query",
             params={
                 "where": "1=1",
                 "resultRecordCount": limit,
                 "outFields": "*",
                 "f": "geojson",
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
 
     async def __aenter__(self) -> ODPAntwerpen:
```

### Comparing `antwerpen-0.1.0/antwerpen/models.py` & `antwerpen-0.1.1/src/antwerpen/models.py`

 * *Files identical despite different names*

### Comparing `antwerpen-0.1.0/pyproject.toml` & `antwerpen-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,134 @@
 [tool.poetry]
 name = "antwerpen"
-version = "0.1.0"
+version = "0.1.1"
 description = "Asynchronous Python client providing Open Data information of Antwerpen"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-antwerpen"
 repository = "https://github.com/klaasnicolaas/python-antwerpen"
 documentation = "https://github.com/klaasnicolaas/python-antwerpen"
 keywords = ["open", "data", "platform", "antwerpen", "parking", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
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
-    { include = "antwerpen" }
+  { include = "antwerpen", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 pytz = "^2023.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-antwerpen/issues"
 Changelog = "https://github.com/klaasnicolaas/python-antwerpen/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.264"
-aresponses = "^2.1.6"
-black = "^23.3"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.4"
-coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.3"
-pre-commit = "^3.2.0"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.17.0"
-pytest = "^7.2.2"
-pytest-asyncio = ">=0.20.3,<0.22.0"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.2.2"
-types-pytz = "^2023.3.0.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["antwerpen"]
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
+types-pytz = "2023.3.0.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["antwerpen"]
 
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
@@ -154,9 +148,9 @@
 [tool.ruff.isort]
 known-first-party = ["antwerpen"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `antwerpen-0.1.0/PKG-INFO` & `antwerpen-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antwerpen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asynchronous Python client providing Open Data information of Antwerpen
 Home-page: https://github.com/klaasnicolaas/python-antwerpen
 License: MIT
 Keywords: open,data,platform,antwerpen,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -14,18 +14,14 @@
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
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-antwerpen/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-antwerpen/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-antwerpen
```

