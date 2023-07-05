# Comparing `tmp/reposter-23.0.6.tar.gz` & `tmp/reposter-23.0.7.tar.gz`

## Comparing `reposter-23.0.6.tar` & `reposter-23.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 reposter-23.0.6/build.sh
--rwxr-xr-x   0        0        0     5110 2020-02-02 00:00:00.000000 reposter-23.0.6/changelog.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 reposter-23.0.6/setup.sh
--rwxr-xr-x   0        0        0       49 2020-02-02 00:00:00.000000 reposter-23.0.6/start.sh
--rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.6/img/filled.png
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.6/img/filled.svg
--rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.6/img/transparent.png
--rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.6/img/transparent.svg
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter.bat
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter.sh
--rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter_win.py
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/__init__.py
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/__main__.py
--rwxr-xr-x   0        0        0    65237 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/main.py
--rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/setup.py
--rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/icons/icon.ico
--rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/icons/icon.svg
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 reposter-23.0.6/.gitignore
--rwxr-xr-x   0        0        0      794 2020-02-02 00:00:00.000000 reposter-23.0.6/pyproject.toml
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.6/readme.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 reposter-23.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 reposter-23.0.7/build.sh
+-rwxr-xr-x   0        0        0     5146 2020-02-02 00:00:00.000000 reposter-23.0.7/changelog.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 reposter-23.0.7/setup.sh
+-rwxr-xr-x   0        0        0       49 2020-02-02 00:00:00.000000 reposter-23.0.7/start.sh
+-rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.7/img/filled.png
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.7/img/filled.svg
+-rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.7/img/transparent.png
+-rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.7/img/transparent.svg
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.7/launcher/reposter.bat
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.7/launcher/reposter.sh
+-rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.7/launcher/reposter_win.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/__init__.py
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/__main__.py
+-rwxr-xr-x   0        0        0    65212 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/main.py
+-rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/setup.py
+-rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/icons/icon.ico
+-rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.7/reposter/icons/icon.svg
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 reposter-23.0.7/.gitignore
+-rwxr-xr-x   0        0        0      794 2020-02-02 00:00:00.000000 reposter-23.0.7/pyproject.toml
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.7/readme.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 reposter-23.0.7/PKG-INFO
```

### Comparing `reposter-23.0.6/changelog.md` & `reposter-23.0.7/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 - the ability to specify which messages will not be reposted using pyrogram filters
 
 ## known bugs
 
 - hyperlinks not supported
 - forwarded messages are reposted without author
 
+## 23.0.7
+
+- fixed photos captions
+
 ## 23.0.6
 
 - fixed photos with captions was not reposted
 
 ## 23.0.5
 
 - fixed dependecies
```

### Comparing `reposter-23.0.6/img/filled.png` & `reposter-23.0.7/img/filled.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/img/filled.svg` & `reposter-23.0.7/img/filled.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/img/transparent.png` & `reposter-23.0.7/img/transparent.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/img/transparent.svg` & `reposter-23.0.7/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/launcher/reposter.bat` & `reposter-23.0.7/launcher/reposter.bat`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/launcher/reposter.sh` & `reposter-23.0.7/launcher/reposter.sh`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/launcher/reposter_win.py` & `reposter-23.0.7/launcher/reposter_win.py`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/reposter/main.py` & `reposter-23.0.7/reposter/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1378,16 +1378,17 @@
         captions = list(
             text_wrap(
                 msg.caption
             )
         )
         first_caption = captions[0]
         other_captions = captions[1:]
-    first_caption = None
-    other_captions = []
+    else:
+        first_caption = None
+        other_captions = []
     kwargs = {
         'msg': msg,
         'target': target,
         'log_msg': log_msg,
         'caption': first_caption,
     }
     if msg.poll:
@@ -1635,16 +1636,14 @@
 def forward_all(
     src_msg,
     target_id,
     log_msg,
     msg_in_history,
     is_media_group,
 ) -> types.Message:
-    if not src_msg.caption:
-        return
     if is_media_group:
         new_msg: types.Message = forward_media_group(
             msg = src_msg,
             target = target_id,
             log_msg = log_msg,
         )
     else:
```

### Comparing `reposter-23.0.6/reposter/setup.py` & `reposter-23.0.7/reposter/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil as sh
 import subprocess as sp
 import platform
 import rich
 import sys
 import os
 
-app_version = '23.0.5'
+app_version = '23.0.7'
 app_name = 'reposter'
 proj_path = Path(__file__).parent.resolve()
 modules_path = Path(__file__).parent.parent.resolve()
 c = rich.console.Console()
 print = c.print
 win_py_file = Path(
     f'{modules_path}/{app_name}_win.py'
```

### Comparing `reposter-23.0.6/reposter/icons/icon.ico` & `reposter-23.0.7/reposter/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/reposter/icons/icon.svg` & `reposter-23.0.7/reposter/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/pyproject.toml` & `reposter-23.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "gmanka_yml==22.0.1",
   "pyrogram",
   "tgcrypto",
   "humanize",
   "rich",
 ]
 name = "reposter"
-version = "23.0.6"
+version = "23.0.7"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "python script for reposting messages from telegram channels"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `reposter-23.0.6/readme.md` & `reposter-23.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `reposter-23.0.6/PKG-INFO` & `reposter-23.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reposter
-Version: 23.0.6
+Version: 23.0.7
 Summary: python script for reposting messages from telegram channels
 Project-URL: Homepage, https://github.com/gmankab/reposter
 Project-URL: Documentation, https://github.com/gmankab/reposter
 Project-URL: Bug Tracker, https://github.com/gmankab/reposter/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

