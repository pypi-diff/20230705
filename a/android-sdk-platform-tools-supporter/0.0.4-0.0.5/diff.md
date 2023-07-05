# Comparing `tmp/android-sdk-platform-tools-supporter-0.0.4.tar.gz` & `tmp/android-sdk-platform-tools-supporter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.4.tar", last modified: Wed Jul  5 11:22:45 2023, max compression
+gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.5.tar", last modified: Wed Jul  5 14:54:43 2023, max compression
```

## Comparing `android-sdk-platform-tools-supporter-0.0.4.tar` & `android-sdk-platform-tools-supporter-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:22:45.676385 android-sdk-platform-tools-supporter-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1192 2023-07-05 11:22:45.676385 android-sdk-platform-tools-supporter-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-05 11:22:44.000000 android-sdk-platform-tools-supporter-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:22:45.675385 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 11:22:44.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-07-05 11:22:44.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-07-05 11:22:44.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter/android_sdk_platform_tools_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:22:45.675385 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1192 2023-07-05 11:22:45.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-05 11:22:45.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 11:22:45.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 11:22:45.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 11:22:45.000000 android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 11:22:45.676385 android-sdk-platform-tools-supporter-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 11:22:44.000000 android-sdk-platform-tools-supporter-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:54:43.394734 android-sdk-platform-tools-supporter-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-05 14:54:43.393734 android-sdk-platform-tools-supporter-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-05 14:54:22.000000 android-sdk-platform-tools-supporter-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:54:43.393734 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 14:54:22.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-05 14:54:22.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:54:43.393734 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-05 14:54:43.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-05 14:54:43.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:54:43.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:54:22.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 14:54:43.000000 android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:54:43.394734 android-sdk-platform-tools-supporter-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 14:54:22.000000 android-sdk-platform-tools-supporter-0.0.5/setup.py
```

### Comparing `android-sdk-platform-tools-supporter-0.0.4/PKG-INFO` & `android-sdk-platform-tools-supporter-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 Metadata-Version: 2.1
 Name: android-sdk-platform-tools-supporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Android sdk platform tools supporter
 Home-page: https://github.com/automatethem/android-sdk-platform-tools-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # android-sdk-platform-tools-supporter
 
 ```
-import sys
-sys.path.append("/opt")
-import common
-
-https://www.bangseongbeom.com/sys-path-pythonpath.html
-```
-
-```
 import os
 import time
 from android_sdk_platform_tools_supporter.android_sdk_platform_tools import AndroidSdkPlatformTools
 from python_supporter.check_ip import check_ip #pip install python-supporter
 
 base_directory = os.path.dirname(__file__) + "/platform-tools"
 platform_tools = AndroidSdkPlatformTools(base_directory)
```

### Comparing `android-sdk-platform-tools-supporter-0.0.4/README.md` & `android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# android-sdk-platform-tools-supporter
-
-```
-import sys
-sys.path.append("/opt")
-import common
+Metadata-Version: 2.1
+Name: android-sdk-platform-tools-supporter
+Version: 0.0.5
+Summary: Android sdk platform tools supporter
+Home-page: https://github.com/automatethem/android-sdk-platform-tools-supporter
+Author: Sang Ki Kwon
+Author-email: automatethem@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
 
-https://www.bangseongbeom.com/sys-path-pythonpath.html
-```
+# android-sdk-platform-tools-supporter
 
 ```
 import os
 import time
 from android_sdk_platform_tools_supporter.android_sdk_platform_tools import AndroidSdkPlatformTools
 from python_supporter.check_ip import check_ip #pip install python-supporter
```

### Comparing `android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py` & `android-sdk-platform-tools-supporter-0.0.5/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             return []
     
     def data_disable(self):
         if self.base_directory:
             adb = f"{self.base_directory}/platform-tools/adb"
         else:
             adb = "adb"
-        cmd = f"{adb} -s {self.device} shell svc data disable"
+        cmd = f"{adb} -s {self.devices[0]} shell svc data disable"
         os.system(cmd)
 
     def data_enable(self):
         if self.base_directory:
             adb = f"{self.base_directory}/platform-tools/adb"
         else:
             adb = "adb"
-        cmd = f"{adb} -s {self.device} shell svc data enable"
+        cmd = f"{adb} -s {self.devices[0]} shell svc data enable"
         os.system(cmd)
```

### Comparing `android-sdk-platform-tools-supporter-0.0.4/android_sdk_platform_tools_supporter.egg-info/PKG-INFO` & `android-sdk-platform-tools-supporter-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: android-sdk-platform-tools-supporter
-Version: 0.0.4
-Summary: Android sdk platform tools supporter
-Home-page: https://github.com/automatethem/android-sdk-platform-tools-supporter
-Author: Sang Ki Kwon
-Author-email: automatethem@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
 # android-sdk-platform-tools-supporter
 
 ```
-import sys
-sys.path.append("/opt")
-import common
-
-https://www.bangseongbeom.com/sys-path-pythonpath.html
-```
-
-```
 import os
 import time
 from android_sdk_platform_tools_supporter.android_sdk_platform_tools import AndroidSdkPlatformTools
 from python_supporter.check_ip import check_ip #pip install python-supporter
 
 base_directory = os.path.dirname(__file__) + "/platform-tools"
 platform_tools = AndroidSdkPlatformTools(base_directory)
```

### Comparing `android-sdk-platform-tools-supporter-0.0.4/setup.py` & `android-sdk-platform-tools-supporter-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-platform-tools-supporter',
-	version='0.0.4',
+	version='0.0.5',
 	description='Android sdk platform tools supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-platform-tools-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

