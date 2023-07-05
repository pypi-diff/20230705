# Comparing `tmp/mass_driver_plugins-0.3.2.tar.gz` & `tmp/mass_driver_plugins-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_driver_plugins-0.3.2.tar", max compression
+gzip compressed data, was "mass_driver_plugins-0.4.0.tar", max compression
```

## Comparing `mass_driver_plugins-0.3.2.tar` & `mass_driver_plugins-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2520 2023-01-17 14:11:51.400445 mass_driver_plugins-0.3.2/README.md
--rw-r--r--   0        0        0     2612 2023-06-10 13:55:46.946336 mass_driver_plugins-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-01-17 14:11:51.400445 mass_driver_plugins-0.3.2/src/mass_driver_plugins/__init__.py
--rw-r--r--   0        0        0      756 2023-01-17 14:11:51.400445 mass_driver_plugins-0.3.2/src/mass_driver_plugins/cli.py
--rw-r--r--   0        0        0     2785 2023-03-15 22:00:51.349024 mass_driver_plugins-0.3.2/src/mass_driver_plugins/jsonpatch.py
--rw-r--r--   0        0        0     2283 2023-03-15 22:00:51.349024 mass_driver_plugins-0.3.2/src/mass_driver_plugins/poetry.py
--rw-r--r--   0        0        0       26 2023-01-17 14:11:51.400445 mass_driver_plugins-0.3.2/src/mass_driver_plugins/py.typed
--rw-r--r--   0        0        0     8507 2023-03-28 22:52:08.804000 mass_driver_plugins-0.3.2/src/mass_driver_plugins/surgical.py
--rw-r--r--   0        0        0     1038 2023-03-15 22:00:51.349024 mass_driver_plugins-0.3.2/src/mass_driver_plugins/template.py
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 mass_driver_plugins-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2520 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/README.md
+-rw-r--r--   0        0        0     2612 2023-07-05 00:44:09.249599 mass_driver_plugins-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/__init__.py
+-rw-r--r--   0        0        0      756 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/cli.py
+-rw-r--r--   0        0        0     2845 2023-07-05 00:40:22.790344 mass_driver_plugins-0.4.0/src/mass_driver_plugins/jsonpatch.py
+-rw-r--r--   0        0        0     2354 2023-07-05 00:40:30.318451 mass_driver_plugins-0.4.0/src/mass_driver_plugins/poetry.py
+-rw-r--r--   0        0        0       26 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/py.typed
+-rw-r--r--   0        0        0     8578 2023-07-05 00:40:35.454524 mass_driver_plugins-0.4.0/src/mass_driver_plugins/surgical.py
+-rw-r--r--   0        0        0      886 2023-07-05 00:40:39.494582 mass_driver_plugins-0.4.0/src/mass_driver_plugins/template.py
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 mass_driver_plugins-0.4.0/PKG-INFO
```

### Comparing `mass_driver_plugins-0.3.2/README.md` & `mass_driver_plugins-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.3.2/pyproject.toml` & `mass_driver_plugins-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "mass_driver_plugins"
-version = "0.3.2"
+version = "0.4.0"
 description = "Experimental plugin ecosystem for Mass Driver"
 authors = ["Jb Doyon <jb@jiby.tech>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 mass-driver-plugins = "mass_driver_plugins.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 # The project that these plugins extend
-mass-driver = "^0.14"
+mass-driver = "^0.15"
 # Poetry driver
 poetry-core = "*"
 # Json path resolving within
 jsonpointer = "*"
 # And json patching itself via pointers
 jsonpatch = "*"
 # Templates
```

### Comparing `mass_driver_plugins-0.3.2/src/mass_driver_plugins/cli.py` & `mass_driver_plugins-0.4.0/src/mass_driver_plugins/cli.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.3.2/src/mass_driver_plugins/jsonpatch.py` & `mass_driver_plugins-0.4.0/src/mass_driver_plugins/jsonpatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """A JSON Patch (RFC6902) PatchDriver"""
 
 
 import json
-from pathlib import Path
 
 import jsonpatch
 from mass_driver.models.patchdriver import PatchDriver, PatchOutcome, PatchResult
-from pydantic import Extra
+from mass_driver.models.repository import ClonedRepo
+from pydantic import Extra, FilePath
 from ruamel import yaml
 
 
 class JsonPatchBase(PatchDriver):
     """Base class for dict-based editing, regardless of type of file"""
 
-    target_file: Path
+    target_file: FilePath
     """File on which to apply Json Patch"""
     patch: list[dict] | str
     """JSON Patch, from RFC 6902"""
 
     class Config:
         """Configuration of the JsonPatch class"""
 
@@ -27,20 +27,20 @@
         """Load a data-tree particular file language of the day"""
         raise NotImplementedError("No serialize function implemented")
 
     def serialize(self, file_dict: dict, fd):
         """Dump a data-tree back to string in the particular file language of the day"""
         raise NotImplementedError("No deserialize function implemented")
 
-    def run(self, repo: Path) -> PatchResult:
+    def run(self, repo: ClonedRepo) -> PatchResult:
         """Patch the given file"""
         patch = self.patch
         if isinstance(self.patch, list):
             patch = jsonpatch.JsonPatch(self.patch)
-        json_filepath_abs = repo / self.target_file
+        json_filepath_abs = repo.cloned_path / self.target_file
         if not json_filepath_abs.is_file():
             return PatchResult(
                 outcome=PatchOutcome.PATCH_DOES_NOT_APPLY,
                 details="No such file to patch",
             )
         try:
             with open(json_filepath_abs, "rb") as json_file:
```

### Comparing `mass_driver_plugins-0.3.2/src/mass_driver_plugins/poetry.py` & `mass_driver_plugins-0.4.0/src/mass_driver_plugins/poetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 from jsonpointer import resolve_pointer, set_pointer
 from mass_driver.models.patchdriver import PatchDriver, PatchOutcome, PatchResult
+from mass_driver.models.repository import ClonedRepo
 from poetry.core.pyproject.toml import PyProjectTOML
 
 
 def get_pyproject(repo_path: Path):
     """Grab the pyproject object"""
     return PyProjectTOML(repo_path / "pyproject.toml")
 
@@ -46,17 +47,17 @@
         if self.package_group:
             return (
                 f"/tool/poetry/group/{self.package_group}/dependencies/{self.package}"
             )
         else:
             return f"/tool/poetry/dependencies/{self.package}"
 
-    def run(self, repo: Path) -> PatchResult:
+    def run(self, repo: ClonedRepo) -> PatchResult:
         """Process the major bump file"""
-        project = get_pyproject(repo)
+        project = get_pyproject(repo.cloned_path)
         dep_version = resolve_pointer(project.data, self.json_pointer, None)
         if not dep_version:
             return PatchResult(
                 outcome=PatchOutcome.PATCH_DOES_NOT_APPLY,
                 details=f"Didn't find {self.package} in pyproject.toml test deps!",
             )
         major_version, *other_versions = dep_version.split(".")
```

### Comparing `mass_driver_plugins-0.3.2/src/mass_driver_plugins/surgical.py` & `mass_driver_plugins-0.4.0/src/mass_driver_plugins/surgical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Edit files via tree-sitter"""
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 
 from mass_driver.models.patchdriver import PatchDriver, PatchOutcome, PatchResult
+from mass_driver.models.repository import ClonedRepo
 from tree_sitter import Node, Parser
 from tree_sitter_languages import get_language
 
 
 class SurgicalFileEditor(PatchDriver):
     """
     Edit files surgically, parsing them with tree-sitter
@@ -39,17 +40,17 @@
         """Refine keyword matches"""
         raise NotImplementedError("Base class doesn't know to refine node search")
 
     def surgical_edit(self, text, bad_nodes: list[Any]) -> str:
         """Surgically edit the file to fix the badness"""
         raise NotImplementedError("Base class doesn't know to surgically edit the file")
 
-    def run(self, repo: Path) -> PatchResult:
+    def run(self, repo: ClonedRepo) -> PatchResult:
         """Process the template file"""
-        target_fullpath = repo / Path(self.target_file)
+        target_fullpath = repo.cloned_path / Path(self.target_file)
         content_str = target_fullpath.read_text()
         language = get_language(self.language)
         query = language.query(self.query)
         parser = Parser()
         parser.set_language(language)
         tree = parser.parse(bytes(content_str, "utf8"))
         captures = query.captures(tree.root_node)
```

### Comparing `mass_driver_plugins-0.3.2/src/mass_driver_plugins/template.py` & `mass_driver_plugins-0.4.0/src/mass_driver_plugins/template.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """Create templated files via Jinja2"""
-from pathlib import Path
-from typing import Any
 
 from jinja2 import Environment
 from mass_driver.models.patchdriver import PatchDriver, PatchOutcome, PatchResult
+from mass_driver.models.repository import ClonedRepo
 
 
 class TemplatedFile(PatchDriver):
     """Create a file via Jinja template filling"""
 
     target_file: str
     """The file to expand via template"""
     template: str
     """A jinja2 template"""
-    context: dict[str, Any]
-    """Per repo context for template expansion, with repo name as key"""
     jinja_args: dict
     """Extra args to give jinja templating"""
 
-    def run(self, repo: Path) -> PatchResult:
+    def run(self, repo: ClonedRepo) -> PatchResult:
         """Process the template file"""
         env = Environment(**self.jinja_args, autoescape=True)
         template = env.from_string(self.template)
-        repo_name = repo.name
-        context = self.context.get(repo_name)
-        rendered = template.render(context)
-        with open(repo / Path(self.target_file), "w") as fd:
+        rendered = template.render(repo.patch_data)
+        with open(repo.cloned_path / self.target_file, "w") as fd:
             fd.write(rendered)
         return PatchResult(outcome=PatchOutcome.PATCHED_OK)
```

### Comparing `mass_driver_plugins-0.3.2/PKG-INFO` & `mass_driver_plugins-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mass-driver-plugins
-Version: 0.3.2
+Version: 0.4.0
 Summary: Experimental plugin ecosystem for Mass Driver
 Author: Jb Doyon
 Author-email: jb@jiby.tech
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonpatch
 Requires-Dist: jsonpointer
-Requires-Dist: mass-driver (>=0.14,<0.15)
+Requires-Dist: mass-driver (>=0.15,<0.16)
 Requires-Dist: poetry-core
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tree-sitter
 Requires-Dist: tree-sitter-languages
 Description-Content-Type: text/markdown
 
 # Mass Driver Plugins
```

