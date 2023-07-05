# Comparing `tmp/typeset_soren_n-2.0.1.tar.gz` & `tmp/typeset_soren_n-2.0.2.tar.gz`

## Comparing `typeset_soren_n-2.0.1.tar` & `typeset_soren_n-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 typeset_soren_n-2.0.1/Cargo.toml
--rw-r--r--   0     1001      123      102 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/.github/dependabot.yml
--rw-r--r--   0     1001      123     2983 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/.gitignore
--rw-r--r--   0     1001      123      160 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/.readthedocs.yaml
--rw-r--r--   0     1001      123     1072 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/LICENSE
--rw-r--r--   0     1001      123    11133 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/README.md
--rw-r--r--   0     1001      123      861 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/pyproject.toml
--rw-r--r--   0     1001      123      990 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/src/layout.pest
--rw-r--r--   0     1001      123     3819 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/src/lib.rs
--rw-r--r--   0     1001      123     5628 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/src/parser.rs
--rw-r--r--   0     1001      123    12500 2023-06-22 08:16:56.000000 typeset_soren_n-2.0.1/Cargo.lock
--rw-r--r--   0        0        0    11994 1970-01-01 00:00:00.000000 typeset_soren_n-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 typeset_soren_n-2.0.2/Cargo.toml
+-rw-r--r--   0     1001      123      102 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2983 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/.gitignore
+-rw-r--r--   0     1001      123      160 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/.readthedocs.yaml
+-rw-r--r--   0     1001      123     1072 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/LICENSE
+-rw-r--r--   0     1001      123    11133 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/README.md
+-rw-r--r--   0     1001      123      861 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/pyproject.toml
+-rw-r--r--   0     1001      123      990 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/src/layout.pest
+-rw-r--r--   0     1001      123     3819 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     5628 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/src/parser.rs
+-rw-r--r--   0     1001      123    12501 2023-07-05 15:50:28.000000 typeset_soren_n-2.0.2/Cargo.lock
+-rw-r--r--   0        0        0    11994 1970-01-01 00:00:00.000000 typeset_soren_n-2.0.2/PKG-INFO
```

### Comparing `typeset_soren_n-2.0.1/Cargo.toml` & `typeset_soren_n-2.0.2/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "typeset-py"
 description = "A DSL for defining source code pretty printers"
-version = "2.0.1"
+version = "2.0.2"
 edition = "2021"
 authors = ["Soren Norbaek <sorennorbaek@gmail.com>"]
 homepage = "https://docs.rs/typeset/latest/typeset/"
 repository = "https://github.com/soren-n/typeset-py"
 documentation = "https://docs.rs/typeset/latest/typeset/"
 keywords = ["dsl", "pretty", "printer"]
 categories = ["compilers", "template-engine"]
@@ -17,10 +17,10 @@
 name = "typeset"
 crate-type = ["cdylib"]
 
 [dependencies]
 lazy_static = "1.4.0"
 pest = "2.7.0"
 pest_derive = "2.7.0"
-pyo3 = "0.19.0"
+pyo3 = "0.19.1"
 pyo3-log = "0.8.2"
-typeset = "2.0.1"
+typeset = "2.0.2"
```

### Comparing `typeset_soren_n-2.0.1/.github/workflows/CI.yml` & `typeset_soren_n-2.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/.gitignore` & `typeset_soren_n-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/LICENSE` & `typeset_soren_n-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/README.md` & `typeset_soren_n-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/pyproject.toml` & `typeset_soren_n-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/src/layout.pest` & `typeset_soren_n-2.0.2/src/layout.pest`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/src/lib.rs` & `typeset_soren_n-2.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/src/parser.rs` & `typeset_soren_n-2.0.2/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typeset_soren_n-2.0.1/Cargo.lock` & `typeset_soren_n-2.0.2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -194,53 +194,53 @@
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -251,40 +251,40 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -369,24 +369,24 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "typeset"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09f12915b23cffdd5303150e257b679009608d905374f57f9c1876a25309458c"
+checksum = "166fb515ebc4803b995bc586d7e2a5cc4da9b3de5da669056a26cfaf0364d704"
 dependencies = [
  "bumpalo",
 ]
 
 [[package]]
 name = "typeset-py"
-version = "2.0.1"
+version = "2.0.2"
 dependencies = [
  "lazy_static",
  "pest",
  "pest_derive",
  "pyo3",
  "pyo3-log",
  "typeset",
@@ -396,17 +396,17 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `typeset_soren_n-2.0.1/PKG-INFO` & `typeset_soren_n-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeset-soren-n
-Version: 2.0.1
+Version: 2.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 License-File: LICENSE
 Summary: A DSL for defining source code pretty printers
 Keywords: dsl,pretty,printer
```

