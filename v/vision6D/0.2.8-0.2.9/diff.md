# Comparing `tmp/vision6D-0.2.8.tar.gz` & `tmp/vision6D-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-cr8lmfij\vision6D-0.2.8.tar", last modified: Fri Jun 30 14:18:17 2023, max compression
+gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-0iowuqvv\vision6D-0.2.9.tar", last modified: Wed Jul  5 00:52:47 2023, max compression
```

## Comparing `vision6D-0.2.8.tar` & `vision6D-0.2.9.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.213688 vision6D-0.2.8/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1361 2023-06-30 14:18:17.213688 vision6D-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.8/README.md
--rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0     2050 2023-06-30 14:18:17.217684 vision6D-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      345 2023-06-30 14:14:27.000000 vision6D-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.076685 vision6D-0.2.8/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.8/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.8/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.088681 vision6D-0.2.8/vision6D/
--rw-rw-rw-   0        0        0     1050 2023-06-26 14:07:57.000000 vision6D-0.2.8/vision6D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.151682 vision6D-0.2.8/vision6D/components/
--rw-rw-rw-   0        0        0      403 2023-06-25 23:11:35.000000 vision6D-0.2.8/vision6D/components/__init__.py
--rw-rw-rw-   0        0        0     1735 2023-06-25 17:11:58.000000 vision6D-0.2.8/vision6D/components/camera_store.py
--rw-rw-rw-   0        0        0     2417 2023-06-26 02:53:06.000000 vision6D-0.2.8/vision6D/components/folder_store.py
--rw-rw-rw-   0        0        0     1998 2023-06-27 14:55:28.000000 vision6D-0.2.8/vision6D/components/image_store.py
--rw-rw-rw-   0        0        0     2756 2023-06-28 13:51:18.000000 vision6D-0.2.8/vision6D/components/mask_store.py
--rw-rw-rw-   0        0        0     6338 2023-06-27 14:55:54.000000 vision6D-0.2.8/vision6D/components/mesh_store.py
--rw-rw-rw-   0        0        0      242 2023-06-24 14:48:03.000000 vision6D-0.2.8/vision6D/components/singleton.py
--rw-rw-rw-   0        0        0     1983 2023-06-26 03:58:35.000000 vision6D-0.2.8/vision6D/components/video_store.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.167685 vision6D-0.2.8/vision6D/containers/
--rw-rw-rw-   0        0        0      429 2023-06-26 19:34:52.000000 vision6D-0.2.8/vision6D/containers/__init__.py
--rw-rw-rw-   0        0        0     3815 2023-06-27 01:22:39.000000 vision6D-0.2.8/vision6D/containers/camera_container.py
--rw-rw-rw-   0        0        0     4027 2023-06-29 13:21:48.000000 vision6D-0.2.8/vision6D/containers/image_container.py
--rw-rw-rw-   0        0        0     5492 2023-06-29 13:21:55.000000 vision6D-0.2.8/vision6D/containers/mask_container.py
--rw-rw-rw-   0        0        0    17728 2023-06-29 13:22:01.000000 vision6D-0.2.8/vision6D/containers/mesh_container.py
--rw-rw-rw-   0        0        0    11023 2023-06-29 14:00:00.000000 vision6D-0.2.8/vision6D/containers/pnp_container.py
--rw-rw-rw-   0        0        0     9570 2023-06-28 23:58:17.000000 vision6D-0.2.8/vision6D/containers/video_folder_container.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.179691 vision6D-0.2.8/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.8/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0    12109 2023-06-06 19:10:46.000000 vision6D-0.2.8/vision6D/data/style.qss
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.183685 vision6D-0.2.8/vision6D/entry/
--rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.8/vision6D/entry/__init__.py
--rw-rw-rw-   0        0        0      428 2023-06-26 13:21:29.000000 vision6D-0.2.8/vision6D/entry/main.py
--rw-rw-rw-   0        0        0    33624 2023-06-29 13:18:10.000000 vision6D-0.2.8/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    16150 2023-06-28 23:06:33.000000 vision6D-0.2.8/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.210687 vision6D-0.2.8/vision6D/widgets/
--rw-rw-rw-   0        0        0      583 2023-06-26 03:46:38.000000 vision6D-0.2.8/vision6D/widgets/__init__.py
--rw-rw-rw-   0        0        0     3216 2023-06-26 04:19:25.000000 vision6D-0.2.8/vision6D/widgets/calibration_pop_window.py
--rw-rw-rw-   0        0        0     1789 2023-06-26 04:18:34.000000 vision6D-0.2.8/vision6D/widgets/camera_props_input_dialog.py
--rw-rw-rw-   0        0        0     1437 2023-06-28 02:56:35.000000 vision6D-0.2.8/vision6D/widgets/custom_qt_interactor.py
--rw-rw-rw-   0        0        0     2314 2023-06-26 16:29:32.000000 vision6D-0.2.8/vision6D/widgets/get_text_dialog.py
--rw-rw-rw-   0        0        0     3539 2023-06-27 03:53:28.000000 vision6D-0.2.8/vision6D/widgets/label_window.py
--rw-rw-rw-   0        0        0     1063 2023-06-26 04:18:12.000000 vision6D-0.2.8/vision6D/widgets/popup_dialog.py
--rw-rw-rw-   0        0        0     6876 2023-06-26 04:17:38.000000 vision6D-0.2.8/vision6D/widgets/video_player.py
--rw-rw-rw-   0        0        0     5509 2023-06-26 04:17:03.000000 vision6D-0.2.8/vision6D/widgets/video_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.132683 vision6D-0.2.8/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1361 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1363 2023-06-30 14:18:17.000000 vision6D-0.2.8/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 14:18:17.000000 vision6D-0.2.8/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.878274 vision6D-0.2.9/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1364 2023-07-05 00:52:47.879274 vision6D-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.9/README.md
+-rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0     2111 2023-07-05 00:52:47.882274 vision6D-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-07-05 00:46:04.000000 vision6D-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.762274 vision6D-0.2.9/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.9/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.9/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.766274 vision6D-0.2.9/vision6D/
+-rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.830274 vision6D-0.2.9/vision6D/components/
+-rw-rw-rw-   0        0        0      403 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/__init__.py
+-rw-rw-rw-   0        0        0     1965 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/camera_store.py
+-rw-rw-rw-   0        0        0     2647 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/folder_store.py
+-rw-rw-rw-   0        0        0     2229 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/image_store.py
+-rw-rw-rw-   0        0        0     2980 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/mask_store.py
+-rw-rw-rw-   0        0        0     6567 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/mesh_store.py
+-rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/singleton.py
+-rw-rw-rw-   0        0        0     2206 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/video_store.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.845273 vision6D-0.2.9/vision6D/containers/
+-rw-rw-rw-   0        0        0      429 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/__init__.py
+-rw-rw-rw-   0        0        0     4061 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/camera_container.py
+-rw-rw-rw-   0        0        0     4274 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/image_container.py
+-rw-rw-rw-   0        0        0     5739 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/mask_container.py
+-rw-rw-rw-   0        0        0    17556 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/mesh_container.py
+-rw-rw-rw-   0        0        0    11304 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/pnp_container.py
+-rw-rw-rw-   0        0        0     9828 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/video_folder_container.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.851272 vision6D-0.2.9/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.9/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.855273 vision6D-0.2.9/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.9/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    35066 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/mainwindow.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.858274 vision6D-0.2.9/vision6D/tools/
+-rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/tools/__init__.py
+-rw-rw-rw-   0        0        0    16464 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.876274 vision6D-0.2.9/vision6D/widgets/
+-rw-rw-rw-   0        0        0      583 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/widgets/calibration_pop_window.py
+-rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/camera_props_input_dialog.py
+-rw-rw-rw-   0        0        0     1722 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/custom_qt_interactor.py
+-rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/get_text_dialog.py
+-rw-rw-rw-   0        0        0     3766 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/label_window.py
+-rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/popup_dialog.py
+-rw-rw-rw-   0        0        0     7083 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/video_player.py
+-rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/video_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.807274 vision6D-0.2.9/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1396 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.8/LICENSE` & `vision6D-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/PKG-INFO` & `vision6D-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.8
+Version: 0.2.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
-Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
+Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vision6D-0.2.8/README.md` & `vision6D-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/setup.cfg` & `vision6D-0.2.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e38 0d0a 7572  sion = 0.2.8..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e39 0d0a 7572  sion = 0.2.9..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -34,96 +34,99 @@
 00000210: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
 00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000230: 6f6e 203a 3a20 332e 390d 0a70 726f 6a65  on :: 3.9..proje
 00000240: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
 00000250: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
 00000260: 3a2f 2f67 6974 6875 622e 636f 6d2f 796b  ://github.com/yk
 00000270: 7a7a 6b79 2f76 6973 696f 6e36 442f 6973  zzky/vision6D/is
-00000280: 7375 6573 0d0a 0d0a 5b6f 7074 696f 6e73  sues....[options
-00000290: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
-000002a0: 6e64 3a0d 0a69 6e63 6c75 6465 5f70 6163  nd:..include_pac
-000002b0: 6b61 6765 5f64 6174 6120 3d20 7472 7565  kage_data = true
-000002c0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-000002d0: 7320 3d20 3e3d 2033 2e36 0d0a 7465 7374  s = >= 3.6..test
-000002e0: 5f73 7569 7465 203d 2074 6573 7473 0d0a  _suite = tests..
-000002f0: 7365 7475 705f 7265 7175 6972 6573 203d  setup_requires =
-00000300: 200d 0a09 7365 7475 7074 6f6f 6c73 0d0a   ...setuptools..
-00000310: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000320: 203d 200d 0a09 7079 7669 7374 613e 3d30   = ...pyvista>=0
-00000330: 2e33 392e 310d 0a09 6e75 6d70 793e 3d31  .39.1...numpy>=1
-00000340: 2e32 332e 350d 0a09 6d61 7470 6c6f 746c  .23.5...matplotl
-00000350: 6962 3e3d 332e 352e 320d 0a09 7472 696d  ib>=3.5.2...trim
-00000360: 6573 683e 3d33 2e31 342e 300d 0a09 6561  esh>=3.14.0...ea
-00000370: 7379 6469 6374 3e3d 312e 390d 0a09 7069  sydict>=1.9...pi
-00000380: 6c6c 6f77 3e3d 392e 322e 300d 0a09 7363  llow>=9.2.0...sc
-00000390: 6970 793e 3d31 2e38 2e31 0d0a 0970 7974  ipy>=1.8.1...pyt
-000003a0: 6573 743e 3d37 2e32 2e30 0d0a 0970 7974  est>=7.2.0...pyt
-000003b0: 6573 742d 6c61 7a79 2d66 6978 7475 7265  est-lazy-fixture
-000003c0: 3e3d 302e 362e 330d 0a09 7072 652d 636f  >=0.6.3...pre-co
-000003d0: 6d6d 6974 3e3d 322e 3231 2e30 0d0a 096f  mmit>=2.21.0...o
-000003e0: 7065 6e63 762d 7079 7468 6f6e 2d68 6561  pencv-python-hea
-000003f0: 646c 6573 733e 3d34 2e37 2e30 2e36 380d  dless>=4.7.0.68.
-00000400: 0a09 7363 696b 6974 2d69 6d61 6765 3e3d  ..scikit-image>=
-00000410: 302e 3139 2e33 0d0a 0963 6861 7264 6574  0.19.3...chardet
-00000420: 3e3d 352e 312e 300d 0a09 7079 6765 6f64  >=5.1.0...pygeod
-00000430: 6573 6963 3e3d 302e 312e 380d 0a09 5079  esic>=0.1.8...Py
-00000440: 5174 353e 3d35 2e31 352e 390d 0a09 7079  Qt5>=5.15.9...py
-00000450: 7669 7374 6171 743e 3d30 2e31 302e 300d  vistaqt>=0.10.0.
-00000460: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000470: 6167 655f 6461 7461 5d0d 0a2a 203d 202a  age_data]..* = *
-00000480: 2e70 6e67 2c20 2a2e 6a70 672c 202a 2e71  .png, *.jpg, *.q
-00000490: 6d6c 0d0a 0d0a 5b62 6469 7374 5f77 6865  ml....[bdist_whe
-000004a0: 656c 5d0d 0a75 6e69 7665 7273 616c 203d  el]..universal =
-000004b0: 2074 7275 650d 0a0d 0a5b 7364 6973 745d   true....[sdist]
-000004c0: 0d0a 666f 726d 6174 7320 3d20 7a69 702c  ..formats = zip,
-000004d0: 2067 7a74 6172 0d0a 0d0a 5b63 6f76 6572   gztar....[cover
-000004e0: 6167 653a 7265 706f 7274 5d0d 0a73 686f  age:report]..sho
-000004f0: 775f 6d69 7373 696e 6720 3d20 7472 7565  w_missing = true
-00000500: 0d0a 6578 636c 7564 655f 6c69 6e65 7320  ..exclude_lines 
-00000510: 3d20 0d0a 0970 7261 676d 613a 206e 6f20  = ...pragma: no 
-00000520: 636f 7665 720d 0a09 6966 2046 616c 7365  cover...if False
-00000530: 0d0a 0d0a 5b67 7265 656e 5d0d 0a66 696c  ....[green]..fil
-00000540: 652d 7061 7474 6572 6e20 3d20 7465 7374  e-pattern = test
-00000550: 5f2a 2e70 790d 0a76 6572 626f 7365 203d  _*.py..verbose =
-00000560: 2032 0d0a 6e6f 2d73 6b69 702d 7265 706f   2..no-skip-repo
-00000570: 7274 203d 2074 7275 650d 0a71 7569 6574  rt = true..quiet
-00000580: 2d73 7464 6f75 7420 3d20 7472 7565 0d0a  -stdout = true..
-00000590: 7275 6e2d 636f 7665 7261 6765 203d 2074  run-coverage = t
-000005a0: 7275 650d 0a0d 0a5b 7079 646f 6373 7479  rue....[pydocsty
-000005b0: 6c65 5d0d 0a6d 6174 6368 2d64 6972 203d  le]..match-dir =
-000005c0: 2028 3f21 7465 7374 7329 283f 2172 6573   (?!tests)(?!res
-000005d0: 6f75 7263 6573 2928 3f21 646f 6373 295b  ources)(?!docs)[
-000005e0: 5e5c 2e5d 2e2a 0d0a 6d61 7463 6820 3d20  ^\.].*..match = 
-000005f0: 283f 2174 6573 7429 283f 2173 6574 7570  (?!test)(?!setup
-00000600: 295b 5e5c 2e5f 5d2e 2a5c 2e70 790d 0a69  )[^\._].*\.py..i
-00000610: 6e68 6572 6974 203d 2066 616c 7365 0d0a  nherit = false..
-00000620: 6967 6e6f 7265 203d 2044 3230 302c 2044  ignore = D200, D
-00000630: 3230 332c 2044 3231 332c 2044 3430 362c  203, D213, D406,
-00000640: 2044 3430 370d 0a0d 0a5b 666c 616b 6538   D407....[flake8
-00000650: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
-00000660: 7468 203d 2039 390d 0a64 6f63 7465 7374  th = 99..doctest
-00000670: 7320 3d20 5472 7565 0d0a 6578 636c 7564  s = True..exclud
-00000680: 6520 3d20 2e67 6974 2c20 2e65 6767 732c  e = .git, .eggs,
-00000690: 205f 5f70 7963 6163 6865 5f5f 2c20 7465   __pycache__, te
-000006a0: 7374 732f 2c20 646f 6373 2f2c 2062 7569  sts/, docs/, bui
-000006b0: 6c64 2f2c 2064 6973 742f 0d0a 0d0a 5b6d  ld/, dist/....[m
-000006c0: 7970 795d 0d0a 6469 7361 6c6c 6f77 5f61  ypy]..disallow_a
-000006d0: 6e79 5f64 6563 6f72 6174 6564 203d 2074  ny_decorated = t
-000006e0: 7275 650d 0a64 6973 616c 6c6f 775f 616e  rue..disallow_an
-000006f0: 795f 6765 6e65 7269 6373 203d 2074 7275  y_generics = tru
-00000700: 650d 0a64 6973 616c 6c6f 775f 616e 795f  e..disallow_any_
-00000710: 756e 696d 706f 7274 6564 203d 2066 616c  unimported = fal
-00000720: 7365 0d0a 6469 7361 6c6c 6f77 5f73 7562  se..disallow_sub
-00000730: 636c 6173 7369 6e67 5f61 6e79 203d 2066  classing_any = f
-00000740: 616c 7365 0d0a 6469 7361 6c6c 6f77 5f75  alse..disallow_u
-00000750: 6e74 7970 6564 5f63 616c 6c73 203d 2074  ntyped_calls = t
-00000760: 7275 650d 0a64 6973 616c 6c6f 775f 756e  rue..disallow_un
-00000770: 7479 7065 645f 6465 6673 203d 2074 7275  typed_defs = tru
-00000780: 650d 0a69 676e 6f72 655f 6d69 7373 696e  e..ignore_missin
-00000790: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
-000007a0: 0d0a 7761 726e 5f75 6e75 7365 645f 6967  ..warn_unused_ig
-000007b0: 6e6f 7265 7320 3d20 7472 7565 0d0a 7761  nores = true..wa
-000007c0: 726e 5f72 6574 7572 6e5f 616e 7920 3d20  rn_return_any = 
-000007d0: 7472 7565 0d0a 0d0a 5b65 6767 5f69 6e66  true....[egg_inf
-000007e0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000007f0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000800: 0d0a                                     ..
+00000280: 7375 6573 0d0a 0944 6f63 756d 656e 7461  sues...Documenta
+00000290: 7469 6f6e 203d 2068 7474 7073 3a2f 2f76  tion = https://v
+000002a0: 6973 696f 6e36 642e 7265 6164 7468 6564  ision6d.readthed
+000002b0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000002c0: 2f0d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  /....[options]..
+000002d0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000002e0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+000002f0: 655f 6461 7461 203d 2074 7275 650d 0a70  e_data = true..p
+00000300: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000310: 203e 3d20 332e 360d 0a74 6573 745f 7375   >= 3.6..test_su
+00000320: 6974 6520 3d20 7465 7374 730d 0a73 6574  ite = tests..set
+00000330: 7570 5f72 6571 7569 7265 7320 3d20 0d0a  up_requires = ..
+00000340: 0973 6574 7570 746f 6f6c 730d 0a69 6e73  .setuptools..ins
+00000350: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000360: 0d0a 0970 7976 6973 7461 3e3d 302e 3339  ...pyvista>=0.39
+00000370: 2e31 0d0a 096e 756d 7079 3e3d 312e 3233  .1...numpy>=1.23
+00000380: 2e35 0d0a 096d 6174 706c 6f74 6c69 623e  .5...matplotlib>
+00000390: 3d33 2e35 2e32 0d0a 0974 7269 6d65 7368  =3.5.2...trimesh
+000003a0: 3e3d 332e 3134 2e30 0d0a 0965 6173 7964  >=3.14.0...easyd
+000003b0: 6963 743e 3d31 2e39 0d0a 0970 696c 6c6f  ict>=1.9...pillo
+000003c0: 773e 3d39 2e32 2e30 0d0a 0973 6369 7079  w>=9.2.0...scipy
+000003d0: 3e3d 312e 382e 310d 0a09 7079 7465 7374  >=1.8.1...pytest
+000003e0: 3e3d 372e 322e 300d 0a09 7079 7465 7374  >=7.2.0...pytest
+000003f0: 2d6c 617a 792d 6669 7874 7572 653e 3d30  -lazy-fixture>=0
+00000400: 2e36 2e33 0d0a 0970 7265 2d63 6f6d 6d69  .6.3...pre-commi
+00000410: 743e 3d32 2e32 312e 300d 0a09 6f70 656e  t>=2.21.0...open
+00000420: 6376 2d70 7974 686f 6e2d 6865 6164 6c65  cv-python-headle
+00000430: 7373 3e3d 342e 372e 302e 3638 0d0a 0973  ss>=4.7.0.68...s
+00000440: 6369 6b69 742d 696d 6167 653e 3d30 2e31  cikit-image>=0.1
+00000450: 392e 330d 0a09 6368 6172 6465 743e 3d35  9.3...chardet>=5
+00000460: 2e31 2e30 0d0a 0970 7967 656f 6465 7369  .1.0...pygeodesi
+00000470: 633e 3d30 2e31 2e38 0d0a 0950 7951 7435  c>=0.1.8...PyQt5
+00000480: 3e3d 352e 3135 2e39 0d0a 0970 7976 6973  >=5.15.9...pyvis
+00000490: 7461 7174 3e3d 302e 3130 2e30 0d0a 0d0a  taqt>=0.10.0....
+000004a0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000004b0: 5f64 6174 615d 0d0a 2a20 3d20 2a2e 706e  _data]..* = *.pn
+000004c0: 672c 202a 2e6a 7067 2c20 2a2e 716d 6c0d  g, *.jpg, *.qml.
+000004d0: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
+000004e0: 0d0a 756e 6976 6572 7361 6c20 3d20 7472  ..universal = tr
+000004f0: 7565 0d0a 0d0a 5b73 6469 7374 5d0d 0a66  ue....[sdist]..f
+00000500: 6f72 6d61 7473 203d 207a 6970 2c20 677a  ormats = zip, gz
+00000510: 7461 720d 0a0d 0a5b 636f 7665 7261 6765  tar....[coverage
+00000520: 3a72 6570 6f72 745d 0d0a 7368 6f77 5f6d  :report]..show_m
+00000530: 6973 7369 6e67 203d 2074 7275 650d 0a65  issing = true..e
+00000540: 7863 6c75 6465 5f6c 696e 6573 203d 200d  xclude_lines = .
+00000550: 0a09 7072 6167 6d61 3a20 6e6f 2063 6f76  ..pragma: no cov
+00000560: 6572 0d0a 0969 6620 4661 6c73 650d 0a0d  er...if False...
+00000570: 0a5b 6772 6565 6e5d 0d0a 6669 6c65 2d70  .[green]..file-p
+00000580: 6174 7465 726e 203d 2074 6573 745f 2a2e  attern = test_*.
+00000590: 7079 0d0a 7665 7262 6f73 6520 3d20 320d  py..verbose = 2.
+000005a0: 0a6e 6f2d 736b 6970 2d72 6570 6f72 7420  .no-skip-report 
+000005b0: 3d20 7472 7565 0d0a 7175 6965 742d 7374  = true..quiet-st
+000005c0: 646f 7574 203d 2074 7275 650d 0a72 756e  dout = true..run
+000005d0: 2d63 6f76 6572 6167 6520 3d20 7472 7565  -coverage = true
+000005e0: 0d0a 0d0a 5b70 7964 6f63 7374 796c 655d  ....[pydocstyle]
+000005f0: 0d0a 6d61 7463 682d 6469 7220 3d20 283f  ..match-dir = (?
+00000600: 2174 6573 7473 2928 3f21 7265 736f 7572  !tests)(?!resour
+00000610: 6365 7329 283f 2164 6f63 7329 5b5e 5c2e  ces)(?!docs)[^\.
+00000620: 5d2e 2a0d 0a6d 6174 6368 203d 2028 3f21  ].*..match = (?!
+00000630: 7465 7374 2928 3f21 7365 7475 7029 5b5e  test)(?!setup)[^
+00000640: 5c2e 5f5d 2e2a 5c2e 7079 0d0a 696e 6865  \._].*\.py..inhe
+00000650: 7269 7420 3d20 6661 6c73 650d 0a69 676e  rit = false..ign
+00000660: 6f72 6520 3d20 4432 3030 2c20 4432 3033  ore = D200, D203
+00000670: 2c20 4432 3133 2c20 4434 3036 2c20 4434  , D213, D406, D4
+00000680: 3037 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  07....[flake8]..
+00000690: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
+000006a0: 3d20 3939 0d0a 646f 6374 6573 7473 203d  = 99..doctests =
+000006b0: 2054 7275 650d 0a65 7863 6c75 6465 203d   True..exclude =
+000006c0: 202e 6769 742c 202e 6567 6773 2c20 5f5f   .git, .eggs, __
+000006d0: 7079 6361 6368 655f 5f2c 2074 6573 7473  pycache__, tests
+000006e0: 2f2c 2064 6f63 732f 2c20 6275 696c 642f  /, docs/, build/
+000006f0: 2c20 6469 7374 2f0d 0a0d 0a5b 6d79 7079  , dist/....[mypy
+00000700: 5d0d 0a64 6973 616c 6c6f 775f 616e 795f  ]..disallow_any_
+00000710: 6465 636f 7261 7465 6420 3d20 7472 7565  decorated = true
+00000720: 0d0a 6469 7361 6c6c 6f77 5f61 6e79 5f67  ..disallow_any_g
+00000730: 656e 6572 6963 7320 3d20 7472 7565 0d0a  enerics = true..
+00000740: 6469 7361 6c6c 6f77 5f61 6e79 5f75 6e69  disallow_any_uni
+00000750: 6d70 6f72 7465 6420 3d20 6661 6c73 650d  mported = false.
+00000760: 0a64 6973 616c 6c6f 775f 7375 6263 6c61  .disallow_subcla
+00000770: 7373 696e 675f 616e 7920 3d20 6661 6c73  ssing_any = fals
+00000780: 650d 0a64 6973 616c 6c6f 775f 756e 7479  e..disallow_unty
+00000790: 7065 645f 6361 6c6c 7320 3d20 7472 7565  ped_calls = true
+000007a0: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
+000007b0: 6564 5f64 6566 7320 3d20 7472 7565 0d0a  ed_defs = true..
+000007c0: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
+000007d0: 6d70 6f72 7473 203d 2074 7275 650d 0a77  mports = true..w
+000007e0: 6172 6e5f 756e 7573 6564 5f69 676e 6f72  arn_unused_ignor
+000007f0: 6573 203d 2074 7275 650d 0a77 6172 6e5f  es = true..warn_
+00000800: 7265 7475 726e 5f61 6e79 203d 2074 7275  return_any = tru
+00000810: 650d 0a0d 0a5b 6567 675f 696e 666f 5d0d  e....[egg_info].
+00000820: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000830: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `vision6D-0.2.8/test/test_create_dataset.py` & `vision6D-0.2.9/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/test/test_projection.py` & `vision6D-0.2.9/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/vision6D/__init__.py` & `vision6D-0.2.9/vision6D/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     # },
 }
 
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
 from .mainwindow import MyMainWindow
-from . import utils
+from . import tools
 from . import widgets
 from . import components
 from . import containers
 
 all = [
     'MyMainWindow',
     'Interface',
-    'utils',
+    'tools',
     'widgets',
     'components',
     'containers'
 ]
```

### Comparing `vision6D-0.2.8/vision6D/components/camera_store.py` & `vision6D-0.2.9/vision6D/components/camera_store.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: camera_store.py
+@time: 2023-07-03 20:22
+@desc: create store for camera related base functions
+'''
+
 import math
 import pyvista as pv
 import numpy as np
 from . import Singleton
 
 # contains mesh objects
```

### Comparing `vision6D-0.2.8/vision6D/components/folder_store.py` & `vision6D-0.2.9/vision6D/components/folder_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: folder_store.py
+@time: 2023-07-03 20:23
+@desc: create store for folder related base functions
+'''
+
 import os
 import re
 import pathlib
 
 import numpy as np
 
 from . import Singleton
```

### Comparing `vision6D-0.2.8/vision6D/components/mask_store.py` & `vision6D-0.2.9/vision6D/components/mask_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,36 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: mask_store.py
+@time: 2023-07-03 20:24
+@desc: create store for mask related functions
+'''
+
 import pathlib
 
 import cv2
 import PIL.Image
 import numpy as np
 import pyvista as pv
 
 from . import Singleton
-from .. import utils
+from ..tools import utils
 
 # contains mesh objects
 
 class MaskStore(metaclass=Singleton):
     def __init__(self):
         self.reset()
-
-    def reset(self):
         self.mirror_x = False
         self.mirror_y = False
 
+    def reset(self):
         self.mask_path = None
         self.mask_actor = None
         self.mask_opacity = 0.3
     
     def add_mask(self, mask_source):
         if isinstance(mask_source, pathlib.WindowsPath) or isinstance(mask_source, str):
             self.mask_path = str(mask_source)
```

### Comparing `vision6D-0.2.8/vision6D/components/mesh_store.py` & `vision6D-0.2.9/vision6D/components/mesh_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: mesh_store.py
+@time: 2023-07-03 20:24
+@desc: create store for mesh related base functions
+'''
+
 import pathlib
 
 import trimesh
 import pyvista as pv
 import numpy as np
 
 from . import Singleton
-from .. import utils
+from ..tools import utils
 
 # contains mesh objects
 
 class MeshStore(metaclass=Singleton):
     def __init__(self, window_size):
         self.reset()
         self.render = utils.create_render(window_size[0], window_size[1])
 
     def reset(self):
-        self.mirror_x = False
-        self.mirror_y = False
-
         self.reference = None
         self.mesh_path = None
         self.mesh_name = None
+        self.mirror_x = False
+        self.mirror_y = False
         self.mesh_actors = {}
         self.meshdict = {}
         self.latlon = utils.load_latitude_longitude()
         
         self.colors = ["cyan", "magenta", "yellow", "lime", "dodgerblue", "darkviolet", "darkorange", "darkgrey"]
         self.used_colors = []
         self.mesh_colors = {}
```

### Comparing `vision6D-0.2.8/vision6D/components/video_store.py` & `vision6D-0.2.9/vision6D/components/video_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: video_store.py
+@time: 2023-07-03 20:25
+@desc: create store for video related functions
+'''
+
 import cv2
 import numpy as np
 
 from . import Singleton
 from ..widgets import VideoPlayer
 from ..widgets import VideoSampler
```

### Comparing `vision6D-0.2.8/vision6D/containers/camera_container.py` & `vision6D-0.2.9/vision6D/containers/camera_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: camera_container.py
+@time: 2023-07-03 20:25
+@desc: create container for camera related actions in application
+'''
+
 import ast
 
 import numpy as np
 import PIL.Image
 
 from PyQt5 import QtWidgets
```

### Comparing `vision6D-0.2.8/vision6D/containers/image_container.py` & `vision6D-0.2.9/vision6D/containers/image_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: image_container.py
+@time: 2023-07-03 20:26
+@desc: create container for image related actions in application
+'''
 
 import pathlib
 import PIL.Image
 from PyQt5 import QtWidgets
 
-from .. import utils
+from ..tools import utils
 from ..components import CameraStore
 from ..components import ImageStore
 
 class ImageContainer:
     def __init__(self, 
                 plotter,
                 hintLabel,
```

### Comparing `vision6D-0.2.8/vision6D/containers/mask_container.py` & `vision6D-0.2.9/vision6D/containers/mask_container.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: mask_container.py
+@time: 2023-07-03 20:26
+@desc: create container for mask related actions in application
+'''
+
 import pathlib
 
 import numpy as np
 import pyvista as pv
 import PIL.Image
 
 from PyQt5 import QtWidgets
 
-from .. import utils
+from ..tools import utils
 from ..components import CameraStore
 from ..components import ImageStore
 from ..components import MaskStore
 from ..widgets import LabelWindow
 
 class MaskContainer:
     def __init__(self,
```

### Comparing `vision6D-0.2.8/vision6D/containers/mesh_container.py` & `vision6D-0.2.9/vision6D/containers/mesh_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,29 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: mesh_container.py
+@time: 2023-07-03 20:27
+@desc: create container for mesh related actions in application
+'''
+
 import ast
 import copy
 import pathlib
 
 import trimesh
 import PIL.Image
 import numpy as np
 import pyvista as pv
 
 from PyQt5 import QtWidgets
 
-from .. import utils
+from ..tools import utils
 from ..components import CameraStore
 from ..components import MaskStore
 from ..components import MeshStore
 from ..widgets import GetTextDialog
 
 class MeshContainer:
     def __init__(self, 
@@ -53,18 +63,15 @@
         self.mesh_store = MeshStore()
 
     def add_mesh_file(self, mesh_path='', prompt=False):
         if prompt: 
             mesh_path, _ = QtWidgets.QFileDialog().getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)") 
         if mesh_path:
             self.hintLabel.hide()
-            transformation_matrix = self.mesh_store.transformation_matrix
-            if self.mesh_store.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
-            if self.mesh_store.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix                   
-            self.add_mesh(mesh_path, transformation_matrix)
+            self.add_mesh(mesh_path)
 
     def mirror_mesh(self, direction):
         if direction == 'x': self.mesh_store.mirror_x = not self.mesh_store.mirror_x
         elif direction == 'y': self.mesh_store.mirror_y = not self.mesh_store.mirror_y
         transformation_matrix = self.mesh_store.initial_pose
         if self.mesh_store.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
         if self.mesh_store.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
@@ -90,15 +97,16 @@
             self.mesh_store.mesh_actors[self.mesh_store.mesh_name] = actor
             self.color_button.setText(self.mesh_store.mesh_colors[self.mesh_store.mesh_name])
 
             # add remove current mesh to removeMenu
             if self.mesh_store.mesh_name not in self.track_actors_names:
                 self.track_actors_names.append(self.mesh_store.mesh_name)
                 self.add_button_actor_name(self.mesh_store.mesh_name)
-            self.check_button(actor_name=self.mesh_store.mesh_name, output_text=False) #* very important for mirroring
+            #* very important for mirroring
+            self.check_button(actor_name=self.mesh_store.mesh_name, output_text=False) 
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "The mesh format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
     
     def set_spacing(self):
         checked_button = self.button_group_actors_names.checkedButton()
         if checked_button:
             actor_name = checked_button.text()
```

### Comparing `vision6D-0.2.8/vision6D/containers/pnp_container.py` & `vision6D-0.2.9/vision6D/containers/pnp_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: pnp_container.py
+@time: 2023-07-03 20:27
+@desc: create container for PnP related algorithms in application
+'''
+
+import math
 
 import trimesh
 import numpy as np
-import math
+import matplotlib.pyplot as plt
 
 from PyQt5 import QtWidgets
 
-from .. import utils
+from ..tools import utils
 from ..components import CameraStore
 from ..components import MaskStore
 from ..components import MeshStore
 
 class PnPContainer:
     def __init__(self, plotter, export_mesh_render, output_text):
         self.plotter = plotter
```

### Comparing `vision6D-0.2.8/vision6D/containers/video_folder_container.py` & `vision6D-0.2.9/vision6D/containers/video_folder_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: video_folder_container.py
+@time: 2023-07-03 20:28
+@desc: create container for video/folder related actions in application
+'''
+
 import os
 import pathlib
 
 import numpy as np
 import PIL.Image
 
 from PyQt5 import QtWidgets
```

### Comparing `vision6D-0.2.8/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.9/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/vision6D/data/style.qss` & `vision6D-0.2.9/vision6D/data/style.qss`

 * *Files 1% similar despite different names*

```diff
@@ -160,19 +160,14 @@
      border-left-width: 0px;
      border-left-color: darkgray;
      border-left-style: solid; /* just a single line */
      border-top-right-radius: 3px; /* same radius as the QComboBox */
      border-bottom-right-radius: 3px;
  }
 
-QComboBox::down-arrow
-{
-     image: url(:/dark_orange/img/down_arrow.png);
-}
-
 QGroupBox
 {
     border: 1px solid darkgray;
     margin-top: 10px;
 }
 
 QGroupBox:focus
@@ -344,15 +339,14 @@
     border: 1px solid #6c6c6c;
     spacing: 3px; /* spacing between items in the tool bar */
 }
 
 QToolBar::handle
 {
      spacing: 3px; /* spacing between items in the tool bar */
-     background: url(:/dark_orange/img/handle.png);
 }
 
 QMenu::separator
 {
     height: 2px;
     background-color: QLinearGradient(x1:0, y1:0, x2:0, y2:1, stop:0 #161616, stop: 0.5 #151515, stop: 0.6 #212121, stop:1 #343434);
     color: white;
@@ -462,25 +456,19 @@
 }
 
 QRadioButton::indicator:hover, QCheckBox::indicator:hover
 {
     border: 1px solid #ffaa00;
 }
 
-QCheckBox::indicator:checked
-{
-    image:url(:/dark_orange/img/checkbox.png);
-}
-
 QCheckBox::indicator:disabled, QRadioButton::indicator:disabled
 {
     border: 1px solid #444;
 }
 
-
 QSlider::groove:horizontal {
     border: 1px solid #3A3939;
     height: 8px;
     background: #201F1F;
     margin: 2px 0;
     border-radius: 2px;
 }
```

### Comparing `vision6D-0.2.8/vision6D/mainwindow.py` & `vision6D-0.2.9/vision6D/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: mainwindow.py
+@time: 2023-07-03 20:33
+@desc: the mainwindow to run application
+'''
+
 # General import
 import os
 os.environ["QT_API"] = "pyqt5" # Setting the Qt bindings for QtPy
 import json
 import copy
 import functools
 
@@ -155,14 +165,18 @@
                                                         output_text=self.output_text)
 
     def key_bindings(self):
         # Camera related key bindings
         QtWidgets.QShortcut(QtGui.QKeySequence("c"), self).activated.connect(self.camera_container.reset_camera)
         QtWidgets.QShortcut(QtGui.QKeySequence("z"), self).activated.connect(self.camera_container.zoom_out)
         QtWidgets.QShortcut(QtGui.QKeySequence("x"), self).activated.connect(self.camera_container.zoom_in)
+
+        # Mirror related key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("o"), self).activated.connect(lambda direction='x': self.mirror_actors(direction))
+        QtWidgets.QShortcut(QtGui.QKeySequence("p"), self).activated.connect(lambda direction='y': self.mirror_actors(direction))
         
         # Image related key bindings
         QtWidgets.QShortcut(QtGui.QKeySequence("b"), self).activated.connect(lambda up=True: self.image_container.toggle_image_opacity(up))
         QtWidgets.QShortcut(QtGui.QKeySequence("n"), self).activated.connect(lambda up=False: self.image_container.toggle_image_opacity(up))
 
         # Mask related key bindings
         QtWidgets.QShortcut(QtGui.QKeySequence("t"), self).activated.connect(self.mask_container.reset_mask)
@@ -255,19 +269,14 @@
 
         # Add camera related actions
         CameraMenu = mainMenu.addMenu('Camera')
         CameraMenu.addAction('Calibrate', self.camera_container.camera_calibrate)
         CameraMenu.addAction('Reset Camera (d)', self.camera_container.reset_camera)
         CameraMenu.addAction('Zoom In (x)', self.camera_container.zoom_in)
         CameraMenu.addAction('Zoom Out (z)', self.camera_container.zoom_out)
-
-        # add mirror actors related actions
-        mirrorMenu = mainMenu.addMenu('Mirror')
-        mirrorMenu.addAction('Mirror X axis', functools.partial(self.mirror_actors, direction='x'))
-        mirrorMenu.addAction('Mirror Y axis', functools.partial(self.mirror_actors, direction='y'))
         
         # Add register related actions
         RegisterMenu = mainMenu.addMenu('Register')
         RegisterMenu.addAction('Reset GT Pose (k)', self.mesh_container.reset_gt_pose)
         RegisterMenu.addAction('Reset Mask (t)', self.mask_container.reset_mask)
         RegisterMenu.addAction('Update GT Pose (l)', self.mesh_container.update_gt_pose)
         RegisterMenu.addAction('Undo Pose (s)', self.mesh_container.undo_pose)
@@ -388,14 +397,24 @@
         display_layout.addLayout(actor_grid_layout)
 
         # Create the spacing button
         self.spacing_button = QtWidgets.QPushButton("Spacing")
         self.spacing_button.clicked.connect(self.mesh_container.set_spacing)
         actor_grid_layout.addWidget(self.spacing_button, 1, 0)
 
+        # Create the mirror x button
+        self.mirror_x_button = QtWidgets.QPushButton("Mirror X")
+        self.mirror_x_button.clicked.connect(lambda _, direction="x": self.mirror_actors(direction))
+        actor_grid_layout.addWidget(self.mirror_x_button, 1, 1)
+
+        # Create the mirror y button
+        self.mirror_y_button = QtWidgets.QPushButton("Mirror Y")
+        self.mirror_y_button.clicked.connect(lambda _, direction="y": self.mirror_actors(direction))
+        actor_grid_layout.addWidget(self.mirror_y_button, 1, 2)
+
         # Create a scroll area for the buttons
         scroll_area = QtWidgets.QScrollArea()
         scroll_area.setWidgetResizable(True)
         display_layout.addWidget(scroll_area)
 
         # Create a container widget for the buttons
         button_container = QtWidgets.QWidget()
@@ -589,18 +608,26 @@
                 self.play_video_button.setText(f"Frame ({self.folder_store.current_frame}/{self.folder_store.total_frame})")
                 self.camera_container.reset_camera()
             else:
                 self.folder_store.reset()
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "Not a valid folder, please reload a folder", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def mirror_actors(self, direction):
-        if self.image_store.image_path: self.image_container.mirror_image(direction)
-        if self.mask_store.mask_path: self.mask_container.mirror_mask(direction)
-        if self.mesh_store.reference: self.mesh_container.mirror_mesh(direction)
-   
+        checked_button = self.button_group_actors_names.checkedButton()
+        if checked_button:
+            actor_name = checked_button.text()
+            if actor_name == 'image':
+                self.image_container.mirror_image(direction)
+            elif actor_name == 'mask':
+                self.mask_container.mirror_mask(direction)
+            elif actor_name in self.mesh_store.mesh_actors:
+                self.mesh_container.mirror_mesh(direction)
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+
     def remove_actor(self, button):
         name = button.text()
         if name == 'image': 
             actor = self.image_store.image_actor
             self.image_store.reset()
         elif name == 'mask':
             actor = self.mask_store.mask_actor
@@ -631,26 +658,36 @@
 
     def clear_plot(self):
         # Clear out everything in the remove menu
         for button in self.button_group_actors_names.buttons():
             name = button.text()
             if name == 'image': actor = self.image_store.image_actor
             elif name == 'mask': actor = self.mask_store.mask_actor
-            elif name in self.mesh_store.mesh_actors: actor = self.mesh_store.mesh_actors[name]
+            elif name in self.mesh_store.mesh_actors: 
+                actor = self.mesh_store.mesh_actors[name]
+                self.mesh_store.remove_mesh(name)
+                self.color_button.setText("Color")
             self.plotter.remove_actor(actor)
             # remove the button from the button group
             self.button_group_actors_names.removeButton(button)
             # remove the button from the self.button_layout widget
             self.button_layout.removeWidget(button)
             # offically delete the button
             button.deleteLater()
 
         self.image_store.reset()
+        self.image_store.mirror_x = False
+        self.image_store.mirror_y = False
+
         self.mask_store.reset()
+        self.mask_store.mirror_x = False
+        self.mask_store.mirror_y = False
+
         self.mesh_store.reset()
+
         self.video_store.reset()
         self.folder_store.reset()
 
         # Re-initial the dictionaries
         self.workspace_path = ''
         self.track_actors_names.clear()
```

### Comparing `vision6D-0.2.8/vision6D/utils.py` & `vision6D-0.2.9/vision6D/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: utils.py
+@time: 2023-07-03 20:34
+@desc: the util functions for whole application
+'''
+
 import __future__
 import copy
 import logging
 
 import numpy as np
 import pathlib
-import os
+
 import pyvista as pv
 import matplotlib.pyplot as plt
 from easydict import EasyDict
 import trimesh
 from PIL import Image
 import cv2
 # import pygeodesic.geodesic as geodesic
 import vtk.util.numpy_support as vtknp
 import json
-
-CWD = pathlib.Path(os.path.abspath(__file__)).parent
 logger = logging.getLogger("vision6D")
 
 def fread(fid, _len, _type):
     if _len == 0:
         return np.empty(0)
     if _type == "int16":
         _type = np.int16
@@ -276,15 +284,16 @@
 
     rt = np.vstack((np.hstack((R, t)), np.array([0,0,0,1])))
 
     return rt
 
 def load_latitude_longitude():
     # get the latitude and longitude
-    with open(CWD / "data" / "ossiclesCoordinateMapping.json", "r") as f: data = json.load(f)
+    latlon_path = pathlib.Path.cwd() / "vision6D" / "data" / "ossiclesCoordinateMapping.json" # latlon_map_path = pkg_resources.resource_filename('vision6D', 'data/ossiclesCoordinateMapping.json')
+    with open(latlon_path, "r") as f: data = json.load(f)
     
     latitude = np.array(data['latitude']).reshape((len(data['latitude'])), 1)
     longitude = np.array(data['longitude']).reshape((len(data['longitude'])), 1)
     placeholder = np.zeros((len(data['longitude']), 1))
     
     # set the latlon attribute
     latlon = np.hstack((latitude, longitude, placeholder))
```

### Comparing `vision6D-0.2.8/vision6D/widgets/__init__.py` & `vision6D-0.2.9/vision6D/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.8/vision6D/widgets/calibration_pop_window.py` & `vision6D-0.2.9/vision6D/widgets/calibration_pop_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: calibration_pop_window.py
+@time: 2023-07-03 20:29
+@desc: pop window for camera calibration
+'''
+
 # General import
 import numpy as np
 from skimage.metrics import peak_signal_noise_ratio, structural_similarity
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui
 from PyQt5.QtCore import Qt
```

### Comparing `vision6D-0.2.8/vision6D/widgets/camera_props_input_dialog.py` & `vision6D-0.2.9/vision6D/widgets/camera_props_input_dialog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: camera_props_input_dialog.py
+@time: 2023-07-03 20:30
+@desc: pop window for camera props input dialog
+'''
+
 # General import
 import numpy as np
 
 # Qt5 import
 from PyQt5 import QtWidgets
 
 # self defined package import
```

### Comparing `vision6D-0.2.8/vision6D/widgets/get_text_dialog.py` & `vision6D-0.2.9/vision6D/widgets/get_text_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: get_text_dialog.py
+@time: 2023-07-03 20:31
+@desc: get the text dialog for user input
+'''
+
 # General import
 import numpy as np
 
 # Qt5 import
 from PyQt5 import QtWidgets
 
 # self defined package import
```

### Comparing `vision6D-0.2.8/vision6D/widgets/label_window.py` & `vision6D-0.2.9/vision6D/widgets/label_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: label_window.py
+@time: 2023-07-03 20:32
+@desc: create the window for mask labeling/drawing
+'''
+
 # General import
 import numpy as np
 import cv2
 import pathlib
 import PIL.Image
 
 # Qt5 import
```

### Comparing `vision6D-0.2.8/vision6D/widgets/popup_dialog.py` & `vision6D-0.2.9/vision6D/widgets/popup_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: popup_dialog.py
+@time: 2023-07-03 20:32
+@desc: create the dialog for popup window
+'''
+
 # General import
 import numpy as np
 
 # Qt5 import
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import Qt
```

### Comparing `vision6D-0.2.8/vision6D/widgets/video_player.py` & `vision6D-0.2.9/vision6D/widgets/video_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: video_player.py
+@time: 2023-07-03 20:33
+@desc: create the video player
+'''
+
 # General import
 import numpy as np
 import cv2
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui, QtCore
 from PyQt5.QtCore import Qt
```

### Comparing `vision6D-0.2.8/vision6D/widgets/video_sampler.py` & `vision6D-0.2.9/vision6D/widgets/video_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+'''
+@author: Yike (Nicole) Zhang
+@license: (C) Copyright.
+@contact: yike.zhang@vanderbilt.edu
+@software: Vision6D
+@file: video_sampler.py
+@time: 2023-07-03 20:33
+@desc: create the video sampler
+'''
+
 # General import
 import numpy as np
 import cv2
 import pathlib
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui
```

### Comparing `vision6D-0.2.8/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.9/vision6D.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.8
+Version: 0.2.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
-Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
+Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vision6D-0.2.8/vision6D.egg-info/SOURCES.txt` & `vision6D-0.2.9/vision6D.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 test/test_create_dataset.py
 test/test_projection.py
 vision6D/__init__.py
 vision6D/mainwindow.py
-vision6D/utils.py
 vision6D.egg-info/PKG-INFO
 vision6D.egg-info/SOURCES.txt
 vision6D.egg-info/dependency_links.txt
 vision6D.egg-info/entry_points.txt
 vision6D.egg-info/requires.txt
 vision6D.egg-info/top_level.txt
 vision6D/components/__init__.py
@@ -30,14 +29,16 @@
 vision6D/containers/mesh_container.py
 vision6D/containers/pnp_container.py
 vision6D/containers/video_folder_container.py
 vision6D/data/ossiclesCoordinateMapping.json
 vision6D/data/style.qss
 vision6D/entry/__init__.py
 vision6D/entry/main.py
+vision6D/tools/__init__.py
+vision6D/tools/utils.py
 vision6D/widgets/__init__.py
 vision6D/widgets/calibration_pop_window.py
 vision6D/widgets/camera_props_input_dialog.py
 vision6D/widgets/custom_qt_interactor.py
 vision6D/widgets/get_text_dialog.py
 vision6D/widgets/label_window.py
 vision6D/widgets/popup_dialog.py
```

