# Comparing `tmp/micrOSDevToolKit-1.17.5.tar.gz` & `tmp/micrOSDevToolKit-1.17.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.17.5.tar", last modified: Wed Jul  5 12:39:47 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.17.6.tar", last modified: Wed Jul  5 12:56:53 2023, max compression
```

## Comparing `micrOSDevToolKit-1.17.5.tar` & `micrOSDevToolKit-1.17.6.tar`

### file list

```diff
@@ -1,121 +1,191 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.751896 micrOSDevToolKit-1.17.5/
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 12:39:47.751370 micrOSDevToolKit-1.17.5/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.17.5/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.17.5/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.611029 micrOSDevToolKit-1.17.5/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.611392 micrOSDevToolKit-1.17.5/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.5/media/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.611844 micrOSDevToolKit-1.17.5/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.612370 micrOSDevToolKit-1.17.5/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/micrOS/micropython/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.682684 micrOSDevToolKit-1.17.5/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-03-15 14:20:02.000000 micrOSDevToolKit-1.17.5/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.17.5/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6361 2023-06-15 14:14:20.000000 micrOSDevToolKit-1.17.5/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2475 2023-03-12 13:18:33.000000 micrOSDevToolKit-1.17.5/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-06-28 17:39:05.000000 micrOSDevToolKit-1.17.5/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-04 18:36:50.000000 micrOSDevToolKit-1.17.5/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.17.5/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     2363 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.5/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.17.5/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.17.5/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.17.5/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-03-04 23:34:06.000000 micrOSDevToolKit-1.17.5/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-06-19 16:03:31.000000 micrOSDevToolKit-1.17.5/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-04 18:31:06.000000 micrOSDevToolKit-1.17.5/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.17.5/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:02.000000 micrOSDevToolKit-1.17.5/micrOS/source/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.5/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.17.5/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-03-12 13:21:42.000000 micrOSDevToolKit-1.17.5/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.17.5/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.17.5/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.686077 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 12:39:47.000000 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     3104 2023-07-05 12:39:47.000000 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 12:39:47.000000 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 12:39:47.000000 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 12:39:47.000000 micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 12:39:47.752218 micrOSDevToolKit-1.17.5/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 12:39:27.000000 micrOSDevToolKit-1.17.5/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.711407 micrOSDevToolKit-1.17.5/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.17.5/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.17.5/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31256 2023-06-14 11:56:34.000000 micrOSDevToolKit-1.17.5/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.17.5/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.740866 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.746880 micrOSDevToolKit-1.17.5/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.17.5/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.17.5/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.17.5/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.17.5/toolkit/micrOSdashboard.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.17.5/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:47.749913 micrOSDevToolKit-1.17.5/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.5/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.889765 micrOSDevToolKit-1.17.6/
+-rw-r--r--   0 bnm        (501) staff       (20)       66 2023-07-05 12:55:36.000000 micrOSDevToolKit-1.17.6/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 12:56:53.889064 micrOSDevToolKit-1.17.6/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.17.6/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.17.6/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.568745 micrOSDevToolKit-1.17.6/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.569188 micrOSDevToolKit-1.17.6/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.6/media/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.569611 micrOSDevToolKit-1.17.6/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.621782 micrOSDevToolKit-1.17.6/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.720609 micrOSDevToolKit-1.17.6/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-03-15 14:20:02.000000 micrOSDevToolKit-1.17.6/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.17.6/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6361 2023-06-15 14:14:20.000000 micrOSDevToolKit-1.17.6/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2475 2023-03-12 13:18:33.000000 micrOSDevToolKit-1.17.6/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-06-28 17:39:05.000000 micrOSDevToolKit-1.17.6/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-04 18:36:50.000000 micrOSDevToolKit-1.17.6/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.17.6/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2363 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.6/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.17.6/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.17.6/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.17.6/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-03-04 23:34:06.000000 micrOSDevToolKit-1.17.6/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-06-19 16:03:31.000000 micrOSDevToolKit-1.17.6/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-04 18:31:06.000000 micrOSDevToolKit-1.17.6/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.17.6/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-05 12:39:02.000000 micrOSDevToolKit-1.17.6/micrOS/source/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.6/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.17.6/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-03-12 13:21:42.000000 micrOSDevToolKit-1.17.6/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.17.6/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.17.6/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.724838 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 12:56:53.000000 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     5983 2023-07-05 12:56:53.000000 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 12:56:53.000000 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 12:56:53.000000 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 12:56:53.000000 micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 12:56:53.889935 micrOSDevToolKit-1.17.6/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 12:55:52.000000 micrOSDevToolKit-1.17.6/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.743641 micrOSDevToolKit-1.17.6/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.17.6/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.17.6/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31335 2023-07-05 12:50:59.000000 micrOSDevToolKit-1.17.6/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.17.6/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.807215 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.814509 micrOSDevToolKit-1.17.6/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.17.6/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.17.6/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.17.6/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.17.6/toolkit/micrOSdashboard.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.17.6/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.815793 micrOSDevToolKit-1.17.6/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 12:56:53.887266 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6361 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2475 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12706 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2363 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.6/toolkit/workspace/simulator/urequests.py
```

### Comparing `micrOSDevToolKit-1.17.5/PKG-INFO` & `micrOSDevToolKit-1.17.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.5
+Version: 1.17.6
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.5/README.md` & `micrOSDevToolKit-1.17.6/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/devToolKit.py` & `micrOSDevToolKit-1.17.6/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Common.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.17.6/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Debug.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.17.6/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.17.6/micrOS/source/InterpreterShell.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.17.6/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.17.6/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Network.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Notify.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.17.6/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.17.6/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/Time.py` & `micrOSDevToolKit-1.17.6/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.17.6/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.17.6/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.17.6/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOS/source/urequests.py` & `micrOSDevToolKit-1.17.6/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.17.6/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.5
+Version: 1.17.6
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.5/setup.py` & `micrOSDevToolKit-1.17.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.17.5',
+    version='1.17.6',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.17.5/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.17.6/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.17.6/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.17.6/toolkit/DevEnvUSB.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 
     def get_micropython_binaries(self):
         self.console("------------------------------------------")
         self.console("-         GET MICROPYTHON BINARIES       -", state='imp')
         self.console("------------------------------------------")
         micropython_bins_list = []
 
+        self.console(f"Micropython bin path: {self.micropython_bin_dir_path}")
         mp_bin_list = [binary for binary in LocalMachine.FileHandler.list_dir(self.micropython_bin_dir_path) if
                        binary.endswith('.bin') or binary.endswith('.uf2')]
         for mp_bin in mp_bin_list:
             micropython_bins_list.append(os.path.join(self.micropython_bin_dir_path, mp_bin))
         if len(micropython_bins_list) > 0:
             self.console("Micropython binary was found.", state='ok')
         else:
```

### Comparing `micrOSDevToolKit-1.17.5/toolkit/Gateway.py` & `micrOSDevToolKit-1.17.6/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.17.6/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.17.6/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.17.6/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.17.6/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.17.6/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.17.6/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.17.6/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.17.6/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.5/toolkit/socketClient.py` & `micrOSDevToolKit-1.17.6/toolkit/socketClient.py`

 * *Files identical despite different names*

