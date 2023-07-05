# Comparing `tmp/android-sdk-platform-tools-supporter-0.0.2.tar.gz` & `tmp/android-sdk-platform-tools-supporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.2.tar", last modified: Wed Jul  5 10:54:04 2023, max compression
+gzip compressed data, was "android-sdk-platform-tools-supporter-0.0.3.tar", last modified: Wed Jul  5 11:09:01 2023, max compression
```

## Comparing `android-sdk-platform-tools-supporter-0.0.2.tar` & `android-sdk-platform-tools-supporter-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.180935 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 10:54:04.182935 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 10:54:04.183935 android-sdk-platform-tools-supporter-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 10:54:03.000000 android-sdk-platform-tools-supporter-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:09:01.093206 android-sdk-platform-tools-supporter-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-07-05 11:09:01.093206 android-sdk-platform-tools-supporter-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:09:01.092206 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter/android_sdk_platform_tools_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:09:01.092206 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 11:09:01.093206 android-sdk-platform-tools-supporter-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      660 2023-07-05 11:09:00.000000 android-sdk-platform-tools-supporter-0.0.3/setup.py
```

### Comparing `android-sdk-platform-tools-supporter-0.0.2/android_sdk_platform_tools_supporter/android_sdk_platform_tools.py` & `android-sdk-platform-tools-supporter-0.0.3/android_sdk_platform_tools_supporter/android_sdk_platform_tools_old.py`

 * *Files identical despite different names*

### Comparing `android-sdk-platform-tools-supporter-0.0.2/setup.py` & `android-sdk-platform-tools-supporter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-platform-tools-supporter',
-	version='0.0.2',
+	version='0.0.3',
 	description='Android sdk platform tools supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-platform-tools-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

