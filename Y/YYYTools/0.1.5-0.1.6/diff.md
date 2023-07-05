# Comparing `tmp/YYYTools-0.1.5.tar.gz` & `tmp/YYYTools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\YYYTools-0.1.5.tar", last modified: Sun Nov 13 21:36:32 2022, max compression
+gzip compressed data, was "dist\YYYTools-0.1.6.tar", last modified: Wed Jul  5 20:01:08 2023, max compression
```

## Comparing `YYYTools-0.1.5.tar` & `YYYTools-0.1.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.529014 YYYTools-0.1.5/
--rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      300 2022-11-13 21:36:32.528013 YYYTools-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.457996 YYYTools-0.1.5/YTools/
--rw-rw-rw-   0        0        0       57 2021-12-18 16:09:23.000000 YYYTools-0.1.5/YTools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.459999 YYYTools-0.1.5/YTools/cg/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:52.000000 YYYTools-0.1.5/YTools/cg/__init__.py
--rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.5/YTools/cg/glsl_use.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.462999 YYYTools-0.1.5/YTools/client/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:46.000000 YYYTools-0.1.5/YTools/client/__init__.py
--rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.5/YTools/client/cui.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.465999 YYYTools-0.1.5/YTools/debug/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:45.000000 YYYTools-0.1.5/YTools/debug/__init__.py
--rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.5/YTools/debug/debug_recursion.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.469000 YYYTools-0.1.5/YTools/deeplearning/
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/deeplearning/__init__.py
--rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/deeplearning/composed_model.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.475002 YYYTools-0.1.5/YTools/experiment_helper/
--rw-rw-rw-   0        0        0      104 2021-12-18 16:09:24.000000 YYYTools-0.1.5/YTools/experiment_helper/__init__.py
--rw-rw-rw-   0        0        0     1822 2021-12-18 16:09:24.000000 YYYTools-0.1.5/YTools/experiment_helper/logger.py
--rw-rw-rw-   0        0        0      646 2021-12-18 16:09:24.000000 YYYTools-0.1.5/YTools/experiment_helper/random_seeder.py
--rw-rw-rw-   0        0        0      194 2021-12-18 16:09:24.000000 YYYTools-0.1.5/YTools/experiment_helper/watch_time.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.480003 YYYTools-0.1.5/YTools/network/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:47.000000 YYYTools-0.1.5/YTools/network/__init__.py
--rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.5/YTools/network/communicate.py
--rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.5/YTools/network/protocol.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.486004 YYYTools-0.1.5/YTools/network/server/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:48.000000 YYYTools-0.1.5/YTools/network/server/__init__.py
--rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.5/YTools/network/server/client.py
--rw-rw-rw-   0        0        0      712 2021-12-18 16:09:48.000000 YYYTools-0.1.5/YTools/network/server/server.py
--rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.5/YTools/network/server/urlconf.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.493006 YYYTools-0.1.5/YTools/system/
--rw-rw-rw-   0        0        0       77 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/__init__.py
--rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/cmd_control.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.496007 YYYTools-0.1.5/YTools/system/fakepath/
--rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/fakepath/__init__.py
--rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/fakepath/fakepath.py
--rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/fileintercept.py
--rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/filewrite.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.501008 YYYTools-0.1.5/YTools/system/locker/
--rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.5/YTools/system/locker/__init__.py
--rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.5/YTools/system/locker/filelock.py
--rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.5/YTools/system/locker/lock.py
--rw-rw-rw-   0        0        0    10592 2021-12-18 16:09:25.000000 YYYTools-0.1.5/YTools/system/static_hash.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.517012 YYYTools-0.1.5/YTools/universe/
--rw-rw-rw-   0        0        0      188 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/__init__.py
--rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.5/YTools/universe/beautiful_str.py
--rw-rw-rw-   0        0        0     1779 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/universe/exceptions.py
--rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/extra_type.py
--rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/universe/filename.py
--rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/myrandom.py
--rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/universe/onexit.py
--rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/pather.py
--rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/save_load.py
--rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.5/YTools/universe/strlen.py
--rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.5/YTools/universe/temp_cwd.py
--rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.5/YTools/universe/timer.py
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.524013 YYYTools-0.1.5/YYYTools.egg-info/
-drwxrwxrwx   0        0        0        0 2022-11-13 21:36:32.526013 YYYTools-0.1.5/YYYTools.egg-info/._DAV/
--rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.5/YYYTools.egg-info/._DAV/.state_for_dir.dir
--rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.5/YYYTools.egg-info/._DAV/.state_for_dir.pag
--rw-rw-rw-   0        0        0      300 2022-11-13 21:36:32.000000 YYYTools-0.1.5/YYYTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2022-11-13 21:36:32.000000 YYYTools-0.1.5/YYYTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-13 21:36:32.000000 YYYTools-0.1.5/YYYTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-11-13 21:36:32.000000 YYYTools-0.1.5/YYYTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-13 21:36:32.000000 YYYTools-0.1.5/YYYTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        5 2022-11-13 21:08:17.000000 YYYTools-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-13 21:36:32.529014 YYYTools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      776 2022-11-13 21:35:43.000000 YYYTools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.089201 YYYTools-0.1.6/
+-rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-05 20:01:08.089201 YYYTools-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:07.995222 YYYTools-0.1.6/YTools/
+-rw-rw-rw-   0        0        0       57 2021-12-18 16:09:23.000000 YYYTools-0.1.6/YTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:07.998224 YYYTools-0.1.6/YTools/cg/
+-rw-rw-rw-   0        0        0        0 2021-12-18 16:09:52.000000 YYYTools-0.1.6/YTools/cg/__init__.py
+-rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.6/YTools/cg/glsl_use.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.002223 YYYTools-0.1.6/YTools/client/
+-rw-rw-rw-   0        0        0        0 2021-12-18 16:09:46.000000 YYYTools-0.1.6/YTools/client/__init__.py
+-rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.6/YTools/client/cui.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.006224 YYYTools-0.1.6/YTools/debug/
+-rw-rw-rw-   0        0        0        0 2021-12-18 16:09:45.000000 YYYTools-0.1.6/YTools/debug/__init__.py
+-rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.6/YTools/debug/debug_recursion.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.010225 YYYTools-0.1.6/YTools/deeplearning/
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/deeplearning/__init__.py
+-rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/deeplearning/composed_model.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.018226 YYYTools-0.1.6/YTools/experiment_helper/
+-rw-rw-rw-   0        0        0      104 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/__init__.py
+-rw-rw-rw-   0        0        0     1822 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/logger.py
+-rw-rw-rw-   0        0        0      646 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/random_seeder.py
+-rw-rw-rw-   0        0        0      194 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/watch_time.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.023228 YYYTools-0.1.6/YTools/network/
+-rw-rw-rw-   0        0        0        0 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/__init__.py
+-rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/communicate.py
+-rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/protocol.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.030229 YYYTools-0.1.6/YTools/network/server/
+-rw-rw-rw-   0        0        0        0 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/__init__.py
+-rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/client.py
+-rw-rw-rw-   0        0        0      751 2023-07-05 19:59:18.000000 YYYTools-0.1.6/YTools/network/server/server.py
+-rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/urlconf.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.043233 YYYTools-0.1.6/YTools/system/
+-rw-rw-rw-   0        0        0       77 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/__init__.py
+-rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/cmd_control.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.047233 YYYTools-0.1.6/YTools/system/fakepath/
+-rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fakepath/__init__.py
+-rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fakepath/fakepath.py
+-rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fileintercept.py
+-rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/filewrite.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.052193 YYYTools-0.1.6/YTools/system/locker/
+-rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/__init__.py
+-rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/filelock.py
+-rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/lock.py
+-rw-rw-rw-   0        0        0    10592 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/static_hash.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.076198 YYYTools-0.1.6/YTools/universe/
+-rw-rw-rw-   0        0        0      188 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/__init__.py
+-rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.6/YTools/universe/beautiful_str.py
+-rw-rw-rw-   0        0        0     1779 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/exceptions.py
+-rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/extra_type.py
+-rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/filename.py
+-rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/myrandom.py
+-rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/onexit.py
+-rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/pather.py
+-rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/save_load.py
+-rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.6/YTools/universe/strlen.py
+-rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/temp_cwd.py
+-rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.084200 YYYTools-0.1.6/YYYTools.egg-info/
+drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.086201 YYYTools-0.1.6/YYYTools.egg-info/._DAV/
+-rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.dir
+-rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.pag
+-rw-rw-rw-   0        0        0      265 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        5 2022-11-13 21:08:17.000000 YYYTools-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:01:08.090201 YYYTools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-07-05 19:59:30.000000 YYYTools-0.1.6/setup.py
```

### Comparing `YYYTools-0.1.5/LICENSE` & `YYYTools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/cg/glsl_use.py` & `YYYTools-0.1.6/YTools/cg/glsl_use.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/client/cui.py` & `YYYTools-0.1.6/YTools/client/cui.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/debug/debug_recursion.py` & `YYYTools-0.1.6/YTools/debug/debug_recursion.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/deeplearning/composed_model.py` & `YYYTools-0.1.6/YTools/deeplearning/composed_model.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/experiment_helper/logger.py` & `YYYTools-0.1.6/YTools/experiment_helper/logger.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/experiment_helper/random_seeder.py` & `YYYTools-0.1.6/YTools/experiment_helper/random_seeder.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/network/communicate.py` & `YYYTools-0.1.6/YTools/network/communicate.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/network/protocol.py` & `YYYTools-0.1.6/YTools/network/protocol.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/network/server/server.py` & `YYYTools-0.1.6/YTools/network/server/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 
 	for url , func in responsers.items():
 		add_response(url , func , configs)
 
 	settings.configure(
 		DEBUG = True,	
 		ROOT_URLCONF = "YTools.network.server.urlconf", 
+		SECRET_KEY = "THEWORLD", # unsafe!!
 	)
 	django.setup()
 
 	ipaddr = "{ip}:{port}".format(ip = ip , port = port)
 	execute_from_command_line(["" , "runserver" , ipaddr])
```

### Comparing `YYYTools-0.1.5/YTools/network/server/urlconf.py` & `YYYTools-0.1.6/YTools/network/server/urlconf.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/system/cmd_control.py` & `YYYTools-0.1.6/YTools/system/cmd_control.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/system/fakepath/fakepath.py` & `YYYTools-0.1.6/YTools/system/fakepath/fakepath.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/system/locker/filelock.py` & `YYYTools-0.1.6/YTools/system/locker/filelock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/system/locker/lock.py` & `YYYTools-0.1.6/YTools/system/locker/lock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/system/static_hash.py` & `YYYTools-0.1.6/YTools/system/static_hash.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/universe/beautiful_str.py` & `YYYTools-0.1.6/YTools/universe/beautiful_str.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/universe/exceptions.py` & `YYYTools-0.1.6/YTools/universe/exceptions.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/universe/extra_type.py` & `YYYTools-0.1.6/YTools/universe/extra_type.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/universe/filename.py` & `YYYTools-0.1.6/YTools/universe/filename.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YTools/universe/timer.py` & `YYYTools-0.1.6/YTools/universe/timer.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YYYTools.egg-info/._DAV/.state_for_dir.pag` & `YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.pag`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/YYYTools.egg-info/SOURCES.txt` & `YYYTools-0.1.6/YYYTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.5/setup.py` & `YYYTools-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     reqs = f.read()
 
 pkgs = [p for p in find_packages() if p.startswith('YTools')]
 print(pkgs)
 
 setup(
     name='YYYTools',
-    version='0.1.5',
+    version='0.1.6',
     url='http://github.com/FFTYYY/YTools',
     description='',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='MIT',
     author = 'Yongyi Yang',
 	author_email = 'yongyi@umich.edu',
```

