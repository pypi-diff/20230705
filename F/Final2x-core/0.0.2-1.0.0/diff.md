# Comparing `tmp/Final2x-core-0.0.2.tar.gz` & `tmp/Final2x-core-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Final2x-core-0.0.2.tar", last modified: Thu Jun 29 16:21:52 2023, max compression
+gzip compressed data, was "Final2x-core-1.0.0.tar", last modified: Wed Jul  5 07:50:00 2023, max compression
```

## Comparing `Final2x-core-0.0.2.tar` & `Final2x-core-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.070593 Final2x-core-0.0.2/Final2x_core/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-29 16:21:23.000000 Final2x-core-0.0.2/Final2x_core/Final2x-core-pip.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2515 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/Final2x_core/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/Final2x_core/src/SRFactory/
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/REALCUGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/REALESRGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRBaseClass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRMD.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/WAIFU2X.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRFactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/Final2x_core/src/SRncnn/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRncnn/SRMDncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/SRqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/Final2x_core/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4832 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/utils/getConfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/utils/progressLog.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-06-29 16:21:50.000000 Final2x-core-0.0.2/Final2x_core/src/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/Final2x_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-29 16:21:52.000000 Final2x-core-0.0.2/Final2x_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-29 16:21:23.000000 Final2x-core-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-29 16:21:23.000000 Final2x-core-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-06-29 16:21:23.000000 Final2x-core-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 16:21:52.074594 Final2x-core-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-06-29 16:21:24.000000 Final2x-core-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.783943 Final2x-core-1.0.0/Final2x_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/Final2x_core/Final2x-core-pip.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/SRFactory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALCUGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALESRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRMD.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/WAIFU2X.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRFactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/SRncnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALCUGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALESRGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/SRMDncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/SRqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/Final2x_core/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/getConfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/progressLog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-05 07:49:59.000000 Final2x-core-1.0.0/Final2x_core/src/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 07:50:00.783943 Final2x-core-1.0.0/Final2x_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7099 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-05 07:50:00.000000 Final2x-core-1.0.0/Final2x_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7099 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-05 07:49:29.000000 Final2x-core-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 07:50:00.787943 Final2x-core-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-05 07:49:30.000000 Final2x-core-1.0.0/setup.py
```

### Comparing `Final2x-core-0.0.2/Final2x_core/__main__.py` & `Final2x-core-1.0.0/Final2x_core/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 else:
     # unfrozen
     projectPATH = Path(__file__).resolve().parent.absolute()
 
 # parse args
 parser = argparse.ArgumentParser()
 parser.description = "when para is not specified, the config.yaml file in the directory will be read automatically"
+parser.add_argument("-b", "--BASE64", help="base64 string for config json", type=str)
 parser.add_argument("-j", "--JSON", help="JSON string for config", type=str)
 parser.add_argument("-y", "--YAML", help="yaml config file path", type=str)
 parser.add_argument("-o", "--OP", help="check install", action="store_true")
 args = parser.parse_args()
 
 if args.OP:
     print("114514")
@@ -53,26 +54,30 @@
 
 def main():
     logger.add(projectPATH / "logs" / "log-{time}.log", encoding="utf-8", retention="60 days")
     logger.info("projectPATH: " + str(projectPATH))
 
     # load config
     config = SRCONFIG()
-    if args.JSON is not None:
+    if args.BASE64 is not None:
+        config.getConfigfromBase64toJson(str(args.BASE64), str(projectPATH / "models"))
+    elif args.JSON is not None:
         config.getConfigfromJson(str(args.JSON), str(projectPATH / "models"))
     elif args.YAML is not None:
         config.getConfigfromYaml(str(args.YAML), str(projectPATH / "models"))
     else:
         config.getConfigfromYaml(str(projectPATH / "config.yaml"), str(projectPATH / "models"))
 
     logger.info("config loaded")
+
+    # 还是不加比较好
     # use cpu if gpu is not available
-    if not cv2.ocl.haveOpenCL() and config.gpuid != -1:
-        logger.warning("gpu is not available, use cpu instead")
-        config.gpuid = -1
+    # if not cv2.ocl.haveOpenCL() and config.gpuid != -1:
+    #     logger.warning("gpu is not available, use cpu instead")
+    #     config.gpuid = -1
 
     SR_queue()
 
     logger.success("______SR_COMPLETED______")
 
     OP = Path(config.outputpath) / "outputs"
     open_folder(str(OP))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Final2x-core-0.0.2/Final2x_core/config.yaml` & `Final2x-core-1.0.0/Final2x_core/config.yaml`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/REALCUGAN.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALCUGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/REALESRGAN.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/REALESRGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRBaseClass.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRBaseClass.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRFactory.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRFactory.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/SRMD.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/SRMD.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/WAIFU2X.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/WAIFU2X.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRFactory/__init__.py` & `Final2x-core-1.0.0/Final2x_core/src/SRFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py` & `Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALCUGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py` & `Final2x-core-1.0.0/Final2x_core/src/SRncnn/REALESRGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRncnn/SRMDncnn.py` & `Final2x-core-1.0.0/Final2x_core/src/SRncnn/SRMDncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py` & `Final2x-core-1.0.0/Final2x_core/src/SRncnn/WAIFU2Xncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/SRqueue.py` & `Final2x-core-1.0.0/Final2x_core/src/SRqueue.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core/src/utils/getConfig.py` & `Final2x-core-1.0.0/Final2x_core/src/utils/getConfig.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import base64
 from pathlib import Path
 from typing import Union
 
 import yaml
 from loguru import logger
 
 try:
@@ -36,15 +37,30 @@
     def getConfigfromJson(self, config: str = "", modelpath: str = "") -> None:
         """
         get config from json string
         :param config: a json string
         :param modelpath: path to model folder
         :return:
         """
-        self._modelpath: str = modelpath
+        self._modelpath = modelpath
+        config = json.loads(config)
+        self._setConfig(config)
+
+    @logger.catch(reraise=True)
+    def getConfigfromBase64toJson(self, config: str = "", modelpath: str = "") -> None:
+        """
+        get config from base64 string
+        :param config: a base64 string
+        :param modelpath: path to model folder
+        :return:
+        """
+        self._modelpath = modelpath
+
+        config = config.encode('utf-8')
+        config = base64.b64decode(config).decode("utf-8")
         config = json.loads(config)
         self._setConfig(config)
 
     @logger.catch(reraise=True)
     def _setConfig(self, config: dict) -> None:
         self.outputpath = config["outputpath"]
         self.gpuid = config["gpuid"]
```

### Comparing `Final2x-core-0.0.2/Final2x_core/src/utils/progressLog.py` & `Final2x-core-1.0.0/Final2x_core/src/utils/progressLog.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/Final2x_core.egg-info/PKG-INFO` & `Final2x-core-1.0.0/Final2x_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 0.0.2
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,152 +28,166 @@
 <h1 align="center"> Final2x-core </h1>
 
 ![MacOS x64](https://img.shields.io/badge/Support-MacOS%20x64-blue?logo=Apple&style=flat-square)
 ![MacOS arm64](https://img.shields.io/badge/Support-MacOS%20arm64-blue?logo=Apple&style=flat-square)
 ![Windows x64](https://img.shields.io/badge/Support-Windows%20x64-blue?logo=Windows&style=flat-square)
 ![Windows arm64](https://img.shields.io/badge/Support-Windows%20arm64-blue?logo=Windows&style=flat-square)
 ![Linux x64](https://img.shields.io/badge/Support-Linux%20x64-blue?logo=Linux&style=flat-square)
-[![codecov](https://codecov.io/gh/Tohrusky/Final2x-core/branch/main/graph/badge.svg?token=B2TNKYN4O4)](https://codecov.io/gh/Tohrusky/Final2x-core) 
-[![CI-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml) 
+[![codecov](https://codecov.io/gh/Tohrusky/Final2x-core/branch/main/graph/badge.svg?token=B2TNKYN4O4)](https://codecov.io/gh/Tohrusky/Final2x-core)
+[![CI-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml)
 [![CI-build](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 [![Release](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml)
+[![PIP-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml)
+[![Release-pypi](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/Final2x-core.svg)](https://badge.fury.io/py/Final2x-core)
 ![GitHub](https://img.shields.io/github/license/Tohrusky/Final2x-core)
 
+Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x).
 
-Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x). 
+# Install
+
+Download in [Release](https://github.com/Tohrusky/Final2x-core/releases) or use pip (python >= 3.6, >=3.9 for MacOS
+arm64)
+
+```shell
+pip install Final2x-core
+```
 
 # Use
 
 ```shell
-usage: Final2x-core [-h] [-j JSON]
+usage: Final2x-core [-h] [-b BASE64] [-j JSON] [-y YAML] [-o]
 
-when -j is not specified, the config.yaml file in the directory will be read automatically
+when para is not specified, the config.yaml file in the directory will be read automatically
 
 optional arguments:
   -h, --help            show this help message and exit
-  -j JSON, --JSON JSON  JSON str for config
-
+  -b BASE64, --BASE64 BASE64
+                        base64 string for config json
+  -j JSON, --JSON JSON  JSON string for config
+  -y YAML, --YAML YAML  yaml config file path
+  -o, --OP              check install
 ```
 
 # Config
 
 Pass the config json string to the program through the `-j` parameter.
 
 **PLEASE NOTE: the config is JSON, remove the // comments before use.**
 
-```
+```json
 {
-  "gpuid": 0, // GPU id, >= -1 (-1 for CPU, may not work for some models.)
+  "gpuid": 0,
+  // GPU id, >= -1 (-1 for CPU, may not work for some models.)
   "inputpath": [
     // Input image paths, should be a list.
-    "path/to/img1.jpg", 
+    "path/to/img1.jpg",
     "path/to/img2.png"
   ],
-  "model": "RealCUGAN-pro", // model name
-  "modelscale": 2, // model upscale factor
-  "modelnoise": -1, // DENOISE level
-  "outputpath": "path/to/output", // output path
-  "targetscale": 2.0, 
+  "model": "RealCUGAN-pro",
+  // model name
+  "modelscale": 2,
+  // model upscale factor
+  "modelnoise": -1,
+  // DENOISE level
+  "outputpath": "path/to/output",
+  // output path
+  "targetscale": 2.0,
   // Target upscale factor, upscale multiple times to achieve the target upscale factor.
   // If not invalid, use modelscale.
-  "tta": false // Test Time Augmentation, default false
+  "tta": false
+  // Test Time Augmentation, default false
 }
 ```
 
 **SUPPORTED MODEL LIST:**
 
+```yaml
 - RealCUGAN-se:
     - model: "RealCUGAN-se"
     - scale: 2
-        - noise: -1, 0, 1, 2, 3
+               - noise: -1, 0, 1, 2, 3
     - scale: 3, 4
-        - noise: -1, 0, 3
+               - noise: -1, 0, 3
 
 - RealCUGAN-pro:
     - model: "RealCUGAN-pro"
     - scale: 2, 3
     - noise: -1, 0, 3
 
 - RealESRGAN-animevideov3:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN-animevideov3"
     - scale: 2, 3, 4
 
 - RealESRGAN:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN"
     - scale: 4
 
 - RealESRGAN-anime:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN-anime"
     - scale: 4
 
 - Waifu2x-cunet:
     - model: "Waifu2x-cunet"
     - scale: 1
-        - noise: 0, 1, 2, 3
+               - noise: 0, 1, 2, 3
     - scale: 2
-        - noise: -1, 0, 1, 2, 3
+               - noise: -1, 0, 1, 2, 3
 
 - Waifu2x-upconv_7_anime_style_art_rgb:
     - model: "Waifu2x-upconv_7_anime_style_art_rgb"
     - scale: 2
     - noise: -1, 0, 1, 2, 3
 
 - Waifu2x-upconv_7_photo:
     - model: "Waifu2x-upconv_7_photo"
     - scale: 2
     - noise: -1, 0, 1, 2, 3
 
 - SRMD:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "SRMD"
     - scale: 2, 3, 4
     - noise: -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
+```
 
 # Build
 
 [Github Action](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 
 *The project just only been tested in Ubuntu 18+ and Debian 9+ environments on Linux, so if the project does not work on
 your system, please try building it.*
 
 # Reference
 
 The following references were used in the development of this project:
 
-[ncnn](https://github.com/Tencent/ncnn) - ncnn is a high-performance neural network inference framework developed by
-Tencent AI Lab.
-
-[nihui/realcugan-ncnn-vulkan](https://github.com/nihui/realcugan-ncnn-vulkan) - This project provided the core
-implementation of the Real-CUGAN algorithm using the ncnn and Vulkan libraries.
-
-[xinntao/Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) - This project provided the core
-implementation of the Real-ESRGAN algorithm using the ncnn and Vulkan
-libraries.
-
-[nihui/waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) - This project provided the core
-implementation of the Waifu2x algorithm using the ncnn and Vulkan libraries.
-
-[nihui/srmd-ncnn-vulkan](https://github.com/nihui/srmd-ncnn-vulkan) - This project provided the core implementation of
-the SRMD algorithm using the ncnn and Vulkan libraries.
-
-[realcugan-ncnn-py](https://github.com/Tohrusky/realcugan-ncnn-py) - This project provided the Python Binding for
-realcugan-ncnn-vulkan with PyBind11
-
-[realesrgan-ncnn-py](https://github.com/Tohrusky/realesrgan-ncnn-py) - This project provided the Python Binding for
-realesrgan-ncnn-vulkan with PyBind11
-
-[waifu2x-ncnn-py](https://github.com/Tohrusky/waifu2x-ncnn-py) - This project provided the Python Binding for
-waifu2x-ncnn-vulkan with PyBind11
-
-[srmd-ncnn-py](https://github.com/Tohrusky/srmd-ncnn-py) - This project provided the Python Binding for srmd-ncnn-vulkan
-with PyBind11
+- [ncnn](https://github.com/Tencent/ncnn) - ncnn is a high-performance neural network inference framework developed by
+  Tencent AI Lab.
+- [nihui/realcugan-ncnn-vulkan](https://github.com/nihui/realcugan-ncnn-vulkan) - This project provided the core
+  implementation of the Real-CUGAN algorithm using the ncnn and Vulkan libraries.
+- [xinntao/Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) - This project provided the core
+  implementation of the Real-ESRGAN algorithm using the ncnn and Vulkan
+  libraries.
+- [nihui/waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) - This project provided the core
+  implementation of the Waifu2x algorithm using the ncnn and Vulkan libraries.
+- [nihui/srmd-ncnn-vulkan](https://github.com/nihui/srmd-ncnn-vulkan) - This project provided the core implementation of
+  the SRMD algorithm using the ncnn and Vulkan libraries.
+- [realcugan-ncnn-py](https://github.com/Tohrusky/realcugan-ncnn-py) - This project provided the Python Binding for
+  realcugan-ncnn-vulkan with PyBind11
+- [realesrgan-ncnn-py](https://github.com/Tohrusky/realesrgan-ncnn-py) - This project provided the Python Binding for
+  realesrgan-ncnn-vulkan with PyBind11
+- [waifu2x-ncnn-py](https://github.com/Tohrusky/waifu2x-ncnn-py) - This project provided the Python Binding for
+  waifu2x-ncnn-vulkan with PyBind11
+- [srmd-ncnn-py](https://github.com/Tohrusky/srmd-ncnn-py) - This project provided the Python Binding for
+  srmd-ncnn-vulkan
+  with PyBind11
 
 # License
 
 This project is licensed under the BSD 3-Clause - see
 the [LICENSE file](https://github.com/Tohrusky/Final2x-core/blob/main/LICENSE) for details.
```

### Comparing `Final2x-core-0.0.2/Final2x_core.egg-info/SOURCES.txt` & `Final2x-core-1.0.0/Final2x_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/LICENSE` & `Final2x-core-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Final2x-core-0.0.2/PKG-INFO` & `Final2x-core-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 0.0.2
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,152 +28,166 @@
 <h1 align="center"> Final2x-core </h1>
 
 ![MacOS x64](https://img.shields.io/badge/Support-MacOS%20x64-blue?logo=Apple&style=flat-square)
 ![MacOS arm64](https://img.shields.io/badge/Support-MacOS%20arm64-blue?logo=Apple&style=flat-square)
 ![Windows x64](https://img.shields.io/badge/Support-Windows%20x64-blue?logo=Windows&style=flat-square)
 ![Windows arm64](https://img.shields.io/badge/Support-Windows%20arm64-blue?logo=Windows&style=flat-square)
 ![Linux x64](https://img.shields.io/badge/Support-Linux%20x64-blue?logo=Linux&style=flat-square)
-[![codecov](https://codecov.io/gh/Tohrusky/Final2x-core/branch/main/graph/badge.svg?token=B2TNKYN4O4)](https://codecov.io/gh/Tohrusky/Final2x-core) 
-[![CI-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml) 
+[![codecov](https://codecov.io/gh/Tohrusky/Final2x-core/branch/main/graph/badge.svg?token=B2TNKYN4O4)](https://codecov.io/gh/Tohrusky/Final2x-core)
+[![CI-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-test.yml)
 [![CI-build](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 [![Release](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release.yml)
+[![PIP-test](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/PIP-test.yml)
+[![Release-pypi](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml/badge.svg)](https://github.com/Tohrusky/Final2x-core/actions/workflows/Release-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/Final2x-core.svg)](https://badge.fury.io/py/Final2x-core)
 ![GitHub](https://img.shields.io/github/license/Tohrusky/Final2x-core)
 
+Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x).
 
-Final2x-core is a cross-platform image super-resolution CLI tool for [Final2x](https://github.com/Tohrusky/Final2x). 
+# Install
+
+Download in [Release](https://github.com/Tohrusky/Final2x-core/releases) or use pip (python >= 3.6, >=3.9 for MacOS
+arm64)
+
+```shell
+pip install Final2x-core
+```
 
 # Use
 
 ```shell
-usage: Final2x-core [-h] [-j JSON]
+usage: Final2x-core [-h] [-b BASE64] [-j JSON] [-y YAML] [-o]
 
-when -j is not specified, the config.yaml file in the directory will be read automatically
+when para is not specified, the config.yaml file in the directory will be read automatically
 
 optional arguments:
   -h, --help            show this help message and exit
-  -j JSON, --JSON JSON  JSON str for config
-
+  -b BASE64, --BASE64 BASE64
+                        base64 string for config json
+  -j JSON, --JSON JSON  JSON string for config
+  -y YAML, --YAML YAML  yaml config file path
+  -o, --OP              check install
 ```
 
 # Config
 
 Pass the config json string to the program through the `-j` parameter.
 
 **PLEASE NOTE: the config is JSON, remove the // comments before use.**
 
-```
+```json
 {
-  "gpuid": 0, // GPU id, >= -1 (-1 for CPU, may not work for some models.)
+  "gpuid": 0,
+  // GPU id, >= -1 (-1 for CPU, may not work for some models.)
   "inputpath": [
     // Input image paths, should be a list.
-    "path/to/img1.jpg", 
+    "path/to/img1.jpg",
     "path/to/img2.png"
   ],
-  "model": "RealCUGAN-pro", // model name
-  "modelscale": 2, // model upscale factor
-  "modelnoise": -1, // DENOISE level
-  "outputpath": "path/to/output", // output path
-  "targetscale": 2.0, 
+  "model": "RealCUGAN-pro",
+  // model name
+  "modelscale": 2,
+  // model upscale factor
+  "modelnoise": -1,
+  // DENOISE level
+  "outputpath": "path/to/output",
+  // output path
+  "targetscale": 2.0,
   // Target upscale factor, upscale multiple times to achieve the target upscale factor.
   // If not invalid, use modelscale.
-  "tta": false // Test Time Augmentation, default false
+  "tta": false
+  // Test Time Augmentation, default false
 }
 ```
 
 **SUPPORTED MODEL LIST:**
 
+```yaml
 - RealCUGAN-se:
     - model: "RealCUGAN-se"
     - scale: 2
-        - noise: -1, 0, 1, 2, 3
+               - noise: -1, 0, 1, 2, 3
     - scale: 3, 4
-        - noise: -1, 0, 3
+               - noise: -1, 0, 3
 
 - RealCUGAN-pro:
     - model: "RealCUGAN-pro"
     - scale: 2, 3
     - noise: -1, 0, 3
 
 - RealESRGAN-animevideov3:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN-animevideov3"
     - scale: 2, 3, 4
 
 - RealESRGAN:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN"
     - scale: 4
 
 - RealESRGAN-anime:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "RealESRGAN-anime"
     - scale: 4
 
 - Waifu2x-cunet:
     - model: "Waifu2x-cunet"
     - scale: 1
-        - noise: 0, 1, 2, 3
+               - noise: 0, 1, 2, 3
     - scale: 2
-        - noise: -1, 0, 1, 2, 3
+               - noise: -1, 0, 1, 2, 3
 
 - Waifu2x-upconv_7_anime_style_art_rgb:
     - model: "Waifu2x-upconv_7_anime_style_art_rgb"
     - scale: 2
     - noise: -1, 0, 1, 2, 3
 
 - Waifu2x-upconv_7_photo:
     - model: "Waifu2x-upconv_7_photo"
     - scale: 2
     - noise: -1, 0, 1, 2, 3
 
 - SRMD:
-    - gpuid : >= 0
+    - gpuid: >= 0
     - model: "SRMD"
     - scale: 2, 3, 4
     - noise: -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
+```
 
 # Build
 
 [Github Action](https://github.com/Tohrusky/Final2x-core/actions/workflows/CI-build.yml)
 
 *The project just only been tested in Ubuntu 18+ and Debian 9+ environments on Linux, so if the project does not work on
 your system, please try building it.*
 
 # Reference
 
 The following references were used in the development of this project:
 
-[ncnn](https://github.com/Tencent/ncnn) - ncnn is a high-performance neural network inference framework developed by
-Tencent AI Lab.
-
-[nihui/realcugan-ncnn-vulkan](https://github.com/nihui/realcugan-ncnn-vulkan) - This project provided the core
-implementation of the Real-CUGAN algorithm using the ncnn and Vulkan libraries.
-
-[xinntao/Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) - This project provided the core
-implementation of the Real-ESRGAN algorithm using the ncnn and Vulkan
-libraries.
-
-[nihui/waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) - This project provided the core
-implementation of the Waifu2x algorithm using the ncnn and Vulkan libraries.
-
-[nihui/srmd-ncnn-vulkan](https://github.com/nihui/srmd-ncnn-vulkan) - This project provided the core implementation of
-the SRMD algorithm using the ncnn and Vulkan libraries.
-
-[realcugan-ncnn-py](https://github.com/Tohrusky/realcugan-ncnn-py) - This project provided the Python Binding for
-realcugan-ncnn-vulkan with PyBind11
-
-[realesrgan-ncnn-py](https://github.com/Tohrusky/realesrgan-ncnn-py) - This project provided the Python Binding for
-realesrgan-ncnn-vulkan with PyBind11
-
-[waifu2x-ncnn-py](https://github.com/Tohrusky/waifu2x-ncnn-py) - This project provided the Python Binding for
-waifu2x-ncnn-vulkan with PyBind11
-
-[srmd-ncnn-py](https://github.com/Tohrusky/srmd-ncnn-py) - This project provided the Python Binding for srmd-ncnn-vulkan
-with PyBind11
+- [ncnn](https://github.com/Tencent/ncnn) - ncnn is a high-performance neural network inference framework developed by
+  Tencent AI Lab.
+- [nihui/realcugan-ncnn-vulkan](https://github.com/nihui/realcugan-ncnn-vulkan) - This project provided the core
+  implementation of the Real-CUGAN algorithm using the ncnn and Vulkan libraries.
+- [xinntao/Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) - This project provided the core
+  implementation of the Real-ESRGAN algorithm using the ncnn and Vulkan
+  libraries.
+- [nihui/waifu2x-ncnn-vulkan](https://github.com/nihui/waifu2x-ncnn-vulkan) - This project provided the core
+  implementation of the Waifu2x algorithm using the ncnn and Vulkan libraries.
+- [nihui/srmd-ncnn-vulkan](https://github.com/nihui/srmd-ncnn-vulkan) - This project provided the core implementation of
+  the SRMD algorithm using the ncnn and Vulkan libraries.
+- [realcugan-ncnn-py](https://github.com/Tohrusky/realcugan-ncnn-py) - This project provided the Python Binding for
+  realcugan-ncnn-vulkan with PyBind11
+- [realesrgan-ncnn-py](https://github.com/Tohrusky/realesrgan-ncnn-py) - This project provided the Python Binding for
+  realesrgan-ncnn-vulkan with PyBind11
+- [waifu2x-ncnn-py](https://github.com/Tohrusky/waifu2x-ncnn-py) - This project provided the Python Binding for
+  waifu2x-ncnn-vulkan with PyBind11
+- [srmd-ncnn-py](https://github.com/Tohrusky/srmd-ncnn-py) - This project provided the Python Binding for
+  srmd-ncnn-vulkan
+  with PyBind11
 
 # License
 
 This project is licensed under the BSD 3-Clause - see
 the [LICENSE file](https://github.com/Tohrusky/Final2x-core/blob/main/LICENSE) for details.
```

### Comparing `Final2x-core-0.0.2/setup.py` & `Final2x-core-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-_version: str = "0.0.2"
+_version: str = "1.0.0"
 
 
 def My_find_packages(*tops):
     packages = []
     for d in tops:
         for root, dirs, files in os.walk(d, followlinks=True):
             packages.append(root)
@@ -42,12 +42,12 @@
     },
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=['numpy',
                       'opencv-python',
                       'PyYAML',
                       'loguru',
-                      'realcugan_ncnn_py',
-                      'realesrgan_ncnn_py',
-                      'waifu2x_ncnn_py',
-                      'srmd_ncnn_py']
+                      'realcugan_ncnn_py >= 1.3.0',
+                      'realesrgan_ncnn_py >= 1.3.0',
+                      'waifu2x_ncnn_py >= 1.3.0',
+                      'srmd_ncnn_py >= 1.3.0']
 )
```

