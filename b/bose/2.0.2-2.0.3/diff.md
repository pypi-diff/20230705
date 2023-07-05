# Comparing `tmp/bose-2.0.2.tar.gz` & `tmp/bose-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.2.tar", last modified: Sat Jul  1 15:55:11 2023, max compression
+gzip compressed data, was "bose-2.0.3.tar", last modified: Wed Jul  5 01:36:20 2023, max compression
```

## Comparing `bose-2.0.2.tar` & `bose-2.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:55:11.822726 bose-2.0.2/
--rw-rw-rw-   0        0        0    14240 2023-07-01 15:55:11.822726 bose-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-01 15:55:11.822726 bose-2.0.2/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.2/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.2/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.2/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.2/bose/base_data.py
--rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.2/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.2/bose/beep_utils.py
--rw-rw-rw-   0        0        0    10014 2023-07-01 15:53:31.955272 bose-2.0.2/bose/bose_driver.py
--rw-rw-rw-   0        0        0    10026 2023-07-01 15:54:08.464721 bose-2.0.2/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7700 2023-06-29 13:46:50.340921 bose-2.0.2/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.2/bose/download_driver.py
--rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.2/bose/ip_utils.py
--rw-rw-rw-   0        0        0     2953 2023-06-30 15:33:26.223178 bose-2.0.2/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.2/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.2/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.2/bose/opponent.py
--rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.2/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.2/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.2/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.2/bose/task_config.py
--rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.2/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.2/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-2.0.2/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.2/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.2/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-2.0.2/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-01 15:54:52.364280 bose-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:36:20.736947 bose-2.0.3/
+-rw-rw-rw-   0        0        0    14240 2023-07-05 01:36:20.736947 bose-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 01:36:20.736947 bose-2.0.3/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.3/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.3/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.3/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.3/bose/base_data.py
+-rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.3/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.3/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    10014 2023-07-01 15:53:31.955272 bose-2.0.3/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10026 2023-07-01 15:54:08.464721 bose-2.0.3/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.3/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.3/bose/download_driver.py
+-rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.3/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     2995 2023-07-01 18:25:25.812969 bose-2.0.3/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.3/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.3/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.3/bose/opponent.py
+-rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.3/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.3/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.3/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.3/bose/task_config.py
+-rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.3/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.3/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.3/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.3/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.3/bose/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.3/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-05 01:36:00.489143 bose-2.0.3/setup.py
```

### Comparing `bose-2.0.2/PKG-INFO` & `bose-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.2
+Version: 2.0.3
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-2.0.2/README.rst` & `bose-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/account_generator.py` & `bose-2.0.3/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/analytics.py` & `bose-2.0.3/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/base_data.py` & `bose-2.0.3/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/base_task.py` & `bose-2.0.3/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/bose_driver.py` & `bose-2.0.3/bose/bose_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/bose_undetected_driver.py` & `bose-2.0.3/bose/bose_undetected_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/create_driver.py` & `bose-2.0.3/bose/create_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,48 +68,49 @@
 def delete_profile_path(user_id):
     path = create_profile_path(user_id)
     shutil.rmtree(path, ignore_errors=True)
 
 
 def add_essential_options(options, profile, window_size, user_agent):
     options.add_argument("--start-maximized")
-
-    if window_size == None:
-        if profile == None:
-            window_size = WindowSizeInstance.get_random()
-        else:
-            window_size = WindowSizeInstance.get_hashed(profile)
-    else:
-        if window_size == WindowSize.RANDOM:
-            window_size = WindowSizeInstance.get_random()
-        elif window_size == WindowSize.HASHED:
-            window_size = WindowSizeInstance.get_hashed(profile)
+    if window_size != WindowSize.REAL:
+        if window_size == None:
+            if profile == None:
+                window_size = WindowSizeInstance.get_random()
+            else:
+                window_size = WindowSizeInstance.get_hashed(profile)
         else:
-            window_size = window_size
+            if window_size == WindowSize.RANDOM:
+                window_size = WindowSizeInstance.get_random()
+            elif window_size == WindowSize.HASHED:
+                window_size = WindowSizeInstance.get_hashed(profile)
+            else:
+                window_size = window_size
 
-    window_size = WindowSize.window_size_to_string(window_size)
-    options.add_argument(f"--window-size={window_size}")
+        window_size = WindowSize.window_size_to_string(window_size)
+        options.add_argument(f"--window-size={window_size}")
 
     if profile is not None:
         profile = str(profile)
 
-    if user_agent == None:
-        if profile == None:
-            user_agent = UserAgentInstance.get_random()
-        else:
-            user_agent = UserAgentInstance.get_hashed(profile)
-    else:
-        if user_agent == UserAgent.RANDOM:
-            user_agent = UserAgentInstance.get_random()
-        elif user_agent == UserAgent.HASHED:
-            user_agent = UserAgentInstance.get_hashed(profile)
+    if user_agent != UserAgent.REAL:
+        if user_agent == None:
+            if profile == None:
+                user_agent = UserAgentInstance.get_random()
+            else:
+                user_agent = UserAgentInstance.get_hashed(profile)
         else:
-            user_agent = user_agent
+            if user_agent == UserAgent.RANDOM:
+                user_agent = UserAgentInstance.get_random()
+            elif user_agent == UserAgent.HASHED:
+                user_agent = UserAgentInstance.get_hashed(profile)
+            else:
+                user_agent = user_agent
 
-    add_useragent(options, user_agent)
+        add_useragent(options, user_agent)
 
     has_user = profile is not None
 
     if has_user:
         path = create_profile_path(profile)
         user_data_path = f"--user-data-dir={path}"
         options.add_argument(user_data_path)
```

### Comparing `bose-2.0.2/bose/download_driver.py` & `bose-2.0.3/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/ip_utils.py` & `bose-2.0.3/bose/ip_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/launch_tasks.py` & `bose-2.0.3/bose/launch_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     next_prompt = "Please change your IP and press Enter to continue..."
     
     while True:
         beep_input(next_prompt, should_beep)
         new_ip = get_valid_ip()
 
         if new_ip == current_ip:
-            next_prompt = """In order to proceed, it is necessary to change your IP address as a precautionary measure against Bot Detection. Please visit TODO_LINK to learn how to change your IP. Once you have successfully changed your IP address, please press Enter to continue..."""
+            next_prompt = """In order to proceed, it is necessary to change your IP address as a precautionary measure against Bot Detection. Please visit https://www.omkar.cloud/bose/docs/guides/change-ip/ to learn how to change your IP. Once you have successfully changed your IP address, please press Enter to continue..."""
 
         elif new_ip in seen_ips:
             next_prompt = "Your computer previously had this IP address. Please change your IP and press Enter to continue..."
         else:
             LocalStorage.set_item("seen_ips", LocalStorage.get_item("seen_ips", []) + [current_ip])
             return new_ip
```

### Comparing `bose-2.0.2/bose/local_storage.py` & `bose-2.0.3/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/local_storage_driver.py` & `bose-2.0.3/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/output.py` & `bose-2.0.3/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/profile.py` & `bose-2.0.3/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/schedule_utils.py` & `bose-2.0.3/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/task_info.py` & `bose-2.0.3/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/temp_mail.py` & `bose-2.0.3/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/user_agent.py` & `bose-2.0.3/bose/user_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,19 @@
     elif is_mac():
         return mac
     else:
         return linux
 
 class UserAgent(BaseData):
 
+    REAL = "REAL"
     RANDOM = "RANDOM"
     HASHED = "HASHED"
+    
+    google_bot = "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)" 
 
     user_agent_106 = get_correct_agent("Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.37",
                                        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",
                                        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.37")
 
     user_agent_105 = get_correct_agent("Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36",
                                        "Mozilla/5.0 (Macintosh; Intel Mac OS X) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36",
```

### Comparing `bose-2.0.2/bose/utils.py` & `bose-2.0.3/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.2/bose/window_size.py` & `bose-2.0.3/bose/window_size.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .base_data import BaseData
 
 class WindowSize(BaseData):
 
     RANDOM = "RANDOM"
+    REAL = "REAL"
     HASHED = "HASHED"
 
     window_size_1920_1080 = [1920, 1080, ]
     window_size_1366_768 =  [1366, 768, ]
     window_size_1536_864 =  [1536, 864, ]
     window_size_1280_720 =  [1280, 720, ]
     window_size_1440_900 =  [1440, 900, ]
```

### Comparing `bose-2.0.2/setup.py` & `bose-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.2',
+    version='2.0.3',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

