# Comparing `tmp/nanoCEM-0.0.1.3.tar.gz` & `tmp/nanoCEM-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.3.tar", last modified: Mon Jul  3 10:51:03 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.4.tar", last modified: Wed Jul  5 04:46:05 2023, max compression
```

## Comparing `nanoCEM-0.0.1.3.tar` & `nanoCEM-0.0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:51:03.929075 nanoCEM-0.0.1.3/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.3/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-03 10:51:03.925075 nanoCEM-0.0.1.3/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.3/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:51:03.925075 nanoCEM-0.0.1.3/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9425 2023-07-03 10:47:10.000000 nanoCEM-0.0.1.3/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.3/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.3/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7691 2023-07-03 10:42:53.000000 nanoCEM-0.0.1.3/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.3/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.3/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.3/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10994 2023-07-03 10:50:36.000000 nanoCEM-0.0.1.3/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13844 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.3/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:51:03.925075 nanoCEM-0.0.1.3/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-03 10:51:03.000000 nanoCEM-0.0.1.3/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-03 10:51:03.000000 nanoCEM-0.0.1.3/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-03 10:51:03.000000 nanoCEM-0.0.1.3/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-03 10:51:03.000000 nanoCEM-0.0.1.3/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-03 10:51:03.000000 nanoCEM-0.0.1.3/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-03 10:51:03.929075 nanoCEM-0.0.1.3/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-03 10:51:00.000000 nanoCEM-0.0.1.3/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.4/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.4/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9423 2023-07-04 09:33:19.000000 nanoCEM-0.0.1.4/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.4/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.4/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7706 2023-07-05 04:46:02.000000 nanoCEM-0.0.1.4/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.4/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.4/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.4/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10994 2023-07-03 10:50:36.000000 nanoCEM-0.0.1.4/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13843 2023-07-05 03:24:20.000000 nanoCEM-0.0.1.4/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-05 04:46:02.000000 nanoCEM-0.0.1.4/setup.py
```

### Comparing `nanoCEM-0.0.1.3/LICENSE` & `nanoCEM-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/PKG-INFO` & `nanoCEM-0.0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.3/README.md` & `nanoCEM-0.0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.4/nanoCEM/CE_magnifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
     parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
     add_public_argument(parser_f5c)
     # parser.set_defaults(function='tombo', chrom="1", pos=150280972, len=10, strand='+', cpu=1,input_fast5='/data/current_test_data/samp/cem_test_dna/WGS/single/',\
     #                     control_fast5='/data/current_test_data/samp/cem_test_dna/WGA/single/',output='tombo_result_dna',\
     #                     overplot_number=300,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",\
     #                     basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=False)
-    # parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
-    #                     control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
-    #                     ref="/data/Ecoli_23s/23S_rRNA.fasta",\
-    #                      basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
-    parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
-                        control='/data/Ecoli_23s/data/IVT_negative/file',\
-                        output='f5c_result_rna_new_re',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA_reverse.fasta",rna=True,base_shift=2)
+    parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
+                        control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
+                        ref="/data/Ecoli_23s/23S_rRNA.fasta",\
+                         basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
+    # parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
+    #                     control='/data/Ecoli_23s/data/IVT_negative/file',\
+    #                     output='f5c_result_rna_new_re',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA_reverse.fasta",rna=True,base_shift=2)
     # parser.set_defaults(function='f5c', chrom="1", pos=150280972, len=10, strand='+', cpu=4,input='/data/current_test_data/samp/cem_test_dna/WGS/file',\
     #                     control='/data/current_test_data/samp/cem_test_dna/WGA/file',\
     #                     output='f5c_result_dna_new',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=2)
 
     return parser
 
 if __name__ == '__main__':
```

### Comparing `nanoCEM-0.0.1.3/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.4/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.4/nanoCEM/current_events_magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import argparse
 import os
-from cem_utils import read_fasta_to_dic,reverse_fasta
+from nanoCEM.cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
-from plot import signal_plot
+from nanoCEM.plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
 import warnings
 import time
 warnings.filterwarnings("ignore", category=PlotnineWarning)
 import numpy as np
 def init_parser():
     def add_public_argument(parser_input):
@@ -84,15 +84,15 @@
         print("Output file existed! It will be overwrite after 5 secs ...")
         time.sleep(5)
         print("Continue ...")
 
 
     if args.function == 'tombo' :
 
-        from  nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
+        from nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
         wt_file = create_read_list_file(args.input_fast5, results_path)
         df_wt, aligned_num_wt = extract_group(args, wt_file, subsample_num)
         df_wt['type'] = 'Sample'
         try:
             ivt_file = create_read_list_file(args.control_fast5, results_path)
             df_ivt, aligned_num_ivt = extract_group(args, ivt_file, subsample_num)
             df_ivt['type'] = 'Control'
```

### Comparing `nanoCEM-0.0.1.3/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.4/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/normalization.py` & `nanoCEM-0.0.1.4/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/plot.py` & `nanoCEM-0.0.1.4/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.4/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.3/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.4/nanoCEM/read_tombo_resquiggle.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         if temp_result is None:
             return None
         (raw_data, raw_label, raw_start, raw_length, start_position, strand,chrome) = temp_result
     except Exception as e:
         # print(str(e))
         return None
 
-
     # ~ print(input_file,raw_start,raw_length,raw_label)
     total_seq = "".join([x.decode() for x in raw_label])
     base_len=raw_label.shape[0]
     end_position = start_position+base_len
     if mode:
         raw_data = np.flip(raw_data)
     matrix_feature = extract_feature(raw_data, raw_start, raw_length, total_seq,start_position,end_position,strand)
```

### Comparing `nanoCEM-0.0.1.3/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.4/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.3/setup.py` & `nanoCEM-0.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.3",
+    version="0.0.1.4",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

