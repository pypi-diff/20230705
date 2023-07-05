# Comparing `tmp/nanoCEM-0.0.1.4.tar.gz` & `tmp/nanoCEM-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.4.tar", last modified: Wed Jul  5 04:46:05 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.5.tar", last modified: Wed Jul  5 04:51:42 2023, max compression
```

## Comparing `nanoCEM-0.0.1.4.tar` & `nanoCEM-0.0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.4/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.4/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9423 2023-07-04 09:33:19.000000 nanoCEM-0.0.1.4/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.4/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.4/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7706 2023-07-05 04:46:02.000000 nanoCEM-0.0.1.4/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.4/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.4/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.4/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10994 2023-07-03 10:50:36.000000 nanoCEM-0.0.1.4/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13843 2023-07-05 03:24:20.000000 nanoCEM-0.0.1.4/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-05 04:46:05.000000 nanoCEM-0.0.1.4/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-05 04:46:05.215349 nanoCEM-0.0.1.4/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-05 04:46:02.000000 nanoCEM-0.0.1.4/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.5/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.5/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9423 2023-07-04 09:33:19.000000 nanoCEM-0.0.1.5/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.5/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.5/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7706 2023-07-05 04:51:31.000000 nanoCEM-0.0.1.5/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.5/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.5/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.5/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10994 2023-07-03 10:50:36.000000 nanoCEM-0.0.1.5/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13843 2023-07-05 03:24:20.000000 nanoCEM-0.0.1.5/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-05 04:51:41.000000 nanoCEM-0.0.1.5/setup.py
```

### Comparing `nanoCEM-0.0.1.4/LICENSE` & `nanoCEM-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/PKG-INFO` & `nanoCEM-0.0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.4/README.md` & `nanoCEM-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.5/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.5/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.5/nanoCEM/current_events_magnifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
-        parser_input.add_argument("--overplot-number", default=500, type=int,
+        parser_input.add_argument("--overplot_number", default=500, type=int,
                                   help="Number of read will be used to plot")
         parser_input.add_argument('--rna', action='store_true', help='RNA mode')
     # Define the argument parser
     parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
```

### Comparing `nanoCEM-0.0.1.4/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.5/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/normalization.py` & `nanoCEM-0.0.1.5/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/plot.py` & `nanoCEM-0.0.1.5/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.5/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.5/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.4/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.5/nanoCEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.4/setup.py` & `nanoCEM-0.0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.4",
+    version="0.0.1.5",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

