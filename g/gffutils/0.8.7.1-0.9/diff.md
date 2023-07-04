# Comparing `tmp/gffutils-0.8.7.1.tar.gz` & `tmp/gffutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gffutils-0.8.7.1.tar", last modified: Fri Jan 15 18:53:54 2016, max compression
+gzip compressed data, was "dist/gffutils-0.9.tar", last modified: Wed Aug  9 14:41:45 2017, max compression
```

## Comparing `gffutils-0.8.7.1.tar` & `gffutils-0.9.tar`

### file list

```diff
@@ -1,68 +1,83 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      796 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1796 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1319 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/MANIFEST.in
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/requirements.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2924 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/inspection.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    13644 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/feature.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2924 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/inspect.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/scripts/
--rwxrwxr-x   0 ryan      (1000) ryan      (1000)     6769 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/scripts/gffutils-flybase-convert.py
--rwxrwxr-x   0 ryan      (1000) ryan      (1000)    10532 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/scripts/gffutils-cli
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    50151 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/create.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9128 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/iterators.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2609 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/biopython_integration.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      370 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/exceptions.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2932 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/attributes.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7600 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/pybedtools_integration.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6006 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/gffwriter.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1392 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/convert.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3023 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/constants.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      329 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       18 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/version.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      637 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/test_biopython_integration.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6813 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/expected.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    37109 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/test.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5600 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/ncbi_gff3.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      743 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/c_elegans_WS199_dna_shortened.fa
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      677 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/hybrid1.gff3
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      653 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/wormbase_gff2_alt.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      534 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/jgi_gff2.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1326 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/mouse_extra_comma.gff3
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6560 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/wormbase_gff2.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)  9023416 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/dmel-all-no-analysis-r5.49_50k_lines.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1732 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/random-chr.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1793 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/gff_example1.gff3
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5983 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/FBgn0031208.gtf
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      333 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/gff_example1.gff3.gz
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8407 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/gencode-v19.gtf
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      385 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/glimmer_nokeyval.gff3
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5991 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/FBgn0031208.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    18098 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/c_elegans_WS199_shortened_gff.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    17518 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/F3-unique-3.v2.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       45 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/unsanitized.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6569 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/nonascii
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3016 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/intro_docs_example.gff
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5416 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/ensembl_gtf.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      145 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/data/c_elegans_WS199_ann_gff.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5273 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/parser_test.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5238 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/attr_test_cases.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1367 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/helpers_test.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5714 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/test/feature_test.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    15721 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/helpers.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    45891 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/interface.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9054 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/parser.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7520 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/gffutils/bins.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1076 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1353 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/setup.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      796 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      692 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/README.rst
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       59 2016-01-15 18:53:54.000000 gffutils-0.8.7.1/setup.cfg
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/gffutils.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils.egg-info/top_level.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      950 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2402 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1319 2017-08-09 14:41:43.000000 gffutils-0.9/MANIFEST.in
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2017-08-09 14:41:44.000000 gffutils-0.9/requirements.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/gffutils/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2924 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/inspection.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    14193 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/feature.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2924 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/inspect.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/gffutils/scripts/
+-rwxrwxr-x   0 ryan      (1000) ryan      (1000)     6769 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/scripts/gffutils-flybase-convert.py
+-rwxrwxr-x   0 ryan      (1000) ryan      (1000)    10532 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/scripts/gffutils-cli
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    50856 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/create.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9128 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/iterators.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2609 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/biopython_integration.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      370 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/exceptions.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2932 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/attributes.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7600 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/pybedtools_integration.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6006 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/gffwriter.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1387 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/convert.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3060 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/constants.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      329 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       14 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/version.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/gffutils/test/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      637 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/test_biopython_integration.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6813 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/expected.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    41974 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/test.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/gffutils/test/data/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      332 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gencode.vM8.chromsizes.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2506 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/dm6-chr2L.fa
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      181 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.chromsizes.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5600 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/ncbi_gff3.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      409 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/download-large-annotation-files.sh
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      743 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/c_elegans_WS199_dna_shortened.fa
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      677 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/hybrid1.gff3
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      653 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/wormbase_gff2_alt.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    65996 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.5000_gene_ids.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      534 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/jgi_gff2.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1326 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/mouse_extra_comma.gff3
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6560 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/wormbase_gff2.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)  9023416 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/dmel-all-no-analysis-r5.49_50k_lines.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1732 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/random-chr.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)   106130 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gencode.vM8.5000_gene_ids.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1793 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gff_example1.gff3
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5983 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/FBgn0031208.gtf
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      333 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gff_example1.gff3.gz
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      498 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/keep-order-test.gtf
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8407 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gencode-v19.gtf
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      385 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/glimmer_nokeyval.gff3
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    96019 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.5000_transcript_ids.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5991 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/FBgn0031208.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    18098 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/c_elegans_WS199_shortened_gff.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    17518 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/F3-unique-3.v2.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       45 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/unsanitized.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      287 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/keyval_sep_in_attrs.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)   105353 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/gencode.vM8.5000_transcript_ids.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6569 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/nonascii
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3016 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/intro_docs_example.gff
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5416 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/data/ensembl_gtf.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      145 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/data/c_elegans_WS199_ann_gff.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5273 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/parser_test.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5770 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/attr_test_cases.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1367 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/helpers_test.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7224 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/performance_test.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/test/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5714 2017-08-09 14:41:44.000000 gffutils-0.9/gffutils/test/feature_test.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    15721 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/helpers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    46819 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/interface.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    11612 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/parser.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7520 2017-08-09 14:41:43.000000 gffutils-0.9/gffutils/bins.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1076 2017-08-09 14:41:43.000000 gffutils-0.9/LICENSE
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/doc/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/doc/source/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-08-09 14:41:45.000000 gffutils-0.9/doc/source/_templates/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      527 2017-08-09 14:41:43.000000 gffutils-0.9/doc/source/_templates/class.rst
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1508 2017-08-09 14:41:44.000000 gffutils-0.9/setup.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      950 2017-08-09 14:41:45.000000 gffutils-0.9/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      706 2017-08-09 14:41:43.000000 gffutils-0.9/README.rst
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       59 2017-08-09 14:41:45.000000 gffutils-0.9/setup.cfg
```

### Comparing `gffutils-0.8.7.1/gffutils.egg-info/SOURCES.txt` & `gffutils-0.9/gffutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
+doc/source/_templates/class.rst
 gffutils/__init__.py
 gffutils/attributes.py
 gffutils/bins.py
 gffutils/biopython_integration.py
 gffutils/constants.py
 gffutils/convert.py
 gffutils/create.py
@@ -30,31 +31,42 @@
 gffutils/scripts/gffutils-flybase-convert.py
 gffutils/test/__init__.py
 gffutils/test/attr_test_cases.py
 gffutils/test/expected.py
 gffutils/test/feature_test.py
 gffutils/test/helpers_test.py
 gffutils/test/parser_test.py
+gffutils/test/performance_test.py
 gffutils/test/test.py
 gffutils/test/test_biopython_integration.py
 gffutils/test/data/F3-unique-3.v2.gff
 gffutils/test/data/FBgn0031208.gff
 gffutils/test/data/FBgn0031208.gtf
+gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.5000_gene_ids.txt
+gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.5000_transcript_ids.txt
+gffutils/test/data/Saccharomyces_cerevisiae.R64-1-1.83.chromsizes.txt
 gffutils/test/data/c_elegans_WS199_ann_gff.txt
 gffutils/test/data/c_elegans_WS199_dna_shortened.fa
 gffutils/test/data/c_elegans_WS199_shortened_gff.txt
+gffutils/test/data/dm6-chr2L.fa
 gffutils/test/data/dmel-all-no-analysis-r5.49_50k_lines.gff
+gffutils/test/data/download-large-annotation-files.sh
 gffutils/test/data/ensembl_gtf.txt
 gffutils/test/data/gencode-v19.gtf
+gffutils/test/data/gencode.vM8.5000_gene_ids.txt
+gffutils/test/data/gencode.vM8.5000_transcript_ids.txt
+gffutils/test/data/gencode.vM8.chromsizes.txt
 gffutils/test/data/gff_example1.gff3
 gffutils/test/data/gff_example1.gff3.gz
 gffutils/test/data/glimmer_nokeyval.gff3
 gffutils/test/data/hybrid1.gff3
 gffutils/test/data/intro_docs_example.gff
 gffutils/test/data/jgi_gff2.txt
+gffutils/test/data/keep-order-test.gtf
+gffutils/test/data/keyval_sep_in_attrs.gff
 gffutils/test/data/mouse_extra_comma.gff3
 gffutils/test/data/ncbi_gff3.txt
 gffutils/test/data/nonascii
 gffutils/test/data/random-chr.gff
 gffutils/test/data/unsanitized.gff
 gffutils/test/data/wormbase_gff2.txt
 gffutils/test/data/wormbase_gff2_alt.txt
```

### Comparing `gffutils-0.8.7.1/MANIFEST.in` & `gffutils-0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/inspection.py` & `gffutils-0.9/gffutils/inspection.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/feature.py` & `gffutils-0.9/gffutils/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,22 @@
             The end result is that this instance's `attributes` attribute will
             always be a dictionary.
 
             Upon printing, the attributes will be reconstructed based on this
             dictionary and the dialect -- except if the original attributes
             string was provided, in which case that will be used directly.
 
+            Notes on encoding/decoding: the only time unquoting
+            (e.g., "%2C" becomes ",") happens is if `attributes` is a string
+            and if `settings.ignore_url_escape_characters = False`. If dict or
+            JSON, the contents are used as-is.
+
+            Similarly, the only time characters are quoted ("," becomes "%2C")
+            is when the feature is printed (`__str__` method).
+
         extra : string or list
             Additional fields after the canonical 9 fields for GFF/GTF.
 
             If a string, then first assume it's serialized JSON; if this fails
             then assume it's a tab-delimited string of additional fields.  If
             it's a list already, then use as-is.
 
@@ -110,19 +118,19 @@
             feature is printed.  Mostly useful for testing, where the order is
             important for checking against expected values. Disabled by
             default, since it can be time-consuming over many features.
 
         """
         # start/end can be provided as int-like, ".", or None, but will be
         # converted to int or None
-        if start == ".":
+        if start == "." or start == "":
             start = None
         elif start is not None:
             start = int(start)
-        if end == ".":
+        if end == "." or end == "":
             end = None
         elif end is not None:
             end = int(end)
 
         # Flexible handling of attributes:
         # If dict, then use that; otherwise assume JSON and convert to a dict;
         # otherwise assume original string and convert to a dict.
@@ -220,14 +228,15 @@
     def __str__(self):
         if six.PY3:
             return self.__unicode__()
         else:
             return unicode(self).encode('utf-8')
 
     def __unicode__(self):
+
         # All fields but attributes (and extra).
         items = [getattr(self, k) for k in constants._gffkeys[:-1]]
 
         # Handle start/stop, which are either None or int
         if items[3] is None:
             items[3] = "."
         else:
@@ -260,15 +269,15 @@
     def __ne__(self, other):
         return str(self) != str(other)
 
     def __len__(self):
         return self.stop - self.start + 1
 
     # aliases for official GFF field names; this way x.chrom == x.seqid; and
-    # x.start == x.end.
+    # x.stop == x.end.
     @property
     def chrom(self):
         return self.seqid
 
     @chrom.setter
     def chrom(self, value):
         self.seqid = value
@@ -330,19 +339,22 @@
             reverse-complemented for minus-strand features.
 
         Returns
         -------
         string
         """
         if isinstance(fasta, six.string_types):
-            fasta = Fasta(fasta, as_raw=True)
+            fasta = Fasta(fasta, as_raw=False)
 
         # recall GTF/GFF is 1-based closed;  pyfaidx uses Python slice notation
         # and is therefore 0-based half-open.
-        return fasta[self.chrom][self.start-1:self.stop]
+        seq = fasta[self.chrom][self.start-1:self.stop]
+        if use_strand and self.strand == '-':
+            seq = seq.reverse.complement
+        return seq.seq
 
 
 def feature_from_line(line, dialect=None, strict=True, keep_order=False):
     """
     Given a line from a GFF file, return a Feature object
 
     Parameters
```

### Comparing `gffutils-0.8.7.1/gffutils/inspect.py` & `gffutils-0.9/gffutils/inspect.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/scripts/gffutils-flybase-convert.py` & `gffutils-0.9/gffutils/scripts/gffutils-flybase-convert.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/scripts/gffutils-cli` & `gffutils-0.9/gffutils/scripts/gffutils-cli`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/create.py` & `gffutils-0.9/gffutils/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                  default_encoding='utf-8',
                  disable_infer_genes=False,
                  disable_infer_transcripts=False,
                  infer_gene_extent=True,
                  force_merge_fields=None,
                  text_factory=sqlite3.OptimizedUnicode,
                  pragmas=constants.default_pragmas, _keep_tempfiles=False,
+                 directives=None,
                  **kwargs):
         """
         Base class for _GFFDBCreator and _GTFDBCreator; see create_db()
         function for docs
         """
         self._keep_tempfiles = _keep_tempfiles
         if force_merge_fields is None:
@@ -76,14 +77,17 @@
                     "%s field will be merged for features with the same ID; "
                     "this may result in unusable features." % w)
 
         self.force_merge_fields = force_merge_fields
         self.pragmas = pragmas
         self.merge_strategy = merge_strategy
         self.default_encoding = default_encoding
+        if directives is None:
+            directives = []
+        self.directives = directives
 
         if not infer_gene_extent:
             warnings.warn("'infer_gene_extent' will be deprecated. For now, "
                           "the following equivalent values were automatically "
                           "set: 'disable_infer_genes=True', "
                           "'disable_infer_transcripts=True'. Please use these "
                           "instead in the future.")
@@ -117,14 +121,15 @@
 
         self.iterator = iterators.DataIterator(
             data=data, checklines=checklines, transform=transform,
             force_dialect_check=force_dialect_check, from_string=from_string,
             dialect=dialect
         )
 
+
     def set_verbose(self, verbose=None):
         if verbose == 'debug':
             logger.setLevel(logging.DEBUG)
         elif verbose:
             logger.setLevel(logging.INFO)
         else:
             logger.setLevel(logging.ERROR)
@@ -435,17 +440,18 @@
         """
         Various last-minute stuff to perform after file has been parsed and
         imported.
 
         In general, if you'll be adding stuff to the meta table, do it here.
         """
         c = self.conn.cursor()
+        directives = self.directives + self.iterator.directives
         c.executemany('''
                       INSERT INTO directives VALUES (?)
-                      ''', ((i,) for i in self.iterator.directives))
+                      ''', ((i,) for i in directives))
         c.execute(
             '''
             INSERT INTO meta (version, dialect)
             VALUES (:version, :dialect)''',
             dict(version=version.version,
                  dialect=helpers._jsonify(self.iterator.dialect))
         )
@@ -468,14 +474,24 @@
         c.execute('CREATE INDEX relationsparent ON relations (parent)')
         logger.info("Creating relations(child) index")
         c.execute('DROP INDEX IF EXISTS relationschild')
         c.execute('CREATE INDEX relationschild ON relations (child)')
         logger.info("Creating features(featuretype) index")
         c.execute('DROP INDEX IF EXISTS featuretype')
         c.execute('CREATE INDEX featuretype ON features (featuretype)')
+        logger.info("Creating features (seqid, start, end) index")
+        c.execute('DROP INDEX IF EXISTS seqidstartend')
+        c.execute('CREATE INDEX seqidstartend ON features (seqid, start, end)')
+        logger.info("Creating features (seqid, start, end, strand) index")
+        c.execute('DROP INDEX IF EXISTS seqidstartendstrand')
+        c.execute('CREATE INDEX seqidstartendstrand ON features (seqid, start, end, strand)')
+
+        # speeds computation 1000x in some cases
+        logger.info("Running ANALYSE features")
+        c.execute('ANALYZE features')
 
         self.conn.commit()
 
         self.warnings = self.iterator.warnings
 
     def create(self):
         """
@@ -1100,15 +1116,15 @@
         Using `merge_strategy="error"`, a :class:`gffutils.DuplicateID`
         exception will be raised.  This means you will have to edit the file
         yourself to fix the duplicated IDs.
 
         Using `merge_strategy="warning"`, a warning will be printed to the
         logger, and the duplicate feature will be skipped.
 
-        Using `merge_strategy="replace" will replace the entire existing
+        Using `merge_strategy="replace"` will replace the entire existing
         feature with the new feature.
 
     transform : callable
 
         Function (or other callable object) that accepts a `Feature` object and
         returns a (possibly modified) `Feature` object.
 
@@ -1212,15 +1228,14 @@
         as the suffix fo the tempfile. This can be useful for testing in
         parallel environments.
 
     Returns
     -------
     New :class:`FeatureDB` object.
     """
-
     _locals = locals()
 
     # Check if any older kwargs made it in
     deprecation_handler(kwargs)
 
     kwargs = dict((i, _locals[i]) for i in constants._iterator_kwargs)
 
@@ -1231,24 +1246,24 @@
     iterator = iterators.DataIterator(**kwargs)
 
     kwargs.update(**_locals)
 
     if dialect is None:
         dialect = iterator.dialect
 
-    if isinstance(iterator, iterators._FeatureIterator):
-        # However, a side-effect of this is that  if `data` was a generator,
-        # then we've just consumed `checklines` items (see
-        # iterators.BaseIterator.__init__, which calls iterators.peek).
-        #
-        # But it also chains those consumed items back onto the beginning, and
-        # the result is available as as iterator._iter.
-        #
-        # That's what we should be using now for `data:
-        kwargs['data'] = iterator._iter
+    # However, a side-effect of this is that  if `data` was a generator, then
+    # we've just consumed `checklines` items (see
+    # iterators.BaseIterator.__init__, which calls iterators.peek).
+    #
+    # But it also chains those consumed items back onto the beginning, and the
+    # result is available as as iterator._iter.
+    #
+    # That's what we should be using now for `data:
+    kwargs['data'] = iterator._iter
+    kwargs['directives'] = iterator.directives
 
     # Since we've already checked lines, we don't want to do it again
     kwargs['checklines'] = 0
 
     if force_gff or (dialect['fmt'] == 'gff3'):
         cls = _GFFDBCreator
         id_spec = id_spec or 'ID'
```

### Comparing `gffutils-0.8.7.1/gffutils/iterators.py` & `gffutils-0.9/gffutils/iterators.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/biopython_integration.py` & `gffutils-0.9/gffutils/biopython_integration.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/attributes.py` & `gffutils-0.9/gffutils/attributes.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/pybedtools_integration.py` & `gffutils-0.9/gffutils/pybedtools_integration.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/gffwriter.py` & `gffutils-0.9/gffutils/gffwriter.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/convert.py` & `gffutils-0.9/gffutils/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 """
 Conversion functions that operate on :class:`FeatureDB` classes.
 """
 
 import six
 
-
 def to_bed12(f, db, child_type='exon', name_field='ID'):
     """
     Given a top-level feature (e.g., transcript), construct a BED12 entry
-
     Parameters
     ----------
     f : Feature object or string
         This is the top-level feature represented by one BED12 line.  For
         a canonical GFF or GTF, this will generally be a transcript.
-
     db : a FeatureDB object
         This is need to get the children for the feature
-
     child_type : str
         Featuretypes that will be represented by the BED12 "blocks".  Typically
         "exon".
-
     name_field : str
         Attribute to be used in the "name" field of the BED12 entry.  Usually
         "ID" for GFF; "transcript_id" for GTF.
     """
     if isinstance(f, six.string_types):
         f = db[f]
     children = list(db.children(f, featuretype=child_type, order_by='start'))
```

### Comparing `gffutils-0.8.7.1/gffutils/constants.py` & `gffutils-0.9/gffutils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,12 +135,13 @@
 
     # If these keys exist, then print them in this order.
     'order': ['ID', 'Name', 'gene_id', 'transcript_id'],
 
 }
 
 always_return_list = True
+ignore_url_escape_characters = False
 
 # these keyword args are used by iterators.
 _iterator_kwargs = (
     'data',
     'checklines', 'transform', 'force_dialect_check', 'dialect', 'from_string')
```

### Comparing `gffutils-0.8.7.1/gffutils/test/test_biopython_integration.py` & `gffutils-0.9/gffutils/test/test_biopython_integration.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/expected.py` & `gffutils-0.9/gffutils/test/expected.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/test.py` & `gffutils-0.9/gffutils/test/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from textwrap import dedent
 from . import expected
 from gffutils import example_filename, create, parser, feature
 import gffutils
 import gffutils.helpers as helpers
 import gffutils.gffwriter as gffwriter
 import gffutils.inspect as inspect
 import gffutils.iterators as iterators
@@ -90,28 +91,31 @@
     assert num_features == orig_num_features + 1, num_features
 
 
     # Merging while iterating.  e.g., if you're updating children with gene
     # IDs.
     db = create.create_db(example_filename('FBgn0031208.gff'), ':memory:',
                           verbose=False, force=True, keep_order=True)
-    for gene in db.features_of_type('gene'):
-        for child in list(db.children(gene)):
-            # important: the FBgn0031208.gff file was designed to have some
-            # funky features: there are two exons without ID attributes.  These
-            # are assigned to ids "exon_1" and "exon_2".  Upon update, with
-            # still no ID, we then have two new features "exon_3" and "exon_4".
-            # To prevent this issue, we ensure that the ID attribute exists...
-            child.attributes['gene_id'] = [gene.id]
-            if 'ID' not in child.attributes:
-                child.attributes['ID'] = [child.id]
-            db.update([child], merge_strategy='replace')
+    def gen():
+        for gene in db.features_of_type('gene'):
+            for child in list(db.children(gene)):
+                # important: the FBgn0031208.gff file was designed to have some
+                # funky features: there are two exons without ID attributes.  These
+                # are assigned to ids "exon_1" and "exon_2".  Upon update, with
+                # still no ID, we then have two new features "exon_3" and "exon_4".
+                # To prevent this issue, we ensure that the ID attribute exists...
+                child.attributes['gene_id'] = [gene.id]
+                if 'ID' not in child.attributes:
+                    child.attributes['ID'] = [child.id]
+                yield child
+
+    db.update(gen(), merge_strategy='replace')
 
     print("\n\nafter\n\n")
-    for child in db.children(gene):
+    for child in db.children('FBgn0031208'):
         print(child.id)
         assert child.attributes['gene_id'] == ['FBgn0031208'], (child, child.attributes)
 
     num_entries = 0
     for gene_recs in list(db.iter_by_parent_childs()):
         # Add attribute to each gene record
         rec = gene_recs[0]
@@ -194,15 +198,15 @@
             verbose=False,
             keep_order=True
         )
         self.c = self.db.conn.cursor()
         self.dialect = self.db.dialect
 
     def table_test(self):
-        expected_tables = ['features', 'relations', 'meta', 'directives', 'autoincrements', 'duplicates']
+        expected_tables = ['features', 'relations', 'meta', 'directives', 'autoincrements', 'duplicates', 'sqlite_stat1']
         self.c.execute('select name from sqlite_master where type="table"')
         observed_tables = [i[0] for i in self.c.execute('select name from sqlite_master where type="table"')]
         assert set(expected_tables) == set(observed_tables), observed_tables
 
     def _count1(self,featuretype):
         """Count using SQL"""
         self.c.execute('select count() from features where featuretype = ?',(featuretype,))
@@ -1023,14 +1027,157 @@
         gffutils.create_db(
             gffutils.example_filename('FBgn0031208.gtf'),
             ':memory:',
             infer_gene_extent=False)
         assert len(w) == 1
 
 
+# From #79
+def test_issue_79():
+    gtf = gffutils.example_filename('keep-order-test.gtf')
+    db = gffutils.create_db(gtf, 'tmp.db',
+                       disable_infer_genes=False,
+                       disable_infer_transcripts=False,
+                       id_spec={"gene": "gene_id", "transcript": "transcript_id"},
+                       merge_strategy="create_unique",
+                       keep_order=True,
+                            force=True)
+
+    exp = open(gtf).read()
+    obs = '\n'.join([str(i) for i in db.all_features()])
+    exp_1 = exp.splitlines(True)[0].strip()
+    obs_1 = obs.splitlines(True)[0].strip()
+    print('EXP')
+    print(exp_1)
+    print('OBS')
+    print(obs_1)
+    print('DIFF')
+    print(''.join(difflib.ndiff([exp_1], [obs_1])))
+    assert obs_1 == exp_1
+
+def test_for_analyze():
+    db = gffutils.create_db(
+            gffutils.example_filename('FBgn0031208.gtf'),
+            'deleteme',
+            force=True
+    )
+    assert db._analyzed()
+    db.execute('DROP TABLE sqlite_stat1')
+    assert not db._analyzed()
+
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        db2 = gffutils.FeatureDB('deleteme')
+        assert len(w) == 1
+        assert "analyze" in str(w[-1].message)
+    db.analyze()
+    assert db._analyzed()
+    os.unlink('deleteme')
+
+
+def test_issue_82():
+    # key-val separator is inside an unquoted attribute value
+    x = (
+        'Spenn-ch12\tsgn_markers\tmatch\t2621812\t2622049\t.\t+\t.\t'
+        'Alias=SGN-M1347;ID=T0028;Note=marker name(s): T0028 SGN-M1347 |identity=99.58|escore=2e-126'
+    )
+    y = feature.feature_from_line(x)
+    assert y.attributes['Note'] == ['marker name(s): T0028 SGN-M1347 |identity=99.58|escore=2e-126']
+
+    gffutils.create_db(gffutils.example_filename('keyval_sep_in_attrs.gff'), ':memory:')
+
+def test_sequence():
+    fasta = gffutils.example_filename('dm6-chr2L.fa')
+    f = feature.feature_from_line(
+        'chr2L	FlyBase	gene	154	170	.	+	.	ID=one;')
+    seq = f.sequence(fasta)
+    assert seq == 'aCGAGATGATAATATAT'
+    assert len(seq) == len(f)
+    f.strand = '-'
+    seq = f.sequence(fasta)
+    assert seq == 'ATATATTATCATCTCGt'
+    assert len(seq) == len(f)
+
+def test_issue_85():
+    # when start or stop was empty, #85 would fail Should now work with
+    # blank fields
+    f = feature.feature_from_line('\t'.join([''] * 9))
+
+    # or with "." placeholders
+    f = feature.feature_from_line('\t'.join(['.'] * 9))
+
+
+def test_unquoting():
+    # incoming is encoded
+    s = (
+        'chr1\tAUGUSTUS\tgene\t6950084\t6951407\t0.26\t-\t.\t'
+        'ID=INIL01g00009;GeneSymbol=Ndufaf6;Note=NADH dehydrogenase '
+        '(ubiquinone) complex I%2C assembly factor 6;GO_Terms=GO:0005743|'
+        'GO:0016740|GO:0009058|GO:0032981;PFam=PF00494'
+    )
+    f = feature.feature_from_line(s, keep_order=True)
+
+    # string representation should be identical
+    assert str(f) == s
+
+    # accessing attribute should be decoded
+    n = f['Note']
+    assert n == ['NADH dehydrogenase (ubiquinone) complex I, assembly factor 6']
+
+
+def test_unreasonable_unquoting():
+    s = (
+        'chr1\t.\t.\t1\t2\t0.26\t-\t.\t'
+        'newline=%0A;'
+        'percent=%25;'
+        'null=%00;'
+        'comma=%2C;'
+
+        # The first parent is "A," (A with a comma), the second is "B%"
+        'Parent=A%2C,B%25,C;'
+    )
+    f = feature.feature_from_line(s, keep_order=True)
+    assert f.attributes['newline'][0] == '\n'
+    assert f.attributes['percent'][0] == '%'
+    assert f.attributes['null'][0] == '\x00'
+    assert f.attributes['comma'][0] == ','
+
+    # Commas indicate 
+    assert f.attributes['Parent'] == ['A,', 'B%', 'C']
+    assert str(f) == s
+
+
+def test_unquoting_iter():
+    s = 'chr1\t.\tgene\t1\t2\t.\t-\t.\tID=%2C;'
+    tmp = tempfile.NamedTemporaryFile(delete=False).name
+    with open(tmp, 'w') as fout:
+        fout.write(s + '\n')
+    assert list(gffutils.iterators.DataIterator(tmp))[0]['ID'][0] == ','
+
+def test_db_unquoting():
+    s = dedent(
+        '''
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=a;Note=%2C;
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=b;Note=%2C;
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=c;Note=%2C;
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=d;Note=%2C;
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=e;Note=%2C;
+        chr1\t.\tgene\t1\t2\t.\t-\t.\tID=f;Note=%2C;
+        ''')
+    tmp = tempfile.NamedTemporaryFile(delete=False).name
+    with open(tmp, 'w') as fout:
+        fout.write(s + '\n')
+    db = gffutils.create_db(tmp, ':memory:', checklines=1)
+    assert db['a']['Note'] == [',']
+    assert db['b']['Note'] == [',']
+    assert db['c']['Note'] == [',']
+    assert db['d']['Note'] == [',']
+    assert db['e']['Note'] == [',']
+    assert db['f']['Note'] == [',']
+
 if __name__ == "__main__":
     # this test case fails
     #test_attributes_modify()
     #test_sanitize_gff()
     #test_random_chr()
     #test_nonascii()
     test_iterator_update()
```

### Comparing `gffutils-0.8.7.1/gffutils/test/data/ncbi_gff3.txt` & `gffutils-0.9/gffutils/test/data/ncbi_gff3.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/c_elegans_WS199_dna_shortened.fa` & `gffutils-0.9/gffutils/test/data/c_elegans_WS199_dna_shortened.fa`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/hybrid1.gff3` & `gffutils-0.9/gffutils/test/data/hybrid1.gff3`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/wormbase_gff2_alt.txt` & `gffutils-0.9/gffutils/test/data/wormbase_gff2_alt.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/jgi_gff2.txt` & `gffutils-0.9/gffutils/test/data/jgi_gff2.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/mouse_extra_comma.gff3` & `gffutils-0.9/gffutils/test/data/mouse_extra_comma.gff3`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/wormbase_gff2.txt` & `gffutils-0.9/gffutils/test/data/wormbase_gff2.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/dmel-all-no-analysis-r5.49_50k_lines.gff` & `gffutils-0.9/gffutils/test/data/dmel-all-no-analysis-r5.49_50k_lines.gff`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/random-chr.gff` & `gffutils-0.9/gffutils/test/data/random-chr.gff`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/gff_example1.gff3` & `gffutils-0.9/gffutils/test/data/gff_example1.gff3`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/FBgn0031208.gtf` & `gffutils-0.9/gffutils/test/data/FBgn0031208.gtf`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/gencode-v19.gtf` & `gffutils-0.9/gffutils/test/data/gencode-v19.gtf`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/FBgn0031208.gff` & `gffutils-0.9/gffutils/test/data/FBgn0031208.gff`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/c_elegans_WS199_shortened_gff.txt` & `gffutils-0.9/gffutils/test/data/c_elegans_WS199_shortened_gff.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/F3-unique-3.v2.gff` & `gffutils-0.9/gffutils/test/data/F3-unique-3.v2.gff`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/nonascii` & `gffutils-0.9/gffutils/test/data/nonascii`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/intro_docs_example.gff` & `gffutils-0.9/gffutils/test/data/intro_docs_example.gff`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/data/ensembl_gtf.txt` & `gffutils-0.9/gffutils/test/data/ensembl_gtf.txt`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/parser_test.py` & `gffutils-0.9/gffutils/test/parser_test.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/attr_test_cases.py` & `gffutils-0.9/gffutils/test/attr_test_cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,20 @@
              'Locuslink:2688',
              'Genbank-mRNA:A00469',
              'Swissprot:P01241',
              'PFAM:PF00103',
              'AFFX-U95:1332_f_at',
              'Swissprot:SOMA_HUMAN',
          ],
-         'Note': ['growth%20hormone%201'],
+         'Note': ['growth hormone 1'],
          'Alias': ['GH1']},
 
-        None,
+        'ID=A00469;Dbxref=AFFX-U133:205840_x_at,Locuslink:2688,Genbank-mRNA:'
+        'A00469,Swissprot:P01241,PFAM:PF00103,AFFX-U95:1332_f_at,Swissprot:'
+        'SOMA_HUMAN;Note=growth hormone 1;Alias=GH1',
     ),
 
     # jgi_gff2.txt
     #
     # This file is inconsitent with how it quotes values -- integers are not
     # quoted but string values are.  Only way to make this be invariant is to
     # keep track of the "flavor" of each attribute; not sure it's worth the
@@ -153,25 +155,30 @@
         'rotein_id=YP_885468.1;db_xref=GI:118469242;db_xref=GeneID:4535378;'
         'exon_number=1',
 
         {'ID': ['NC_008596.1:speB:unknown_transcript_1'],
          'Parent': ['NC_008596.1:speB'],
          'locus_tag': ['MSMEG_1072'],
          'EC_number': ['3.5.3.11'],
-         'note': ['identified%20by%20match%20to%20protein%20family%20HMM%20P'
-                  'F00491%3B%20match%20to%20protein%20family%20HMM%20TIGR01'
+         'note': ['identified by match to protein family HMM P'
+                  'F00491; match to protein family HMM TIGR01'
                   '230'],
          'transl_table': ['11'],
          'product': ['agmatinase'],
          'protein_id': ['YP_885468.1'],
          'db_xref': ['GI:118469242', 'GeneID:4535378'],
          'exon_number': ['1'],
          },
 
-        None,
+        'ID=NC_008596.1:speB:unknown_transcript_1;Parent=NC_008596.1:speB;'
+        'locus_tag=MSMEG_1072;EC_number=3.5.3.11;note=identified by mat'
+        'ch to protein family HMM PF00491%3B match to prote'
+        'in family HMM TIGR01230;transl_table=11;product=agmatinase;p'
+        'rotein_id=YP_885468.1;db_xref=GI:118469242;db_xref=GeneID:4535378;'
+        'exon_number=1',
     ),
 
     # wormbase_gff2_alt.txt
     #
     (
         'CDS "cr01.sctg102.wum.2.1"',
```

### Comparing `gffutils-0.8.7.1/gffutils/test/helpers_test.py` & `gffutils-0.9/gffutils/test/helpers_test.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/test/feature_test.py` & `gffutils-0.9/gffutils/test/feature_test.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/helpers.py` & `gffutils-0.9/gffutils/helpers.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/gffutils/interface.py` & `gffutils-0.9/gffutils/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import six
 import sqlite3
 import shutil
+import warnings
 from gffutils import bins
 from gffutils import helpers
 from gffutils import constants
 from gffutils.feature import Feature
 from gffutils.exceptions import FeatureNotFoundError
 
 
@@ -146,14 +147,23 @@
             '''
             SELECT base, n FROM autoincrements
             ''')
         self._autoincrements = dict(c)
 
         self.set_pragmas(pragmas)
 
+        if not self._analyzed():
+            warnings.warn(
+                "It appears that this database has not had the ANALYZE "
+                "sqlite3 command run on it. Doing so can dramatically "
+                "speed up queries, and is done by default for databases "
+                "created with gffutils >0.8.7.1 (this database was "
+                "created with version %s) Consider calling the analyze() "
+                "method of this object." % self.version)
+
     def set_pragmas(self, pragmas):
         """
         Set pragmas for the current database connection.
 
         Parameters
         ----------
         pragmas : dict
@@ -174,14 +184,22 @@
         Returns a feature, adding additional database-specific defaults
         """
         kwargs.setdefault('dialect', self.dialect)
         kwargs.setdefault('keep_order', self.keep_order)
         kwargs.setdefault('sort_attribute_values', self.sort_attribute_values)
         return Feature(**kwargs)
 
+    def _analyzed(self):
+        res = self.execute(
+            """
+            SELECT name FROM sqlite_master WHERE type='table'
+            AND name='sqlite_stat1';
+            """)
+        return len(list(res)) == 1
+
     def schema(self):
         """
         Returns the database schema as a string.
         """
         c = self.conn.cursor()
         c.execute(
             '''
@@ -438,14 +456,22 @@
         Returns
         -------
         A sqlite3.Cursor object that can be iterated over.
         """
         c = self.conn.cursor()
         return c.execute(query)
 
+    def analyze(self):
+        """
+        Runs the sqlite ANALYZE command to potentially speed up queries
+        dramatically.
+        """
+        self.execute('ANALYZE features')
+        self.conn.commit()
+
     def region(self, region=None, seqid=None, start=None, end=None,
                strand=None, featuretype=None, completely_within=False):
         """
         Return features within specified genomic coordinates.
 
         Specifying genomic coordinates can be done in a flexible manner
```

### Comparing `gffutils-0.8.7.1/gffutils/parser.py` & `gffutils-0.9/gffutils/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,81 @@
 # Portions copied over from BCBio.GFF.GFFParser
 
 import re
 import copy
+import collections
+from six.moves import urllib
 from gffutils import constants
 from gffutils.exceptions import AttributeStringError
 
 import logging
 
 formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 gff3_kw_pat = re.compile('\w+=')
 
+# Encoding/decoding notes
+# -----------------------
+# From
+# https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md#description-of-the-format:
+#
+#       GFF3 files are nine-column, tab-delimited, plain text files.
+#       Literal use of tab, newline, carriage return, the percent (%) sign,
+#       and control characters must be encoded using RFC 3986
+#       Percent-Encoding; no other characters may be encoded. Backslash and
+#       other ad-hoc escaping conventions that have been added to the GFF
+#       format are not allowed. The file contents may include any character
+#       in the set supported by the operating environment, although for
+#       portability with other systems, use of Latin-1 or Unicode are
+#       recommended.
+#
+#           tab (%09)
+#           newline (%0A)
+#           carriage return (%0D)
+#           % percent (%25)
+#           control characters (%00 through %1F, %7F)
+#
+#       In addition, the following characters have reserved meanings in
+#       column 9 and must be escaped when used in other contexts:
+#
+#           ; semicolon (%3B)
+#           = equals (%3D)
+#           & ampersand (%26)
+#           , comma (%2C)
+#
+#
+# See also issue #98.
+#
+# Note that spaces are NOT encoded. Some GFF files have spaces encoded; in
+# these cases round-trip invariance will not hold since the %20 will be decoded
+# but not re-encoded.
+_to_quote = '\n\t\r%;=&,'
+_to_quote += ''.join([chr(i) for i in range(32)])
+_to_quote += chr(127)
+
+
+# Caching idea from urllib.parse.Quoter, which uses a defaultdict for
+# efficiency. Here we're sort of doing the reverse of the "reserved" idea used
+# there.
+class Quoter(collections.defaultdict):
+    def __missing__(self, b):
+        if b in _to_quote:
+            res = '%{:02X}'.format(ord(b))
+        else:
+            res = b
+        self[b] = res
+        return res
+
+quoter = Quoter()
+
 
 def _reconstruct(keyvals, dialect, keep_order=False,
                  sort_attribute_values=False):
     """
     Reconstructs the original attributes string according to the dialect.
 
     Parameters
@@ -42,25 +98,35 @@
     """
     if not dialect:
         raise AttributeStringError()
     if not keyvals:
         return ""
     parts = []
 
+    # Re-encode when reconstructing attributes
+    if constants.ignore_url_escape_characters or dialect['fmt'] != 'gff3':
+        attributes = keyvals
+    else:
+        attributes = {}
+        for k, v in keyvals.items():
+            attributes[k] = []
+            for i in v:
+                attributes[k].append(''.join([quoter[j] for j in i]))
+
     # May need to split multiple values into multiple key/val pairs
     if dialect['repeated keys']:
         items = []
-        for key, val in keyvals.items():
+        for key, val in attributes.items():
             if len(val) > 1:
                 for v in val:
                     items.append((key, [v]))
             else:
                 items.append((key, val))
     else:
-        items = list(keyvals.items())
+        items = list(attributes.items())
 
     def sort_key(x):
         # sort keys by their order in the dialect; anything not in there will
         # be in arbitrary order at the end.
         try:
             return dialect['order'].index(x[0])
         except ValueError:
@@ -83,15 +149,18 @@
                 # Surround with quotes if needed
                 if dialect['quoted GFF2 values']:
                     val_str = '"%s"' % val_str
 
                 # Typically "=" for GFF3 or " " otherwise
                 part = dialect['keyval separator'].join([key, val_str])
         else:
-            part = key
+            if dialect['fmt'] == 'gtf':
+                part = dialect['keyval separator'].join([key, '""'])
+            else:
+                part = key
         parts.append(part)
 
     # Typically ";" or "; "
     parts_str = dialect['field separator'].join(parts)
 
     # Sometimes need to add this
     if dialect['trailing semicolon']:
@@ -112,14 +181,27 @@
     Lots of logic here to handle all the corner cases.
 
     If `dialect` is None, then do all the logic to infer a dialect from this
     attribute string.
 
     Otherwise, use the provided dialect (and return it at the end).
     """
+
+    def _unquote_quals(quals, dialect):
+        """
+        Handles the unquoting (decoding) of percent-encoded characters.
+
+        See notes on encoding/decoding above.
+        """
+        if not constants.ignore_url_escape_characters and dialect['fmt'] == 'gff3':
+            for key, vals in quals.items():
+                unquoted = [urllib.parse.unquote(v) for v in vals]
+                quals[key] = unquoted
+        return quals
+
     infer_dialect = False
     if dialect is None:
         # Make a copy of default dialect so it can be modified as needed
         dialect = copy.copy(constants.dialect)
         infer_dialect = True
     from gffutils import feature
     quals = feature.dict_class()
@@ -156,19 +238,22 @@
         quoted = dialect['quoted GFF2 values']
         for item in key_vals:
             # Easy if it follows spec
             if len(item) == 2:
                 key, val = item
 
             # Only key provided?
-            else:
-                assert len(item) == 1, item
+            elif len(item) == 1:
                 key = item[0]
                 val = ''
 
+            else:
+                key = item[0]
+                val = dialect['keyval separator'].join(item[1:])
+
             try:
                 quals[key]
             except KeyError:
                 quals[key] = []
 
             if quoted:
                 if (len(val) > 0 and val[0] == '"' and val[-1] == '"'):
@@ -177,14 +262,15 @@
             if val:
                 # TODO: if there are extra commas for a value, just use empty
                 # strings
                 # quals[key].extend([v for v in val.split(',') if v])
                 vals = val.split(',')
                 quals[key].extend(vals)
 
+        quals = _unquote_quals(quals, dialect)
         return quals, dialect
 
     # If we got here, then we need to infer the dialect....
     #
     # Reset the order to an empty list so that it will only be populated with
     # keys that are found in the file.
     dialect['order'] = []
@@ -225,18 +311,24 @@
     for item in key_vals:
 
         # Easy if it follows spec
         if len(item) == 2:
             key, val = item
 
         # Only key provided?
+        elif len(item) == 1:
+                key = item[0]
+                val = ''
+
+        # Pathological cases where values of a key have within them the key-val
+        # separator, e.g.,
+        #  Alias=SGN-M1347;ID=T0028;Note=marker name(s): T0028 SGN-M1347 |identity=99.58|escore=2e-126
         else:
-            assert len(item) == 1, item
             key = item[0]
-            val = ''
+            val = dialect['keyval separator'].join(item[1:])
 
         # Is the key already in there?
         if key in quals:
             dialect['repeated keys'] = True
         else:
             quals[key] = []
 
@@ -254,33 +346,15 @@
                     "Internally inconsistent attributes formatting: "
                     "some have repeated keys, some do not.")
             quals[key].extend(vals)
 
         # keep track of the order of keys
         dialect['order'].append(key)
 
-    #for key, vals in quals.items():
-    #
-        # TODO: urllib.unquote breaks round trip invariance for "hybrid1.gff3"
-        # test file.  This is because the "Note" field has %xx escape chars,
-        # but "Dbxref" has ":" which, if everything were consistent, should
-        # have also been escaped.
-        #
-        # (By the way, GFF3 spec says only literal use of \t, \n, \r, %, and
-        # control characters should be encoded)
-        #
-        # Solution 1: don't unquote
-        # Solution 2: store, along with each attribute, whether or not it
-        #             should be quoted later upon reconstruction
-        # Solution 3: don't care about invariance
-
-        # unquoted = [urllib.unquote(v) for v in vals]
-
-        #quals[key] = vals
-
     if (
         (dialect['keyval separator'] == ' ') and
         (dialect['quoted GFF2 values'])
     ):
         dialect['fmt'] = 'gtf'
 
+    quals = _unquote_quals(quals, dialect)
     return quals, dialect
```

### Comparing `gffutils-0.8.7.1/gffutils/bins.py` & `gffutils-0.9/gffutils/bins.py`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/LICENSE` & `gffutils-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gffutils-0.8.7.1/setup.py` & `gffutils-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,24 @@
     scripts=['gffutils/scripts/gffutils-cli'],
     author='Ryan Dale',
     package_dir={'gffutils': 'gffutils'},
     package_data = {'gffutils': ['test/data/*']},
     description="Work with GFF and GTF files in a flexible "
     "database framework",
     author_email='dalerr@niddk.nih.gov',
-    url='none',
+    url='https://github.com/daler/gffutils',
     classifiers=[
         'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: GNU General Public License (GPL)',
+        'License :: OSI Approved :: MIT License',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `gffutils-0.8.7.1/README.rst` & `gffutils-0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 .. image:: https://badge.fury.io/py/gffutils.svg
     :target: http://badge.fury.io/py/gffutils
 
 .. image:: https://pypip.in/d/gffutils/badge.png
     :target: https://pypi.python.org/pypi/gffutils
 
 
-See docs at http://daler.github.io/gffutils.
 
 ``gffutils`` is a Python package for working with and manipulating the GFF and
 GTF format files typically used for genomic annotations.  Files are loaded into
 a sqlite3 database, allowing much more complex manipulation of hierarchical
 features (e.g., genes, transcripts, and exons) than is possible with plain-text
 methods alone.
+
+See documentation at **http://daler.github.io/gffutils**.
```

