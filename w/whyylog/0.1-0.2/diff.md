# Comparing `tmp/whyylog-0.1.tar.gz` & `tmp/whyylog-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyylog-0.1.tar", last modified: Wed Jul  5 13:08:02 2023, max compression
+gzip compressed data, was "whyylog-0.2.tar", last modified: Wed Jul  5 14:50:39 2023, max compression
```

## Comparing `whyylog-0.1.tar` & `whyylog-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 13:08:02.337832 whyylog-0.1/
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)    35149 2023-06-26 15:18:33.000000 whyylog-0.1/LICENSE
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1883 2023-07-05 13:08:02.337832 whyylog-0.1/PKG-INFO
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1405 2023-06-26 15:18:33.000000 whyylog-0.1/README.md
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       79 2023-07-05 13:08:02.337832 whyylog-0.1/setup.cfg
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)      912 2023-07-05 13:07:50.000000 whyylog-0.1/setup.py
-drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 13:08:02.337832 whyylog-0.1/whylog/
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       33 2023-07-05 12:57:07.000000 whyylog-0.1/whylog/__init__.py
-drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 13:08:02.337832 whyylog-0.1/whylog/src/
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       33 2023-07-05 12:57:55.000000 whyylog-0.1/whylog/src/__init__.py
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     5463 2023-07-05 13:01:01.000000 whyylog-0.1/whylog/src/whylog.py
-drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 13:08:02.337832 whyylog-0.1/whyylog.egg-info/
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1883 2023-07-05 13:08:02.000000 whyylog-0.1/whyylog.egg-info/PKG-INFO
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)      223 2023-07-05 13:08:02.000000 whyylog-0.1/whyylog.egg-info/SOURCES.txt
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)        1 2023-07-05 13:08:02.000000 whyylog-0.1/whyylog.egg-info/dependency_links.txt
--rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)        7 2023-07-05 13:08:02.000000 whyylog-0.1/whyylog.egg-info/top_level.txt
+drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 14:50:39.855155 whyylog-0.2/
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)    35149 2023-06-26 15:18:33.000000 whyylog-0.2/LICENSE
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1997 2023-07-05 14:50:39.855155 whyylog-0.2/PKG-INFO
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1519 2023-07-05 14:47:03.000000 whyylog-0.2/README.md
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       79 2023-07-05 14:50:39.855155 whyylog-0.2/setup.cfg
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)      912 2023-07-05 14:49:10.000000 whyylog-0.2/setup.py
+drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 14:50:39.855155 whyylog-0.2/whylog/
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       33 2023-07-05 12:57:07.000000 whyylog-0.2/whylog/__init__.py
+drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 14:50:39.855155 whyylog-0.2/whylog/src/
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)       33 2023-07-05 12:57:55.000000 whyylog-0.2/whylog/src/__init__.py
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     5463 2023-07-05 13:01:01.000000 whyylog-0.2/whylog/src/whylog.py
+drwxr-xr-x   0 iamlrk    (1000) iamlrk    (1000)        0 2023-07-05 14:50:39.855155 whyylog-0.2/whyylog.egg-info/
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)     1997 2023-07-05 14:50:39.000000 whyylog-0.2/whyylog.egg-info/PKG-INFO
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)      223 2023-07-05 14:50:39.000000 whyylog-0.2/whyylog.egg-info/SOURCES.txt
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)        1 2023-07-05 14:50:39.000000 whyylog-0.2/whyylog.egg-info/dependency_links.txt
+-rw-r--r--   0 iamlrk    (1000) iamlrk    (1000)        7 2023-07-05 14:50:39.000000 whyylog-0.2/whyylog.egg-info/top_level.txt
```

### Comparing `whyylog-0.1/LICENSE` & `whyylog-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whyylog-0.1/PKG-INFO` & `whyylog-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: whyylog
-Version: 0.1
+Version: 0.2
 Summary: Prints out a log message to terminal in color
 Home-page: https://github.com/iamlrk/ylog
 Author-email: <lepakshiramkiran@hotmail.com>
 Keywords: python,logging,log,print
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ylog
+# whylog
 
 This is an library to print color-coded log messages to the terminal. It prints in the following format.
 
 `TIME [LOG TYPE] (file names) > (path of the call|line no): Message.`
 
 ## Log Levels
 
@@ -34,24 +34,30 @@
 |         8 | None          | NA          | NA               |
 
 ## Usage
 
 ### Code
 
 ```python
-from ylog import Log
+from whylog import Log
 
-log = Log(loglevel=8)
+def main():
+    test()
 
-log.emergency('Test emergency Print by importing')
-log.alert('Test alert Print by importing')
-log.critical('Test crtical Print by importing')
-log.error('Test error Print by importing')
-log.warning('Test warning Print by importing')
-log.notice('Test notice Print by importing')
-log.debug('Test Debug Print by importing')
-log.info('Test info Print by importing')
+def test():
+    log = Log(loglevel=8)
+    log.emergency('Test emergency Print by importing')
+    log.alert('Test alert Print by importing')
+    log.critical('Test crtical Print by importing')
+    log.error('Test error Print by importing')
+    log.warning('Test warning Print by importing')
+    log.notice('Test notice Print by importing')
+    log.debug('Test Debug Print by importing')
+    log.info('Test info Print by importing')
+
+if __name__ == '__main__':
+    main()
 ```
 
 ### Output
 
 ![Output](images/output.png)
```

### Comparing `whyylog-0.1/README.md` & `whyylog-0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ylog
+# whylog
 
 This is an library to print color-coded log messages to the terminal. It prints in the following format.
 
 `TIME [LOG TYPE] (file names) > (path of the call|line no): Message.`
 
 ## Log Levels
 
@@ -20,24 +20,30 @@
 |         8 | None          | NA          | NA               |
 
 ## Usage
 
 ### Code
 
 ```python
-from ylog import Log
+from whylog import Log
 
-log = Log(loglevel=8)
+def main():
+    test()
 
-log.emergency('Test emergency Print by importing')
-log.alert('Test alert Print by importing')
-log.critical('Test crtical Print by importing')
-log.error('Test error Print by importing')
-log.warning('Test warning Print by importing')
-log.notice('Test notice Print by importing')
-log.debug('Test Debug Print by importing')
-log.info('Test info Print by importing')
+def test():
+    log = Log(loglevel=8)
+    log.emergency('Test emergency Print by importing')
+    log.alert('Test alert Print by importing')
+    log.critical('Test crtical Print by importing')
+    log.error('Test error Print by importing')
+    log.warning('Test warning Print by importing')
+    log.notice('Test notice Print by importing')
+    log.debug('Test Debug Print by importing')
+    log.info('Test info Print by importing')
+
+if __name__ == '__main__':
+    main()
 ```
 
 ### Output
 
 ![Output](images/output.png)
```

### Comparing `whyylog-0.1/setup.py` & `whyylog-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1' 
+VERSION = '0.2' 
 DESCRIPTION = 'Prints out a log message to terminal in color'
 with open('README.md', 'r') as r:
     LONG_DESCRIPTION = r.read()
 
 # Setting up
 setup(
        # the name must match the folder name 'simpleopers'
```

### Comparing `whyylog-0.1/whylog/src/whylog.py` & `whyylog-0.2/whylog/src/whylog.py`

 * *Files identical despite different names*

### Comparing `whyylog-0.1/whyylog.egg-info/PKG-INFO` & `whyylog-0.2/whyylog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: whyylog
-Version: 0.1
+Version: 0.2
 Summary: Prints out a log message to terminal in color
 Home-page: https://github.com/iamlrk/ylog
 Author-email: <lepakshiramkiran@hotmail.com>
 Keywords: python,logging,log,print
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ylog
+# whylog
 
 This is an library to print color-coded log messages to the terminal. It prints in the following format.
 
 `TIME [LOG TYPE] (file names) > (path of the call|line no): Message.`
 
 ## Log Levels
 
@@ -34,24 +34,30 @@
 |         8 | None          | NA          | NA               |
 
 ## Usage
 
 ### Code
 
 ```python
-from ylog import Log
+from whylog import Log
 
-log = Log(loglevel=8)
+def main():
+    test()
 
-log.emergency('Test emergency Print by importing')
-log.alert('Test alert Print by importing')
-log.critical('Test crtical Print by importing')
-log.error('Test error Print by importing')
-log.warning('Test warning Print by importing')
-log.notice('Test notice Print by importing')
-log.debug('Test Debug Print by importing')
-log.info('Test info Print by importing')
+def test():
+    log = Log(loglevel=8)
+    log.emergency('Test emergency Print by importing')
+    log.alert('Test alert Print by importing')
+    log.critical('Test crtical Print by importing')
+    log.error('Test error Print by importing')
+    log.warning('Test warning Print by importing')
+    log.notice('Test notice Print by importing')
+    log.debug('Test Debug Print by importing')
+    log.info('Test info Print by importing')
+
+if __name__ == '__main__':
+    main()
 ```
 
 ### Output
 
 ![Output](images/output.png)
```

