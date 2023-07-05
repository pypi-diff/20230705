# Comparing `tmp/t265-0.1.0.tar.gz` & `tmp/t265-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t265-0.1.0.tar", last modified: Wed Jul  5 00:47:53 2023, max compression
+gzip compressed data, was "t265-0.1.1.tar", last modified: Wed Jul  5 01:02:00 2023, max compression
```

## Comparing `t265-0.1.0.tar` & `t265-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 00:47:53.870202 t265-0.1.0/
--rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 t265-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      527 2023-07-05 00:47:53.870202 t265-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-07-05 00:15:37.000000 t265-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 00:47:53.870202 t265-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-05 00:47:46.000000 t265-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:47:53.869202 t265-0.1.0/t265.egg-info/
--rw-rw-rw-   0        0        0      527 2023-07-05 00:47:53.000000 t265-0.1.0/t265.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-07-05 00:47:53.000000 t265-0.1.0/t265.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:47:53.000000 t265-0.1.0/t265.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 00:47:53.000000 t265-0.1.0/t265.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:47:53.000000 t265-0.1.0/t265.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 01:02:00.367553 t265-0.1.1/
+-rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 t265-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      563 2023-07-05 01:02:00.366553 t265-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-07-05 00:15:37.000000 t265-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 01:02:00.367553 t265-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-07-05 01:01:16.000000 t265-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:02:00.366553 t265-0.1.1/t265.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-07-05 01:02:00.000000 t265-0.1.1/t265.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-05 01:02:00.000000 t265-0.1.1/t265.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:02:00.000000 t265-0.1.1/t265.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-05 01:02:00.000000 t265-0.1.1/t265.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:02:00.000000 t265-0.1.1/t265.egg-info/top_level.txt
```

### Comparing `t265-0.1.0/PKG-INFO` & `t265-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.0
+Version: 0.1.1
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
-Platform: UNKNOWN
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-
-UNKNOWN
-
```

### Comparing `t265-0.1.0/setup.py` & `t265-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,26 @@
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
+# from pathlib import Path
+# this_directory = Path(__file__).parent
+# long_description = (this_directory / "README.md").read_text()
+
+
 setup(
     name='t265',
-    version='0.1.0',
+    version='0.1.1',
     description='t265 Tracking camera API wrapper',
     author='Yusuke Tanaka',
     license='LGPLv3',
+    project_urls={'GitHub':'https://github.com/Suke0811/Localization_T265'},
     packages=find_packages(include=['t265', 't265.*']),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Robot Framework',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
```

### Comparing `t265-0.1.0/t265.egg-info/PKG-INFO` & `t265-0.1.1/t265.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.0
+Version: 0.1.1
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
-Platform: UNKNOWN
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-
-UNKNOWN
-
```

