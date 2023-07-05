# Comparing `tmp/dithering-0.1.15.tar.gz` & `tmp/dithering-0.1.17.tar.gz`

## Comparing `dithering-0.1.15.tar` & `dithering-0.1.17.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dithering-0.1.15/Cargo.toml
--rw-r--r--   0     1001      123     2805 2023-07-05 11:50:43.000000 dithering-0.1.15/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-05 11:50:43.000000 dithering-0.1.15/.gitignore
--rw-r--r--   0     1001      123     1067 2023-07-05 11:50:43.000000 dithering-0.1.15/LICENSE
--rw-r--r--   0     1001      123      500 2023-07-05 11:50:43.000000 dithering-0.1.15/README.md
--rw-r--r--   0     1001      123      103 2023-07-05 11:50:43.000000 dithering-0.1.15/dithering.pyi
--rw-r--r--   0     1001      123      369 2023-07-05 11:50:43.000000 dithering-0.1.15/pyproject.toml
--rw-r--r--   0     1001      123      337 2023-07-05 11:50:43.000000 dithering-0.1.15/setup.py
--rw-r--r--   0     1001      123      212 2023-07-05 11:50:43.000000 dithering-0.1.15/src/lib.rs
--rw-r--r--   0     1001      123       51 2023-07-05 11:50:43.000000 dithering-0.1.15/src/methods/mod.rs
--rw-r--r--   0     1001      123      888 2023-07-05 11:50:43.000000 dithering-0.1.15/src/methods/ordered.rs
--rw-r--r--   0     1001      123     9356 2023-07-05 11:50:43.000000 dithering-0.1.15/Cargo.lock
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 dithering-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 dithering-0.1.17/Cargo.toml
+-rw-r--r--   0     1001      123     2805 2023-07-05 13:18:31.000000 dithering-0.1.17/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-05 13:18:31.000000 dithering-0.1.17/.gitignore
+-rw-r--r--   0     1001      123     1067 2023-07-05 13:18:31.000000 dithering-0.1.17/LICENSE
+-rw-r--r--   0     1001      123      500 2023-07-05 13:18:31.000000 dithering-0.1.17/README.md
+-rw-r--r--   0     1001      123      103 2023-07-05 13:18:31.000000 dithering-0.1.17/dithering.pyi
+-rw-r--r--   0     1001      123      369 2023-07-05 13:18:31.000000 dithering-0.1.17/pyproject.toml
+-rw-r--r--   0     1001      123      212 2023-07-05 13:18:31.000000 dithering-0.1.17/src/lib.rs
+-rw-r--r--   0     1001      123       51 2023-07-05 13:18:31.000000 dithering-0.1.17/src/methods/mod.rs
+-rw-r--r--   0     1001      123      888 2023-07-05 13:18:31.000000 dithering-0.1.17/src/methods/ordered.rs
+-rw-r--r--   0     1001      123     9356 2023-07-05 13:18:31.000000 dithering-0.1.17/Cargo.lock
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 dithering-0.1.17/PKG-INFO
```

### Comparing `dithering-0.1.15/.github/workflows/CI.yml` & `dithering-0.1.17/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dithering-0.1.15/.gitignore` & `dithering-0.1.17/.gitignore`

 * *Files identical despite different names*

### Comparing `dithering-0.1.15/LICENSE` & `dithering-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `dithering-0.1.15/src/methods/ordered.rs` & `dithering-0.1.17/src/methods/ordered.rs`

 * *Files identical despite different names*

### Comparing `dithering-0.1.15/Cargo.lock` & `dithering-0.1.17/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dithering"
-version = "0.1.15"
+version = "0.1.17"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `dithering-0.1.15/PKG-INFO` & `dithering-0.1.17/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dithering
-Version: 0.1.15
+Version: 0.1.17
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
+Author: Patrik Larsson <patrik@backyardml.se>
+Author-email: Patrik Larsson <patrik@backyardml.se>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ## Dithering 
 ### Overview
 Welcome to Dithering, a project that brings efficient Rust implementation of various image dithering methods to be used in Python!
```

