# Comparing `tmp/nonebot_plugin_update-0.1.1.tar.gz` & `tmp/nonebot_plugin_update-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_update-0.1.1.tar", last modified: Wed Jul  5 13:16:38 2023, max compression
+gzip compressed data, was "nonebot_plugin_update-0.1.2.tar", last modified: Wed Jul  5 13:24:18 2023, max compression
```

## Comparing `nonebot_plugin_update-0.1.1.tar` & `nonebot_plugin_update-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-07-05 12:55:17.428356 nonebot_plugin_update-0.1.1/LICENSE
--rw-r--r--   0        0        0     2759 2023-07-05 12:55:17.428356 nonebot_plugin_update-0.1.1/README.md
--rw-r--r--   0        0        0     1075 2023-07-05 12:50:20.671660 nonebot_plugin_update-0.1.1/nonebot_plugin_update/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-05 13:06:08.412550 nonebot_plugin_update-0.1.1/nonebot_plugin_update/check.py
--rw-r--r--   0        0        0      216 2023-07-05 11:16:41.744356 nonebot_plugin_update-0.1.1/nonebot_plugin_update/config.py
--rw-r--r--   0        0        0      499 2023-07-05 12:41:02.472912 nonebot_plugin_update-0.1.1/nonebot_plugin_update/model.py
--rw-r--r--   0        0        0       92 2023-07-05 13:04:48.840875 nonebot_plugin_update-0.1.1/nonebot_plugin_update/version.py
--rw-r--r--   0        0        0      700 2023-07-05 13:16:38.882572 nonebot_plugin_update-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 nonebot_plugin_update-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-05 12:55:17.428356 nonebot_plugin_update-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2759 2023-07-05 12:55:17.428356 nonebot_plugin_update-0.1.2/README.md
+-rw-r--r--   0        0        0     1112 2023-07-05 13:22:37.125694 nonebot_plugin_update-0.1.2/nonebot_plugin_update/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-05 13:06:08.412550 nonebot_plugin_update-0.1.2/nonebot_plugin_update/check.py
+-rw-r--r--   0        0        0      216 2023-07-05 11:16:41.744356 nonebot_plugin_update-0.1.2/nonebot_plugin_update/config.py
+-rw-r--r--   0        0        0      499 2023-07-05 12:41:02.472912 nonebot_plugin_update-0.1.2/nonebot_plugin_update/model.py
+-rw-r--r--   0        0        0       92 2023-07-05 13:22:45.897673 nonebot_plugin_update-0.1.2/nonebot_plugin_update/version.py
+-rw-r--r--   0        0        0      700 2023-07-05 13:24:18.709459 nonebot_plugin_update-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 nonebot_plugin_update-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_update-0.1.1/LICENSE` & `nonebot_plugin_update-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_update-0.1.1/README.md` & `nonebot_plugin_update-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_update-0.1.1/nonebot_plugin_update/__init__.py` & `nonebot_plugin_update-0.1.2/nonebot_plugin_update/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata, require
 
 from .check import check_update
 from .version import __version__
 
 require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_localstore")
 
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-update",
     description="用于检测 Nonebot 插件更新的 Nonebot 插件",
     usage="发送 /npu help 查看帮助",
     homepage="https://github.com/Aunly/nonebot-plugin-update",
```

### Comparing `nonebot_plugin_update-0.1.1/nonebot_plugin_update/check.py` & `nonebot_plugin_update-0.1.2/nonebot_plugin_update/check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_update-0.1.1/pyproject.toml` & `nonebot_plugin_update-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "nonebot-plugin-localstore>=0.5.0",
     "packaging>=23.1",
     "nonebot-plugin-apscheduler>=0.3.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.1"
+version = "0.1.2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `nonebot_plugin_update-0.1.1/PKG-INFO` & `nonebot_plugin_update-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-update
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用于检测 Nonebot 插件更新的 Nonebot 插件
 Author-Email: djkcyl <cyl@cyllive.cn>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2[fastapi,httpx]>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.3
 Requires-Dist: nonebot-plugin-localstore>=0.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-update Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-update Version: 0.1.2 Summary:
 ç¨äºæ£æµ Nonebot æä»¶æ´æ°ç Nonebot æä»¶ Author-Email: djkcyl
 cyllive.cn> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2
 [fastapi,httpx]>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.3 Requires-
 Dist: nonebot-plugin-localstore>=0.5.0 Requires-Dist: packaging>=23.1 Requires-
 Dist: nonebot-plugin-apscheduler>=0.3.0 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

