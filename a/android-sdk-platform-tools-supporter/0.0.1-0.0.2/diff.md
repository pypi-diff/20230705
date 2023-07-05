# Comparing `tmp/android-sdk-platform-tools-supporter-0.0.1.tar.gz` & `tmp/android-sdk-platform-tools-supporter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.1.tar", last modified: Wed Jul  5 10:50:21 2023, max compression
+gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.2.tar", last modified: Wed Jul  5 10:54:04 2023, max compression
```

## Comparing `android-sdk-platform-tools-supporter-0.0.1.tar` & `android-sdk-platform-tools-supporter-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:50:21.532219 android-sdk-platform-tools-supporter-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:50:21.532219 android-sdk-platform-tools-supporter-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-05 10:50:20.000000 android-sdk-platform-tools-supporter-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:50:21.530219 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 10:50:20.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-05 10:50:20.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:50:21.531219 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:50:21.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-05 10:50:21.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:50:21.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:50:21.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 10:50:21.000000 android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:50:21.532219 android-sdk-platform-tools-supporter-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 10:50:20.000000 android-sdk-platform-tools-supporter-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.180935 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:54:04.183935 android-sdk-platform-tools-supporter-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/setup.py
```

### Comparing `android-sdk-platform-tools-supporter-0.0.1/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py` & `android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 import platform
 import subprocess
+import zipfile
 
 class AndroidSdkPlatformTools:
     def __init__(self, base_directory):
         super().__init__()
         self.base_directory = base_directory
         self.device = None
         self.ip = None
 
         if not os.path.exists(f"{self.base_directory}/platform-tools"):
-        import zipfile
-        if platform.system() == 'Darwin': #맥
-            from_zip = f"{self.base_directory}/platform-tools_r34.0.3-darwin.zip"
-        elif platform.system() == 'Windows': #윈도우
-            from_zip = f"{self.base_directory}/platform-tools_r34.0.3-windows.zip"
-        elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
-            from_zip = f"{self.base_directory}/platform-tools_r34.0.3-linux.zip"
-        zip_file = zipfile.ZipFile(from_zip)
-        zip_file.extractall(self.base_directory)
-        zip_file.close()
+            if platform.system() == 'Darwin': #맥
+                from_zip = f"{self.base_directory}/platform-tools_r34.0.3-darwin.zip"
+            elif platform.system() == 'Windows': #윈도우
+                from_zip = f"{self.base_directory}/platform-tools_r34.0.3-windows.zip"
+            elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+                from_zip = f"{self.base_directory}/platform-tools_r34.0.3-linux.zip"
+            zip_file = zipfile.ZipFile(from_zip)
+            zip_file.extractall(self.base_directory)
+            zip_file.close()
         
     def check_devices(self):    
         cmd = f"{self.base_directory}/platform-tools/adb"
         outputs = subprocess.check_output([cmd, "devices"]).decode('utf-8')
         device = None
         for output in outputs.split("\n")[1:]:
             output = output.strip()
```

### Comparing `android-sdk-platform-tools-supporter-0.0.1/setup.py` & `android-sdk-platform-tools-supporter-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-platform-tools-supporter',
-	version='0.0.1',
+	version='0.0.2',
 	description='Android sdk platform tools supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-platform-tools-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

