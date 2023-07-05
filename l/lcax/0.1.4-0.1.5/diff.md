# Comparing `tmp/lcax-0.1.4.tar.gz` & `tmp/lcax-0.1.5.tar.gz`

## Comparing `lcax-0.1.4.tar` & `lcax-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123     1039 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/csharp.yaml
--rw-r--r--   0     1001      123     1303 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/docs.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/javascript.yaml
--rw-r--r--   0     1001      123     1363 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/python.yaml
--rw-r--r--   0     1001      123      843 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/release.yaml
--rw-r--r--   0     1001      123      863 2023-07-05 11:21:28.000000 lcax-0.1.4/.github/workflows/rust.yaml
--rw-r--r--   0     1001      123     3182 2023-07-05 11:21:28.000000 lcax-0.1.4/.gitignore
--rw-r--r--   0     1001      123      560 2023-07-05 11:21:28.000000 lcax-0.1.4/COPYRIGHT
--rw-r--r--   0     1001      123    12302 2023-07-05 11:21:34.000000 lcax-0.1.4/Cargo.lock
--rw-r--r--   0     1001      123    10173 2023-07-05 11:21:28.000000 lcax-0.1.4/LICENSE
--rw-r--r--   0     1001      123      516 2023-07-05 11:21:28.000000 lcax-0.1.4/README.md
--rw-r--r--   0     1001      123    59384 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/assets/benchmark.png
--rw-r--r--   0     1001      123    24746 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/assets/epdx.png
--rw-r--r--   0     1001      123   660950 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/assets/lcax project.jpeg
--rw-r--r--   0     1001      123     1342 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/data_structure.md
--rw-r--r--   0     1001      123     1859 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/index.md
--rw-r--r--   0     1001      123      127 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      123      335 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      123        0 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/schemas/.gitkeep
--rw-r--r--   0     1001      123      507 2023-07-05 11:21:28.000000 lcax-0.1.4/docs/schemas.md
--rw-r--r--   0     1001      123     1047 2023-07-05 11:21:28.000000 lcax-0.1.4/mkdocs.yml
--rw-r--r--   0     1001      123      100 2023-07-05 11:21:28.000000 lcax-0.1.4/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      123      136 2023-07-05 11:22:11.000000 lcax-0.1.4/packages/python/src/lcax/lcax/__init__.py
--rw-r--r--   0     1001      123      118 2023-07-05 11:22:11.000000 lcax-0.1.4/packages/python/src/lcax/lcax/ffi.py
--rw-r--r--   0     1001      123     5916 2023-07-05 11:22:12.000000 lcax-0.1.4/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      123        0 2023-07-05 11:21:28.000000 lcax-0.1.4/packages/python/tests/.gitkeep
--rw-r--r--   0     1001      123      947 2023-07-05 11:21:28.000000 lcax-0.1.4/pyproject.toml
--rwxr-xr-x   0     1001      123      801 2023-07-05 11:22:43.000000 lcax-0.1.4/run-maturin-action.sh
--rw-r--r--   0     1001      123       16 2023-07-05 11:21:28.000000 lcax-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123     3136 2023-07-05 11:21:28.000000 lcax-0.1.4/src/project.rs
--rw-r--r--   0     1001      123      201 2023-07-05 11:21:28.000000 lcax-0.1.4/src/schemars.rs
--rw-r--r--   0     1001      123        0 2023-07-05 11:21:28.000000 lcax-0.1.4/tests/.gitkeep
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      123     1039 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/cicd.yaml
+-rw-r--r--   0     1001      123        0 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/csharp.yaml
+-rw-r--r--   0     1001      123     1303 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/docs.yaml
+-rw-r--r--   0     1001      123        0 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/javascript.yaml
+-rw-r--r--   0     1001      123     1363 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/python.yaml
+-rw-r--r--   0     1001      123      877 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/release.yaml
+-rw-r--r--   0     1001      123      863 2023-07-05 13:09:06.000000 lcax-0.1.5/.github/workflows/rust.yaml
+-rw-r--r--   0     1001      123     3182 2023-07-05 13:09:06.000000 lcax-0.1.5/.gitignore
+-rw-r--r--   0     1001      123      560 2023-07-05 13:09:06.000000 lcax-0.1.5/COPYRIGHT
+-rw-r--r--   0     1001      123    12302 2023-07-05 13:09:13.000000 lcax-0.1.5/Cargo.lock
+-rw-r--r--   0     1001      123    10173 2023-07-05 13:09:06.000000 lcax-0.1.5/LICENSE
+-rw-r--r--   0     1001      123      516 2023-07-05 13:09:06.000000 lcax-0.1.5/README.md
+-rw-r--r--   0     1001      123    59384 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/assets/benchmark.png
+-rw-r--r--   0     1001      123    24746 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/assets/epdx.png
+-rw-r--r--   0     1001      123   660950 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/assets/lcax project.jpeg
+-rw-r--r--   0     1001      123     1342 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/data_structure.md
+-rw-r--r--   0     1001      123    16040 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/examples/basic_project.json
+-rw-r--r--   0     1001      123      139 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/examples.md
+-rw-r--r--   0     1001      123     1859 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/index.md
+-rw-r--r--   0     1001      123      127 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0     1001      123      335 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/overrides/stylesheets/extra.css
+-rw-r--r--   0     1001      123        0 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/schemas/.gitkeep
+-rw-r--r--   0     1001      123      507 2023-07-05 13:09:06.000000 lcax-0.1.5/docs/schemas.md
+-rw-r--r--   0     1001      123     1073 2023-07-05 13:09:06.000000 lcax-0.1.5/mkdocs.yml
+-rw-r--r--   0     1001      123      100 2023-07-05 13:09:06.000000 lcax-0.1.5/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      123      136 2023-07-05 13:09:46.000000 lcax-0.1.5/packages/python/src/lcax/lcax/__init__.py
+-rw-r--r--   0     1001      123      118 2023-07-05 13:09:46.000000 lcax-0.1.5/packages/python/src/lcax/lcax/ffi.py
+-rw-r--r--   0     1001      123     5916 2023-07-05 13:09:47.000000 lcax-0.1.5/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      123        0 2023-07-05 13:09:06.000000 lcax-0.1.5/packages/python/tests/.gitkeep
+-rw-r--r--   0     1001      123      947 2023-07-05 13:09:06.000000 lcax-0.1.5/pyproject.toml
+-rwxr-xr-x   0     1001      123      801 2023-07-05 13:10:19.000000 lcax-0.1.5/run-maturin-action.sh
+-rw-r--r--   0     1001      123       16 2023-07-05 13:09:06.000000 lcax-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      123     3136 2023-07-05 13:09:06.000000 lcax-0.1.5/src/project.rs
+-rw-r--r--   0     1001      123      201 2023-07-05 13:09:06.000000 lcax-0.1.5/src/schemars.rs
+-rw-r--r--   0     1001      123        0 2023-07-05 13:09:06.000000 lcax-0.1.5/tests/.gitkeep
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.5/PKG-INFO
```

### Comparing `lcax-0.1.4/Cargo.toml` & `lcax-0.1.5/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "lcax"
 description = "LCAx is an open, machine and human-readable data format for exchanging LCA results."
-version = "0.1.4"
+version = "0.1.5"
 authors = ["Christian Kongsgaard <christian@kongsgaard.eu>"]
 edition = "2018"
 readme = "README.md"
 license-file = "LICENSE"
 homepage = "https://lcax.kongsgaard.eu"
 documentation = "https://lcax.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/lcax"
```

### Comparing `lcax-0.1.4/.github/workflows/cicd.yaml` & `lcax-0.1.5/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/.github/workflows/docs.yaml` & `lcax-0.1.5/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/.github/workflows/python.yaml` & `lcax-0.1.5/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/.github/workflows/release.yaml` & `lcax-0.1.5/.github/workflows/release.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+name: "Create GitHub Release"
+
 on:
   workflow_call:
 
 permissions:
   contents: write
 
 jobs:
-  rust:
+  release:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/download-artifact@v2
         with:
           name: json-schema
```

### Comparing `lcax-0.1.4/.github/workflows/rust.yaml` & `lcax-0.1.5/.github/workflows/rust.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/.gitignore` & `lcax-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/COPYRIGHT` & `lcax-0.1.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/Cargo.lock` & `lcax-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lcax"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "epdx",
  "schemars",
  "serde",
  "serde_json",
 ]
```

### Comparing `lcax-0.1.4/LICENSE` & `lcax-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/README.md` & `lcax-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/docs/assets/benchmark.png` & `lcax-0.1.5/docs/assets/benchmark.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/docs/assets/epdx.png` & `lcax-0.1.5/docs/assets/epdx.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/docs/assets/lcax project.jpeg` & `lcax-0.1.5/docs/assets/lcax project.jpeg`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/docs/data_structure.md` & `lcax-0.1.5/docs/data_structure.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/docs/index.md` & `lcax-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/mkdocs.yml` & `lcax-0.1.5/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   - pymdownx.tabbed:
       alternate_style: true
 repo_url: https://github.com/ocni-dtu/lcax
 nav:
   - LCAx: index.md
   - Data Structure: data_structure.md
   - Schemas: schemas.md
+  - Examples: examples.md
 extra:
   generator: false
   social:
     - icon: octicons/globe-24
       link: https://kongsgaard.eu
       name: Christian Kongsgaard ApS
     - icon: fontawesome/brands/linkedin
```

### Comparing `lcax-0.1.4/packages/python/src/lcax/pydantic.py` & `lcax-0.1.5/packages/python/src/lcax/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  lcax.schema.json
-#   timestamp: 2023-07-05T11:22:12+00:00
+#   timestamp: 2023-07-05T13:09:47+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
```

### Comparing `lcax-0.1.4/pyproject.toml` & `lcax-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/run-maturin-action.sh` & `lcax-0.1.5/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/src/project.rs` & `lcax-0.1.5/src/project.rs`

 * *Files identical despite different names*

### Comparing `lcax-0.1.4/PKG-INFO` & `lcax-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lcax
-Version: 0.1.4
+Version: 0.1.5
 Requires-Dist: cffi
 Requires-Dist: mkdocs-material >=8.1.4,<9.0.0; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1,<2.0.0; extra == 'doc'
-Requires-Dist: pytest; extra == 'tests'
-Requires-Dist: pytest-datafixtures; extra == 'tests'
 Requires-Dist: pydantic >=1.8.2,<2.0.0; extra == 'code-gen'
 Requires-Dist: datamodel-code-generator; extra == 'code-gen'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-datafixtures; extra == 'tests'
 Provides-Extra: doc
-Provides-Extra: tests
 Provides-Extra: code-gen
+Provides-Extra: tests
 License-File: LICENSE
 License-File: LICENSE
 Summary: LCAx is an open, machine and human-readable data format for exchanging LCA results.
 Home-Page: https://lcax.kongsgaard.eu
 Author: Christian Kongsgaard <christian@kongsgaard.eu>
 Author-email: Christian Kongsgaard <christian@kongsgaard.eu>
 Requires-Python: >=3.10
```

