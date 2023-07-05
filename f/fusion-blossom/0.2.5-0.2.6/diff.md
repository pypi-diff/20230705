# Comparing `tmp/fusion_blossom-0.2.5.tar.gz` & `tmp/fusion_blossom-0.2.6.tar.gz`

## Comparing `fusion_blossom-0.2.5.tar` & `fusion_blossom-0.2.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 fusion_blossom-0.2.5/Cargo.toml
--rw-r--r--   0      501       20      766 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/.gitignore
--rw-r--r--   0      501       20      587 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/CHANGELOG.md
--rw-r--r--   0      501       20      294 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/CITATION.cff
--rw-r--r--   0      501       20    52074 2023-06-24 19:12:20.000000 fusion_blossom-0.2.5/Cargo.lock
--rw-r--r--   0      501       20     1063 2022-04-15 02:53:09.000000 fusion_blossom-0.2.5/LICENSE
--rw-r--r--   0      501       20    12493 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/README.md
--rw-r--r--   0      501       20      731 2022-04-19 19:09:23.000000 fusion_blossom-0.2.5/blossomV/blossomV.cpp
--rw-r--r--   0      501       20     2183 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/build.rs
--rwxr-xr-x   0      501       20      172 2022-10-08 02:57:09.000000 fusion_blossom-0.2.5/install_environment.sh
--rw-rw-r--   0      501       20     1040 2022-04-19 03:09:55.000000 fusion_blossom-0.2.5/katex-header.html
--rw-r--r--   0      501       20     2390 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/pyproject.toml
--rw-r--r--   0      501       20       32 2023-05-29 20:07:24.000000 fusion_blossom-0.2.5/rust-toolchain.toml
--rw-r--r--   0      501       20       48 2023-06-25 03:00:38.000000 fusion_blossom-0.2.5/rustfmt.toml
--rw-r--r--   0      501       20       49 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/.gitignore
--rw-r--r--   0      501       20     5126 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/NOTES.md
--rw-r--r--   0      501       20     1695 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/scripts/count_Rust_LOC.py
--rw-r--r--   0      501       20     1930 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo.py
--rw-r--r--   0      501       20     1461 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo_local_render.py
--rw-r--r--   0      501       20     1293 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/demo_visualizer.py
--rw-r--r--   0      501       20      801 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/scripts/generate_icon.py
--rw-r--r--   0      501       20    26333 2023-06-25 03:14:00.000000 fusion_blossom-0.2.5/src/bin/aps2023.rs
--rw-r--r--   0      501       20    31586 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/bin/fusion-paper.rs
--rw-r--r--   0      501       20     3928 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/bin/partition-strategy.rs
--rw-r--r--   0      501       20     2834 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/blossom_v.rs
--rw-r--r--   0      501       20   170898 2022-10-09 15:39:13.000000 fusion_blossom-0.2.5/src/bottle.py
--rw-r--r--   0      501       20    47658 2023-06-25 03:04:12.000000 fusion_blossom-0.2.5/src/cli.rs
--rw-r--r--   0      501       20    15491 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/complete_graph.rs
--rw-r--r--   0      501       20    69826 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module.rs
--rw-r--r--   0      501       20    87247 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module_parallel.rs
--rw-r--r--   0      501       20   142629 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/dual_module_serial.rs
--rw-r--r--   0      501       20    55382 2023-06-25 03:16:42.000000 fusion_blossom-0.2.5/src/example_codes.rs
--rw-r--r--   0      501       20    38310 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/example_partition.rs
--rw-r--r--   0      501       20     5557 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/src/helper.py
--rw-r--r--   0      501       20    10844 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/lib.rs
--rw-r--r--   0      501       20       91 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/main.rs
--rw-r--r--   0      501       20    33564 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/mwpm_solver.rs
--rw-r--r--   0      501       20    27238 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/pointers.rs
--rw-r--r--   0      501       20    25243 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module.rs
--rw-r--r--   0      501       20    49538 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module_parallel.rs
--rw-r--r--   0      501       20   129499 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/primal_module_serial.rs
--rw-r--r--   0      501       20    37642 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/util.rs
--rw-r--r--   0      501       20    41597 2023-06-25 02:54:13.000000 fusion_blossom-0.2.5/src/visualize.rs
--rwxr-xr-x   0      501       20      615 2023-06-25 01:30:13.000000 fusion_blossom-0.2.5/test.sh
--rwxr-xr-x   0      501       20      860 2023-06-25 01:42:55.000000 fusion_blossom-0.2.5/test_build.sh
--rwxr-xr-x   0      501       20      742 2023-06-25 02:49:16.000000 fusion_blossom-0.2.5/test_check.sh
--rwxr-xr-x   0      501       20       81 2023-06-24 17:38:10.000000 fusion_blossom-0.2.5/test_python.sh
--rw-r--r--   0      501       20      825 2023-06-24 17:52:59.000000 fusion_blossom-0.2.5/tests/python/test_demo.py
--rw-r--r--   0      501       20     1528 2023-06-24 18:21:06.000000 fusion_blossom-0.2.5/tests/python/test_dynamic_weights.py
--rw-r--r--   0      501       20      517 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/cmd.js
--rw-r--r--   0      501       20       97 2022-04-20 18:38:15.000000 fusion_blossom-0.2.5/visualize/data/NOTE.md
--rw-r--r--   0      501       20     1115 2022-07-22 14:56:08.000000 fusion_blossom-0.2.5/visualize/data/filter_data.py
--rw-r--r--   0      501       20    41031 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/gui3d.js
--rw-r--r--   0      501       20      447 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/icon.svg
--rw-r--r--   0      501       20   222696 2022-04-28 01:17:21.000000 fusion_blossom-0.2.5/visualize/img/basic_CSS_3D_bottom_image.png
--rw-r--r--   0      501       20   585200 2022-10-07 19:20:39.000000 fusion_blossom-0.2.5/visualize/img/parallel_circuit_level.png
--rw-r--r--   0      501       20   481044 2022-10-07 19:19:34.000000 fusion_blossom-0.2.5/visualize/img/parallel_phenomenological.png
--rw-r--r--   0      501       20    70570 2022-10-07 19:18:06.000000 fusion_blossom-0.2.5/visualize/img/parallel_simple.png
--rw-r--r--   0      501       20    83192 2022-10-07 19:15:51.000000 fusion_blossom-0.2.5/visualize/img/serial_example.png
--rw-r--r--   0      501       20    90978 2022-10-07 18:59:02.000000 fusion_blossom-0.2.5/visualize/img/serial_random.png
--rw-r--r--   0      501       20    63904 2022-10-07 19:14:29.000000 fusion_blossom-0.2.5/visualize/img/serial_simple.png
--rw-r--r--   0      501       20    14997 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/index.html
--rw-r--r--   0      501       20    16448 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/index.js
--rw-r--r--   0      501       20     3884 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/mocker.js
--rw-r--r--   0      501       20   237147 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/package-lock.json
--rw-r--r--   0      501       20      472 2022-11-10 18:11:59.000000 fusion_blossom-0.2.5/visualize/package.json
--rw-r--r--   0      501       20    39914 2023-06-02 18:21:20.000000 fusion_blossom-0.2.5/visualize/partition-profile.html
--rw-r--r--   0      501       20     9266 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/patches.js
--rw-r--r--   0      501       20     8259 2023-05-16 01:08:37.000000 fusion_blossom-0.2.5/visualize/primal.js
--rwxr-xr-x   0      501       20     2446 2022-12-11 15:29:34.000000 fusion_blossom-0.2.5/visualize/server.py
--rw-r--r--   0        0        0    13954 1970-01-01 00:00:00.000000 fusion_blossom-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 fusion_blossom-0.2.6/Cargo.toml
+-rw-r--r--   0      501       20      766 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/.gitignore
+-rw-r--r--   0      501       20      587 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/CHANGELOG.md
+-rw-r--r--   0      501       20      294 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/CITATION.cff
+-rw-r--r--   0      501       20    52074 2023-07-05 02:55:40.000000 fusion_blossom-0.2.6/Cargo.lock
+-rw-r--r--   0      501       20     1063 2022-04-15 02:53:09.000000 fusion_blossom-0.2.6/LICENSE
+-rw-r--r--   0      501       20    12493 2023-06-02 18:21:20.000000 fusion_blossom-0.2.6/README.md
+-rw-r--r--   0      501       20      731 2022-04-19 19:09:23.000000 fusion_blossom-0.2.6/blossomV/blossomV.cpp
+-rw-r--r--   0      501       20     2183 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/build.rs
+-rwxr-xr-x   0      501       20      172 2022-10-08 02:57:09.000000 fusion_blossom-0.2.6/install_environment.sh
+-rw-rw-r--   0      501       20     1040 2022-04-19 03:09:55.000000 fusion_blossom-0.2.6/katex-header.html
+-rw-r--r--   0      501       20     2297 2023-07-05 02:57:45.000000 fusion_blossom-0.2.6/pyproject.toml
+-rw-r--r--   0      501       20       32 2023-05-29 20:07:24.000000 fusion_blossom-0.2.6/rust-toolchain.toml
+-rw-r--r--   0      501       20       48 2023-06-25 03:00:38.000000 fusion_blossom-0.2.6/rustfmt.toml
+-rw-r--r--   0      501       20       49 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/.gitignore
+-rw-r--r--   0      501       20     5126 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/NOTES.md
+-rw-r--r--   0      501       20     1695 2023-06-02 18:21:20.000000 fusion_blossom-0.2.6/scripts/count_Rust_LOC.py
+-rw-r--r--   0      501       20     1930 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/demo.py
+-rw-r--r--   0      501       20     1461 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/demo_local_render.py
+-rw-r--r--   0      501       20     1293 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/demo_visualizer.py
+-rw-r--r--   0      501       20      801 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/scripts/generate_icon.py
+-rw-r--r--   0      501       20    26333 2023-06-25 03:14:00.000000 fusion_blossom-0.2.6/src/bin/aps2023.rs
+-rw-r--r--   0      501       20    31586 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/bin/fusion-paper.rs
+-rw-r--r--   0      501       20     3928 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/bin/partition-strategy.rs
+-rw-r--r--   0      501       20     2834 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/blossom_v.rs
+-rw-r--r--   0      501       20   170898 2022-10-09 15:39:13.000000 fusion_blossom-0.2.6/src/bottle.py
+-rw-r--r--   0      501       20    47658 2023-06-25 03:04:12.000000 fusion_blossom-0.2.6/src/cli.rs
+-rw-r--r--   0      501       20    15491 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/complete_graph.rs
+-rw-r--r--   0      501       20    69826 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/dual_module.rs
+-rw-r--r--   0      501       20    87247 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/dual_module_parallel.rs
+-rw-r--r--   0      501       20   142629 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/dual_module_serial.rs
+-rw-r--r--   0      501       20    55382 2023-06-25 03:16:42.000000 fusion_blossom-0.2.6/src/example_codes.rs
+-rw-r--r--   0      501       20    38310 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/example_partition.rs
+-rw-r--r--   0      501       20     5557 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/src/helper.py
+-rw-r--r--   0      501       20    10844 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/lib.rs
+-rw-r--r--   0      501       20       91 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/main.rs
+-rw-r--r--   0      501       20    33564 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/mwpm_solver.rs
+-rw-r--r--   0      501       20    27238 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/pointers.rs
+-rw-r--r--   0      501       20    25243 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/primal_module.rs
+-rw-r--r--   0      501       20    49538 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/primal_module_parallel.rs
+-rw-r--r--   0      501       20   129499 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/primal_module_serial.rs
+-rw-r--r--   0      501       20    37872 2023-07-03 13:53:07.000000 fusion_blossom-0.2.6/src/util.rs
+-rw-r--r--   0      501       20    41597 2023-06-25 02:54:13.000000 fusion_blossom-0.2.6/src/visualize.rs
+-rwxr-xr-x   0      501       20      615 2023-06-25 01:30:13.000000 fusion_blossom-0.2.6/test.sh
+-rwxr-xr-x   0      501       20      860 2023-06-25 01:42:55.000000 fusion_blossom-0.2.6/test_build.sh
+-rwxr-xr-x   0      501       20      742 2023-06-25 02:49:16.000000 fusion_blossom-0.2.6/test_check.sh
+-rwxr-xr-x   0      501       20       81 2023-06-24 17:38:10.000000 fusion_blossom-0.2.6/test_python.sh
+-rw-r--r--   0      501       20      825 2023-06-24 17:52:59.000000 fusion_blossom-0.2.6/tests/python/test_demo.py
+-rw-r--r--   0      501       20     1528 2023-06-24 18:21:06.000000 fusion_blossom-0.2.6/tests/python/test_dynamic_weights.py
+-rw-r--r--   0      501       20      517 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/cmd.js
+-rw-r--r--   0      501       20       97 2022-04-20 18:38:15.000000 fusion_blossom-0.2.6/visualize/data/NOTE.md
+-rw-r--r--   0      501       20     1115 2022-07-22 14:56:08.000000 fusion_blossom-0.2.6/visualize/data/filter_data.py
+-rw-r--r--   0      501       20    41031 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/gui3d.js
+-rw-r--r--   0      501       20      447 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/icon.svg
+-rw-r--r--   0      501       20   222696 2022-04-28 01:17:21.000000 fusion_blossom-0.2.6/visualize/img/basic_CSS_3D_bottom_image.png
+-rw-r--r--   0      501       20   585200 2022-10-07 19:20:39.000000 fusion_blossom-0.2.6/visualize/img/parallel_circuit_level.png
+-rw-r--r--   0      501       20   481044 2022-10-07 19:19:34.000000 fusion_blossom-0.2.6/visualize/img/parallel_phenomenological.png
+-rw-r--r--   0      501       20    70570 2022-10-07 19:18:06.000000 fusion_blossom-0.2.6/visualize/img/parallel_simple.png
+-rw-r--r--   0      501       20    83192 2022-10-07 19:15:51.000000 fusion_blossom-0.2.6/visualize/img/serial_example.png
+-rw-r--r--   0      501       20    90978 2022-10-07 18:59:02.000000 fusion_blossom-0.2.6/visualize/img/serial_random.png
+-rw-r--r--   0      501       20    63904 2022-10-07 19:14:29.000000 fusion_blossom-0.2.6/visualize/img/serial_simple.png
+-rw-r--r--   0      501       20    14997 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/index.html
+-rw-r--r--   0      501       20    16448 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/index.js
+-rw-r--r--   0      501       20     3884 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/mocker.js
+-rw-r--r--   0      501       20   237147 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/package-lock.json
+-rw-r--r--   0      501       20      472 2022-11-10 18:11:59.000000 fusion_blossom-0.2.6/visualize/package.json
+-rw-r--r--   0      501       20    39914 2023-06-02 18:21:20.000000 fusion_blossom-0.2.6/visualize/partition-profile.html
+-rw-r--r--   0      501       20     9266 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/patches.js
+-rw-r--r--   0      501       20     8259 2023-05-16 01:08:37.000000 fusion_blossom-0.2.6/visualize/primal.js
+-rwxr-xr-x   0      501       20     2446 2022-12-11 15:29:34.000000 fusion_blossom-0.2.6/visualize/server.py
+-rw-r--r--   0        0        0    13954 1970-01-01 00:00:00.000000 fusion_blossom-0.2.6/PKG-INFO
```

### Comparing `fusion_blossom-0.2.5/Cargo.toml` & `fusion_blossom-0.2.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fusion-blossom"
-version = "0.2.5"
+version = "0.2.6"
 authors = ["Yue Wu <wuyue16pku@gmail.com>"]
 edition = "2021"
 license = "MIT"
 description = "A fast minimum-weight perfect matching solver for quantum error correction"
 readme = "README.md"
 homepage = "https://fusionblossom.com"
 repository = "https://github.com/yuewuo/fusion-blossom"
```

### Comparing `fusion_blossom-0.2.5/.gitignore` & `fusion_blossom-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/CHANGELOG.md` & `fusion_blossom-0.2.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/Cargo.lock` & `fusion_blossom-0.2.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -742,15 +742,15 @@
  "serde_json",
  "urlencoding",
  "weak-table",
 ]
 
 [[package]]
 name = "fusion-blossom"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "cc",
  "cfg-if",
  "chrono",
  "clap",
  "core_affinity",
  "derivative",
```

### Comparing `fusion_blossom-0.2.5/LICENSE` & `fusion_blossom-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/README.md` & `fusion_blossom-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/blossomV/blossomV.cpp` & `fusion_blossom-0.2.6/blossomV/blossomV.cpp`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/build.rs` & `fusion_blossom-0.2.6/build.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/katex-header.html` & `fusion_blossom-0.2.6/katex-header.html`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/pyproject.toml` & `fusion_blossom-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,17 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 
 # by default remove blossom V in the build because of license issue;
 # users can enable blossom V by removing `remove_blossom_v` feature, at the responsibility of users
 [tool.maturin]
-# features = ["python_binding", "remove_blossom_v", "u32_index", "dangerous_pointer"]
-features = ["python_binding", "remove_blossom_v"]
+features = ["python_binding", "remove_blossom_v", "dangerous_pointer", "u32_index", "i32_weight"]
 # Yue 2022.10.8: when maturin is called from `pip wheel`, it doesn't enable the above features, and thus pyo3 is not enabled
 #     since it cannot find pyo3, it falls back to use cffi (which is really confusing because I don't use cffi at all!)
 #     in order to solve cffi issue, I append "cffi" after requires = ["maturin>=0.12,<0.13"], and it works and generate some wheels
 #     but the problem remains: the wheel actually doesn't contain anything, simply because "python_binding" is not enabled
 #     I have to add `bindings = "pyo3"` to explicitly tell maturin to use pyo3, and then it complains that it cannot find pyo3
 #     later on I realize I have to provide the features in `cargo-extra-args` (credit to https://github.com/PyO3/maturin/issues/211)
 # conclusion: when calling `maturin develop`, it can read `features` above; but when called from `pip wheel`, it takes value below
 bindings = "pyo3"
-# cargo-extra-args = "--features python_binding,remove_blossom_v,u32_index,dangerous_pointer"
-cargo-extra-args = "--features python_binding,remove_blossom_v"
+cargo-extra-args = "--features python_binding,remove_blossom_v,dangerous_pointer,u32_index,i32_weight"
```

### Comparing `fusion_blossom-0.2.5/scripts/NOTES.md` & `fusion_blossom-0.2.6/scripts/NOTES.md`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/scripts/count_Rust_LOC.py` & `fusion_blossom-0.2.6/scripts/count_Rust_LOC.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/scripts/demo.py` & `fusion_blossom-0.2.6/scripts/demo.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/scripts/demo_local_render.py` & `fusion_blossom-0.2.6/scripts/demo_local_render.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/scripts/demo_visualizer.py` & `fusion_blossom-0.2.6/scripts/demo_visualizer.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/scripts/generate_icon.py` & `fusion_blossom-0.2.6/scripts/generate_icon.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/bin/aps2023.rs` & `fusion_blossom-0.2.6/src/bin/aps2023.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/bin/fusion-paper.rs` & `fusion_blossom-0.2.6/src/bin/fusion-paper.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/bin/partition-strategy.rs` & `fusion_blossom-0.2.6/src/bin/partition-strategy.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/blossom_v.rs` & `fusion_blossom-0.2.6/src/blossom_v.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/bottle.py` & `fusion_blossom-0.2.6/src/bottle.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/cli.rs` & `fusion_blossom-0.2.6/src/cli.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/complete_graph.rs` & `fusion_blossom-0.2.6/src/complete_graph.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/dual_module.rs` & `fusion_blossom-0.2.6/src/dual_module.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/dual_module_parallel.rs` & `fusion_blossom-0.2.6/src/dual_module_parallel.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/dual_module_serial.rs` & `fusion_blossom-0.2.6/src/dual_module_serial.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/example_codes.rs` & `fusion_blossom-0.2.6/src/example_codes.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/example_partition.rs` & `fusion_blossom-0.2.6/src/example_partition.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/helper.py` & `fusion_blossom-0.2.6/src/helper.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/lib.rs` & `fusion_blossom-0.2.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/mwpm_solver.rs` & `fusion_blossom-0.2.6/src/mwpm_solver.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/pointers.rs` & `fusion_blossom-0.2.6/src/pointers.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/primal_module.rs` & `fusion_blossom-0.2.6/src/primal_module.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/primal_module_parallel.rs` & `fusion_blossom-0.2.6/src/primal_module_parallel.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/primal_module_serial.rs` & `fusion_blossom-0.2.6/src/primal_module_serial.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/src/util.rs` & `fusion_blossom-0.2.6/src/util.rs`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,30 @@
     /// the vertices corresponding to defect measurements
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
     pub defect_vertices: Vec<VertexIndex>,
     /// the edges that experience erasures, i.e. known errors;
     /// note that erasure decoding can also be implemented using `dynamic_weights`,
     /// but for user convenience we keep this interface
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    #[serde(default = "default_erasures")]
     pub erasures: Vec<EdgeIndex>,
     /// general dynamically weighted edges
     #[cfg_attr(feature = "python_binding", pyo3(get, set))]
+    #[serde(default = "default_dynamic_weights")]
     pub dynamic_weights: Vec<(EdgeIndex, Weight)>,
 }
 
+pub fn default_dynamic_weights() -> Vec<(EdgeIndex, Weight)> {
+    vec![]
+}
+
+pub fn default_erasures() -> Vec<EdgeIndex> {
+    vec![]
+}
+
 impl SyndromePattern {
     pub fn new(defect_vertices: Vec<VertexIndex>, erasures: Vec<EdgeIndex>) -> Self {
         Self {
             defect_vertices,
             erasures,
             dynamic_weights: vec![],
         }
```

### Comparing `fusion_blossom-0.2.5/src/visualize.rs` & `fusion_blossom-0.2.6/src/visualize.rs`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/test.sh` & `fusion_blossom-0.2.6/test.sh`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/test_build.sh` & `fusion_blossom-0.2.6/test_build.sh`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/test_check.sh` & `fusion_blossom-0.2.6/test_check.sh`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/tests/python/test_demo.py` & `fusion_blossom-0.2.6/tests/python/test_demo.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/tests/python/test_dynamic_weights.py` & `fusion_blossom-0.2.6/tests/python/test_dynamic_weights.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/cmd.js` & `fusion_blossom-0.2.6/visualize/cmd.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/data/filter_data.py` & `fusion_blossom-0.2.6/visualize/data/filter_data.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/gui3d.js` & `fusion_blossom-0.2.6/visualize/gui3d.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/basic_CSS_3D_bottom_image.png` & `fusion_blossom-0.2.6/visualize/img/basic_CSS_3D_bottom_image.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/parallel_circuit_level.png` & `fusion_blossom-0.2.6/visualize/img/parallel_circuit_level.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/parallel_phenomenological.png` & `fusion_blossom-0.2.6/visualize/img/parallel_phenomenological.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/parallel_simple.png` & `fusion_blossom-0.2.6/visualize/img/parallel_simple.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/serial_example.png` & `fusion_blossom-0.2.6/visualize/img/serial_example.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/serial_random.png` & `fusion_blossom-0.2.6/visualize/img/serial_random.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/img/serial_simple.png` & `fusion_blossom-0.2.6/visualize/img/serial_simple.png`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/index.html` & `fusion_blossom-0.2.6/visualize/index.html`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/index.js` & `fusion_blossom-0.2.6/visualize/index.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/mocker.js` & `fusion_blossom-0.2.6/visualize/mocker.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/package-lock.json` & `fusion_blossom-0.2.6/visualize/package-lock.json`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/partition-profile.html` & `fusion_blossom-0.2.6/visualize/partition-profile.html`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/patches.js` & `fusion_blossom-0.2.6/visualize/patches.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/primal.js` & `fusion_blossom-0.2.6/visualize/primal.js`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/visualize/server.py` & `fusion_blossom-0.2.6/visualize/server.py`

 * *Files identical despite different names*

### Comparing `fusion_blossom-0.2.5/PKG-INFO` & `fusion_blossom-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion_blossom
-Version: 0.2.5
+Version: 0.2.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

