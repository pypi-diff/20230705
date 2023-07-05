# Comparing `tmp/dissect.volume-3.6.dev1.tar.gz` & `tmp/dissect.volume-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.volume-3.6.dev1.tar", last modified: Fri Jun 16 12:51:26 2023, max compression
+gzip compressed data, was "dissect.volume-3.6.dev2.tar", last modified: Tue Jun 27 07:49:35 2023, max compression
```

## Comparing `dissect.volume-3.6.dev1.tar` & `dissect.volume-3.6.dev2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.510661 dissect.volume-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/bsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/disk/schemes/mbr.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/ldm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.522661 dissect.volume-3.6.dev1/dissect/volume/lvm/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/lvm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/lvm/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/dissect/volume/vss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.518661 dissect.volume-3.6.dev1/dissect.volume.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:51:26.000000 dissect.volume-3.6.dev1/dissect.volume.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 12:51:16.000000 dissect.volume-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.522661 dissect.volume-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/apm.bin
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/bsd.bin
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/bsd64.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_4k.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_esxi.bin
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_hybrid.bin
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/gpt_no_name_xff.bin
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/lvm.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/data/mbr.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:26.526661 dissect.volume-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_bsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tests/test_mbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:51:12.000000 dissect.volume-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.146331 dissect.volume-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 07:49:35.146331 dissect.volume-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.118331 dissect.volume-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.130331 dissect.volume-3.6.dev2/dissect/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:20.000000 dissect.volume-3.6.dev2/dissect/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.130331 dissect.volume-3.6.dev2/dissect/volume/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.134331 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/bsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/disk/schemes/mbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/ldm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.134331 dissect.volume-3.6.dev2/dissect/volume/lvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/lvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/lvm/lvm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/lvm/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/lvm/physical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/dissect/volume/vss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.126331 dissect.volume-3.6.dev2/dissect.volume.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 07:49:35.000000 dissect.volume-3.6.dev2/dissect.volume.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-27 07:49:35.000000 dissect.volume-3.6.dev2/dissect.volume.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:35.000000 dissect.volume-3.6.dev2/dissect.volume.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:35.000000 dissect.volume-3.6.dev2/dissect.volume.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:35.000000 dissect.volume-3.6.dev2/dissect.volume.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-27 07:49:25.000000 dissect.volume-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:35.146331 dissect.volume-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.138331 dissect.volume-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:20.000000 dissect.volume-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.142331 dissect.volume-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/apm.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/bsd.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/bsd64.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/gpt.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/gpt_4k.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/gpt_esxi.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/gpt_hybrid.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/gpt_no_name_xff.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/lvm.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/data/mbr.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:35.142331 dissect.volume-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/test_apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/test_bsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/test_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tests/test_mbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:49:19.000000 dissect.volume-3.6.dev2/tox.ini
```

### Comparing `dissect.volume-3.6.dev1/LICENSE` & `dissect.volume-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/PKG-INFO` & `dissect.volume-3.6.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.volume
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
 Project-URL: repository, https://github.com/fox-it/dissect.volume
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.volume-3.6.dev1/README.md` & `dissect.volume-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/disk.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/partition.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/partition.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/apm.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/schemes/apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/bsd.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/schemes/bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/gpt.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/schemes/gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/disk/schemes/mbr.py` & `dissect.volume-3.6.dev2/dissect/volume/disk/schemes/mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/ldm.py` & `dissect.volume-3.6.dev2/dissect/volume/ldm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/lvm/lvm2.py` & `dissect.volume-3.6.dev2/dissect/volume/lvm/lvm2.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/lvm/metadata.py` & `dissect.volume-3.6.dev2/dissect/volume/lvm/metadata.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/lvm/physical.py` & `dissect.volume-3.6.dev2/dissect/volume/lvm/physical.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect/volume/vss.py` & `dissect.volume-3.6.dev2/dissect/volume/vss.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/dissect.volume.egg-info/PKG-INFO` & `dissect.volume-3.6.dev2/dissect.volume.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.volume
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for different disk volume and partition systems, for example LVM2, GPT and MBR
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.volume
 Project-URL: repository, https://github.com/fox-it/dissect.volume
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.volume-3.6.dev1/dissect.volume.egg-info/SOURCES.txt` & `dissect.volume-3.6.dev2/dissect.volume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/pyproject.toml` & `dissect.volume-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/conftest.py` & `dissect.volume-3.6.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/apm.bin` & `dissect.volume-3.6.dev2/tests/data/apm.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/bsd.bin` & `dissect.volume-3.6.dev2/tests/data/bsd.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/bsd64.bin.gz` & `dissect.volume-3.6.dev2/tests/data/bsd64.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/gpt.bin` & `dissect.volume-3.6.dev2/tests/data/gpt.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/gpt_4k.bin` & `dissect.volume-3.6.dev2/tests/data/gpt_4k.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/gpt_esxi.bin` & `dissect.volume-3.6.dev2/tests/data/gpt_esxi.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/gpt_hybrid.bin` & `dissect.volume-3.6.dev2/tests/data/gpt_hybrid.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/gpt_no_name_xff.bin` & `dissect.volume-3.6.dev2/tests/data/gpt_no_name_xff.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/lvm.bin.gz` & `dissect.volume-3.6.dev2/tests/data/lvm.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/data/mbr.bin` & `dissect.volume-3.6.dev2/tests/data/mbr.bin`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/docs/Makefile` & `dissect.volume-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/docs/conf.py` & `dissect.volume-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/test_apm.py` & `dissect.volume-3.6.dev2/tests/test_apm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/test_bsd.py` & `dissect.volume-3.6.dev2/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/test_gpt.py` & `dissect.volume-3.6.dev2/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/test_lvm.py` & `dissect.volume-3.6.dev2/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tests/test_mbr.py` & `dissect.volume-3.6.dev2/tests/test_mbr.py`

 * *Files identical despite different names*

### Comparing `dissect.volume-3.6.dev1/tox.ini` & `dissect.volume-3.6.dev2/tox.ini`

 * *Files identical despite different names*

