# Comparing `tmp/rcsb.utils.targets-0.72.tar.gz` & `tmp/rcsb.utils.targets-0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.72.tar", last modified: Tue Jun 13 13:17:42 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.73.tar", last modified: Wed Jul  5 13:34:44 2023, max compression
```

## Comparing `rcsb.utils.targets-0.72.tar` & `rcsb.utils.targets-0.73.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/
--rw-r--r--   0 vsts      (1001) docker     (122)     6083 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9534 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:05:54.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-06-13 13:04:47.000000 rcsb.utils.targets-0.72/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-06-13 13:17:42.641846 rcsb.utils.targets-0.72/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-06-13 13:04:47.000000 rcsb.utils.targets-0.72/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.859373 rcsb.utils.targets-0.73/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.863374 rcsb.utils.targets-0.73/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9534 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9506 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20796 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.863374 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-05 13:21:55.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/setup.py
```

### Comparing `rcsb.utils.targets-0.72/HISTORY.txt` & `rcsb.utils.targets-0.73/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,9 @@
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
    2-May-2023  - V0.69 Remove depth field from CARD lineage tree
    5-May-2023  - V0.70 Actually check cache files exist in PharosTargetProvider testCache()
   22-May-2023  - V0.71 Add retries to tox task for MMseqs2 download
-  13-Jun-2023  - V0.72 Improve logging
+  13-Jun-2023  - V0.72 Improve logging
+   3-Jul-2023  - V0.73 imgt.org no longer supports http
```

### Comparing `rcsb.utils.targets-0.72/LICENSE` & `rcsb.utils.targets-0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/PKG-INFO` & `rcsb.utils.targets-0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.72
+Version: 0.73
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.72/README.md` & `rcsb.utils.targets-0.73/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 logger = logging.getLogger(__name__)
 
 
 class IMGTTargetFeatureProvider(StashableBase):
     """Accessors for IMGT (The International Immunogenetic Information System) target features"""
 
     # Link out using the IMGT -
-    # http://www.imgt.org/3Dstructure-DB/cgi/details.cgi?pdbcode=5w5m&Part=Chain
+    # https://www.imgt.org/3Dstructure-DB/cgi/details.cgi?pdbcode=5w5m&Part=Chain
     #
     def __init__(self, **kwargs):
         #
         self.__cachePath = kwargs.get("cachePath", ".")
         useCache = kwargs.get("useCache", True)
         self.__dirName = "IMGT-features"
         super(IMGTTargetFeatureProvider, self).__init__(self.__cachePath, [self.__dirName])
```

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:           IMGTTargetProvider.py
 #  Date:           5-Jul-2021 jdw
 #
 #  Updated:
 #   14-Mar-2023 dwp  Add timeout to IMGT data file fetch
+#    3-Jul-2023 aae  imgt.org no longer supports http
 #
 ##
 """
 Accessors for IMGT target annotations.
 """
 
 import datetime
@@ -63,16 +64,16 @@
         imgtDataPath = os.path.join(self.__dirPath, "imgt-data.json")
         #
         logger.info("useCache %r imgtFeaturePath %r", useCache, imgtDataPath)
         if useCache and self.__mU.exists(imgtDataPath):
             imgtD = self.__mU.doImport(imgtDataPath, fmt="json")
             self.__version = imgtD["version"]
         else:
-            imgtDumpUrl = imgtDumpUrl if imgtDumpUrl else "http://www.imgt.org/download/3Dstructure-DB/IMGT3DFlatFiles.tgz"
-            imgtReadmeUrl = "http://www.imgt.org/download/3Dstructure-DB/RELEASE"
+            imgtDumpUrl = imgtDumpUrl if imgtDumpUrl else "https://www.imgt.org/download/3Dstructure-DB/IMGT3DFlatFiles.tgz"
+            imgtReadmeUrl = "https://www.imgt.org/download/3Dstructure-DB/RELEASE"
             imgtDumpFileName = fU.getFileName(imgtDumpUrl)
             imgtDumpPath = os.path.join(dirPath, imgtDumpFileName)
             imgtReleasePath = os.path.join(dirPath, "IMGT-release.txt")
             _, fn = os.path.split(imgtDumpUrl)
             imgtFlatFilePath = os.path.join(self.__dirPath, fn[:-4])
             #
             logger.info("Fetching url %s path %s", imgtDumpUrl, imgtDumpPath)
@@ -119,17 +120,17 @@
             15. reverse complementary (if it is)
 
         """
         # --
         fU = FileUtil()
         fU.mkdir(self.__dirPath)
         if withGaps:
-            imgtTargetUrl = "http://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-AA-WithGaps-F+ORF+inframeP"
+            imgtTargetUrl = "https://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-AA-WithGaps-F+ORF+inframeP"
         else:
-            imgtTargetUrl = "http://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-AA-WithoutGaps-F+ORF+inframeP"
+            imgtTargetUrl = "https://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-AA-WithoutGaps-F+ORF+inframeP"
         imgtTargetFileName = fU.getFileName(imgtTargetUrl)
         rawFastaPath = os.path.join(self.__dirPath, imgtTargetFileName)
         # --
         logger.debug("Fetching url %s path %s", imgtTargetUrl, rawFastaPath)
         ok = fU.get(imgtTargetUrl, rawFastaPath)
         logger.info("Fetch status (%r) url %s path %s", ok, imgtTargetUrl, rawFastaPath)
         # --
```

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.72
+Version: 0.73
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.72/setup.py` & `rcsb.utils.targets-0.73/setup.py`

 * *Files identical despite different names*

