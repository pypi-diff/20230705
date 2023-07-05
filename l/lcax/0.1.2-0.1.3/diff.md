# Comparing `tmp/lcax-0.1.2.tar.gz` & `tmp/lcax-0.1.3.tar.gz`

## Comparing `lcax-0.1.2.tar` & `lcax-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     1039 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/csharp.yaml
--rw-r--r--   0     1001      123     1152 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/docs.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/javascript.yaml
--rw-r--r--   0     1001      123     1363 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/python.yaml
--rw-r--r--   0     1001      123      615 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/release.yaml
--rw-r--r--   0     1001      123      713 2023-07-05 09:01:30.000000 lcax-0.1.2/.github/workflows/rust.yaml
--rw-r--r--   0     1001      123     3182 2023-07-05 09:01:30.000000 lcax-0.1.2/.gitignore
--rw-r--r--   0     1001      123      560 2023-07-05 09:01:30.000000 lcax-0.1.2/COPYRIGHT
--rw-r--r--   0     1001      123    12302 2023-07-05 09:01:44.000000 lcax-0.1.2/Cargo.lock
--rw-r--r--   0     1001      123    10173 2023-07-05 09:01:30.000000 lcax-0.1.2/LICENSE
--rw-r--r--   0     1001      123      516 2023-07-05 09:01:30.000000 lcax-0.1.2/README.md
--rw-r--r--   0     1001      123    59384 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/assets/benchmark.png
--rw-r--r--   0     1001      123    24746 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/assets/epdx.png
--rw-r--r--   0     1001      123   660950 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/assets/lcax project.jpeg
--rw-r--r--   0     1001      123     1342 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/data_structure.md
--rw-r--r--   0     1001      123     1859 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/index.md
--rw-r--r--   0     1001      123      127 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      123      335 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      123        0 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/schemas/.gitkeep
--rw-r--r--   0     1001      123      397 2023-07-05 09:01:30.000000 lcax-0.1.2/docs/schemas.md
--rw-r--r--   0     1001      123     1047 2023-07-05 09:01:30.000000 lcax-0.1.2/mkdocs.yml
--rw-r--r--   0     1001      123      100 2023-07-05 09:01:30.000000 lcax-0.1.2/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      123      136 2023-07-05 09:02:29.000000 lcax-0.1.2/packages/python/src/lcax/lcax/__init__.py
--rw-r--r--   0     1001      123      118 2023-07-05 09:02:29.000000 lcax-0.1.2/packages/python/src/lcax/lcax/ffi.py
--rw-r--r--   0     1001      123     5916 2023-07-05 09:02:30.000000 lcax-0.1.2/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      123        0 2023-07-05 09:01:30.000000 lcax-0.1.2/packages/python/tests/.gitkeep
--rw-r--r--   0     1001      123      947 2023-07-05 09:01:30.000000 lcax-0.1.2/pyproject.toml
--rwxr-xr-x   0     1001      123      801 2023-07-05 09:03:06.000000 lcax-0.1.2/run-maturin-action.sh
--rw-r--r--   0     1001      123       16 2023-07-05 09:01:30.000000 lcax-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123     3136 2023-07-05 09:01:30.000000 lcax-0.1.2/src/project.rs
--rw-r--r--   0     1001      123      201 2023-07-05 09:01:30.000000 lcax-0.1.2/src/schemars.rs
--rw-r--r--   0     1001      123        0 2023-07-05 09:01:30.000000 lcax-0.1.2/tests/.gitkeep
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     1039 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/cicd.yaml
+-rw-r--r--   0     1001      123        0 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/csharp.yaml
+-rw-r--r--   0     1001      123     1303 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/docs.yaml
+-rw-r--r--   0     1001      123        0 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/javascript.yaml
+-rw-r--r--   0     1001      123     1363 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/python.yaml
+-rw-r--r--   0     1001      123      615 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/release.yaml
+-rw-r--r--   0     1001      123      863 2023-07-05 11:16:18.000000 lcax-0.1.3/.github/workflows/rust.yaml
+-rw-r--r--   0     1001      123     3182 2023-07-05 11:16:18.000000 lcax-0.1.3/.gitignore
+-rw-r--r--   0     1001      123      560 2023-07-05 11:16:18.000000 lcax-0.1.3/COPYRIGHT
+-rw-r--r--   0     1001      123    12302 2023-07-05 11:16:28.000000 lcax-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      123    10173 2023-07-05 11:16:18.000000 lcax-0.1.3/LICENSE
+-rw-r--r--   0     1001      123      516 2023-07-05 11:16:18.000000 lcax-0.1.3/README.md
+-rw-r--r--   0     1001      123    59384 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/assets/benchmark.png
+-rw-r--r--   0     1001      123    24746 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/assets/epdx.png
+-rw-r--r--   0     1001      123   660950 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/assets/lcax project.jpeg
+-rw-r--r--   0     1001      123     1342 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/data_structure.md
+-rw-r--r--   0     1001      123     1859 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/index.md
+-rw-r--r--   0     1001      123      127 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0     1001      123      335 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/overrides/stylesheets/extra.css
+-rw-r--r--   0     1001      123        0 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/schemas/.gitkeep
+-rw-r--r--   0     1001      123      507 2023-07-05 11:16:18.000000 lcax-0.1.3/docs/schemas.md
+-rw-r--r--   0     1001      123     1047 2023-07-05 11:16:18.000000 lcax-0.1.3/mkdocs.yml
+-rw-r--r--   0     1001      123      100 2023-07-05 11:16:18.000000 lcax-0.1.3/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      123      136 2023-07-05 11:17:06.000000 lcax-0.1.3/packages/python/src/lcax/lcax/__init__.py
+-rw-r--r--   0     1001      123      118 2023-07-05 11:17:06.000000 lcax-0.1.3/packages/python/src/lcax/lcax/ffi.py
+-rw-r--r--   0     1001      123     5916 2023-07-05 11:17:07.000000 lcax-0.1.3/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      123        0 2023-07-05 11:16:18.000000 lcax-0.1.3/packages/python/tests/.gitkeep
+-rw-r--r--   0     1001      123      947 2023-07-05 11:16:18.000000 lcax-0.1.3/pyproject.toml
+-rwxr-xr-x   0     1001      123      801 2023-07-05 11:17:37.000000 lcax-0.1.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123       16 2023-07-05 11:16:18.000000 lcax-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123     3136 2023-07-05 11:16:18.000000 lcax-0.1.3/src/project.rs
+-rw-r--r--   0     1001      123      201 2023-07-05 11:16:18.000000 lcax-0.1.3/src/schemars.rs
+-rw-r--r--   0     1001      123        0 2023-07-05 11:16:18.000000 lcax-0.1.3/tests/.gitkeep
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.3/PKG-INFO
```

### Comparing `lcax-0.1.2/Cargo.toml` & `lcax-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "lcax"
 description = "LCAx is an open, machine and human-readable data format for exchanging LCA results."
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Christian Kongsgaard <christian@kongsgaard.eu>"]
 edition = "2018"
 readme = "README.md"
 license-file = "LICENSE"
 homepage = "https://lcax.kongsgaard.eu"
 documentation = "https://lcax.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/lcax"
```

### Comparing `lcax-0.1.2/.github/workflows/cicd.yaml` & `lcax-0.1.3/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/.github/workflows/docs.yaml` & `lcax-0.1.3/.github/workflows/docs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,22 @@
           path: docs/schemas/
 
       - uses: actions/download-artifact@v2
         with:
           name: pydantic-schema
           path: docs/schemas/
 
+      - uses: actions/download-artifact@v2
+        with:
+          name: rust-schema
+          path: docs/schemas/
+
       - name: Build Docs
         run: |
+          source venv/bin/activate
           mkdocs build
 
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
         with:
           path: './site'
```

### Comparing `lcax-0.1.2/.github/workflows/python.yaml` & `lcax-0.1.3/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/.github/workflows/release.yaml` & `lcax-0.1.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/.github/workflows/rust.yaml` & `lcax-0.1.3/.github/workflows/rust.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,15 @@
 
       - name: Upload JSON Schema
         uses: actions/upload-artifact@v3
         with:
           name: json-schema
           path: 'lcax.schema.json'
 
+      - name: Upload Rust Schema
+        uses: actions/upload-artifact@v3
+        with:
+          name: rust-schema
+          path: 'src/project.rs'
+
       - name: Publish Crate
         run: cargo publish --allow-dirty --target x86_64-unknown-linux-gnu --token ${{ secrets.cargo_token }}
```

### Comparing `lcax-0.1.2/.gitignore` & `lcax-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/COPYRIGHT` & `lcax-0.1.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/Cargo.lock` & `lcax-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lcax"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "epdx",
  "schemars",
  "serde",
  "serde_json",
 ]
```

### Comparing `lcax-0.1.2/LICENSE` & `lcax-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/README.md` & `lcax-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/docs/assets/benchmark.png` & `lcax-0.1.3/docs/assets/benchmark.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/docs/assets/epdx.png` & `lcax-0.1.3/docs/assets/epdx.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/docs/assets/lcax project.jpeg` & `lcax-0.1.3/docs/assets/lcax project.jpeg`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/docs/data_structure.md` & `lcax-0.1.3/docs/data_structure.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/docs/index.md` & `lcax-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/mkdocs.yml` & `lcax-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/packages/python/src/lcax/pydantic.py` & `lcax-0.1.3/packages/python/src/lcax/pydantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  lcax.schema.json
-#   timestamp: 2023-07-05T09:02:30+00:00
+#   timestamp: 2023-07-05T11:17:07+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
```

### Comparing `lcax-0.1.2/pyproject.toml` & `lcax-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/run-maturin-action.sh` & `lcax-0.1.3/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/src/project.rs` & `lcax-0.1.3/src/project.rs`

 * *Files identical despite different names*

### Comparing `lcax-0.1.2/PKG-INFO` & `lcax-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: lcax
-Version: 0.1.2
+Version: 0.1.3
 Requires-Dist: cffi
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-datafixtures; extra == 'tests'
 Requires-Dist: pydantic >=1.8.2,<2.0.0; extra == 'code-gen'
 Requires-Dist: datamodel-code-generator; extra == 'code-gen'
 Requires-Dist: mkdocs-material >=8.1.4,<9.0.0; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1,<2.0.0; extra == 'doc'
-Requires-Dist: pytest; extra == 'tests'
-Requires-Dist: pytest-datafixtures; extra == 'tests'
+Provides-Extra: tests
 Provides-Extra: code-gen
 Provides-Extra: doc
-Provides-Extra: tests
 License-File: LICENSE
 License-File: LICENSE
 Summary: LCAx is an open, machine and human-readable data format for exchanging LCA results.
 Home-Page: https://lcax.kongsgaard.eu
 Author: Christian Kongsgaard <christian@kongsgaard.eu>
 Author-email: Christian Kongsgaard <christian@kongsgaard.eu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/ocni-dtu/lcax
 Project-URL: homepage, https://lcax.kongsgaard.eu
 Project-URL: documentation, https://lcax.kongsgaard.eu
+Project-URL: repository, https://github.com/ocni-dtu/lcax
 
 # LCAx
 
 The goal for LCAx is to make an open, machine and human-readable data format for exchanging LCA results,
 EPD's and assemblies. 
 
 We propose a simple three level data format with information on project, assembly and EPD level,
```

