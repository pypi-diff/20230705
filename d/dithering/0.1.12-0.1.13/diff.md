# Comparing `tmp/dithering-0.1.12.tar.gz` & `tmp/dithering-0.1.13.tar.gz`

## Comparing `dithering-0.1.12.tar` & `dithering-0.1.13.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dithering-0.1.12/Cargo.toml
--rw-r--r--   0     1001      123     2805 2023-07-05 09:03:08.000000 dithering-0.1.12/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-05 09:03:08.000000 dithering-0.1.12/.gitignore
--rw-r--r--   0     1001      123     1067 2023-07-05 09:03:08.000000 dithering-0.1.12/LICENSE
--rw-r--r--   0     1001      123      500 2023-07-05 09:03:08.000000 dithering-0.1.12/README.md
--rw-r--r--   0     1001      123      103 2023-07-05 09:03:08.000000 dithering-0.1.12/dithering.pyi
--rw-r--r--   0     1001      123      369 2023-07-05 09:03:08.000000 dithering-0.1.12/pyproject.toml
--rw-r--r--   0     1001      123      337 2023-07-05 09:03:08.000000 dithering-0.1.12/setup.py
--rw-r--r--   0     1001      123      212 2023-07-05 09:03:08.000000 dithering-0.1.12/src/lib.rs
--rw-r--r--   0     1001      123       51 2023-07-05 09:03:08.000000 dithering-0.1.12/src/methods/mod.rs
--rw-r--r--   0     1001      123      888 2023-07-05 09:03:08.000000 dithering-0.1.12/src/methods/ordered.rs
--rw-r--r--   0     1001      123     9356 2023-07-05 09:03:08.000000 dithering-0.1.12/Cargo.lock
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 dithering-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dithering-0.1.13/Cargo.toml
+-rw-r--r--   0     1001      123     2805 2023-07-05 09:48:26.000000 dithering-0.1.13/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-05 09:48:26.000000 dithering-0.1.13/.gitignore
+-rw-r--r--   0     1001      123     1067 2023-07-05 09:48:26.000000 dithering-0.1.13/LICENSE
+-rw-r--r--   0     1001      123      500 2023-07-05 09:48:26.000000 dithering-0.1.13/README.md
+-rw-r--r--   0     1001      123      103 2023-07-05 09:48:26.000000 dithering-0.1.13/dithering.pyi
+-rw-r--r--   0     1001      123      369 2023-07-05 09:48:26.000000 dithering-0.1.13/pyproject.toml
+-rw-r--r--   0     1001      123      337 2023-07-05 09:48:26.000000 dithering-0.1.13/setup.py
+-rw-r--r--   0     1001      123      212 2023-07-05 09:48:26.000000 dithering-0.1.13/src/lib.rs
+-rw-r--r--   0     1001      123       51 2023-07-05 09:48:26.000000 dithering-0.1.13/src/methods/mod.rs
+-rw-r--r--   0     1001      123      888 2023-07-05 09:48:26.000000 dithering-0.1.13/src/methods/ordered.rs
+-rw-r--r--   0     1001      123     9356 2023-07-05 09:48:26.000000 dithering-0.1.13/Cargo.lock
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 dithering-0.1.13/PKG-INFO
```

### Comparing `dithering-0.1.12/.github/workflows/CI.yml` & `dithering-0.1.13/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dithering-0.1.12/.gitignore` & `dithering-0.1.13/.gitignore`

 * *Files identical despite different names*

### Comparing `dithering-0.1.12/LICENSE` & `dithering-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `dithering-0.1.12/src/methods/ordered.rs` & `dithering-0.1.13/src/methods/ordered.rs`

 * *Files identical despite different names*

### Comparing `dithering-0.1.12/Cargo.lock` & `dithering-0.1.13/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dithering"
-version = "0.1.12"
+version = "0.1.13"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `dithering-0.1.12/PKG-INFO` & `dithering-0.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dithering
-Version: 0.1.12
+Version: 0.1.13
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

