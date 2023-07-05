# Comparing `tmp/dithering-0.1.0.tar.gz` & `tmp/dithering-0.1.11.tar.gz`

## Comparing `dithering-0.1.0.tar` & `dithering-0.1.11.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 dithering-0.1.0/Cargo.toml
--rw-r--r--   0      503       20     2807 2023-07-04 19:41:25.000000 dithering-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      503       20      685 2023-07-04 19:23:22.000000 dithering-0.1.0/.gitignore
--rw-r--r--   0      503       20     1067 2023-07-04 19:25:49.000000 dithering-0.1.0/LICENSE
--rw-r--r--   0      503       20      149 2023-07-04 19:55:15.000000 dithering-0.1.0/README.md
--rw-r--r--   0      503       20      103 2023-07-04 19:29:37.000000 dithering-0.1.0/dithering.pyi
--rw-r--r--   0      503       20      369 2023-07-04 19:23:22.000000 dithering-0.1.0/pyproject.toml
--rw-r--r--   0      503       20     1031 2023-07-04 19:55:35.000000 dithering-0.1.0/src/lib.rs
--rw-r--r--   0      503       20     9355 2023-07-04 19:27:33.000000 dithering-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 dithering-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dithering-0.1.11/Cargo.toml
+-rw-r--r--   0     1001      123     2805 2023-07-05 07:16:50.000000 dithering-0.1.11/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-05 07:16:50.000000 dithering-0.1.11/.gitignore
+-rw-r--r--   0     1001      123     1067 2023-07-05 07:16:50.000000 dithering-0.1.11/LICENSE
+-rw-r--r--   0     1001      123      500 2023-07-05 07:16:50.000000 dithering-0.1.11/README.md
+-rw-r--r--   0     1001      123      103 2023-07-05 07:16:50.000000 dithering-0.1.11/dithering.pyi
+-rw-r--r--   0     1001      123      369 2023-07-05 07:16:50.000000 dithering-0.1.11/pyproject.toml
+-rw-r--r--   0     1001      123     1031 2023-07-05 07:16:50.000000 dithering-0.1.11/src/lib.rs
+-rw-r--r--   0     1001      123     9356 2023-07-05 07:16:59.000000 dithering-0.1.11/Cargo.lock
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 dithering-0.1.11/PKG-INFO
```

### Comparing `dithering-0.1.0/.github/workflows/CI.yml` & `dithering-0.1.11/.github/workflows/CI.yml`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    if: startsWith(github.ref, 'refs/tags/')
     needs: [linux, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
```

### Comparing `dithering-0.1.0/.gitignore` & `dithering-0.1.11/.gitignore`

 * *Files identical despite different names*

### Comparing `dithering-0.1.0/LICENSE` & `dithering-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `dithering-0.1.0/src/lib.rs` & `dithering-0.1.11/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dithering-0.1.0/Cargo.lock` & `dithering-0.1.11/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dithering"
-version = "0.1.0"
+version = "0.1.11"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

