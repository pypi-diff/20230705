# Comparing `tmp/micrOSDevToolKit-1.17.1.tar.gz` & `tmp/micrOSDevToolKit-1.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.17.1.tar", last modified: Wed Jul  5 11:34:12 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.17.2.tar", last modified: Wed Jul  5 11:43:23 2023, max compression
```

## Comparing `micrOSDevToolKit-1.17.1.tar` & `micrOSDevToolKit-1.17.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.114241 micrOSDevToolKit-1.17.1/
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 11:34:12.113512 micrOSDevToolKit-1.17.1/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.17.1/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.17.1/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.070289 micrOSDevToolKit-1.17.1/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.1/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.070836 micrOSDevToolKit-1.17.1/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.1/media/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.071226 micrOSDevToolKit-1.17.1/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.1/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.071623 micrOSDevToolKit-1.17.1/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.1/micrOS/micropython/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.074575 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 11:34:11.000000 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     1372 2023-07-05 11:34:11.000000 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 11:34:11.000000 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 11:34:11.000000 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 11:34:11.000000 micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 11:34:12.114426 micrOSDevToolKit-1.17.1/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 11:33:33.000000 micrOSDevToolKit-1.17.1/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.082831 micrOSDevToolKit-1.17.1/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.17.1/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.17.1/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31256 2023-06-14 11:56:34.000000 micrOSDevToolKit-1.17.1/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.17.1/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.096657 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.109250 micrOSDevToolKit-1.17.1/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.17.1/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.17.1/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.17.1/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.17.1/toolkit/micrOSdashboard.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.17.1/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:34:12.112047 micrOSDevToolKit-1.17.1/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.1/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.499323 micrOSDevToolKit-1.17.2/
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 11:43:23.498781 micrOSDevToolKit-1.17.2/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.17.2/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.17.2/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.442954 micrOSDevToolKit-1.17.2/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.2/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.443377 micrOSDevToolKit-1.17.2/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.2/media/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.443815 micrOSDevToolKit-1.17.2/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.2/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.444254 micrOSDevToolKit-1.17.2/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.2/micrOS/micropython/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.447119 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 11:43:23.000000 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     1372 2023-07-05 11:43:23.000000 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 11:43:23.000000 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 11:43:23.000000 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 11:43:23.000000 micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 11:43:23.499491 micrOSDevToolKit-1.17.2/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 11:42:39.000000 micrOSDevToolKit-1.17.2/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.461516 micrOSDevToolKit-1.17.2/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.17.2/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.17.2/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31256 2023-06-14 11:56:34.000000 micrOSDevToolKit-1.17.2/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.17.2/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.490256 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.495833 micrOSDevToolKit-1.17.2/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.17.2/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.17.2/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.17.2/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.17.2/toolkit/micrOSdashboard.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.17.2/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 11:43:23.497257 micrOSDevToolKit-1.17.2/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.2/toolkit/workspace/__init__.py
```

### Comparing `micrOSDevToolKit-1.17.1/PKG-INFO` & `micrOSDevToolKit-1.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.1
+Version: 1.17.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.1/README.md` & `micrOSDevToolKit-1.17.2/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/devToolKit.py` & `micrOSDevToolKit-1.17.2/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.1
+Version: 1.17.2
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.1/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.17.2/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/setup.py` & `micrOSDevToolKit-1.17.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.17.1',
+    version='1.17.2',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.17.1/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.17.2/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.17.2/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.17.2/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/Gateway.py` & `micrOSDevToolKit-1.17.2/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.17.2/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.17.2/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.17.2/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.17.2/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.17.2/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.17.2/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.17.2/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.17.2/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.1/toolkit/socketClient.py` & `micrOSDevToolKit-1.17.2/toolkit/socketClient.py`

 * *Files identical despite different names*

