# Comparing `tmp/LinuxRecycle-1.9.3.tar.gz` & `tmp/LinuxRecycle-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LinuxRecycle-1.9.3.tar", last modified: Fri Aug 14 02:49:13 2020, max compression
+gzip compressed data, was "LinuxRecycle-1.9.4.tar", last modified: Wed Jul  5 07:05:46 2023, max compression
```

## Comparing `LinuxRecycle-1.9.3.tar` & `LinuxRecycle-1.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/
--rwxr-xr-x   0 root         (0) root         (0)    35149 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      801 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/LinuxRecycle.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       47 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      801 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      381 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/linuxrecycle/
--rw-r--r--   0 root         (0) root         (0)     2223 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/AutoRegularTask.py
--rwxr-xr-x   0 root         (0) root         (0)     4984 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/DB.py
--rw-r--r--   0 root         (0) root         (0)      520 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/__init__.py
--rw-r--r--   0 root         (0) root         (0)      591 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/argv.py
--rwxr-xr-x   0 root         (0) root         (0)     2659 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/auto_clear.py
--rwxr-xr-x   0 root         (0) root         (0)     2163 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/config.py
--rwxr-xr-x   0 root         (0) root         (0)     1489 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/main.py
--rwxr-xr-x   0 root         (0) root         (0)     3042 2020-08-14 02:48:21.000000 LinuxRecycle-1.9.3/linuxrecycle/oper.py
--rwxr-xr-x   0 root         (0) root         (0)     1332 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/printDB.py
--rwxr-xr-x   0 root         (0) root         (0)     1211 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/recover.py
--rw-r--r--   0 root         (0) root         (0)      642 2020-07-14 06:24:05.000000 LinuxRecycle-1.9.3/linuxrecycle/setCrontab.py
--rwxr-xr-x   0 root         (0) root         (0)     2271 2020-08-14 02:47:38.000000 LinuxRecycle-1.9.3/linuxrecycle/trashInfo.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-08-14 02:49:13.000000 LinuxRecycle-1.9.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1415 2020-08-14 02:49:11.000000 LinuxRecycle-1.9.3/setup.py
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/
+-rwxr-xr-x   0 maxx      (1000) research  (1001)    35149 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/LICENSE
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.090639 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/
+-rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/PKG-INFO
+-rw-r--r--   0 maxx      (1000) research  (1001)      546 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/SOURCES.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)        1 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/dependency_links.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)      168 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/entry_points.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)       10 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/requires.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)       13 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/top_level.txt
+-rwxr-xr-x   0 maxx      (1000) research  (1001)       47 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/MANIFEST.in
+-rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/PKG-INFO
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1530 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/README.md
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/linuxrecycle/
+-rw-r--r--   0 maxx      (1000) research  (1001)     2223 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/AutoRegularTask.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     4984 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/DB.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      520 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/__init__.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      591 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/argv.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2648 2023-07-05 06:50:50.000000 LinuxRecycle-1.9.4/linuxrecycle/auto_clear.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2163 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/config.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1489 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/main.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2958 2023-07-05 06:50:34.000000 LinuxRecycle-1.9.4/linuxrecycle/oper.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1332 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/printDB.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1211 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/recover.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      642 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/setCrontab.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2271 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/trashInfo.py
+-rw-r--r--   0 maxx      (1000) research  (1001)       38 2023-07-05 07:05:46.093639 LinuxRecycle-1.9.4/setup.cfg
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1510 2023-07-05 07:05:44.000000 LinuxRecycle-1.9.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `LinuxRecycle-1.9.3/LICENSE` & `LinuxRecycle-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/LinuxRecycle.egg-info/SOURCES.txt` & `LinuxRecycle-1.9.4/LinuxRecycle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/AutoRegularTask.py` & `LinuxRecycle-1.9.4/linuxrecycle/AutoRegularTask.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/DB.py` & `LinuxRecycle-1.9.4/linuxrecycle/DB.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/__init__.py` & `LinuxRecycle-1.9.4/linuxrecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/argv.py` & `LinuxRecycle-1.9.4/linuxrecycle/argv.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/auto_clear.py` & `LinuxRecycle-1.9.4/linuxrecycle/auto_clear.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,16 @@
 def main():
     """
     1. select the record with time less than t_0 and exits = ""exits
     2. delete them and update the data base
     """
     conn = sqlite3.connect(config.local_config.get('core', 'data_base_file'))
     t0 = time.time() - 3600.0 * 24.0 * config.local_config.getint('core', 'keep_days')
-    print("delete files more than {} days".format(
-        config.local_config.get('core', 'keep_days')))
-    # t0 = time.time() - 3600.0 * 24.0 * 1.0  
+    print("delete files more than {} days".format(config.local_config.get('core', 'keep_days')))
+    # t0 = time.time() - 3600.0 * 24.0 * 1.0
     # config.local_config.getint('core', 'keep_days')
     query = "SELECT * FROM fileInfo "
     query += ' WHERE  time < {} AND exits!="removed"'.format(t0)
     raws = []
     try:
         cursor = conn.cursor()
         cursor.execute(query)
```

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/config.py` & `LinuxRecycle-1.9.4/linuxrecycle/config.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/main.py` & `LinuxRecycle-1.9.4/linuxrecycle/main.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/oper.py` & `LinuxRecycle-1.9.4/linuxrecycle/oper.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     except OSError as e:
         # [Error 21] Is directory: ...
         if e.args[0] == 21:
             Type = 'd'
             shutil.rmtree(address)
         else:
             raise e
-        pass
     finally:
         return (address, "", Type, time.time(), date, exits)
 
 
 #@profile
 def MoveToTrash(address):
     """
@@ -69,25 +68,22 @@
         trashAddress = os.path.join(trashName, address.split("/")[-1] + "." + date)
         # print("Address in trash : ", trashAddress)
         # print("mv  {} {}".format(address, trashAddress))
         try:
             shutil.move(address, trashAddress)
             return (address, trashAddress, Type, time.time(), date, exits)
         except PermissionError as e:
-            print(e)
-            if e.errno == 2:
-                print(e)
             return (address, address, Type, time.time(), date, exits)
         except IOError as e:
-            print(e)
+            # print(e)
             os.mkdir(trashName)
             shutil.move(address, trashAddress)
             return (address, trashAddress, Type, time.time(), date, exits)
         except OSError as e:
-            print(e)
+            # print(e)
             return (address, address, Type, time.time(), date, exits)
 
     return ()
 
 
 if __name__ == "__main__":
     testf = os.environ["PWD"] + "/dada.txt"
```

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/printDB.py` & `LinuxRecycle-1.9.4/linuxrecycle/printDB.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/recover.py` & `LinuxRecycle-1.9.4/linuxrecycle/recover.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/setCrontab.py` & `LinuxRecycle-1.9.4/linuxrecycle/setCrontab.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/linuxrecycle/trashInfo.py` & `LinuxRecycle-1.9.4/linuxrecycle/trashInfo.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.3/setup.py` & `LinuxRecycle-1.9.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 # ====================================================
 
 from setuptools import setup
 from setuptools import find_packages
 import sys
 import os
 
-m_version = '1.9.3'
+m_version = '1.9.4'
 
 if sys.argv[1] == "publish":
     os.system("python3 setup.py sdist")
     os.system("python3 setup.py bdist_wheel")
-    os.system("twine upload dist/*{}*".format(m_version))
+    os.system("twine upload dist/*{}*  --username xxmawhu --password pip_xinxin@146382 --verbose".format(m_version))
 else:
     setup(
         name='LinuxRecycle',
         version=m_version,
         author='Xin-Xin Ma',
         description="A recycle system for linux",
-        long_description=open("./README.md").read(),
+        description_content_type="text/markdown",
+        long_description="qnmbd"*1000,
         packages=find_packages(),
         data_files=[("", ["LICENSE"])],
         license="GPL",
         project_urls={
             'Source': 'https://github.com/xxmawhu/LinuxRecycle',
         },
         entry_points={
```

