# Comparing `tmp/sweep-2.0.1.0-py3.10.egg` & `tmp/sweep-2.0.1.1-py3.10.egg`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 16081 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     6204 b- defN 23-Jul-02 02:14 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-02 02:14 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-02 02:14 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-02 02:14 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       32 b- defN 23-Jul-02 02:14 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-02 02:14 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-02 02:14 sweep/__init__.pyc
--rw-rw-rw-  2.0 fat      698 b- defN 23-Jul-02 02:14 sweep/calc_proj_mat_size.pyc
--rw-rw-rw-  2.0 fat     3244 b- defN 23-Jul-02 02:14 sweep/default_proj_mat_ope.pyc
--rw-rw-rw-  2.0 fat     5282 b- defN 23-Jul-02 02:14 sweep/fas2sweep.pyc
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-02 02:14 sweep/fastaread.pyc
--rw-rw-rw-  2.0 fat      565 b- defN 23-Jul-02 02:14 sweep/is_orthonormal.pyc
--rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-02 02:14 sweep/orthbase.pyc
--rw-rw-rw-  2.0 fat      350 b- defN 23-Jul-02 02:14 sweep/sweep_support/__init__.pyc
--rw-rw-rw-  2.0 fat      601 b- defN 23-Jul-02 02:14 sweep/sweep_support/aa2idx.pyc
--rw-rw-rw-  2.0 fat      807 b- defN 23-Jul-02 02:14 sweep/sweep_support/aa2int.pyc
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-02 02:14 sweep/sweep_support/generate_chunk.pyc
--rw-rw-rw-  2.0 fat      301 b- defN 23-Jul-02 02:14 sweep/sweep_support/ij2inds.pyc
--rw-rw-rw-  2.0 fat      815 b- defN 23-Jul-02 02:14 sweep/sweep_support/mask2vec_bin.pyc
--rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-02 02:14 sweep/sweep_support/mask2vec_count.pyc
--rw-rw-rw-  2.0 fat      762 b- defN 23-Jul-02 02:14 sweep/sweep_support/nt2int.pyc
--rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-02 02:14 sweep/sweep_support/orth.pyc
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-02 02:14 sweep/sweep_support/seq2list.pyc
-23 files, 24240 bytes uncompressed, 13089 bytes compressed:  46.0%
+Zip file size: 16086 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     6201 b- defN 23-Jul-05 03:28 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-05 03:28 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-05 03:28 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-05 03:28 EGG-INFO/not-zip-safe
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jul-05 03:28 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-05 03:28 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-05 03:28 sweep/__init__.pyc
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Jul-05 03:28 sweep/calc_proj_mat_size.pyc
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-Jul-05 03:28 sweep/default_proj_mat_ope.pyc
+-rw-rw-rw-  2.0 fat     5282 b- defN 23-Jul-05 03:28 sweep/fas2sweep.pyc
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-05 03:28 sweep/fastaread.pyc
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Jul-05 03:28 sweep/is_orthonormal.pyc
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-05 03:28 sweep/orthbase.pyc
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Jul-05 03:28 sweep/sweep_support/__init__.pyc
+-rw-rw-rw-  2.0 fat      601 b- defN 23-Jul-05 03:28 sweep/sweep_support/aa2idx.pyc
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jul-05 03:28 sweep/sweep_support/aa2int.pyc
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-05 03:28 sweep/sweep_support/generate_chunk.pyc
+-rw-rw-rw-  2.0 fat      301 b- defN 23-Jul-05 03:28 sweep/sweep_support/ij2inds.pyc
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Jul-05 03:28 sweep/sweep_support/mask2vec_bin.pyc
+-rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-05 03:28 sweep/sweep_support/mask2vec_count.pyc
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Jul-05 03:28 sweep/sweep_support/nt2int.pyc
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-05 03:28 sweep/sweep_support/orth.pyc
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-05 03:28 sweep/sweep_support/seq2list.pyc
+23 files, 24237 bytes uncompressed, 13094 bytes compressed:  46.0%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sweep
-Version: 2.0.1.0
+Version: 2.0.1.1
 Summary: SWeeP is a tool for representing large biological sequences datasets in compact vectors
 Home-page: https://github.com/diogomachado-bioinfo/sweep
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 
   -----------------------------------
   SWeeP: Sequence Window Projection
   -----------------------------------
 
-This Python package implements the SWeeP (Sequence Window Projection)
+This Python package implements the SWeeP (Spaced Words Projection)
 algorithm for representing large biological sequence datasets in compact
 vectors. SWeeP allows efficient processing and analysis of sequence data
 by converting sequences into fixed-length feature vectors.
 
 # Installation
 
 To use SWeeP in Python, install the package with the following command:
```

