# Comparing `tmp/ssfMiscUtilities-0.0.2.tar.gz` & `tmp/ssfMiscUtilities-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssfMiscUtilities-0.0.2.tar", last modified: Wed Mar 15 13:42:28 2023, max compression
+gzip compressed data, was "ssfMiscUtilities-0.0.3.tar", last modified: Wed Jul  5 14:51:36 2023, max compression
```

## Comparing `ssfMiscUtilities-0.0.2.tar` & `ssfMiscUtilities-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 fragoso  (1452202861) 384566875        0 2023-03-15 13:42:28.048554 ssfMiscUtilities-0.0.2/
--rw-rw-r--   0 fragoso  (1452202861) 384566875    11337 2023-01-20 02:50:04.000000 ssfMiscUtilities-0.0.2/LICENSE
--rw-rw-r--   0 fragoso  (1452202861) 384566875      111 2023-01-20 02:50:04.000000 ssfMiscUtilities-0.0.2/MANIFEST.in
--rw-r--r--   0 fragoso  (1452202861) 384566875     1037 2023-03-15 13:42:28.048300 ssfMiscUtilities-0.0.2/PKG-INFO
--rw-r--r--   0 fragoso  (1452202861) 384566875      218 2023-03-15 13:40:03.000000 ssfMiscUtilities-0.0.2/README.md
--rw-r--r--   0 fragoso  (1452202861) 384566875      981 2023-03-15 13:41:57.000000 ssfMiscUtilities-0.0.2/settings.ini
--rw-r--r--   0 fragoso  (1452202861) 384566875       38 2023-03-15 13:42:28.048692 ssfMiscUtilities-0.0.2/setup.cfg
--rw-rw-r--   0 fragoso  (1452202861) 384566875     2560 2023-01-20 02:50:04.000000 ssfMiscUtilities-0.0.2/setup.py
-drwxr-xr-x   0 fragoso  (1452202861) 384566875        0 2023-03-15 13:42:28.045071 ssfMiscUtilities-0.0.2/ssfMiscUtilities/
--rw-r--r--   0 fragoso  (1452202861) 384566875       22 2023-03-15 13:42:17.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities/__init__.py
--rw-r--r--   0 fragoso  (1452202861) 384566875     4363 2023-03-15 13:42:17.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities/_modidx.py
--rw-r--r--   0 fragoso  (1452202861) 384566875      142 2023-03-15 13:34:07.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities/core.py
--rw-r--r--   0 fragoso  (1452202861) 384566875     1951 2023-03-15 13:42:17.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities/generic.py
--rw-r--r--   0 fragoso  (1452202861) 384566875     9281 2023-03-15 13:42:17.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities/lsf_interactive.py
-drwxr-xr-x   0 fragoso  (1452202861) 384566875        0 2023-03-15 13:42:28.047787 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/
--rw-r--r--   0 fragoso  (1452202861) 384566875     1037 2023-03-15 13:42:27.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/PKG-INFO
--rw-r--r--   0 fragoso  (1452202861) 384566875      478 2023-03-15 13:42:28.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 fragoso  (1452202861) 384566875        1 2023-03-15 13:42:27.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 fragoso  (1452202861) 384566875       54 2023-03-15 13:42:27.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/entry_points.txt
--rw-r--r--   0 fragoso  (1452202861) 384566875        1 2023-03-15 13:37:01.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/not-zip-safe
--rw-r--r--   0 fragoso  (1452202861) 384566875        7 2023-03-15 13:42:27.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/requires.txt
--rw-r--r--   0 fragoso  (1452202861) 384566875       17 2023-03-15 13:42:27.000000 ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/top_level.txt
+drwxr-sr-x   0 fragoso   (8659) metagen   (1225)        0 2023-07-05 14:51:36.509275 ssfMiscUtilities-0.0.3/
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)    11337 2023-03-15 13:45:02.000000 ssfMiscUtilities-0.0.3/LICENSE
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)      111 2023-03-15 13:45:02.000000 ssfMiscUtilities-0.0.3/MANIFEST.in
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     1017 2023-07-05 14:51:36.507115 ssfMiscUtilities-0.0.3/PKG-INFO
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)      218 2023-03-15 13:45:02.000000 ssfMiscUtilities-0.0.3/README.md
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)      981 2023-07-05 14:50:40.000000 ssfMiscUtilities-0.0.3/settings.ini
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)       38 2023-07-05 14:51:36.511347 ssfMiscUtilities-0.0.3/setup.cfg
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     2560 2023-03-15 13:45:02.000000 ssfMiscUtilities-0.0.3/setup.py
+drwxr-sr-x   0 fragoso   (8659) metagen   (1225)        0 2023-07-05 14:51:36.456730 ssfMiscUtilities-0.0.3/ssfMiscUtilities/
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)       22 2023-07-05 14:50:49.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities/__init__.py
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     4363 2023-07-05 14:50:49.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities/_modidx.py
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)      142 2023-03-15 13:45:02.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities/core.py
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     1930 2023-07-05 14:50:49.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities/generic.py
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     9281 2023-07-05 14:50:49.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities/lsf_interactive.py
+drwxr-sr-x   0 fragoso   (8659) metagen   (1225)        0 2023-07-05 14:51:36.499929 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)     1017 2023-07-05 14:51:35.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)      478 2023-07-05 14:51:36.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)        1 2023-07-05 14:51:35.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)       54 2023-07-05 14:51:35.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/entry_points.txt
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)        1 2023-03-15 13:46:16.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/not-zip-safe
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)        7 2023-07-05 14:51:35.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/requires.txt
+-rw-r--r--   0 fragoso   (8659) metagen   (1225)       17 2023-07-05 14:51:35.000000 ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/top_level.txt
```

### Comparing `ssfMiscUtilities-0.0.2/LICENSE` & `ssfMiscUtilities-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssfMiscUtilities-0.0.2/PKG-INFO` & `ssfMiscUtilities-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ssfMiscUtilities
-Version: 0.0.2
+Version: 0.0.3
 Summary: ssf miscellaneous utils
 Home-page: https://github.com/SantiagoSanchezF/ssfMiscUtilities
 Author: Santiago Sanchez
 Author-email: santiago.s.fragoso@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,9 +32,7 @@
 ``` sh
 pip install ssfMiscUtilities
 ```
 
 ## How to use
 
 find specific usage in notebooks of github repo
-
-
```

### Comparing `ssfMiscUtilities-0.0.2/settings.ini` & `ssfMiscUtilities-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ssfMiscUtilities
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ssfMiscUtilities
```

### Comparing `ssfMiscUtilities-0.0.2/setup.py` & `ssfMiscUtilities-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ssfMiscUtilities-0.0.2/ssfMiscUtilities/_modidx.py` & `ssfMiscUtilities-0.0.3/ssfMiscUtilities/_modidx.py`

 * *Files identical despite different names*

### Comparing `ssfMiscUtilities-0.0.2/ssfMiscUtilities/generic.py` & `ssfMiscUtilities-0.0.3/ssfMiscUtilities/generic.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,20 +39,19 @@
                     var, 
                     str(hard),
                     # str(hard) if type(hard)!=str else f"'{hard}'",
                     line)
             h.write(line)
 
 # %% ../nbs/generic.ipynb 15
-def split_list(li:list,chunks:int):
+def split_list(lst:list,n:int):
     "split a list into N chunks"
-    le = int(len(li)/(chunks-1))
-    res = [li[(i*le):(i+1)*le] for i in range(chunks)]
-    if res[-1] == []: res.pop()
-    return res
+    k, m = divmod(len(lst), n)
+    return list(lst[i * k + min(i, m):(i + 1) * k + min(i + 1, m)] for i in range(n))
+
 
 # %% ../nbs/generic.ipynb 16
 def lmap(func,li:list):
     "map a list with funtion"
     return list(map(func,li))
 
 # %% ../nbs/generic.ipynb 17
```

### Comparing `ssfMiscUtilities-0.0.2/ssfMiscUtilities/lsf_interactive.py` & `ssfMiscUtilities-0.0.3/ssfMiscUtilities/lsf_interactive.py`

 * *Files identical despite different names*

### Comparing `ssfMiscUtilities-0.0.2/ssfMiscUtilities.egg-info/PKG-INFO` & `ssfMiscUtilities-0.0.3/ssfMiscUtilities.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ssfMiscUtilities
-Version: 0.0.2
+Version: 0.0.3
 Summary: ssf miscellaneous utils
 Home-page: https://github.com/SantiagoSanchezF/ssfMiscUtilities
 Author: Santiago Sanchez
 Author-email: santiago.s.fragoso@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,9 +32,7 @@
 ``` sh
 pip install ssfMiscUtilities
 ```
 
 ## How to use
 
 find specific usage in notebooks of github repo
-
-
```

