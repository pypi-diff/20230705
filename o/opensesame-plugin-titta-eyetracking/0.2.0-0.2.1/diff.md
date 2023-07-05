# Comparing `tmp/opensesame-plugin-titta_eyetracking-0.2.0.tar.gz` & `tmp/opensesame-plugin-titta_eyetracking-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame-plugin-titta_eyetracking-0.2.0.tar", last modified: Tue Jul  4 21:26:11 2023, max compression
+gzip compressed data, was "opensesame-plugin-titta_eyetracking-0.2.1.tar", last modified: Tue Jul  4 21:33:34 2023, max compression
```

## Comparing `opensesame-plugin-titta_eyetracking-0.2.0.tar` & `opensesame-plugin-titta_eyetracking-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.254871 opensesame-plugin-titta_eyetracking-0.2.0/
--rw-r--r--   0 bob       (1000) bob       (1000)     3078 2023-07-04 21:15:23.000000 opensesame-plugin-titta_eyetracking-0.2.0/.gitignore
--rwxrwxr--   0 bob       (1000) bob       (1000)    14184 2023-06-02 07:45:26.000000 opensesame-plugin-titta_eyetracking-0.2.0/LICENSE.md
--rw-r--r--   0 bob       (1000) bob       (1000)      106 2022-10-27 05:29:28.000000 opensesame-plugin-titta_eyetracking-0.2.0/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-04 21:26:11.254871 opensesame-plugin-titta_eyetracking-0.2.0/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     1576 2023-07-04 13:28:27.000000 opensesame-plugin-titta_eyetracking-0.2.0/README.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.251871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-04 21:26:11.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     1714 2023-07-04 21:26:11.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-04 21:26:11.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-04 21:26:11.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/top_level.txt
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.249871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.251871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/
--rw-r--r--   0 bob       (1000) bob       (1000)      256 2023-07-04 13:42:52.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate.md
--rw-r--r--   0 bob       (1000) bob       (1000)      809 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1561 2023-07-04 12:53:05.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1330 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.252871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/
--rw-r--r--   0 bob       (1000) bob       (1000)     1953 2023-07-04 13:42:33.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1450 2023-06-29 21:35:34.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init.png
--rw-r--r--   0 bob       (1000) bob       (1000)     2276 2023-07-04 12:52:34.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2156 2023-06-29 21:34:54.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.253871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/
--rw-r--r--   0 bob       (1000) bob       (1000)      381 2023-07-04 13:42:16.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message.md
--rw-r--r--   0 bob       (1000) bob       (1000)      805 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1092 2023-06-28 21:33:32.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1305 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.253871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/
--rw-r--r--   0 bob       (1000) bob       (1000)      269 2023-07-04 13:42:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording.md
--rw-r--r--   0 bob       (1000) bob       (1000)      807 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1324 2023-06-28 21:33:38.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1300 2023-06-29 21:34:53.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:26:11.254871 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/
--rw-r--r--   0 bob       (1000) bob       (1000)      267 2023-07-04 13:42:01.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.md
--rw-r--r--   0 bob       (1000) bob       (1000)      802 2023-06-29 21:35:34.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1387 2023-06-29 12:16:56.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1292 2023-06-29 21:34:53.000000 opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)       38 2023-07-04 21:26:11.254871 opensesame-plugin-titta_eyetracking-0.2.0/setup.cfg
--rw-r--r--   0 bob       (1000) bob       (1000)     4097 2023-07-04 13:35:41.000000 opensesame-plugin-titta_eyetracking-0.2.0/setup.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.382387 opensesame-plugin-titta_eyetracking-0.2.1/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3078 2023-07-04 21:15:23.000000 opensesame-plugin-titta_eyetracking-0.2.1/.gitignore
+-rwxrwxr--   0 bob       (1000) bob       (1000)    14184 2023-06-02 07:45:26.000000 opensesame-plugin-titta_eyetracking-0.2.1/LICENSE.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      106 2022-10-27 05:29:28.000000 opensesame-plugin-titta_eyetracking-0.2.1/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-04 21:33:34.382387 opensesame-plugin-titta_eyetracking-0.2.1/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1576 2023-07-04 13:28:27.000000 opensesame-plugin-titta_eyetracking-0.2.1/README.md
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.379387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-04 21:33:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1734 2023-07-04 21:33:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-04 21:33:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-04 21:33:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/top_level.txt
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.377387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.379387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/
+-rw-r--r--   0 bob       (1000) bob       (1000)      256 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      809 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1561 2023-07-04 12:53:05.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1330 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.380387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1953 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1450 2023-06-29 21:35:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2276 2023-07-04 12:52:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2156 2023-06-29 21:34:54.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.380387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/
+-rw-r--r--   0 bob       (1000) bob       (1000)      381 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      805 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1092 2023-06-28 21:33:32.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1305 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.381387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/
+-rw-r--r--   0 bob       (1000) bob       (1000)      269 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      807 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1324 2023-06-28 21:33:38.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1300 2023-06-29 21:34:53.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-04 21:33:34.382387 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/
+-rw-r--r--   0 bob       (1000) bob       (1000)      267 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      802 2023-06-29 21:35:34.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1387 2023-06-29 12:16:56.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1292 2023-06-29 21:34:53.000000 opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-07-04 21:33:34.382387 opensesame-plugin-titta_eyetracking-0.2.1/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)     4097 2023-07-04 21:32:35.000000 opensesame-plugin-titta_eyetracking-0.2.1/setup.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      232 2023-07-04 21:24:56.000000 opensesame-plugin-titta_eyetracking-0.2.1/stdeb.cfg
```

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/.gitignore` & `opensesame-plugin-titta_eyetracking-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/LICENSE.md` & `opensesame-plugin-titta_eyetracking-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/PKG-INFO` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: opensesame-plugin-titta_eyetracking
-Version: 0.2.0
+Name: opensesame-plugin-titta-eyetracking
+Version: 0.2.1
 Summary: Titta Eye Tracking plugin for OpenSesame
 Home-page: https://github.com/dev-jam/opensesame-plugin-titta_eyetracking
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/README.md` & `opensesame-plugin-titta_eyetracking-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO` & `opensesame-plugin-titta_eyetracking-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: opensesame-plugin-titta-eyetracking
-Version: 0.2.0
+Name: opensesame-plugin-titta_eyetracking
+Version: 0.2.1
 Summary: Titta Eye Tracking plugin for OpenSesame
 Home-page: https://github.com/dev-jam/opensesame-plugin-titta_eyetracking
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE.md
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
+stdeb.cfg
 opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO
 opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt
 opensesame_plugin_titta_eyetracking.egg-info/dependency_links.txt
 opensesame_plugin_titta_eyetracking.egg-info/top_level.txt
 opensesame_plugins/titta_calibrate/info.yaml
 opensesame_plugins/titta_calibrate/titta_calibrate.md
 opensesame_plugins/titta_calibrate/titta_calibrate.png
```

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate.py` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate.py`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_calibrate/titta_calibrate_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/info.yaml` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/info.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Titta Eye Tracking Init.
-version: 0.2.0
+version: 0.2.1
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Titta Eye Tracking"
 date: "2023"
 controls:
 -
     type: "checkbox"
@@ -50,8 +50,8 @@
     label: "\n\n\nTitta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. \n\n\
     Cite as:\n\nNiehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8\n\n\
     Please mention: Bob Rosbag as creator of this plugin\n\n
     For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.\n\n\
     To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker."
 -
     type: "text"
-    label: "Version 0.2.0"
+    label: "Version 0.2.1"
```

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init.py` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init.py`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_init/titta_init_large.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_init/titta_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message.py` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message.py`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_send_message/titta_send_message_large.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_send_message/titta_send_message_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording.py` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording.py`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_start_recording/titta_start_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording.py`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png` & `opensesame-plugin-titta_eyetracking-0.2.1/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.2.0/setup.py` & `opensesame-plugin-titta_eyetracking-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         with open('README.md') as fd:
             return fd.read()
     return 'No readme information'
 
 
 setup(
     name='opensesame-plugin-titta_eyetracking',
-    version='0.2.0',
+    version='0.2.1',
     description='Titta Eye Tracking plugin for OpenSesame',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='Bob Rosbag',
     author_email='debian@bobrosbag.nl',
     url='https://github.com/dev-jam/opensesame-plugin-titta_eyetracking',
     # Classifiers used by PyPi if you upload the plugin there
```

