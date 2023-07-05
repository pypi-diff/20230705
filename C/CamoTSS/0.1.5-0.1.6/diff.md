# Comparing `tmp/CamoTSS-0.1.5.tar.gz` & `tmp/CamoTSS-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CamoTSS-0.1.5.tar", last modified: Mon Apr 17 06:48:24 2023, max compression
+gzip compressed data, was "dist/CamoTSS-0.1.6.tar", last modified: Wed Jul  5 01:35:15 2023, max compression
```

## Comparing `CamoTSS-0.1.5.tar` & `CamoTSS-0.1.6.tar`

### file list

```diff
@@ -1,69 +1,28 @@
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1810 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/.gitignore
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/__init__.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/bin/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/bin/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5403 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/bin/count.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/model/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      877 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/model/logistic_4feature_model.sav
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/utils/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/build_ref.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    24214 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/get_counts.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/get_inputfile_toBrie.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       22 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/version.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS.egg-info/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1405 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS.egg-info/SOURCES.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/dependency_links.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       51 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/entry_points.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      191 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/requires.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/top_level.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11357 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/LICENSE
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2401 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/README.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/docs/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     6762 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/Makefile
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     9651 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/conf.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/docs/image/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   366757 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/image/classifier.png
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   289172 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/image/flow_chart.png
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1765 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/index.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      709 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/install.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3034 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/preprocess.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      100 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/release.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      231 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/requirements.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3582 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/run_CamoTSS.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/notebook/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   358197 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1D_classifier.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2156 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1E.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   127734 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1H.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   583027 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2A.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   299812 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2E.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  2294709 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2F.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   148134 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2H.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   346423 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  1205611 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig3_NPC.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109335 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    76297 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig4I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109166 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/runBRIE.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/setup.cfg
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2339 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/setup.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  9240576 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/test/32_4_feature.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144) 25807864 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/Homo_sapiens.GRCh38.105.chr_test.gtf
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    31059 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/cellbarcode_to_CamoTSS.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      999 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/logistic_36feature_model.sav
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/count/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  3196749 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/fetch_reads.pkl
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11380 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/fourFeature.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  6498398 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/keepdict.pkl
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   626958 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/scTSS_count_all.h5ad
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   125160 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/scTSS_count_two.h5ad
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/ref_file/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   161683 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/ref_file/ref_TSS.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    35122 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/ref_file/ref_gene.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   191754 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/train_fromSCAFE.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    51540 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/trian_ourself_dataset.csv
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:15.016058 CamoTSS-0.1.6/
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:14.996058 CamoTSS-0.1.6/CamoTSS/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-04-17 06:48:01.000000 CamoTSS-0.1.6/CamoTSS/__init__.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:14.997058 CamoTSS-0.1.6/CamoTSS/bin/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.6/CamoTSS/bin/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     6415 2023-06-13 08:52:23.000000 CamoTSS-0.1.6/CamoTSS/bin/count.py
+-rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)     2220 2023-04-22 07:43:26.000000 CamoTSS-0.1.6/CamoTSS/bin/reads2.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:14.998058 CamoTSS-0.1.6/CamoTSS/model/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      740 2023-06-16 06:48:58.000000 CamoTSS-0.1.6/CamoTSS/model/logistic_4feature_model.sav
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:15.015058 CamoTSS-0.1.6/CamoTSS/utils/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.6/CamoTSS/utils/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-04-17 06:48:01.000000 CamoTSS-0.1.6/CamoTSS/utils/build_ref.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    23107 2023-06-14 08:33:44.000000 CamoTSS-0.1.6/CamoTSS/utils/get_counts.py
+-rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)     7464 2023-06-14 08:30:04.000000 CamoTSS-0.1.6/CamoTSS/utils/get_ctss.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-04-17 06:48:01.000000 CamoTSS-0.1.6/CamoTSS/utils/get_inputfile_toBrie.py
+-rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)     8035 2023-06-13 06:18:33.000000 CamoTSS-0.1.6/CamoTSS/utils/toolbox.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       22 2023-07-04 03:00:36.000000 CamoTSS-0.1.6/CamoTSS/version.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-07-05 01:35:14.997058 CamoTSS-0.1.6/CamoTSS.egg-info/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     4484 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      525 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/SOURCES.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/dependency_links.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       52 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/entry_points.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      179 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/requires.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-07-05 01:35:14.000000 CamoTSS-0.1.6/CamoTSS.egg-info/top_level.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     4484 2023-07-05 01:35:15.015058 CamoTSS-0.1.6/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3149 2023-07-05 01:00:16.000000 CamoTSS-0.1.6/README.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-07-05 01:35:15.016058 CamoTSS-0.1.6/setup.cfg
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2325 2023-06-13 06:28:05.000000 CamoTSS-0.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `CamoTSS-0.1.5/CamoTSS/bin/count.py` & `CamoTSS-0.1.6/CamoTSS/bin/count.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from optparse import OptionParser,OptionGroup
 from ..version import __version__
 import sys
 from ..utils.build_ref import get_TSSref,get_generef,get_filter_TSS
 from ..utils.get_counts import get_TSS_count
+from ..utils.get_ctss import get_CTSS_count
 import pyranges as pr
 import os
 import pandas as pd
 import time 
 
 
 START_TIME = time.time()
@@ -15,15 +16,16 @@
 def main():
     parser = OptionParser()
     parser.add_option('--gtf','-g',dest='gtf_file',default=None,help='The annotation gtf file for your analysing species.')
     parser.add_option('--cellbarcodeFile','-c',dest='cdrFile',default=None,help='The file include cell barcode which users want to keep in the downstream analysis.')
     parser.add_option('--bam','-b',dest='bam_file',default=None,help='The bam file of aligned from Cellranger or other single cell aligned software.')
     parser.add_option('--outdir','-o',dest='out_dir',default=None,help='The directory for output [default : $bam_file]') #what should be after $
     parser.add_option('--refFasta','-r',dest='refFasta',default=None,help='The directory for reference genome fasta file') #what should be after $
-    parser.add_option('--mode','-m',dest='mode',default=None,help='You can select run by finding novel TSS cluster mode [TC]. If you also want to detect CTSS within one cluster, you can use [CTSS] mode')
+    parser.add_option('--mode','-m',dest='mode',default=None,help='You can select run by finding novel TSS cluster and CTSS within one cluster [TC+CTSS]. \
+                        If you just want to detect TSS cluster, you can use [TC] mode. If you just want to detect CTSS, you can use [CTSS] mode which is based on the output of [TC mode]')
 
    
    
     group0=OptionGroup(parser,"Optional arguments")
 
     group0.add_option("--minCount",type="int",dest="minCount",default=50,
     help="Minimum UMI counts for TC in all cells [default: 50]")
@@ -36,106 +38,134 @@
     
     group0.add_option('--clusterDistance',type="float",dest='clusterDistance',default=300,
     help="The minimum distance between two cluster transcription start site [default: 300]")
 
     group0.add_option('--InnerDistance',type="float",dest='InnerDistance',default=100,
     help="The resolution of each cluster [default: 100]")
 
-    group0.add_option('--windowSize',type="float",dest='windowSize',default=15,
+    group0.add_option('--windowSize',type="int",dest='windowSize',default=15,
     help="The width of sliding window [default: 15]")
 
-    group0.add_option('--minCTSSCount',type="float",dest='minCTSSCount',default=100,
-    help="The minimum UMI counts for each CTSS [default: 100]")
 
-    group0.add_option('--minFC',type="float",dest='minFC',default=6,
-    help="The minimum fold change for filtering CTSS [default: 6]")
 
+    group1=OptionGroup(parser,"Optional arguments")
 
+    group1.add_option('--minCTSSCount',type="float",dest='minCTSSCount',default=100,
+    help="The minimum UMI counts for each CTSS [default: 100]")
 
+    group1.add_option('--minFC',type="float",dest='minFC',default=6,
+    help="The minimum fold change for filtering CTSS [default: 6]")
 
 
 
     parser.add_option_group(group0)
+    parser.add_option_group(group1)
+
+
     (options, args) = parser.parse_args()
 
     
     #this means that if users do not input any argument, then direct produce help. then end.
     if len(sys.argv[1:]) == 0:
         print('Welcome to CamoTSS v%s!\n'%(__version__))
         print("use -h or --help for help on argument.")
         sys.exit(1)
 
 
-    #output file 
-    if options.out_dir is None:
-        print("Warning: no outDir provided, we use $bamfilePath/CamoTSS\n")
-        out_dir = os.path.dirname(os.path.abspath(options.bam_file)) + "/CamoTSS"
-    # elif os.path.dirname(options.out_dir) == "":
-    #     out_dir= "./" + options.out_dir
-    else:
-        out_dir = options.out_dir
-    if not os.path.exists(out_dir):
-        os.mkdir(out_dir)
-    #print(out_dir)
 
-    if options.cdrFile is None:
-        print("Error: Need --cdrFile for cell barcode file.")
-        sys.exit(1)
 
-    if options.refFasta is None:
-        print("Error: Need --refFasta for reference fasta file.")
-        sys.exit(1)
 
-
-    #bam file
-    if options.bam_file is None:
-        print("Error: Need --bam for aligned file.")
+    if options.mode is None:
+        print("Error: Need --mode to select the mode what you prefer.")
         sys.exit(1)
+
     
-   
-        
-    #gtf file
-    if options.gtf_file is None:
-        print("Error: Need --gtf for annotation file.")
-        sys.exit(1)
-    else:
-        gr = pr.read_gtf(options.gtf_file)
-        grdf = gr.df
-        ref_out_dir=str(out_dir)+'/ref_file/'
-        if not os.path.exists(ref_out_dir):
-            os.mkdir(ref_out_dir)
-        tssrefpath=get_TSSref(grdf,ref_out_dir)
-        tssdf=pd.read_csv(tssrefpath,delimiter='\t')
-        generefpath=get_generef(grdf,tssdf,ref_out_dir)
+    if (options.mode=='TC') or (options.mode=='TC+CTSS'):
+        if options.cdrFile is None:
+            print("Error: Need --cdrFile for cell barcode file.")
+            sys.exit(1)
+
+        if options.refFasta is None:
+            print("Error: Need --refFasta for reference fasta file.")
+            sys.exit(1)
+
+        #bam file
+        if options.bam_file is None:
+            print("Error: Need --bam for aligned file.")
+            sys.exit(1)
+
+
+            #output file 
+        if options.out_dir is None:
+            print("Warning: no outDir provided, we use $bamfilePath/CamoTSS\n")
+            out_dir = os.path.dirname(os.path.abspath(options.bam_file)) + "/CamoTSS"
+        else:
+            out_dir = options.out_dir
+        if not os.path.exists(out_dir):
+            os.mkdir(out_dir)
+
+
+        #gtf file
+        if options.gtf_file is None:
+            print("Error: Need --gtf for annotation file.")
+            sys.exit(1)
+        else:
+            gr = pr.read_gtf(options.gtf_file)
+            grdf = gr.df
+            ref_out_dir=str(out_dir)+'/ref_file/'
+            if not os.path.exists(ref_out_dir):
+                os.mkdir(ref_out_dir)
+            tssrefpath=get_TSSref(grdf,ref_out_dir)
+            tssdf=pd.read_csv(tssrefpath,delimiter='\t')
+            generefpath=get_generef(grdf,tssdf,ref_out_dir)
+
+
+    elif options.mode=='CTSS':
+        if options.out_dir is None:
+            print("Error: Need --outdir which includes subdir '/ref_file' and '/count'")
+            sys.exit(1)
+
+        out_dir=options.out_dir
+
 
     bam_file=options.bam_file
     minCount=options.minCount
     cellBarcodePath=options.cdrFile
     n_proc=options.nproc
     maxReadCount=options.maxReadCount
     clusterDistance=options.clusterDistance
     InnerDistance=options.InnerDistance
     fastqFilePath=options.refFasta
     windowSize=options.windowSize
     minCTSSCount=options.minCTSSCount
     minFC=options.minFC
+    
 
 
 
 
         
     if options.mode == "TC":
         getTSScount=get_TSS_count(generefpath,tssrefpath,bam_file,fastqFilePath,out_dir,cellBarcodePath,n_proc,minCount,maxReadCount,clusterDistance,InnerDistance,windowSize,minCTSSCount,minFC)
         scadata=getTSScount.produce_sclevel()
 
-    elif options.mode=="CTSS":
+    elif options.mode=="TC+CTSS":
+        # ctss_out_dir=str(options.out_dir)+'/CTSS/'
+        # if not os.path.exists(ctss_out_dir):
+        #     os.mkdir(ctss_out_dir)
         getTSScount=get_TSS_count(generefpath,tssrefpath,bam_file,fastqFilePath,out_dir,cellBarcodePath,n_proc,minCount,maxReadCount,clusterDistance,InnerDistance,windowSize,minCTSSCount,minFC)
         scadata=getTSScount.produce_sclevel()
         twoctssadata=getTSScount.produce_CTSS_adata()
 
+
+    elif options.mode=='CTSS':
+        getctsscount=get_CTSS_count(out_dir,minCTSSCount,minFC,n_proc,windowSize)   # should create CTSS 
+        ctssadata=getctsscount.produce_CTSS_adata()
+
+
     else:
         print('Do not have this mode. Please check your spell!')
         run_time = time.time() - START_TIME
         print("[CamoTSS] All done: %d min %.1f sec" %(int(run_time / 60), 
                                                   run_time % 60))
```

### Comparing `CamoTSS-0.1.5/CamoTSS/utils/build_ref.py` & `CamoTSS-0.1.6/CamoTSS/utils/build_ref.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.5/CamoTSS/utils/get_counts.py` & `CamoTSS-0.1.6/CamoTSS/utils/get_counts.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,73 +11,26 @@
 import time
 import random
 import pickle
 import statistics
 import editdistance
 import warnings
 from pathlib import Path
-import sys
-from brie.utils import fetch_reads
+from .toolbox import check_pysam_chrom,fetch_reads
+
 
 
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings("ignore", category=Warning)
 
 
 
 
 
-
-
-global CACHE_CHROM
-global CACHE_SAMFILE
-CACHE_CHROM = None
-CACHE_SAMFILE = None
-
-def check_pysam_chrom(samFile,chrom=None):
-    """
-    check samFile is a file name or a pysam object, and if chrom format.
-    """
-    global CACHE_CHROM
-    global CACHE_SAMFILE
-
-    if CACHE_CHROM is not None:
-        if (samFile==CACHE_SAMFILE) and (chrom==CACHE_CHROM):
-            return CACHE_SAMFILE,CACHE_CHROM
-
-    
-    if type(samFile)==str or type(samFile)==np.str_:
-        ftype=samFile.split(".")[-1]
-        if ftype != "bam" and ftype!="sam" and ftype!="cram":
-            print("Error: file type need suffix of bam, sam or cram")
-            sys.exit(1)
-        if ftype == "cram":
-            samFile=pysam.AlignmentFile(samFile,'rc')
-        elif ftype=="bam":
-            samFile=pysam.AlignmentFile(samFile,'rb')
-        else:
-            samFile=pysam.AlignmentFile(samFile,'r')
-
-    if chrom is not None:
-        if chrom not in samFile.references:
-            if chrom.startswith("chr"):
-                chrom=chrom.split('chr')[1]
-            else:
-                chrom="chr"+chrom
-        if chrom not in samFile.references:
-            print("Can't find reference %s in samFile"%chrom)
-            return samFile,None
-
-    CACHE_CHROM=chrom
-    CACHE_SAMFILE=samFile
-    return samFile,chrom
-
-
-
 def get_fastq_file(fastqFilePath):
     fastqFile=pysam.FastaFile(fastqFilePath)
     return fastqFile
 
 
 
 
@@ -86,21 +39,20 @@
 
 
     def __init__(self,generefPath,tssrefPath,bamfilePath,fastqFilePath,outdir,cellBarcodePath,nproc,minCount,maxReadCount,clusterDistance,InnerDistance,windowSize,minCTSSCount,minFC):
         self.generefdf=pd.read_csv(generefPath,delimiter='\t')
         self.generefdf['len']=self.generefdf['End']-self.generefdf['Start']
         self.tssrefdf=pd.read_csv(tssrefPath,delimiter='\t')
         self.bamfilePath=bamfilePath
+        self.outdir=outdir
         self.count_out_dir=str(outdir)+'/count/'
         if not os.path.exists(self.count_out_dir):
             os.mkdir(self.count_out_dir)
 
-        self.ctss_out_dir=str(outdir)+'/CTSS/'
-        if not os.path.exists(self.ctss_out_dir):
-            os.mkdir(self.ctss_out_dir)
+
 
 
         self.minCount=minCount
         self.cellBarcode=pd.read_csv(cellBarcodePath,delimiter='\t')['cell_id'].values
         self.nproc=nproc
         self.maxReadCount=maxReadCount
         self.clusterDistance=clusterDistance
@@ -109,15 +61,15 @@
         self.windowSize=windowSize
         self.minCTSSCount=minCTSSCount
         self.minFC=minFC
 
         
 
     def _getreads(self,bamfilePath,fastqFilePath,geneid):
-        #fetch reads1 in gene 
+        #fetch reads1 in gene ; In this step, we remove the umi duplicates. 
         samFile, _chrom = check_pysam_chrom(bamfilePath, str(self.generefdf.loc[geneid]['Chromosome']))
         reads = fetch_reads(samFile, _chrom,  self.generefdf.loc[geneid]['Start'] , self.generefdf.loc[geneid]['End'],  trimLen_max=100)
         reads1_umi = reads["reads1"]
 
 
 
         #select according to GX tag and CB (filter according to user owned cell)
@@ -268,17 +220,17 @@
 
 
 
         for geneidSec, reslsSec in zip(readls,altTSSls):
             altTSSdict[geneidSec]=reslsSec
         altTSSdict={k: v for k, v in altTSSdict.items() if v}
 
-        # tss_output=self.count_out_dir+'gene_with_onecluster.pkl'
-        # with open(tss_output,'wb') as f:
-        #     pickle.dump(altTSSdict,f)
+        tss_output=self.count_out_dir+'before_cluster_peak.pkl'
+        with open(tss_output,'wb') as f:
+            pickle.dump(altTSSdict,f)
 
         print('do clustering Time elapsed',int(time.time()-start_time),'seconds.')
 
         return altTSSdict
 
 
     def _filter_false_positive(self):
@@ -312,14 +264,15 @@
 
         # cluster_output=self.count_out_dir+'before_filter_cluster.pkl'
         # with open(cluster_output,'wb') as f:
         #     pickle.dump(clusterdict,f)
 
         
         fourfeaturedf=pd.DataFrame(clusterdict).T 
+        fourfeaturedf.columns=['UMI_count','SD','summit_UMI_count','unencoded_G_percent','NO.TSS','gene_id','summit_position']
         fourfeature_output=self.count_out_dir+'fourFeature.csv'
         fourfeaturedf.to_csv(fourfeature_output)
 
         print('one_gene_with_two_TSS_fourfeature : %i'%(len(fourfeaturedf)))
         test_X=fourfeaturedf.iloc[:,0:4]
         # print('hello')
 
@@ -333,27 +286,27 @@
 
         pathstr=str(Path(os.path.dirname(os.path.abspath(__file__))).parents[0])+'/model/logistic_4feature_model.sav'
         loaded_model = pickle.load(open(pathstr, 'rb'))
         test_Y=loaded_model.predict(test_X.values)
 
         #do filtering, the result of this step should be output as final h5ad file display at single cell level. 
         afterfiltereddf=fourfeaturedf[test_Y==1]
-        afterfiltereddf.columns=['all_counts','std','summit_count','unencoded_G_percent','TSS.no','gene_id','summit_position']
+        afterfiltereddf.columns=['UMI_count','SD','summit_UMI_count','unencoded_G_percent','NO.TSS','gene_id','summit_position']
 
-        # afterfilter_output=self.count_out_dir+'afterfiltered.csv'
-        # afterfiltereddf.to_csv(afterfilter_output)
+        afterfilter_output=self.count_out_dir+'afterfiltered.csv'
+        afterfiltereddf.to_csv(afterfilter_output)
 
 
         allgeneID=afterfiltereddf['gene_id'].unique()
         keepdict={}
         for i in allgeneID:
             selectgeneiddf=afterfiltereddf[afterfiltereddf['gene_id']==i]
             keeptranscriptls=[]
             for j in selectgeneiddf.index:
-                index=afterfiltereddf.loc[j]['TSS.no']
+                index=afterfiltereddf.loc[j]['NO.TSS']
                 keeptranscriptls.append(altTSSdict[i][index])
             keepdict[i]=keeptranscriptls
 
 
 
         tss_output=self.count_out_dir+'keepdict.pkl'
         with open(tss_output,'wb') as f:
@@ -455,15 +408,15 @@
         #transcriptdfls=[]
 
         cellIDls=[]
         for i in range(0,len(extendls)):
             cellID=np.unique(extendls[i][1][1])
             cellIDls.append(list(cellID))
         cellIDset = set([item for sublist in cellIDls for item in sublist])
-        finaldf=pd.DataFrame(index=cellIDset)
+        finaldf=pd.DataFrame(index=list(cellIDset))
 
 
 
         for i in range(0,len(extendls)):
             transcriptid=extendls[i][0]       
             cellID,count=np.unique(extendls[i][1][1],return_counts=True)
             transcriptdf=pd.DataFrame({'cell_id':cellID,transcriptid:count})
@@ -497,15 +450,15 @@
 
             tempdf=tempdf.sort_values('transcript_id',ascending=False)
             tempdf['diff']=tempdf['TSS_start'].diff()
             keepdf=tempdf[tempdf['diff'].isna()|tempdf['diff'].abs().ge(self.clusterDistance)]    #want to get TSS whose cluster distance is more than user defined.
             #keepdf=keepdf.iloc[:2,:]
             keepdfls.append(keepdf) 
 
-        print(keepdfls)
+        #print(keepdfls)
 
 
         allkeepdf=reduce(lambda x,y:pd.concat([x,y]),keepdfls)
         finaltwodf=allkeepdf[allkeepdf.duplicated('gene_id',keep=False)] 
         finaltwoadata=adata[:,adata.var.index.isin(finaltwodf['transcript_id'])]  
 
         sc_output_h5ad=self.count_out_dir+'scTSS_count_two.h5ad'
@@ -553,14 +506,15 @@
             TSS=sortfinalarray.T[0]
             count=sortfinalarray.T[1]
 
 
         #do something with sliding windows algorithm   
         storels=[]
         for i in range(len(TSS) - self.windowSize + 1):
+            #print(i)
             onewindow=TSS[i: i + self.windowSize]
             correspondingcount=count[i: i + self.windowSize]
             middlecount=correspondingcount[leftIndex]
             foldchange=(middlecount+1)/(sum(correspondingcount)/len(correspondingcount)+1)
             storels.append([onewindow[leftIndex],correspondingcount[leftIndex],foldchange])
             
         foldchangels=[i[2] for i in storels]
@@ -577,42 +531,38 @@
         alloneclusterdf['gene_id']=alloneclusterdf['Unnamed: 0'].str.split('*',expand=True)[0]
         alloneclusterdf['TSS_start']=alloneclusterdf['Unnamed: 0'].str.split('*',expand=True)[1].str.split('_',expand=True)[0].astype('float')
         alloneclusterdf['TSS_end']=alloneclusterdf['Unnamed: 0'].str.split('_',expand=True)[1].astype('float')
 
         self.generefdf.reset_index(inplace=True)
         
 
-        print(self.generefdf)
+        #print(self.generefdf)
         stranddf=self.generefdf[['Strand','gene_id']]
         alloneclusterdf=alloneclusterdf.merge(stranddf,on='gene_id')
 
 
 
 
+        start_time=time.time()
 
-
-        pool = multiprocessing.Pool(processes=self.nproc)
-        allsortls=[]
+        allsortfddict={}
 
         for i in range(0,len(alloneclusterdf)):
-            
             geneID=alloneclusterdf['gene_id'][i]
-            genereads=fetchadata[geneID]
+            # print(geneID)
+            genereads=self.fetchadata[geneID]
+            clusterID=alloneclusterdf['Unnamed: 0'][i]
             TSS_start=alloneclusterdf['TSS_start'][i]
             TSS_end=alloneclusterdf['TSS_end'][i]
             strand=alloneclusterdf['Strand'][i]
-            allsortls.append(pool.apply_async(self.window_sliding,(genereads,TSS_start,TSS_end,strand)))
+            windowreturn=self.window_sliding(genereads,TSS_start,TSS_end,strand)
+            allsortfddict[clusterID]=windowreturn
 
-        pool.close()
-        pool.join()
-        results=[res.get() for res in allsortls]
 
-        allsortfddict={}
-        for geneid,resls in zip(alloneclusterdf['Unnamed: 0'],results):
-            allsortfddict[geneid]=resls  
+        print('window sliding Time elapsed',int(time.time()-start_time),'seconds.')
 
         
         ctssOutPath=self.ctss_out_dir+'CTSS_foldchange.pkl'
         with open(ctssOutPath,'wb') as f:
             pickle.dump(allsortfddict,f)
 
         return allsortfddict
@@ -630,14 +580,24 @@
 
 
 
 
     def produce_CTSS_adata(self):
         ctime=time.time()
 
+
+        self.ctss_out_dir=str(self.outdir)+'/CTSS/'
+        if not os.path.exists(self.ctss_out_dir):
+            os.mkdir(self.ctss_out_dir)
+
+
+
+
+
+
         readspath=self.count_out_dir+'fetch_reads.pkl'
         with open(readspath,'rb') as f:
             fetchadata=pickle.load(f)
 
         allsortfddict=self._get_CTSS(fetchadata)
         keepdict={}
         for ctssid in allsortfddict.keys():
@@ -674,14 +634,15 @@
             cellID,count=np.unique(cellIDdict[clusterID],return_counts=True)
             CTSSdf=pd.DataFrame({'cell_id':cellID,clusterID:count})
             CTSSdf.set_index('cell_id',inplace=True)
             ctssfinaldf[clusterID]=ctssfinaldf.index.map(CTSSdf[clusterID])
 
 
         ctssfinaldf.fillna(0,inplace=True)
+        #print(ctssfinaldf)
         ctssadata=ad.AnnData(ctssfinaldf)
 
         ctssvardf=pd.DataFrame(ctssadata.var.copy())
         ctssvardf.reset_index(inplace=True)
         ctssvardf.columns=['clusterID']
         ctssvardf['gene_id']=ctssvardf['clusterID'].str.split('*',expand=True)[0]
         ctssvardf['CTSS']=ctssvardf['clusterID'].str.split('#',expand=True)[1].str.split('@',expand=True)[0]
```

### Comparing `CamoTSS-0.1.5/CamoTSS/utils/get_inputfile_toBrie.py` & `CamoTSS-0.1.6/CamoTSS/utils/get_inputfile_toBrie.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.5/CamoTSS.egg-info/PKG-INFO` & `CamoTSS-0.1.6/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: CamoTSS
-Version: 0.1.5
-Summary: CamoTSS: Detection alternative TSS in single cells
-Home-page: https://github.com/StatBiomed/CamoTSS
-Author: ['Ruiyan Hou']
-Author-email: ruiyan@connect.hku.hk
-License: Apache-2.0
-Keywords: Transcript Start Site,single-cell RNA-seq
-Requires-Python: >=3.5
-Provides-Extra: docs
-License-File: LICENSE
-
 ============================================================
 CamoTSS for alternative TSS analysis in single cells
 ============================================================
 |pypi| 
 
 .. |pypi| image:: https://badge.fury.io/py/CamoTSS.svg
        :target: https://pypi.org/project/CamoTSS/
@@ -49,27 +36,41 @@
 Here, you can download some large file include genome.fa, possorted_genome_bam_filtered.bam.
 
 Alternatively, you can also download the reference genome fasta file from Ensembl or Genecode or website of 10x Genomics. 
  
 Run CamoTSS 
 =============
 
-Here are two modes in CamoTSS : **TC** and **CTSS**. 
+Here are three modes in CamoTSS : **TC+CTSS** , **TC** and **CTSS**.
+
+When you run **TC+CTSS** mode, you will get TC result and then get the CTSS result based on the TC.
+
+When you run **TC** mode, you will only get the TC result.
+
+The **TC+CTSS** and **TC** mode have the same required files.
+
+The --outdir is the only required parameter for **CTSS** mode. But the outdir should include output of TC.  
+
+If you want to run **CTSS** mode, you must based on the output of TC.
+
+You can run CamoTSS **TC+CTSS** mode by using test file according to the following code.
+
+For the remaining modes, you can check this document_.
 
-You can run CamoTSS by using test file according to the following code.
+.. _document: https://camotss.readthedocs.io/en/latest/run_CamoTSS.html
 
 .. code-block:: bash
 
    #!/bin/bash 
    gtfFile= $CamoTSS/test/Homo_sapiens.GRCh38.105.chr_test.gtf
    fastaFile = $download/genome.fa
    bamFile= $download/possorted_genome_bam_filtered.bam
    cellbarcodeFile=$CamoTSS/test/cellbarcode_to_CamoTSS
 
-   CamoTSS --gtf gtfFile --refFasta fastaFile --bam bamFile -c cellbarcodeFile -o CamoTSS_out --mode TC
+   CamoTSS --gtf gtfFile --refFasta fastaFile --bam bamFile -c cellbarcodeFile -o CamoTSS_out --mode TC+CTSS
 
 
 Alternative TSS or CTSS detecting
 =================================
 
 To identify alternative TSS usage or alternative CTSS usage, Brie2 (Huang & Sanguinetti, 2021) is recommend to be used. 
 
@@ -100,15 +101,15 @@
 .. _Detect alternative TSS/CTSS: https://camotss.readthedocs.io/en/latest/runBRIE.html
 
 
 
 Reference
 ===========
 
-Coming soon
+Hou, R., Hon, C. C., & Huang, Y. (2023). CamoTSS: analysis of alternative transcription start sites for cellular phenotypes and regulatory patterns from 5'scRNA-seq data. bioRxiv, 2023-04.
```

### Comparing `CamoTSS-0.1.5/setup.py` & `CamoTSS-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 exec(open("./CamoTSS/version.py").read())
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
     
 reqs = ['numpy>=1.9.0', 'scipy>=1.4.0', 'matplotlib','anndata>=0.6','pyranges>=0.0.115',
-'scanpy>=1.5','pysam>=0.15.2','brie>=2.2.0','pandas>=0.23.0','scikit-learn>=0.23','editdistance>=0.3.1']
+'scanpy>=1.5','pysam>=0.15.2','pandas>=0.23.0','scikit-learn>=0.23','editdistance>=0.3.1']
 
 setup(
     name='CamoTSS',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
```

