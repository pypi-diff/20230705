# Comparing `tmp/ns_asphalt9-0.0.7.tar.gz` & `tmp/ns_asphalt9-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns_asphalt9-0.0.7.tar", last modified: Mon Jul  3 16:01:06 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.0.8.tar", last modified: Wed Jul  5 10:04:44 2023, max compression
```

## Comparing `ns_asphalt9-0.0.7.tar` & `ns_asphalt9-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/
--rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.0.7/LICENSE
--rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/MANIFEST.in
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.0.7/README.md
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/
--rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/
--rw-r--r--   0 sunhao     (501) staff       (20)      208 2023-07-02 11:42:33.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)      336 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4033 2023-07-02 14:34:15.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/cache.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3037 2023-07-03 15:58:21.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/consts.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/controller.py
--rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)    18706 2023-07-02 12:06:23.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/
--rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/ocr.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 sunhao     (501) staff       (20)    12155 2023-07-02 12:33:09.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/pages.py
--rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2572 2023-07-02 14:53:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.0.7/ns_asphalt9/main.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-03 16:01:06.000000 ns_asphalt9-0.0.7/setup.cfg
--rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.7/setup.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290847 ns_asphalt9-0.0.8/
+-rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.8/LICENSE
+-rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.8/MANIFEST.in
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-05 10:04:44.290941 ns_asphalt9-0.0.8/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.8/README.md
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.276636 ns_asphalt9-0.0.8/ns_asphalt9/
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.282048 ns_asphalt9-0.0.8/ns_asphalt9/core/
+-rw-r--r--   0 neo.sun    (502) staff       (20)       20 2023-06-30 07:48:40.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.283440 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/
+-rw-r--r--   0 neo.sun    (502) staff       (20)      222 2023-07-03 09:32:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      477 2023-07-03 09:32:06.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     4033 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3917 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3777 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/cache.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3037 2023-07-03 02:10:16.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/consts.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2146 2023-06-30 07:54:21.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/controller.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      634 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.285020 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    18706 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.288715 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1530 2023-06-30 07:54:36.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1841 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    12760 2023-07-03 09:48:32.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/pages.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2572 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290310 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1016 2023-06-30 07:53:42.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1993 2023-06-30 07:53:54.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      862 2023-06-30 07:54:03.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     5558 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/main.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.278630 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-07-05 10:04:44.291709 ns_asphalt9-0.0.8/setup.cfg
+-rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.8/setup.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290585 ns_asphalt9-0.0.8/tests/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.8/tests/test_ocr.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ns_asphalt9-0.0.7/LICENSE` & `ns_asphalt9-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/PKG-INFO` & `ns_asphalt9-0.0.8/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
-Name: ns_asphalt9
-Version: 0.0.7
+Name: ns-asphalt9
+Version: 0.0.8
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
-Description: # ns_asphalt9 
-        
-        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-        
-        
-        ### 硬件依赖
-            
-        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-           
-           用于switch画面输入到虚拟机
-        
-        2. **蓝牙(必选)**
-           
-           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-        
-        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-           
-           同时输出switch到显示器和采集卡，方便debug
-        
-        
-        ### 使用教程
-        
-        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-        
-        
-        ### 免责声明
-        
-        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-        
-        
-        ### 许可证
-        
-        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ns_asphalt9 
+
+基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+
+
+### 硬件依赖
+    
+1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+   
+   用于switch画面输入到虚拟机
+
+2. **蓝牙(必选)**
+   
+   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+
+3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+   
+   同时输出switch到显示器和采集卡，方便debug
+
+
+### 使用教程
+
+[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+
+
+### 免责声明
+
+ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+
+
+### 许可证
+
+![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.7/README.md` & `ns_asphalt9-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/pages.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,38 +158,59 @@
     name = consts.world_series
     feature = "WORLD SERIES|MY POSITION|SERIES SCORE|NEXT MILESTONE|LEADERBOARD|PLAY"
     part_match = True
 
     action = staticmethod(pro.press_button)
     args = (Buttons.A, 3)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "WORLD SERIES" in text:
+            match_count += 3
+        return match_count
+
 
 @cache_decorator("page")
 class TrialSeries(Page):
     """多人二尾流"""
 
     name = consts.trial_series
     feature = "TRIAL SERIES|MY POSITION|SERIES SCORE|NEXT MILESTONE|LEADERBOARD|PLAY"
     part_match = True
 
     action = staticmethod(pro.press_button)
     args = (Buttons.A, 3)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "TRIAL SERIES" in text:
+            match_count += 3
+        return match_count
+
 
 @cache_decorator("page")
 class LimitedSeries(Page):
     """多人二限时赛事"""
 
     name = consts.limited_series
     feature = "LIMITED SERIES|MY POSITION|SERIES SCORE|NEXT MILESTONE|LEADERBOARD|PLAY"
     part_match = True
 
     action = staticmethod(pro.press_button)
     args = (Buttons.A, 3)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "LIMITED SERIES" in text:
+            match_count += 3
+        return match_count
+
 
 @cache_decorator("page")
 class CarHunt(Page):
     """寻车"""
 
     name = consts.carhunt
     feature = "CAR HUNT:.*CAR HUNT EVENT PACK"
@@ -431,16 +452,15 @@
 class SystemError(Page):
     """系统错误"""
 
     name = consts.system_error
     feature = "software.*closed"
     part_match = False
 
-    action = staticmethod(pro.press_group)
-    args = ([Buttons.A] * 3, 3)
+    action = staticmethod(actions.system_error)
 
 
 @cache_decorator("page")
 class ServerError(Page):
     """服务错误"""
 
     name = consts.server_error
```

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9/main.py` & `ns_asphalt9-0.0.8/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
-Name: ns-asphalt9
-Version: 0.0.7
+Name: ns_asphalt9
+Version: 0.0.8
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
-Description: # ns_asphalt9 
-        
-        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-        
-        
-        ### 硬件依赖
-            
-        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-           
-           用于switch画面输入到虚拟机
-        
-        2. **蓝牙(必选)**
-           
-           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-        
-        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-           
-           同时输出switch到显示器和采集卡，方便debug
-        
-        
-        ### 使用教程
-        
-        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-        
-        
-        ### 免责声明
-        
-        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-        
-        
-        ### 许可证
-        
-        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ns_asphalt9 
+
+基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+
+
+### 硬件依赖
+    
+1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+   
+   用于switch画面输入到虚拟机
+
+2. **蓝牙(必选)**
+   
+   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+
+3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+   
+   同时输出switch到显示器和采集卡，方便debug
+
+
+### 使用教程
+
+[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+
+
+### 免责声明
+
+ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+
+
+### 许可证
+
+![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.7/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.0.8/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 ns_asphalt9/core/gui/images/home.png
 ns_asphalt9/core/gui/images/logo.png
 ns_asphalt9/core/gui/images/settings.png
 ns_asphalt9/core/utils/__init__.py
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/fetch_cars.py
 ns_asphalt9/core/utils/log.py
-ns_asphalt9/core/utils/timer.py
+ns_asphalt9/core/utils/timer.py
+tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.0.7/setup.cfg` & `ns_asphalt9-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.7
+version = 0.0.8
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

