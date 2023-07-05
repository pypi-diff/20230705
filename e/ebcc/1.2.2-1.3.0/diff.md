# Comparing `tmp/ebcc-1.2.2.tar.gz` & `tmp/ebcc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebcc-1.2.2.tar", last modified: Mon Jun 26 10:45:21 2023, max compression
+gzip compressed data, was "ebcc-1.3.0.tar", last modified: Wed Jul  5 18:02:30 2023, max compression
```

## Comparing `ebcc-1.2.2.tar` & `ebcc-1.3.0.tar`

### file list

```diff
@@ -1,105 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:45:21.111140 ebcc-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-26 10:45:21.111140 ebcc-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 10:44:49.000000 ebcc-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:45:21.091140 ebcc-1.2.2/ebcc/
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/ansatz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/brueckner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:45:21.107140 ebcc-1.2.2/ebcc/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)    90928 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)   372119 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSDTQ.py
--rw-r--r--   0 runner    (1001) docker     (123)    62920 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    84310 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    59435 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/GQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)    67025 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)    76198 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)   374219 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)    85622 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)   108143 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    82752 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    52559 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/RQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)   126372 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)   103569 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)   364753 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)   551371 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)   269935 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)   327657 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)   264194 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)   130503 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/UQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/eris.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/fock.py
--rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/gebcc.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    69098 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/rebcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/reom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    31845 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/uebcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/ueom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27074 2023-06-26 10:44:49.000000 ebcc-1.2.2/ebcc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:45:21.095140 ebcc-1.2.2/ebcc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-26 10:45:21.000000 ebcc-1.2.2/ebcc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-26 10:45:21.000000 ebcc-1.2.2/ebcc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:45:21.000000 ebcc-1.2.2/ebcc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 10:45:21.000000 ebcc-1.2.2/ebcc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:45:21.000000 ebcc-1.2.2/ebcc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-26 10:44:49.000000 ebcc-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:45:21.111140 ebcc-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:45:21.111140 ebcc-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSDTQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_GQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_RQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCC2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCC3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCD.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSDT.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSD_SD_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSD_SD_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSD_S_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UCCSDxTx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UMP2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_UQCISD.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_brueckner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-26 10:44:49.000000 ebcc-1.2.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:30.271359 ebcc-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-05 18:02:30.271359 ebcc-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-05 18:01:57.000000 ebcc-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:30.255359 ebcc-1.3.0/ebcc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/ansatz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/brueckner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:30.263359 ebcc-1.3.0/ebcc/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90928 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   372119 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSDTQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62920 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84310 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59435 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61785 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/GQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67025 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76198 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)   374219 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85622 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108143 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82752 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135353 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52559 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/RQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126372 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103569 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364753 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551371 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269935 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)   327657 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264194 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)   562100 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130503 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/UQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/eris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/gebcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71774 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/rebcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/reom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33619 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/uebcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/ueom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29462 2023-07-05 18:01:57.000000 ebcc-1.3.0/ebcc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:30.255359 ebcc-1.3.0/ebcc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-05 18:02:30.000000 ebcc-1.3.0/ebcc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-05 18:02:30.000000 ebcc-1.3.0/ebcc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:02:30.000000 ebcc-1.3.0/ebcc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 18:02:30.000000 ebcc-1.3.0/ebcc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 18:02:30.000000 ebcc-1.3.0/ebcc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-05 18:01:57.000000 ebcc-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:02:30.271359 ebcc-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:30.271359 ebcc-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSDTQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_GQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_RQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCC2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCC3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSD_SD_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSD_SD_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSD_S_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSDtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UCCSDxTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UMP2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_UQCISD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_brueckner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-05 18:01:57.000000 ebcc-1.3.0/tests/test_util.py
```

### Comparing `ebcc-1.2.2/PKG-INFO` & `ebcc-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcc
-Version: 1.2.2
+Version: 1.3.0
 Summary: Coupled cluster calculations on electron-boson systems
 Keywords: quantum,chemistry,electronic,structure,coupled,cluster,electron,boson,ccsd
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
```

### Comparing `ebcc-1.2.2/README.md` & `ebcc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/__init__.py` & `ebcc-1.3.0/ebcc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 >>> mf = scf.RHF(mol)
 >>> mf.kernel()
 >>> ccsd = EBCC(mf)
 >>> ccsd.kernel()
 
 """
 
-__version__ = "1.2.2"
+__version__ = "1.3.0"
 
 import logging
 import os
 import subprocess
 import sys
 
 # --- Logging:
```

### Comparing `ebcc-1.2.2/ebcc/ansatz.py` & `ebcc-1.3.0/ebcc/ansatz.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "CCSD": ("CCSD", "", 0, 0),
     "CCSDT": ("CCSDT", "", 0, 0),
     "CCSDTQ": ("CCSDTQ", "", 0, 0),
     "CCSD(T)": ("CCSD(T)", "", 0, 0),
     "CC2": ("CC2", "", 0, 0),
     "CC3": ("CC3", "", 0, 0),
     "QCISD": ("QCISD", "", 0, 0),
+    "CCSDt'": ("CCSDt'", "", 0, 0),
     "CCSD-S-1-1": ("CCSD", "S", 1, 1),
     "CCSD-SD-1-1": ("CCSD", "SD", 1, 1),
     "CCSD-SD-1-2": ("CCSD", "SD", 1, 2),
 }
 
 
 def name_to_identifier(name):
@@ -33,14 +34,15 @@
     >>> identifier_to_name("CCSD-SD-1-2")
     CCSD_SD_1_2
     """
 
     iden = name.replace("(", "x").replace(")", "x")
     iden = iden.replace("[", "y").replace("]", "y")
     iden = iden.replace("-", "_")
+    iden = iden.replace("'", "p")
 
     return iden
 
 
 def identifity_to_name(iden):
     """Convert an ansatz identifier to a name.
 
@@ -51,14 +53,15 @@
     """
 
     name = iden.replace("-", "_")
     while "x" in name:
         name = name.replace("x", "(", 1).replace("x", ")", 1)
     while "y" in name:
         name = name.replace("y", "(", 1).replace("y", ")", 1)
+    name = name.replace("p", "'")
 
     return name
 
 
 class Ansatz:
     """Ansatz class.
 
@@ -169,128 +172,141 @@
             calculation.
         """
         return all(
             ansatz.startswith("MP") or ansatz == ""
             for ansatz in (self.fermion_ansatz, self.boson_ansatz)
         )
 
-    @property
-    def correlated_cluster_ranks(self):
-        """Get a list of cluster operator rank numbers for each of
-        the fermionic, bosonic, and coupling ansatzes, for the
-        correlated space (see space.py).
+    def fermionic_cluster_ranks(self, spin_type="G"):
+        """Get a list of cluster operator ranks for the fermionic
+        space.
 
         Returns
         -------
-        ranks : tuple of tuple of int
-            Cluster operator ranks for the fermionic, bosonic, and
-            coupling ansatzes, for the correlated space.
+        ranks : list of tuples
+            List of cluster operator ranks, each element is a tuple
+            containing the name, the slices and the rank.
         """
 
         ranks = []
+        if not self.fermion_ansatz:
+            return ranks
 
         notations = {
-            "S": [1],
-            "D": [2],
-            "T": [3],
-            "Q": [4],
-            "2": [1, 2],
-            "3": [1, 2, 3],
-            "4": [1, 2, 3, 4],
+            "S": [("t1", "ov", 1)],
+            "D": [("t2", "oovv", 2)],
+            "T": [("t3", "ooovvv", 3)],
+            "t'": [("t3", "OOOVVV", 3)],
         }
-
-        for i, op in enumerate([self.fermion_ansatz, self.boson_ansatz]):
-            # Remove any perturbative corrections
-            while "(" in op:
-                start = op.index("(")
-                end = op.index(")")
-                op = op[:start]
-                if (end + 1) < len(op):
-                    op += op[end + 1 :]
-
-            # Check in order of longest -> shortest string in case
-            # one method name starts with a substring equal to the
-            # name of another method
-            if i == 0:
-                for method_type in sorted(METHOD_TYPES, key=len)[::-1]:
-                    if op.startswith(method_type):
-                        op = op.lstrip(method_type)
-                        break
-
-            # If it's Moller-Plesset perturbation theory, we only
-            # need to initialise second-order amplitudes
-            if method_type == "MP":
-                op = "D"
-
-            # Remove any lower case characters, as these correspond
-            # to active space
-            op = "".join([char for char in op if char.isupper() or char.isnumeric()])
-
-            # Determine the ranks
-            ranks_entry = set()
-            for char in op:
-                for rank in notations[char]:
-                    ranks_entry.add(rank)
-            ranks.append(tuple(sorted(list(ranks_entry))))
-
-        # Get the coupling ranks
-        for op in [self.fermion_coupling_rank, self.boson_coupling_rank]:
-            ranks.append(tuple(range(1, op + 1)))
-
-        return tuple(ranks)
-
-    @property
-    def active_cluster_ranks(self):
-        """Get a list of cluster operator rank numbers for each of
-        the fermionic, bosonic, and coupling ansatzes, for the
-        active space (see space.py).
+        if spin_type == "R":
+            notations["Q"] = [("t4a", "oooovvvv", 4), ("t4b", "oooovvvv", 4)]
+        else:
+            notations["Q"] = [("t4", "oooovvvv", 4)]
+        notations["2"] = notations["S"] + notations["D"]
+        notations["3"] = notations["2"] + notations["T"]
+        notations["4"] = notations["3"] + notations["Q"]
+
+        # Remove any perturbative corrections
+        op = self.fermion_ansatz
+        while "(" in op:
+            start = op.index("(")
+            end = op.index(")")
+            op = op[:start]
+            if (end + 1) < len(op):
+                op += op[end + 1 :]
+
+        # Check in order of longest to shortest string in case one
+        # method name starts with a substring equal to the name of
+        # another method
+        for method_type in sorted(METHOD_TYPES, key=len)[::-1]:
+            if op.startswith(method_type):
+                op = op.lstrip(method_type)
+                break
+
+        # If it's MP we only ever need to initialise second-order
+        # amplitudes
+        if method_type == "MP":
+            op = "D"
+
+        # Determine the ranks
+        for key in sorted(notations.keys(), key=len)[::-1]:
+            if key in op:
+                ranks += notations[key]
+                op = op.replace(key, "")
+
+        # Check there are no duplicates
+        if len(ranks) != len(set(ranks)):
+            raise util.ModelNotImplemented("Duplicate ranks in %s" % self.fermion_ansatz)
+
+        # Sort the ranks by the cluster operator dimension
+        ranks = sorted(ranks, key=lambda x: x[2])
+
+        return ranks
+
+    def bosonic_cluster_ranks(self, spin_type="G"):
+        """Get a list of cluster operator ranks for the bosonic
+        space.
 
         Returns
         -------
-        ranks : tuple of tuple of int
-            Cluster operator ranks for the fermionic, bosonic, and
-            coupling ansatzes, for the active space.
+        ranks : list of tuples
+            List of cluster operator ranks, each element is a tuple
+            containing the name, the slices and the rank.
         """
 
         ranks = []
+        if not self.boson_ansatz:
+            return ranks
 
         notations = {
-            "s": [1],
-            "d": [2],
-            "t": [3],
-            "q": [4],
+            "S": [("s1", "b", 1)],
+            "D": [("s2", "bb", 2)],
+            "T": [("s3", "bbb", 3)],
         }
+        notations["2"] = notations["S"] + notations["D"]
+        notations["3"] = notations["2"] + notations["T"]
+
+        # Remove any perturbative corrections
+        op = self.boson_ansatz
+        while "(" in op:
+            start = op.index("(")
+            end = op.index(")")
+            op = op[:start]
+            if (end + 1) < len(op):
+                op += op[end + 1 :]
+
+        # Determine the ranks
+        for key in sorted(notations.keys(), key=len)[::-1]:
+            if key in op:
+                ranks += notations[key]
+                op = op.replace(key, "")
+
+        # Check there are no duplicates
+        if len(ranks) != len(set(ranks)):
+            raise util.ModelNotImplemented("Duplicate ranks in %s" % self.boson_ansatz)
+
+        # Sort the ranks by the cluster operator dimension
+        ranks = sorted(ranks, key=lambda x: x[2])
+
+        return ranks
+
+    def coupling_cluster_ranks(self, spin_type="G"):
+        """Get a list of cluster operator ranks for the coupling
+        between fermionic and bosonic spaces.
+
+        Returns
+        -------
+        ranks : list of tuple
+            List of cluster operator ranks, each element is a tuple
+            containing the name, slice, fermionic rank and bosonic
+            rank.
+        """
+
+        ranks = []
 
-        for i, op in enumerate([self.fermion_ansatz, self.boson_ansatz]):
-            # Remove any perturbative corrections
-            while "(" in op:
-                start = op.index("(")
-                end = op.index(")")
-                op = op[:start]
-                if (end + 1) < len(op):
-                    op += op[end + 1 :]
-
-            # Check in order of longest -> shortest string in case
-            # one method name starts with a substring equal to the
-            # name of another method
-            if i == 0:
-                for method_type in sorted(METHOD_TYPES, key=len)[::-1]:
-                    if op.startswith(method_type):
-                        op = op.lstrip(method_type)
-                        break
-
-            # Remove any lower case characters, as these correspond
-            # to active space
-            op = "".join([char for char in op if char.islower()])
-
-            # Determine the ranks
-            ranks_entry = set()
-            for char in op:
-                for rank in notations[char]:
-                    ranks_entry.add(rank)
-            ranks.append(tuple(sorted(list(ranks_entry))))
-
-        # Get the coupling ranks
-        # FIXME how to handle? if it's ever supported
-        ranks.append(tuple())
+        for fermion_rank in range(1, self.fermion_coupling_rank + 1):
+            for boson_rank in range(1, self.boson_coupling_rank + 1):
+                name = f"u{fermion_rank}{boson_rank}"
+                key = "b" * boson_rank + "o" * fermion_rank + "v" * fermion_rank
+                ranks.append((name, key, fermion_rank, boson_rank))
 
-        return tuple(ranks)
+        return ranks
```

### Comparing `ebcc-1.2.2/ebcc/brueckner.py` & `ebcc-1.3.0/ebcc/brueckner.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,29 +126,29 @@
             amplitudes = self.cc.amplitudes
 
         nocc = self.cc.space.ncocc
         ci = u[:nocc, :nocc]
         ca = u[nocc:, nocc:]
 
         # Transform T amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[0]:
-            args = [self.cc.amplitudes["t%d" % n], tuple(range(n * 2))]
+        for name, key, n in self.cc.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            args = [self.cc.amplitudes[name], tuple(range(n * 2))]
             for i in range(n):
                 args += [ci, (i, i + n * 2)]
             for i in range(n):
                 args += [ca, (i + n, i + n * 3)]
             args += [tuple(range(n * 2, n * 4))]
-            self.cc.amplitudes["t%d" % n] = util.einsum(*args)
+            self.cc.amplitudes[name] = util.einsum(*args)
 
         # Transform S amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.cc.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented  # TODO
 
         # Transform U amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.cc.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented  # TODO
 
         return self.cc.amplitudes
 
     def get_t1_norm(self, amplitudes=None):
         """Get the norm of the T1 amplitude."""
 
@@ -260,14 +260,18 @@
         self.cc.log.debug("")
         self.cc.log.debug("Time elapsed: %s", timer.format_time(timer()))
         self.cc.log.debug("")
         self.cc.log.debug("")
 
         return self.cc.e_corr
 
+    @property
+    def spin_type(self):
+        return self.cc.spin_type
+
 
 @util.inherit_docstrings
 class BruecknerUEBCC(BruecknerREBCC):
     def get_rotation_matrix(self, u_tot=None, diis=None, t1=None):
         if t1 is None:
             t1 = self.cc.t1
         if u_tot is None:
@@ -331,30 +335,30 @@
             amplitudes = self.cc.amplitudes
 
         nocc = (self.cc.space[0].ncocc, self.cc.space[1].ncocc)
         ci = {"a": u[0][: nocc[0], : nocc[0]], "b": u[1][: nocc[1], : nocc[1]]}
         ca = {"a": u[0][nocc[0] :, nocc[0] :], "b": u[1][nocc[1] :, nocc[1] :]}
 
         # Transform T amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.cc.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             for comb in util.generate_spin_combinations(n, unique=True):
-                args = [getattr(self.cc.amplitudes["t%d" % n], comb), tuple(range(n * 2))]
+                args = [getattr(self.cc.amplitudes[name], comb), tuple(range(n * 2))]
             for i in range(n):
                 args += [ci[comb[i]], (i, i + n * 2)]
             for i in range(n):
                 args += [ca[comb[i + n]], (i + n, i + n * 3)]
             args += [tuple(range(n * 2, n * 4))]
-            setattr(self.cc.amplitudes["t%d" % n], comb, util.einsum(*args))
+            setattr(self.cc.amplitudes[name], comb, util.einsum(*args))
 
         # Transform S amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.cc.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented  # TODO
 
         # Transform U amplitudes:
-        for n in self.cc.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.cc.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented  # TODO
 
         return self.cc.amplitudes
 
     def get_t1_norm(self, amplitudes=None):
         if amplitudes is None:
             amplitudes = self.cc.amplitudes
```

### Comparing `ebcc-1.2.2/ebcc/codegen/GCC2.py` & `ebcc-1.3.0/ebcc/codegen/GCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCC3.py` & `ebcc-1.3.0/ebcc/codegen/GCC3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCD.py` & `ebcc-1.3.0/ebcc/codegen/GCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSD.py` & `ebcc-1.3.0/ebcc/codegen/GCCSD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSDT.py` & `ebcc-1.3.0/ebcc/codegen/GCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSDTQ.py` & `ebcc-1.3.0/ebcc/codegen/GCCSDTQ.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSD_SD_1_1.py` & `ebcc-1.3.0/ebcc/codegen/GCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSD_SD_1_2.py` & `ebcc-1.3.0/ebcc/codegen/GCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSD_S_1_1.py` & `ebcc-1.3.0/ebcc/codegen/GCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GCCSDxTx.py` & `ebcc-1.3.0/ebcc/codegen/GCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GMP3.py` & `ebcc-1.3.0/ebcc/codegen/GMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/GQCISD.py` & `ebcc-1.3.0/ebcc/codegen/GQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCC2.py` & `ebcc-1.3.0/ebcc/codegen/RCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCC3.py` & `ebcc-1.3.0/ebcc/codegen/RCC3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCD.py` & `ebcc-1.3.0/ebcc/codegen/RCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSD.py` & `ebcc-1.3.0/ebcc/codegen/RCCSD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSDT.py` & `ebcc-1.3.0/ebcc/codegen/RCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSD_SD_1_1.py` & `ebcc-1.3.0/ebcc/codegen/RCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSD_SD_1_2.py` & `ebcc-1.3.0/ebcc/codegen/RCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSD_S_1_1.py` & `ebcc-1.3.0/ebcc/codegen/RCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RCCSDxTx.py` & `ebcc-1.3.0/ebcc/codegen/RCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RMP3.py` & `ebcc-1.3.0/ebcc/codegen/RMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/RQCISD.py` & `ebcc-1.3.0/ebcc/codegen/RQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCC2.py` & `ebcc-1.3.0/ebcc/codegen/UCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCC3.py` & `ebcc-1.3.0/ebcc/codegen/UCC3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCD.py` & `ebcc-1.3.0/ebcc/codegen/UCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSD.py` & `ebcc-1.3.0/ebcc/codegen/UCCSD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSDT.py` & `ebcc-1.3.0/ebcc/codegen/UCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSD_SD_1_1.py` & `ebcc-1.3.0/ebcc/codegen/UCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSD_SD_1_2.py` & `ebcc-1.3.0/ebcc/codegen/UCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSD_S_1_1.py` & `ebcc-1.3.0/ebcc/codegen/UCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UCCSDxTx.py` & `ebcc-1.3.0/ebcc/codegen/UCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UMP3.py` & `ebcc-1.3.0/ebcc/codegen/UMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/codegen/UQCISD.py` & `ebcc-1.3.0/ebcc/codegen/UQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/dump.py` & `ebcc-1.3.0/ebcc/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,42 +101,48 @@
             kwargs["converged"] = ebcc.converged
         if ebcc.converged_lambda is not None:
             kwargs["converged_lambda"] = ebcc.converged_lambda
         dump(self.name, "misc", kwargs)
 
         # Write the amplitudes
         if ebcc.spin_type == "U":
-            dump(
-                self.name,
-                "amplitudes",
-                {
-                    key: ({**val} if isinstance(val, (util.Namespace, dict)) else val)
-                    for key, val in ebcc.amplitudes.items()
-                },
-            )
-            dump(
-                self.name,
-                "lambdas",
-                {
-                    key: ({**val} if isinstance(val, (util.Namespace, dict)) else val)
-                    for key, val in ebcc.lambdas.items()
-                },
-            )
+            if ebcc.amplitudes is not None:
+                dump(
+                    self.name,
+                    "amplitudes",
+                    {
+                        key: ({**val} if isinstance(val, (util.Namespace, dict)) else val)
+                        for key, val in ebcc.amplitudes.items()
+                    },
+                )
+            if ebcc.lambdas is not None:
+                dump(
+                    self.name,
+                    "lambdas",
+                    {
+                        key: ({**val} if isinstance(val, (util.Namespace, dict)) else val)
+                        for key, val in ebcc.lambdas.items()
+                    },
+                )
         else:
-            dump(self.name, "amplitudes", {**ebcc.amplitudes})
-            dump(self.name, "lambdas", {**ebcc.lambdas})
+            if ebcc.amplitudes is not None:
+                dump(self.name, "amplitudes", {**ebcc.amplitudes})
+            if ebcc.lambdas is not None:
+                dump(self.name, "lambdas", {**ebcc.lambdas})
 
     def read(self, cls: Type[util.AbstractEBCC], log: logging.Logger = None):
         """
         Load the file to an EBCC object.
         """
 
         # Load the options
         dic = load(self.name, "options")
-        options = cls.Options(**dic)
+        options = cls.Options()
+        for key, val in dic.items():
+            setattr(options, key, val)
 
         # Load the miscellaneous data
         misc = load(self.name, "misc")
         spin_type = misc.pop("spin_type").decode("ascii")
 
         # Load the mean-field data
         mf_cls = {"G": scf.GHF, "U": scf.UHF, "R": scf.RHF}[spin_type]
```

### Comparing `ebcc-1.2.2/ebcc/eris.py` & `ebcc-1.3.0/ebcc/eris.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 self.__dict__[key] = block
             return self.__dict__[key]
         else:
             slices = []
             for i, k in enumerate(key):
                 slices.append(self.slices[i][k])
             si, sj, sk, sl = slices
-            block = self.array[si, sj, sk, sl]
+            block = self.array[si][:, sj][:, :, sk][:, :, :, sl]
             return block
 
 
 class UERIs(util.Namespace):
     """
     Electronic repulsion integral container class for `UEBCC`. Consists
     of a namespace of `REBCC` objects, one for each spin signature.
```

### Comparing `ebcc-1.2.2/ebcc/fock.py` & `ebcc-1.3.0/ebcc/fock.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def __getattr__(self, key):
         """Just-in-time attribute getter."""
 
         if key not in self.__dict__.keys():
             ki, kj = key
             i = self.slices[0][ki]
             j = self.slices[1][kj]
-            self.__dict__[key] = self.array[i, j].copy()
+            self.__dict__[key] = self.array[i][:, j].copy()
 
             if self.shift:
                 xi = self.xi
                 g = self.g.__getattr__(f"b{ki}{kj}")
                 g += self.g.__getattr__(f"b{kj}{ki}").transpose(0, 2, 1)
                 self.__dict__[key] -= util.einsum("I,Ipq->pq", xi, g)
```

### Comparing `ebcc-1.2.2/ebcc/gebcc.py` & `ebcc-1.3.0/ebcc/gebcc.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,45 +43,48 @@
         # RHF->GHF and UHF->GHF may have inconsistent ordering
         return mf.to_uhf().to_ghf()
 
     @classmethod
     def from_uebcc(cls, ucc):
         """Initialise a GEBCC object from an UEBCC object."""
 
-        # FIXME test for frozen/active
         orbspin = scf.addons.get_ghf_orbspin(ucc.mf.mo_energy, ucc.mf.mo_occ, False)
-        nocc = sum(ucc.nocc)
-        nvir = sum(ucc.nvir)
+        nocc = ucc.space[0].nocc + ucc.space[1].nocc
+        nvir = ucc.space[0].nvir + ucc.space[1].nvir
         nbos = ucc.nbos
-        slices = {"a": np.where(orbspin == 0)[0], "b": np.where(orbspin == 1)[0]}
-        occs = {"a": np.where(orbspin[:nocc] == 0)[0], "b": np.where(orbspin[:nocc] == 1)[0]}
-        virs = {"a": np.where(orbspin[nocc:] == 0)[0], "b": np.where(orbspin[nocc:] == 1)[0]}
+        sa = np.where(orbspin == 0)[0]
+        sb = np.where(orbspin == 1)[0]
+
+        occupied = np.zeros((nocc + nvir,), dtype=bool)
+        occupied[sa] = ucc.space[0]._occupied.copy()
+        occupied[sb] = ucc.space[1]._occupied.copy()
+        frozen = np.zeros((nocc + nvir,), dtype=bool)
+        frozen[sa] = ucc.space[0]._frozen.copy()
+        frozen[sb] = ucc.space[1]._frozen.copy()
+        active = np.zeros((nocc + nvir,), dtype=bool)
+        active[sa] = ucc.space[0]._active.copy()
+        active[sb] = ucc.space[1]._active.copy()
+        space = Space(occupied, frozen, active)
+
+        slices = util.Namespace(
+            a=util.Namespace(**{k: np.where(orbspin[space.mask(k)] == 0)[0] for k in "oOivVa"}),
+            b=util.Namespace(**{k: np.where(orbspin[space.mask(k)] == 1)[0] for k in "oOivVa"}),
+        )
 
         if ucc.bare_g is not None:
             if np.asarray(ucc.bare_g).ndim == 3:
                 bare_g_a = bare_g_b = ucc.bare_g
             else:
                 bare_g_a, bare_g_b = ucc.bare_g
             g = np.zeros((ucc.nbos, ucc.nmo * 2, ucc.nmo * 2))
-            g[np.ix_(range(ucc.nbos), slices["a"], slices["a"])] = bare_g_a.copy()
-            g[np.ix_(range(ucc.nbos), slices["b"], slices["b"])] = bare_g_b.copy()
+            g[np.ix_(range(ucc.nbos), sa, sa)] = bare_g_a.copy()
+            g[np.ix_(range(ucc.nbos), sb, sb)] = bare_g_b.copy()
         else:
             g = None
 
-        occupied = np.zeros((nocc + nvir,), dtype=bool)
-        occupied[slices["a"]] = ucc.space[0]._occupied.copy()
-        occupied[slices["b"]] = ucc.space[1]._occupied.copy()
-        frozen = np.zeros((nocc + nvir,), dtype=bool)
-        frozen[slices["a"]] = ucc.space[0]._frozen.copy()
-        frozen[slices["b"]] = ucc.space[1]._frozen.copy()
-        active = np.zeros((nocc + nvir,), dtype=bool)
-        active[slices["a"]] = ucc.space[0]._active.copy()
-        active[slices["b"]] = ucc.space[1]._active.copy()
-        space = Space(occupied, frozen, active)
-
         gcc = cls(
             ucc.mf,
             log=ucc.log,
             ansatz=ucc.ansatz,
             space=space,
             omega=ucc.omega,
             g=g,
@@ -95,166 +98,150 @@
 
         has_amps = ucc.amplitudes is not None
         has_lams = ucc.lambdas is not None
 
         if has_amps:
             amplitudes = cls.Amplitudes()
 
-            for n in ucc.ansatz.correlated_cluster_ranks[0]:
-                amplitudes["t%d" % n] = np.zeros((space.ncocc,) * n + (space.ncvir,) * n)
+            for name, key, n in ucc.ansatz.fermionic_cluster_ranks(spin_type=ucc.spin_type):
+                shape = tuple(space.size(k) for k in key)
+                amplitudes[name] = np.zeros(shape)
                 for comb in util.generate_spin_combinations(n, unique=True):
                     done = set()
                     for lperm, lsign in util.permutations_with_signs(tuple(range(n))):
                         for uperm, usign in util.permutations_with_signs(tuple(range(n))):
                             combn = util.permute_string(comb[:n], lperm)
                             combn += util.permute_string(comb[n:], uperm)
                             if combn in done:
                                 continue
-                            mask = np.ix_(
-                                *([occs[c] for c in combn[:n]] + [virs[c] for c in combn[n:]])
-                            )
+                            mask = np.ix_(*[slices[s][k] for s, k in zip(combn, key)])
                             transpose = tuple(lperm) + tuple(p + n for p in uperm)
                             amp = (
-                                getattr(ucc.amplitudes["t%d" % n], comb).transpose(transpose)
+                                getattr(ucc.amplitudes[name], comb).transpose(transpose)
                                 * lsign
                                 * usign
                             )
                             for perm, sign in util.permutations_with_signs(tuple(range(n))):
                                 transpose = tuple(perm) + tuple(range(n, 2 * n))
                                 if util.permute_string(comb[:n], perm) == comb[:n]:
-                                    amplitudes["t%d" % n][mask] += (
-                                        amp.transpose(transpose).copy() * sign
-                                    )
+                                    amplitudes[name][mask] += amp.transpose(transpose).copy() * sign
                             done.add(combn)
 
-            for n in ucc.ansatz.correlated_cluster_ranks[1]:
-                amplitudes["s%d" % n] = ucc.amplitudes["s%d" % n].copy()
+            for name, key, n in ucc.ansatz.bosonic_cluster_ranks(spin_type=ucc.spin_type):
+                amplitudes[name] = ucc.amplitudes[name].copy()
 
-            for nf in ucc.ansatz.correlated_cluster_ranks[2]:
-                for nb in ucc.ansatz.correlated_cluster_ranks[3]:
-                    amplitudes["u%d%d" % (nf, nb)] = np.zeros(
-                        (nbos,) * nb + (space.ncocc,) * nf + (space.ncvir,) * nf
-                    )
-                    for comb in util.generate_spin_combinations(nf):
-                        done = set()
-                        for lperm, lsign in util.permutations_with_signs(tuple(range(nf))):
-                            for uperm, usign in util.permutations_with_signs(tuple(range(nf))):
-                                combn = util.permute_string(comb[:nf], lperm)
-                                combn += util.permute_string(comb[nf:], uperm)
-                                if combn in done:
-                                    continue
-                                mask = np.ix_(
-                                    *([range(nbos)] * nb),
-                                    *(
-                                        [occs[c] for c in combn[:nf]]
-                                        + [virs[c] for c in combn[nf:]]
-                                    ),
-                                )
+            for name, key, nf, nb in ucc.ansatz.coupling_cluster_ranks(spin_type=ucc.spin_type):
+                shape = (nbos,) * nb + tuple(space.size(k) for k in key[nb:])
+                amplitudes[name] = np.zeros(shape)
+                for comb in util.generate_spin_combinations(nf):
+                    done = set()
+                    for lperm, lsign in util.permutations_with_signs(tuple(range(nf))):
+                        for uperm, usign in util.permutations_with_signs(tuple(range(nf))):
+                            combn = util.permute_string(comb[:nf], lperm)
+                            combn += util.permute_string(comb[nf:], uperm)
+                            if combn in done:
+                                continue
+                            mask = np.ix_(
+                                *([range(nbos)] * nb),
+                                *[slices[s][k] for s, k in zip(combn, key[nb:])],
+                            )
+                            transpose = (
+                                tuple(range(nb))
+                                + tuple(p + nb for p in lperm)
+                                + tuple(p + nb + nf for p in uperm)
+                            )
+                            amp = (
+                                getattr(ucc.amplitudes[name], comb).transpose(transpose)
+                                * lsign
+                                * usign
+                            )
+                            for perm, sign in util.permutations_with_signs(tuple(range(nf))):
                                 transpose = (
                                     tuple(range(nb))
-                                    + tuple(p + nb for p in lperm)
-                                    + tuple(p + nb + nf for p in uperm)
+                                    + tuple(p + nb for p in perm)
+                                    + tuple(range(nb + nf, nb + 2 * nf))
                                 )
-                                amp = (
-                                    getattr(ucc.amplitudes["u%d%d" % (nf, nb)], comb).transpose(
-                                        transpose
-                                    )
-                                    * lsign
-                                    * usign
-                                )
-                                for perm, sign in util.permutations_with_signs(tuple(range(nf))):
-                                    transpose = (
-                                        tuple(range(nb))
-                                        + tuple(p + nb for p in perm)
-                                        + tuple(range(nb + nf, nb + 2 * nf))
-                                    )
-                                    if util.permute_string(comb[:nf], perm) == comb[:nf]:
-                                        amplitudes["u%d%d" % (nf, nb)][mask] += (
-                                            amp.transpose(transpose).copy() * sign
-                                        )
-                                done.add(combn)
+                                if util.permute_string(comb[:nf], perm) == comb[:nf]:
+                                    amplitudes[name][mask] += amp.transpose(transpose).copy() * sign
+                            done.add(combn)
 
             gcc.amplitudes = amplitudes
 
         if has_lams:
             lambdas = gcc.init_lams()  # Easier this way - but have to build ERIs...
 
-            for n in ucc.ansatz.correlated_cluster_ranks[0]:
-                lambdas["l%d" % n] = np.zeros((space.ncvir,) * n + (space.ncocc,) * n)
+            for name, key, n in ucc.ansatz.fermionic_cluster_ranks(spin_type=ucc.spin_type):
+                lname = name.replace("t", "l")
+                shape = tuple(space.size(k) for k in key[n:] + key[:n])
+                lambdas[lname] = np.zeros(shape)
                 for comb in util.generate_spin_combinations(n, unique=True):
                     done = set()
                     for lperm, lsign in util.permutations_with_signs(tuple(range(n))):
                         for uperm, usign in util.permutations_with_signs(tuple(range(n))):
                             combn = util.permute_string(comb[:n], lperm)
                             combn += util.permute_string(comb[n:], uperm)
                             if combn in done:
                                 continue
-                            mask = np.ix_(
-                                *([virs[c] for c in combn[:n]] + [occs[c] for c in combn[n:]])
-                            )
+                            mask = np.ix_(*[slices[s][k] for s, k in zip(combn, key[n:] + key[:n])])
                             transpose = tuple(lperm) + tuple(p + n for p in uperm)
                             amp = (
-                                getattr(ucc.lambdas["l%d" % n], comb).transpose(transpose)
+                                getattr(ucc.lambdas[lname], comb).transpose(transpose)
                                 * lsign
                                 * usign
                             )
                             for perm, sign in util.permutations_with_signs(tuple(range(n))):
                                 transpose = tuple(perm) + tuple(range(n, 2 * n))
                                 if util.permute_string(comb[:n], perm) == comb[:n]:
-                                    lambdas["l%d" % n][mask] += (
-                                        amp.transpose(transpose).copy() * sign
-                                    )
+                                    lambdas[lname][mask] += amp.transpose(transpose).copy() * sign
                             done.add(combn)
 
-            for n in ucc.ansatz.correlated_cluster_ranks[1]:
-                lambdas["ls%d" % n] = ucc.lambdas["ls%d" % n].copy()
-
-            for nf in ucc.ansatz.correlated_cluster_ranks[2]:
-                for nb in ucc.ansatz.correlated_cluster_ranks[3]:
-                    lambdas["lu%d%d" % (nf, nb)] = np.zeros(
-                        (nbos,) * nb + (space.ncvir,) * nf + (space.ncocc,) * nf
-                    )
-                    for comb in util.generate_spin_combinations(nf, unique=True):
-                        done = set()
-                        for lperm, lsign in util.permutations_with_signs(tuple(range(nf))):
-                            for uperm, usign in util.permutations_with_signs(tuple(range(nf))):
-                                combn = util.permute_string(comb[:nf], lperm)
-                                combn += util.permute_string(comb[nf:], uperm)
-                                if combn in done:
-                                    continue
-                                mask = np.ix_(
-                                    *([range(nbos)] * nb),
-                                    *(
-                                        [virs[c] for c in combn[:nf]]
-                                        + [occs[c] for c in combn[nf:]]
-                                    ),
-                                )
+            for name, key, n in ucc.ansatz.bosonic_cluster_ranks(spin_type=ucc.spin_type):
+                lname = "l" + name
+                lambdas[lname] = ucc.lambdas[lname].copy()
+
+            for name, key, nf, nb in ucc.ansatz.coupling_cluster_ranks(spin_type=ucc.spin_type):
+                lname = "l" + name
+                shape = (nbos,) * nb + tuple(
+                    space.size(k) for k in key[nb + nf :] + key[nb : nb + nf]
+                )
+                lambdas[lname] = np.zeros(shape)
+                for comb in util.generate_spin_combinations(nf, unique=True):
+                    done = set()
+                    for lperm, lsign in util.permutations_with_signs(tuple(range(nf))):
+                        for uperm, usign in util.permutations_with_signs(tuple(range(nf))):
+                            combn = util.permute_string(comb[:nf], lperm)
+                            combn += util.permute_string(comb[nf:], uperm)
+                            if combn in done:
+                                continue
+                            mask = np.ix_(
+                                *([range(nbos)] * nb),
+                                *[
+                                    slices[s][k]
+                                    for s, k in zip(combn, key[nb + nf :] + key[nb : nb + nf])
+                                ],
+                            )
+                            transpose = (
+                                tuple(range(nb))
+                                + tuple(p + nb for p in lperm)
+                                + tuple(p + nb + nf for p in uperm)
+                            )
+                            amp = (
+                                getattr(ucc.lambdas[lname], comb).transpose(transpose)
+                                * lsign
+                                * usign
+                            )
+                            for perm, sign in util.permutations_with_signs(tuple(range(nf))):
                                 transpose = (
                                     tuple(range(nb))
-                                    + tuple(p + nb for p in lperm)
-                                    + tuple(p + nb + nf for p in uperm)
-                                )
-                                amp = (
-                                    getattr(ucc.lambdas["lu%d%d" % (nf, nb)], comb).transpose(
-                                        transpose
-                                    )
-                                    * lsign
-                                    * usign
+                                    + tuple(p + nb for p in perm)
+                                    + tuple(range(nb + nf, nb + 2 * nf))
                                 )
-                                for perm, sign in util.permutations_with_signs(tuple(range(nf))):
-                                    transpose = (
-                                        tuple(range(nb))
-                                        + tuple(p + nb for p in perm)
-                                        + tuple(range(nb + nf, nb + 2 * nf))
-                                    )
-                                    if util.permute_string(comb[:nf], perm) == comb[:nf]:
-                                        lambdas["lu%d%d" % (nf, nb)][mask] += (
-                                            amp.transpose(transpose).copy() * sign
-                                        )
-                                done.add(combn)
+                                if util.permute_string(comb[:nf], perm) == comb[:nf]:
+                                    lambdas[lname][mask] += amp.transpose(transpose).copy() * sign
+                            done.add(combn)
 
             gcc.lambdas = lambdas
 
         return gcc
 
     @classmethod
     def from_rebcc(cls, rcc):
@@ -263,52 +250,61 @@
         ucc = uebcc.UEBCC.from_rebcc(rcc)
         gcc = cls.from_uebcc(ucc)
 
         return gcc
 
     def init_amps(self, eris=None):
         eris = self.get_eris(eris)
-
         amplitudes = self.Amplitudes()
-        e_ia = lib.direct_sum("i-a->ia", self.eo, self.ev)
 
         # Build T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
-                amplitudes["t%d" % n] = self.fock.vo.T / e_ia
+                ei = getattr(self, "e" + key[0])
+                ea = getattr(self, "e" + key[1])
+                e_ia = lib.direct_sum("i-a->ia", ei, ea)
+                amplitudes[name] = getattr(self.fock, key) / e_ia
             elif n == 2:
-                e_ijab = lib.direct_sum("ia,jb->ijab", e_ia, e_ia)
-                amplitudes["t%d" % n] = eris.oovv / e_ijab
+                ei = getattr(self, "e" + key[0])
+                ej = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                eb = getattr(self, "e" + key[3])
+                e_ia = lib.direct_sum("i-a->ia", ei, ea)
+                e_jb = lib.direct_sum("i-a->ia", ej, eb)
+                e_ijab = lib.direct_sum("ia,jb->ijab", e_ia, e_jb)
+                amplitudes[name] = getattr(eris, key) / e_ijab
             else:
-                amplitudes["t%d" % n] = np.zeros((self.space.ncocc,) * n + (self.space.ncvir,) * n)
+                shape = tuple(self.space.size(k) for k in key)
+                amplitudes[name] = np.zeros(shape)
 
         if self.boson_ansatz:
             # Only true for real-valued couplings:
             h = self.g
             H = self.G
 
         # Build S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
-                amplitudes["s%d" % n] = -H / self.omega
+                amplitudes[name] = -H / self.omega
             else:
-                amplitudes["s%d" % n] = np.zeros((self.nbos,) * n)
+                shape = (self.nbos,) * n
+                amplitudes[name] = np.zeros(shape)
 
         # Build U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                if n == 1:
-                    e_xia = lib.direct_sum("ia-x->xia", e_ia, self.omega)
-                    amplitudes["u%d%d" % (nf, nb)] = h.bov / e_xia
-                else:
-                    amplitudes["u%d%d" % (nf, nb)] = np.zeros(
-                        (self.nbos,) * nb + (self.space.ncocc, self.space.ncvir)
-                    )
+            if n == 1:
+                ei = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                e_xia = lib.direct_sum("i-a-x->xia", ei, ea, self.omega)
+                amplitudes[name] = getattr(h, key) / e_xia
+            else:
+                shape = (self.nbos,) * nb + tuple(self.space.size(k) for k in key[nb:])
+                amplitudes[name] = np.zeros(shape)
 
         return amplitudes
 
     def make_rdm2_f(self, eris=None, amplitudes=None, lambdas=None, hermitise=True):
         func, kwargs = self._load_function(
             "make_rdm2_f",
             eris=eris,
@@ -324,109 +320,102 @@
 
         return dm
 
     def excitations_to_vector_ip(self, *excitations):
         vectors = []
         m = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            subscript = "i" * n + "a" * (n - 1)
-            vectors.append(util.compress_axes(subscript, excitations[m]).ravel())
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[:-1]
+            vectors.append(util.compress_axes(key, excitations[m]).ravel())
             m += 1
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return np.concatenate(vectors)
 
     def excitations_to_vector_ee(self, *excitations):
         vectors = []
         m = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            subscript = "i" * n + "a" * n
-            vectors.append(util.compress_axes(subscript, excitations[m]).ravel())
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(util.compress_axes(key, excitations[m]).ravel())
             m += 1
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return np.concatenate(vectors)
 
     def vector_to_excitations_ip(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            subscript = "i" * n + "a" * (n - 1)
-            size = util.get_compressed_size(subscript, i=self.space.ncocc, a=self.space.ncvir)
-            shape = tuple([self.space.ncocc] * n + [self.space.ncvir] * (n - 1))
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[:-1]
+            size = util.get_compressed_size(key, **{k: self.space.size(k) for k in set(key)})
+            shape = tuple(self.space.size(k) for k in key)
             vn_tril = vector[i0 : i0 + size]
-            vn = util.decompress_axes(subscript, vn_tril, shape=shape)
+            vn = util.decompress_axes(key, vn_tril, shape=shape)
             excitations.append(vn)
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def vector_to_excitations_ea(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            subscript = "a" * n + "i" * (n - 1)
-            size = util.get_compressed_size(subscript, i=self.space.ncocc, a=self.space.ncvir)
-            shape = tuple([self.space.ncvir] * n + [self.space.ncocc] * (n - 1))
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[n:] + key[: n - 1]
+            size = util.get_compressed_size(key, **{k: self.space.size(k) for k in set(key)})
+            shape = tuple(self.space.size(k) for k in key)
             vn_tril = vector[i0 : i0 + size]
-            vn = util.decompress_axes(subscript, vn_tril, shape=shape)
+            vn = util.decompress_axes(key, vn_tril, shape=shape)
             excitations.append(vn)
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def vector_to_excitations_ee(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            subscript = "i" * n + "a" * n
-            size = util.get_compressed_size(subscript, i=self.space.ncocc, a=self.space.ncvir)
-            shape = tuple([self.space.ncocc] * n + [self.space.ncvir] * n)
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            size = util.get_compressed_size(key, **{k: self.space.size(k) for k in set(key)})
+            shape = tuple(self.space.size(k) for k in key)
             vn_tril = vector[i0 : i0 + size]
-            vn = util.decompress_axes(subscript, vn_tril, shape=shape)
+            vn = util.decompress_axes(key, vn_tril, shape=shape)
             excitations.append(vn)
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def get_mean_field_G(self):
         val = lib.einsum("Ipp->I", self.g.boo)
         val -= self.xi * self.omega
```

### Comparing `ebcc-1.2.2/ebcc/geom.py` & `ebcc-1.3.0/ebcc/geom.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/ebcc/rebcc.py` & `ebcc-1.3.0/ebcc/rebcc.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # TODO test bosonic RDMs and lambdas - only regression atm
 # TODO math in docstrings
 # TODO resolve G vs bare_G confusion
 # TODO warnings if amplitudes/lambdas are not converged when calling i.e. DM funcs
 # TODO update docstrings
 # TODO orbspin with cluster spaces?
 # TODO fix TensorSymm and benchmark third order again
+# TODO active spaces for IP/EA
 
 
 class Amplitudes(util.Namespace):
     """Amplitude container class. Consists of a dictionary with keys
     that are strings of the name of each amplitude, and values are
     arrays whose dimension depends on the particular amplitude.
     """
@@ -286,15 +287,15 @@
         self._mo_occ = mo_occ
 
         # Ansatz:
         if isinstance(ansatz, Ansatz):
             self.ansatz = ansatz
         else:
             self.ansatz = Ansatz.from_string(ansatz)
-        self._eqns = self.ansatz._get_eqns(self.__class__.__name__[0])
+        self._eqns = self.ansatz._get_eqns(self.spin_type)
 
         # Space:
         if space is not None:
             self.space = space
         else:
             self.space = self.init_space()
 
@@ -588,25 +589,28 @@
 
         return func, kwargs
 
     def _pack_codegen_kwargs(self, *extra_kwargs, eris=None):
         """Pack all the possible keyword arguments for generated code
         into a dictionary.
         """
+        # TODO change all APIs to take the space object instead of
+        # nocc, nvir, nbos, etc.
 
         eris = self.get_eris(eris)
 
         omega = np.diag(self.omega) if self.omega is not None else None
 
         kwargs = dict(
             f=self.fock,
             v=eris,
             g=self.g,
             G=self.G,
             w=omega,
+            space=self.space,
             nocc=self.space.ncocc,  # FIXME rename?
             nvir=self.space.ncvir,  # FIXME rename?
             nbos=self.nbos,
         )
         for kw in extra_kwargs:
             if kw is not None:
                 kwargs.update(kw)
@@ -643,52 +647,62 @@
         Returns
         -------
         amplitudes : Amplitudes
             Cluster amplitudes.
         """
 
         eris = self.get_eris(eris)
-
         amplitudes = self.Amplitudes()
-        e_ia = lib.direct_sum("i-a->ia", self.eo, self.ev)
 
         # Build T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
-                amplitudes["t%d" % n] = self.fock.vo.T / e_ia
+                ei = getattr(self, "e" + key[0])
+                ea = getattr(self, "e" + key[1])
+                e_ia = lib.direct_sum("i-a->ia", ei, ea)
+                amplitudes[name] = getattr(self.fock, key) / e_ia
             elif n == 2:
-                e_ijab = lib.direct_sum("ia,jb->ijab", e_ia, e_ia)
-                amplitudes["t%d" % n] = eris.ovov.swapaxes(1, 2) / e_ijab
+                ei = getattr(self, "e" + key[0])
+                ej = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                eb = getattr(self, "e" + key[3])
+                e_ia = lib.direct_sum("i-a->ia", ei, ea)
+                e_jb = lib.direct_sum("i-a->ia", ej, eb)
+                e_ijab = lib.direct_sum("ia,jb->ijab", e_ia, e_jb)
+                key_t = key[0] + key[2] + key[1] + key[3]
+                amplitudes[name] = getattr(eris, key_t).swapaxes(1, 2) / e_ijab
             else:
-                amplitudes["t%d" % n] = np.zeros((self.space.ncocc,) * n + (self.space.ncvir,) * n)
+                shape = tuple(self.space.size(k) for k in key)
+                amplitudes[name] = np.zeros(shape)
 
         if self.boson_ansatz:
             # Only true for real-valued couplings:
             h = self.g
             H = self.G
 
         # Build S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
-                amplitudes["s%d" % n] = -H / self.omega
+                amplitudes[name] = -H / self.omega
             else:
-                amplitudes["s%d" % n] = np.zeros((self.nbos,) * n)
+                shape = (self.nbos,) * n
+                amplitudes[name] = np.zeros(shape)
 
         # Build U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                if nb == 1:
-                    e_xia = lib.direct_sum("ia-x->xia", e_ia, self.omega)
-                    amplitudes["u%d%d" % (nf, nb)] = h.bov / e_xia
-                else:
-                    amplitudes["u%d%d" % (nf, nb)] = np.zeros(
-                        (self.nbos,) * nb + (self.space.ncocc, self.space.ncvir)
-                    )
+            if nb == 1:
+                ei = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                e_xia = lib.direct_sum("i-a-x->xia", ei, ea, self.omega)
+                amplitudes[name] = getattr(h, key) / e_xia
+            else:
+                shape = (self.nbos,) * nb + tuple(self.space.size(k) for k in key[nb:])
+                amplitudes[name] = np.zeros(shape)
 
         return amplitudes
 
     def init_lams(self, amplitudes=None):
         """Initialise the lambda amplitudes.
 
         Parameters
@@ -701,33 +715,34 @@
         -------
         lambdas : Amplitudes
             Updated cluster lambda amplitudes.
         """
 
         if amplitudes is None:
             amplitudes = self.amplitudes
-
         lambdas = self.Amplitudes()
 
         # Build L amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
             perm = list(range(n, 2 * n)) + list(range(n))
-            lambdas["l%d" % n] = amplitudes["t%d" % n].transpose(perm)
+            lambdas[lname] = amplitudes[name].transpose(perm)
 
         # Build LS amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            lambdas["ls%d" % n] = amplitudes["s%d" % n]
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            lname = "l" + name
+            lambdas[lname] = amplitudes[name]
 
         # Build LU amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                perm = list(range(nb)) + [nb + 1, nb]
-                lambdas["lu%d%d" % (nf, nb)] = amplitudes["u%d%d" % (nf, nb)].transpose(perm)
+            lname = "l" + name
+            perm = list(range(nb)) + [nb + 1, nb]
+            lambdas[lname] = amplitudes[name].transpose(perm)
 
         return lambdas
 
     def energy(self, eris=None, amplitudes=None):
         """Compute the correlation energy.
 
         Parameters
@@ -802,38 +817,49 @@
             "update_amps",
             eris=eris,
             amplitudes=amplitudes,
         )
         res = func(**kwargs)
         res = {key.rstrip("new"): val for key, val in res.items()}
 
-        e_ia = lib.direct_sum("i-a->ia", self.eo, self.ev)
-
         # Divide T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             perm = list(range(0, n * 2, 2)) + list(range(1, n * 2, 2))
-            d = functools.reduce(np.add.outer, [e_ia] * n)
+            e_ia_list = [
+                lib.direct_sum("i-a->ia", getattr(self, "e" + o), getattr(self, "e" + v))
+                for o, v in zip(key[:n], key[n:])
+            ]
+            d = functools.reduce(np.add.outer, e_ia_list)
             d = d.transpose(perm)
-            res["t%d" % n] /= d
-            res["t%d" % n] += amplitudes["t%d" % n]
+            res[name] /= d
+            res[name] += amplitudes[name]
 
         # Divide S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             d = functools.reduce(np.add.outer, ([-self.omega] * n))
-            res["s%d" % n] /= d
-            res["s%d" % n] += amplitudes["s%d" % n]
+            res[name] /= d
+            res[name] += amplitudes[name]
 
         # Divide U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ia] * nf))
-                res["u%d%d" % (nf, nb)] /= d
-                res["u%d%d" % (nf, nb)] += amplitudes["u%d%d" % (nf, nb)]
+            perm = (
+                list(range(nb))
+                + list(range(nb, nf * 2 + nb, 2))
+                + list(range(nb + 1, nf * 2 + nb, 2))
+            )
+            e_ia_list = [
+                lib.direct_sum("i-a->ia", getattr(self, "e" + o), getattr(self, "e" + v))
+                for o, v in zip(key[nb : nf + nb], key[nf + nb :])
+            ]
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + e_ia_list)
+            d = d.transpose(perm)
+            res[name] /= d
+            res[name] += amplitudes[name]
 
         return res
 
     def update_lams(
         self, eris=None, amplitudes=None, lambdas=None, lambdas_pert=None, perturbative=False
     ):
         """Update the lambda amplitudes.
@@ -854,54 +880,63 @@
             amplitudes. Default value is `False`.
 
         Returns
         -------
         lambdas : Amplitudes
             Updated cluster lambda amplitudes.
         """
+        # TODO active
 
         if lambdas_pert is not None:
             lambdas.update(lambdas_pert)
 
         func, kwargs = self._load_function(
             "update_lams%s" % ("_perturbative" if perturbative else ""),
             eris=eris,
             amplitudes=amplitudes,
             lambdas=lambdas,
         )
         res = func(**kwargs)
         res = {key.rstrip("new"): val for key, val in res.items()}
 
-        e_ai = lib.direct_sum("i-a->ai", self.eo, self.ev)
-
         # Divide T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
             perm = list(range(0, n * 2, 2)) + list(range(1, n * 2, 2))
-            d = functools.reduce(np.add.outer, [e_ai] * n)
+            e_ai_list = [
+                lib.direct_sum("i-a->ai", getattr(self, "e" + o), getattr(self, "e" + v))
+                for o, v in zip(key[:n], key[n:])
+            ]
+            d = functools.reduce(np.add.outer, e_ai_list)
             d = d.transpose(perm)
-            res["l%d" % n] /= d
+            res[lname] /= d
             if not perturbative:
-                res["l%d" % n] += lambdas["l%d" % n]
+                res[lname] += lambdas[lname]
 
         # Divide S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            lname = "l" + name
             d = functools.reduce(np.add.outer, [-self.omega] * n)
-            res["ls%d" % n] /= d
+            res[lname] /= d
             if not perturbative:
-                res["ls%d" % n] += lambdas["ls%d" % n]
+                res[lname] += lambdas[lname]
 
         # Divide U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ai] * nf))
-                res["lu%d%d" % (nf, nb)] /= d
-                if not perturbative:
-                    res["lu%d%d" % (nf, nb)] += lambdas["lu%d%d" % (nf, nb)]
+            lname = "l" + name
+            e_ai_list = [
+                lib.direct_sum("i-a->ai", getattr(self, "e" + o), getattr(self, "e" + v))
+                for o, v in zip(key[nb : nf + nb], key[nf + nb :])
+            ]
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + e_ai_list)
+            res[lname] /= d
+            if not perturbative:
+                res[lname] += lambdas[lname]
 
         if perturbative:
             res = {key + "pert": val for key, val in res.items()}
 
         return res
 
     def make_sing_b_dm(self, eris=None, amplitudes=None, lambdas=None):
@@ -1506,23 +1541,22 @@
         vector : numpy.ndarray
             Single vector consisting of all the amplitudes flattened
             and concatenated. Size depends on the ansatz.
         """
 
         vectors = []
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            vectors.append(amplitudes["t%d" % n].ravel())
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(amplitudes[name].ravel())
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            vectors.append(amplitudes["s%d" % n].ravel())
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(amplitudes[name].ravel())
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                vectors.append(amplitudes["u%d%d" % (nf, nb)].ravel())
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(amplitudes[name].ravel())
 
         return np.concatenate(vectors)
 
     def vector_to_amplitudes(self, vector):
         """Construct all of the amplitudes used in the given ansatz
         from a vector.
 
@@ -1537,32 +1571,31 @@
         amplitudes : Amplitudes
             Cluster amplitudes.
         """
 
         amplitudes = self.Amplitudes()
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            shape = (self.space.ncocc,) * n + (self.space.ncvir,) * n
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            shape = tuple(self.space.size(k) for k in key)
             size = np.prod(shape)
-            amplitudes["t%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            amplitudes[name] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             shape = (self.nbos,) * n
             size = np.prod(shape)
-            amplitudes["s%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            amplitudes[name] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                shape = (self.nbos,) * nb + (self.space.ncocc, self.space.ncvir) * nf
-                size = np.prod(shape)
-                amplitudes["u%d%d" % (nf, nb)] = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            shape = (self.nbos,) * nb + tuple(self.space.size(k) for k in key[nb:])
+            size = np.prod(shape)
+            amplitudes[name] = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
 
         return amplitudes
 
     def lambdas_to_vector(self, lambdas):
         """Construct a vector containing all of the lambda amplitudes
         used in the given ansatz.
 
@@ -1577,23 +1610,22 @@
         vector : numpy.ndarray
             Single vector consisting of all the lambdas flattened
             and concatenated. Size depends on the ansatz.
         """
 
         vectors = []
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            vectors.append(lambdas["l%d" % n].ravel())
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(lambdas[name.replace("t", "l")].ravel())
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            vectors.append(lambdas["ls%d" % n].ravel())
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(lambdas["l" + name].ravel())
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                vectors.append(lambdas["lu%d%d" % (nf, nb)].ravel())
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(lambdas["l" + name].ravel())
 
         return np.concatenate(vectors)
 
     def vector_to_lambdas(self, vector):
         """Construct all of the lambdas used in the given ansatz
         from a vector.
 
@@ -1608,32 +1640,34 @@
         lambdas : Amplitudes
             Cluster lambda amplitudes.
         """
 
         lambdas = self.Amplitudes()
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            shape = (self.space.ncvir,) * n + (self.space.ncocc,) * n
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
+            key = key[n:] + key[:n]
+            shape = tuple(self.space.size(k) for k in key)
             size = np.prod(shape)
-            lambdas["l%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            lambdas[lname] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             shape = (self.nbos,) * n
             size = np.prod(shape)
-            lambdas["ls%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            lambdas["l" + name] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                shape = (self.nbos,) * nb + (self.space.ncvir, self.space.ncocc) * nf
-                size = np.prod(shape)
-                lambdas["lu%d%d" % (nf, nb)] = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            key = key[:nb] + key[nb + nf :] + key[nb : nb + nf]
+            shape = (self.nbos,) * nb + tuple(self.space.size(k) for k in key[nb:])
+            size = np.prod(shape)
+            lambdas["l" + name] = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
 
         return lambdas
 
     def excitations_to_vector_ip(self, *excitations):
         """Construct a vector containing all of the excitation
         amplitudes used in the given ansatz for the IP.
 
@@ -1650,24 +1684,23 @@
             Single vector consisting of all the excitations flattened
             and concatenated. Size depends on the ansatz.
         """
 
         vectors = []
         m = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             vectors.append(excitations[m].ravel())
             m += 1
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return np.concatenate(vectors)
 
     def excitations_to_vector_ea(self, *excitations):
         """Construct a vector containing all of the excitation
         amplitudes used in the given ansatz for the EA.
 
@@ -1722,26 +1755,26 @@
             the name of each excitations, and values are arrays whose
             dimension depends on the particular excitation amplitude.
         """
 
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            shape = (self.space.ncocc,) * n + (self.space.ncvir,) * (n - 1)
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[:-1]
+            shape = tuple(self.space.size(k) for k in key)
             size = np.prod(shape)
             excitations.append(vector[i0 : i0 + size].reshape(shape))
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def vector_to_excitations_ea(self, vector):
         """Construct a vector containing all of the excitation
         amplitudes used in the given ansatz for the EA.
 
@@ -1758,26 +1791,25 @@
             the name of each excitations, and values are arrays whose
             dimension depends on the particular excitation amplitude.
         """
 
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            shape = (self.space.ncvir,) * n + (self.space.ncocc,) * (n - 1)
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[n:] + key[: n - 1]
             size = np.prod(shape)
             excitations.append(vector[i0 : i0 + size].reshape(shape))
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def vector_to_excitations_ee(self, vector):
         """Construct a vector containing all of the excitation
         amplitudes used in the given ansatz for the EE.
 
@@ -1794,26 +1826,25 @@
             the name of each excitations, and values are arrays whose
             dimension depends on the particular excitation amplitude.
         """
 
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            shape = (self.space.ncocc,) * n + (self.space.ncvir,) * n
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            shape = tuple(self.space.size(k) for k in key)
             size = np.prod(shape)
             excitations.append(vector[i0 : i0 + size].reshape(shape))
             i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return tuple(excitations)
 
     def get_mean_field_G(self):
         """Get the mean-field boson non-conserving term of the
         Hamiltonian.
 
@@ -1861,15 +1892,15 @@
         }
 
         class Blocks:
             def __getattr__(selffer, key):
                 assert key[0] == "b"
                 i = slices[key[1]]
                 j = slices[key[2]]
-                return g[:, i, j].copy()
+                return g[:, i][:, :, j].copy()
 
         return Blocks()
 
     def get_fock(self):
         """Get blocks of the Fock matrix, shifted due to bosons where
         the ansatz requires.
 
@@ -2037,32 +2068,56 @@
     @property
     def eo(self):
         """Get the diagonal of the occupied Fock matrix in MO basis,
         shifted due to bosons where the ansatz requires.
 
         Returns
         -------
-        eo : numpy.ndarray (naocc,)
+        eo : numpy.ndarray (ncocc,)
             Diagonal of the occupied Fock matrix in MO basis.
         """
         return np.diag(self.fock.oo)
 
     @property
     def ev(self):
         """Get the diagonal of the virtual Fock matrix in MO basis,
         shifted due to bosons where the ansatz requires.
 
         Returns
         -------
-        ev : numpy.ndarray (navir,)
+        ev : numpy.ndarray (ncvir,)
             Diagonal of the virtual Fock matrix in MO basis.
         """
         return np.diag(self.fock.vv)
 
     @property
+    def eO(self):
+        """Get the diagonal of the active occupied Fock matrix in MO
+        basis, shifted due to bosons where the ansatz requires.
+
+        Returns
+        -------
+        eO : numpy.ndarray (naocc,)
+            Diagonal of the active occupied Fock matrix in MO basis.
+        """
+        return np.diag(self.fock.OO)
+
+    @property
+    def eV(self):
+        """Get the diagonal of the active virtual Fock matrix in MO
+        basis, shifted due to bosons where the ansatz requires.
+
+        Returns
+        -------
+        eV : numpy.ndarray (navir,)
+            Diagonal of the active virtual Fock matrix in MO basis.
+        """
+        return np.diag(self.fock.VV)
+
+    @property
     def e_tot(self):
         """Return the total energy (mean-field plus correlation).
 
         Returns
         -------
         e_tot : float
             Total energy.
```

### Comparing `ebcc-1.2.2/ebcc/reom.py` & `ebcc-1.3.0/ebcc/reom.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,15 +228,19 @@
         if hermitise:
             moments = 0.5 * (moments + moments.swapaxes(1, 2))
 
         return moments
 
     @property
     def name(self):
-        return self.excitation_type.upper() + "-REOM-" + self.ebcc.name
+        return f"{self.excitation_type.upper()}-{self.spin_type}EOM-{self.ebcc.name}"
+
+    @property
+    def spin_type(self):
+        return self.ebcc.spin_type
 
     @property
     def excitation_type(self):
         raise NotImplementedError
 
     @property
     def nmo(self):
@@ -264,24 +268,27 @@
     def matvec(self, vector, eris=None):
         amplitudes = self.vector_to_amplitudes(vector)
         amplitudes = self.ebcc.hbar_matvec_ip(*amplitudes, eris=eris)
         return self.amplitudes_to_vector(*amplitudes)
 
     def diag(self, eris=None):
         parts = []
-        e_ia = lib.direct_sum("i-a->ia", self.ebcc.eo, self.ebcc.ev)
-        e_i = self.ebcc.eo
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            e_list = [
+                lib.direct_sum("i-a->ia", getattr(self.ebcc, "e" + o), getattr(self.ebcc, "e" + v))
+                for o, v in zip(key[: n - 1], key[n : 2 * n - 1])
+            ]
+            e_list.append(getattr(self.ebcc, "e" + key[n - 1]))
             perm = list(range(0, n * 2, 2)) + list(range(1, (n - 1) * 2, 2))
-            d = functools.reduce(np.add.outer, [e_ia] * (n - 1) + [e_i])
+            d = functools.reduce(np.add.outer, e_list)
             d = d.transpose(perm)
             parts.append(d)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
         return self.amplitudes_to_vector(*parts)
 
     def _bras(self, eris=None):
         return self.ebcc.make_ip_mom_bras(eris=eris)
 
@@ -323,24 +330,27 @@
     def matvec(self, vector, eris=None):
         amplitudes = self.vector_to_amplitudes(vector)
         amplitudes = self.ebcc.hbar_matvec_ea(*amplitudes, eris=eris)
         return self.amplitudes_to_vector(*amplitudes)
 
     def diag(self, eris=None):
         parts = []
-        e_ai = lib.direct_sum("a-i->ai", self.ebcc.ev, self.ebcc.eo)
-        e_a = self.ebcc.ev
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            e_list = [
+                lib.direct_sum("i-a->ai", getattr(self.ebcc, "e" + o), getattr(self.ebcc, "e" + v))
+                for o, v in zip(key[: n - 1], key[n : 2 * n - 1])
+            ]
+            e_list.append(-getattr(self.ebcc, "e" + key[2 * n - 1]))
             perm = list(range(0, n * 2, 2)) + list(range(1, (n - 1) * 2, 2))
-            d = functools.reduce(np.add.outer, [e_ai] * (n - 1) + [e_a])
+            d = functools.reduce(np.add.outer, e_list)
             d = d.transpose(perm)
             parts.append(d)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
         return self.amplitudes_to_vector(*parts)
 
     def _bras(self, eris=None):
         return self.ebcc.make_ea_mom_bras(eris=eris)
 
@@ -382,23 +392,26 @@
     def matvec(self, vector, eris=None):
         amplitudes = self.vector_to_amplitudes(vector)
         amplitudes = self.ebcc.hbar_matvec_ee(*amplitudes, eris=eris)
         return self.amplitudes_to_vector(*amplitudes)
 
     def diag(self, eris=None):
         parts = []
-        e_ia = lib.direct_sum("a-i->ia", self.ebcc.ev, self.ebcc.eo)
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            e_list = [
+                lib.direct_sum("a-i->ia", getattr(self.ebcc, "e" + v), getattr(self.ebcc, "e" + o))
+                for o, v in zip(key[:n], key[n:])
+            ]
             perm = list(range(0, n * 2, 2)) + list(range(1, n * 2, 2))
-            d = functools.reduce(np.add.outer, [e_ia] * n)
+            d = functools.reduce(np.add.outer, e_list)
             d = d.transpose(perm)
             parts.append(d)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
         return self.amplitudes_to_vector(*parts)
 
     def bras(self, eris=None):
         bras_raw = list(self.ebcc.make_ee_mom_bras(eris=eris))
         bras = np.array(
```

### Comparing `ebcc-1.2.2/ebcc/uebcc.py` & `ebcc-1.3.0/ebcc/uebcc.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,54 +60,55 @@
 
         has_amps = rcc.amplitudes is not None
         has_lams = rcc.lambdas is not None
 
         if has_amps:
             amplitudes = cls.Amplitudes()
 
-            for n in rcc.ansatz.correlated_cluster_ranks[0]:
-                amplitudes["t%d" % n] = util.Namespace()
+            for name, key, n in ucc.ansatz.fermionic_cluster_ranks(spin_type=ucc.spin_type):
+                amplitudes[name] = util.Namespace()
                 for comb in util.generate_spin_combinations(n, unique=True):
-                    subscript = comb[:n] + comb[n:].upper()
-                    tn = rcc.amplitudes["t%d" % n]
+                    subscript = util.combine_subscripts(key, comb)
+                    tn = rcc.amplitudes[name]
                     tn = util.symmetrise(subscript, tn, symmetry="-" * 2 * n)
-                    setattr(amplitudes["t%d" % n], comb, tn)
+                    setattr(amplitudes[name], comb, tn)
 
-            for n in rcc.ansatz.correlated_cluster_ranks[1]:
-                amplitudes["s%d" % n] = rcc.amplitudes["s%d" % n].copy()
+            for name, key, n in ucc.ansatz.bosonic_cluster_ranks(spin_type=ucc.spin_type):
+                amplitudes[name] = rcc.amplitudes[name].copy()
 
-            for nf in rcc.ansatz.correlated_cluster_ranks[2]:
-                for nb in rcc.ansatz.correlated_cluster_ranks[3]:
-                    amplitudes["u%d%d" % (nf, nb)] = util.Namespace()
-                    for comb in util.generate_spin_combinations(nf, unique=True):
-                        tn = rcc.amplitudes["u%d%d" % (nf, nb)]
-                        setattr(amplitudes["u%d%d" % (nf, nb)], comb, tn)
+            for name, key, nf, nb in ucc.ansatz.coupling_cluster_ranks(spin_type=ucc.spin_type):
+                amplitudes[name] = util.Namespace()
+                for comb in util.generate_spin_combinations(nf, unique=True):
+                    tn = rcc.amplitudes[name]
+                    setattr(amplitudes[name], comb, tn)
 
             ucc.amplitudes = amplitudes
 
         if has_lams:
             lambdas = cls.Amplitudes()
 
-            for n in rcc.ansatz.correlated_cluster_ranks[0]:
-                lambdas["l%d" % n] = util.Namespace()
+            for name, key, n in ucc.ansatz.fermionic_cluster_ranks(spin_type=ucc.spin_type):
+                lname = name.replace("t", "l")
+                lambdas[lname] = util.Namespace()
                 for comb in util.generate_spin_combinations(n, unique=True):
-                    subscript = comb[:n] + comb[n:].upper()
-                    tn = rcc.lambdas["l%d" % n]
+                    subscript = util.combine_subscripts(key, comb)
+                    tn = rcc.lambdas[lname]
                     tn = util.symmetrise(subscript, tn, symmetry="-" * 2 * n)
-                    setattr(lambdas["l%d" % n], comb, tn)
+                    setattr(lambdas[lname], comb, tn)
 
-            for n in rcc.ansatz.correlated_cluster_ranks[1]:
-                lambdas["ls%d" % n] = rcc.lambdas["ls%d" % n].copy()
-
-            for nf in rcc.ansatz.correlated_cluster_ranks[2]:
-                for nb in rcc.ansatz.correlated_cluster_ranks[3]:
-                    lambdas["lu%d%d" % (nf, nb)] = util.Namespace()
-                    for comb in util.generate_spin_combinations(nf, unique=True):
-                        tn = rcc.lambdas["lu%d%d" % (nf, nb)]
-                        setattr(lambdas["lu%d%d" % (nf, nb)], comb, tn)
+            for name, key, n in ucc.ansatz.bosonic_cluster_ranks(spin_type=ucc.spin_type):
+                lname = "l" + name
+                lambdas[lname] = rcc.lambdas[lname].copy()
+
+            for name, key, nf, nb in ucc.ansatz.coupling_cluster_ranks(spin_type=ucc.spin_type):
+                lname = "l" + name
+                lambdas[lname] = util.Namespace()
+                for comb in util.generate_spin_combinations(nf, unique=True):
+                    tn = rcc.lambdas[lname]
+                    setattr(lambdas[lname], comb, tn)
 
             ucc.lambdas = lambdas
 
         return ucc
 
     def _pack_codegen_kwargs(self, *extra_kwargs, eris=None):
         eris = self.get_eris(eris)
@@ -116,14 +117,15 @@
 
         kwargs = dict(
             f=self.fock,
             v=eris,
             g=self.g,
             G=self.G,
             w=omega,
+            space=self.space,
             nocc=(self.space[0].ncocc, self.space[1].ncocc),  # FIXME rename?
             nvir=(self.space[0].ncvir, self.space[1].ncvir),  # FIXME rename?
             nbos=self.nbos,
         )
         for kw in extra_kwargs:
             if kw is not None:
                 kwargs.update(kw)
@@ -144,223 +146,263 @@
             ),
         )
 
         return space
 
     def init_amps(self, eris=None):
         eris = self.get_eris(eris)
-
         amplitudes = self.Amplitudes()
-        e_ia = util.Namespace(
-            aa=lib.direct_sum("i-a->ia", self.eo.a, self.ev.a),
-            bb=lib.direct_sum("i-a->ia", self.eo.b, self.ev.b),
-        )
 
         # Build T amplitudes
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
+                ei = getattr(self, "e" + key[0])
+                ea = getattr(self, "e" + key[1])
+                e_ia = util.Namespace(
+                    aa=lib.direct_sum("i-a->ia", ei.a, ea.a),
+                    bb=lib.direct_sum("i-a->ia", ei.b, ea.b),
+                )
                 tn = util.Namespace(
-                    aa=self.fock.aa.vo.T / e_ia.aa,
-                    bb=self.fock.bb.vo.T / e_ia.bb,
+                    aa=getattr(self.fock.aa, key) / e_ia.aa,
+                    bb=getattr(self.fock.bb, key) / e_ia.bb,
                 )
-                amplitudes["t%d" % n] = tn
+                amplitudes[name] = tn
             elif n == 2:
+                ei = getattr(self, "e" + key[0])
+                ej = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                eb = getattr(self, "e" + key[3])
+                e_ia = util.Namespace(
+                    aa=lib.direct_sum("i-a->ia", ei.a, ea.a),
+                    bb=lib.direct_sum("i-a->ia", ei.b, ea.b),
+                )
                 e_ijab = util.Namespace(
                     aaaa=lib.direct_sum("ia,jb->ijab", e_ia.aa, e_ia.aa),
                     abab=lib.direct_sum("ia,jb->ijab", e_ia.aa, e_ia.bb),
                     bbbb=lib.direct_sum("ia,jb->ijab", e_ia.bb, e_ia.bb),
                 )
+                key_t = key[0] + key[2] + key[1] + key[3]
                 tn = util.Namespace(
-                    aaaa=eris.aaaa.ovov.swapaxes(1, 2) / e_ijab.aaaa,
-                    abab=eris.aabb.ovov.swapaxes(1, 2) / e_ijab.abab,
-                    bbbb=eris.bbbb.ovov.swapaxes(1, 2) / e_ijab.bbbb,
+                    aaaa=getattr(eris.aaaa, key_t).swapaxes(1, 2) / e_ijab.aaaa,
+                    abab=getattr(eris.aabb, key_t).swapaxes(1, 2) / e_ijab.abab,
+                    bbbb=getattr(eris.bbbb, key_t).swapaxes(1, 2) / e_ijab.bbbb,
                 )
                 # TODO generalise:
                 tn.aaaa = 0.5 * (tn.aaaa - tn.aaaa.swapaxes(0, 1))
                 tn.bbbb = 0.5 * (tn.bbbb - tn.bbbb.swapaxes(0, 1))
-                amplitudes["t%d" % n] = tn
+                amplitudes[name] = tn
             else:
                 tn = util.Namespace()
                 for comb in util.generate_spin_combinations(n, unique=True):
-                    shape = tuple(self.space["ab".index(s)].ncocc for s in comb[:n])
-                    shape += tuple(self.space["ab".index(s)].ncvir for s in comb[n:])
+                    shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(comb, key))
                     amp = np.zeros(shape)
                     setattr(tn, comb, amp)
-                amplitudes["t%d" % n] = tn
+                amplitudes[name] = tn
 
         if self.boson_ansatz:
             # Only tue for real-valued couplings:
             h = self.g
             H = self.G
 
         # Build S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             if n == 1:
-                amplitudes["s%d" % n] = -H / self.omega
+                amplitudes[name] = -H / self.omega
             else:
-                amplitudes["s%d" % n] = np.zeros((self.nbos,) * n)
+                shape = (self.nbos,) * n
+                amplitudes[name] = np.zeros(shape)
 
         # Build U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                if nb == 1:
-                    e_xia = util.Namespace(
-                        aa=lib.direct_sum("ia-x->xia", e_ia.aa, self.omega),
-                        bb=lib.direct_sum("ia-x->xia", e_ia.bb, self.omega),
-                    )
-                    u1n = util.Namespace(
-                        aa=h.aa.bov / e_xia.aa,
-                        bb=h.bb.bov / e_xia.bb,
-                    )
-                    amplitudes["u%d%d" % (nf, nb)] = u1n
-                else:
-                    u1n = util.Namespace(
-                        aa=np.zeros((self.nbos,) * nb + (self.space[0].ncocc, self.space[0].ncvir)),
-                        bb=np.zeros((self.nbos,) * nb + (self.space[1].ncocc, self.space[1].ncvir)),
-                    )
-                    amplitudes["u%d%d" % (nf, nb)] = u1n
+            if nb == 1:
+                ei = getattr(self, "e" + key[1])
+                ea = getattr(self, "e" + key[2])
+                e_xia = util.Namespace(
+                    aa=lib.direct_sum("i-a-x->xia", ei.a, ea.a, self.omega),
+                    bb=lib.direct_sum("i-a-x->xia", ei.b, ea.b, self.omega),
+                )
+                u1n = util.Namespace(
+                    aa=getattr(h.aa, key) / e_xia.aa,
+                    bb=getattr(h.bb, key) / e_xia.bb,
+                )
+                amplitudes[name] = u1n
+            else:
+                u1n = util.Namespace(
+                    aa=np.zeros((self.nbos,) * nb + tuple(self.space[0].size(k) for k in key[nb:])),
+                    bb=np.zeros((self.nbos,) * nb + tuple(self.space[0].size(k) for k in key[nb:])),
+                )
+                amplitudes[name] = u1n
 
         return amplitudes
 
     def init_lams(self, amplitudes=None):
         if amplitudes is None:
             amplitudes = self.amplitudes
 
         lambdas = self.Amplitudes()
 
         # Build L amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
             perm = list(range(n, 2 * n)) + list(range(n))
-            lambdas["l%d" % n] = util.Namespace()
-            for key in dict(amplitudes["t%d" % n]).keys():
-                ln = getattr(amplitudes["t%d" % n], key).transpose(perm)
-                setattr(lambdas["l%d" % n], key, ln)
+            lambdas[lname] = util.Namespace()
+            for key in dict(amplitudes[name]).keys():
+                ln = getattr(amplitudes[name], key).transpose(perm)
+                setattr(lambdas[lname], key, ln)
 
         # Build LS amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            lambdas["ls%d" % n] = amplitudes["s%d" % n]
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            lambdas["l" + name] = amplitudes[name]
 
         # Build LU amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                perm = list(range(nb)) + [nb + 1, nb]
-                lambdas["lu%d%d" % (nf, nb)] = util.Namespace()
-                for key in dict(amplitudes["u%d%d" % (nf, nb)]).keys():
-                    lu1n = getattr(amplitudes["u%d%d" % (nf, nb)], key).transpose(perm)
-                    setattr(lambdas["lu%d%d" % (nf, nb)], key, lu1n)
+            perm = list(range(nb)) + [nb + 1, nb]
+            lambdas["l" + name] = util.Namespace()
+            for key in dict(amplitudes[name]).keys():
+                lu1n = getattr(amplitudes[name], key).transpose(perm)
+                setattr(lambdas["l" + name], key, lu1n)
 
         return lambdas
 
     def update_amps(self, eris=None, amplitudes=None):
         func, kwargs = self._load_function(
             "update_amps",
             eris=eris,
             amplitudes=amplitudes,
         )
         res = func(**kwargs)
         res = {key.rstrip("new"): val for key, val in res.items()}
 
-        e_ia = util.Namespace(
-            aa=lib.direct_sum("i-a->ia", self.eo.a, self.ev.a),
-            bb=lib.direct_sum("i-a->ia", self.eo.b, self.ev.b),
-        )
-
         # Divide T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             perm = list(range(0, n * 2, 2)) + list(range(1, n * 2, 2))
             for comb in util.generate_spin_combinations(n, unique=True):
-                subscript = comb[:n] + comb[n:].upper()
-                es = [getattr(e_ia, comb[i] + comb[i + n]) for i in range(n)]
-                d = functools.reduce(np.add.outer, es)
+                subscript = util.combine_subscripts(key, comb)
+                e_ia_list = [
+                    lib.direct_sum(
+                        "i-a->ia",
+                        getattr(getattr(self, "e" + o), so),
+                        getattr(getattr(self, "e" + v), sv),
+                    )
+                    for (o, v), (so, sv) in zip(zip(key[:n], key[n:]), zip(comb[:n], comb[n:]))
+                ]
+                d = functools.reduce(np.add.outer, e_ia_list)
                 d = d.transpose(perm)
-                tn = getattr(res["t%d" % n], comb)
+                tn = getattr(res[name], comb)
                 tn /= d
-                tn += getattr(amplitudes["t%d" % n], comb)
+                tn += getattr(amplitudes[name], comb)
                 tn = util.symmetrise(subscript, tn, symmetry="-" * (2 * n))
-                setattr(res["t%d" % n], comb, tn)
+                setattr(res[name], comb, tn)
 
         # Divide S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             d = functools.reduce(np.add.outer, ([-self.omega] * n))
-            res["s%d" % n] /= d
-            res["s%d" % n] += amplitudes["s%d" % n]
+            res[name] /= d
+            res[name] += amplitudes[name]
 
         # Divide U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ia.aa] * nf))
-                tn = res["u%d%d" % (nf, nb)].aa
-                tn /= d
-                tn += amplitudes["u%d%d" % (nf, nb)].aa
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ia.bb] * nf))
-                res["u%d%d" % (nf, nb)].aa = tn
-                tn = res["u%d%d" % (nf, nb)].bb
-                tn /= d
-                tn += amplitudes["u%d%d" % (nf, nb)].bb
-                res["u%d%d" % (nf, nb)].bb = tn
+            e_ia = util.Namespace(
+                aa=lib.direct_sum(
+                    "i-a->ia",
+                    getattr(self, "e" + key[nb]).a,
+                    getattr(self, "e" + key[nb + 1]).a,
+                ),
+                bb=lib.direct_sum(
+                    "i-a->ia",
+                    getattr(self, "e" + key[nb]).b,
+                    getattr(self, "e" + key[nb + 1]).b,
+                ),
+            )
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ia.aa] * nf))
+            tn = res[name].aa
+            tn /= d
+            tn += amplitudes[name].aa
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ia.bb] * nf))
+            res[name].aa = tn
+            tn = res[name].bb
+            tn /= d
+            tn += amplitudes[name].bb
+            res[name].bb = tn
 
         return res
 
     def update_lams(self, eris=None, amplitudes=None, lambdas=None, lambdas_pert=None):
         func, kwargs = self._load_function(
             "update_lams",
             eris=eris,
             amplitudes=amplitudes,
             lambdas=lambdas,
             lambdas_pert=lambdas_pert,
         )
         res = func(**kwargs)
         res = {key.rstrip("new"): val for key, val in res.items()}
 
-        e_ai = util.Namespace(
-            aa=lib.direct_sum("i-a->ai", self.eo.a, self.ev.a),
-            bb=lib.direct_sum("i-a->ai", self.eo.b, self.ev.b),
-        )
-
         # Divide T amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
             perm = list(range(0, n * 2, 2)) + list(range(1, n * 2, 2))
             for comb in util.generate_spin_combinations(n, unique=True):
-                subscript = comb[:n] + comb[n:].upper()
-                es = [getattr(e_ai, comb[i] + comb[i + n]) for i in range(n)]
-                d = functools.reduce(np.add.outer, es)
+                subscript = util.combine_subscripts(key, comb)
+                e_ai_list = [
+                    lib.direct_sum(
+                        "i-a->ai",
+                        getattr(getattr(self, "e" + o), so),
+                        getattr(getattr(self, "e" + v), sv),
+                    )
+                    for (o, v), (so, sv) in zip(zip(key[:n], key[n:]), zip(comb[:n], comb[n:]))
+                ]
+                d = functools.reduce(np.add.outer, e_ai_list)
                 d = d.transpose(perm)
-                tn = getattr(res["l%d" % n], comb)
+                tn = getattr(res[lname], comb)
                 tn /= d
-                tn += getattr(lambdas["l%d" % n], comb)
+                tn += getattr(lambdas[lname], comb)
                 tn = util.symmetrise(subscript, tn, symmetry="-" * (2 * n))
-                setattr(res["l%d" % n], comb, tn)
+                setattr(res[lname], comb, tn)
 
         # Divide S amplitudes:
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            lname = "l" + name
             d = functools.reduce(np.add.outer, [-self.omega] * n)
-            res["ls%d" % n] /= d
-            res["ls%d" % n] += lambdas["ls%d" % n]
+            res[lname] /= d
+            res[lname] += lambdas[lname]
 
         # Divide U amplitudes:
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ai.aa] * nf))
-                tn = res["lu%d%d" % (nf, nb)].aa
-                tn /= d
-                tn += lambdas["lu%d%d" % (nf, nb)].aa
-                d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ai.bb] * nf))
-                res["lu%d%d" % (nf, nb)].aa = tn
-                tn = res["lu%d%d" % (nf, nb)].bb
-                tn /= d
-                tn += lambdas["lu%d%d" % (nf, nb)].bb
-                res["lu%d%d" % (nf, nb)].bb = tn
+            lname = "l" + name
+            e_ai = util.Namespace(
+                aa=lib.direct_sum(
+                    "i-a->ai",
+                    getattr(self, "e" + key[nb]).a,
+                    getattr(self, "e" + key[nb + 1]).a,
+                ),
+                bb=lib.direct_sum(
+                    "i-a->ai",
+                    getattr(self, "e" + key[nb]).b,
+                    getattr(self, "e" + key[nb + 1]).b,
+                ),
+            )
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ai.aa] * nf))
+            tn = res[lname].aa
+            tn /= d
+            tn += lambdas[lname].aa
+            d = functools.reduce(np.add.outer, ([-self.omega] * nb) + ([e_ai.bb] * nf))
+            res[lname].aa = tn
+            tn = res[lname].bb
+            tn /= d
+            tn += lambdas[lname].bb
+            res[lname].bb = tn
 
         return res
 
     def make_rdm1_f(self, eris=None, amplitudes=None, lambdas=None, hermitise=True):
         func, kwargs = self._load_function(
             "make_rdm1_f",
             eris=eris,
@@ -460,15 +502,15 @@
 
         def constructor(s):
             class Blocks:
                 def __getattr__(selffer, key):
                     assert key[0] == "b"
                     i = slices[s][key[1]]
                     j = slices[s][key[2]]
-                    return g[s][:, i, j].copy()
+                    return g[s][:, i][:, :, j].copy()
 
             return Blocks()
 
         gs = util.Namespace()
         gs.aa = constructor(0)
         gs.bb = constructor(1)
 
@@ -525,315 +567,289 @@
 
     def ee_eom(self, options=None, **kwargs):
         return ueom.EE_UEOM(self, options=options, **kwargs)
 
     def amplitudes_to_vector(self, amplitudes):
         vectors = []
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             for spin in util.generate_spin_combinations(n, unique=True):
-                tn = getattr(amplitudes["t%d" % n], spin)
+                tn = getattr(amplitudes[name], spin)
                 subscript = spin[:n] + spin[n:].upper()
                 vectors.append(util.compress_axes(subscript, tn).ravel())
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            vectors.append(amplitudes["s%d" % n].ravel())
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(amplitudes[name].ravel())
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                vectors.append(amplitudes["u%d%d" % (nf, nb)].aa.ravel())
-                vectors.append(amplitudes["u%d%d" % (nf, nb)].bb.ravel())
+            vectors.append(amplitudes[name].aa.ravel())
+            vectors.append(amplitudes[name].bb.ravel())
 
         return np.concatenate(vectors)
 
     def vector_to_amplitudes(self, vector):
         amplitudes = self.Amplitudes()
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            amplitudes["t%d" % n] = util.Namespace()
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            amplitudes[name] = util.Namespace()
             for spin in util.generate_spin_combinations(n, unique=True):
-                subscript = spin[:n] + spin[n:].upper()
-                size = util.get_compressed_size(
-                    subscript,
-                    a=self.space[0].ncocc,
-                    b=self.space[1].ncocc,
-                    A=self.space[0].ncvir,
-                    B=self.space[1].ncvir,
-                )
-                shape = tuple(
-                    [
-                        *[self.space["ab".index(s)].ncocc for s in spin[:n]],
-                        *[self.space["ab".index(s)].ncvir for s in spin[n:]],
-                    ]
-                )
+                sizes = {
+                    (o, s): self.space[i].size(o) for o in "ovOVia" for i, s in enumerate("ab")
+                }
+                subscript, sizes = util.combine_subscripts(key, spin, sizes=sizes)
+                size = util.get_compressed_size(subscript, **sizes)
+                shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(spin, key))
                 tn_tril = vector[i0 : i0 + size]
                 tn = util.decompress_axes(subscript, tn_tril, shape=shape)
-                setattr(amplitudes["t%d" % n], spin, tn)
+                setattr(amplitudes[name], spin, tn)
                 i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             shape = (self.nbos,) * n
             size = np.prod(shape)
-            amplitudes["s%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            amplitudes[name] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                amplitudes["u%d%d" % (nf, nb)] = util.Namespace()
-                shape = (self.nbos,) * nb + (self.space[0].ncocc, self.space[0].ncvir) * nf
-                size = np.prod(shape)
-                amplitudes["u%d%d" % (nf, nb)].aa = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
-                shape = (self.nbos,) * nb + (self.space[1].ncocc, self.space[1].ncvir) * nf
-                size = np.prod(shape)
-                amplitudes["u%d%d" % (nf, nb)].bb = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
+            amplitudes[name] = util.Namespace()
+            shape = (self.nbos,) * nb + tuple(self.space[0].size(k) for k in key[nb:])
+            size = np.prod(shape)
+            amplitudes[name].aa = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
+            shape = (self.nbos,) * nb + tuple(self.space[1].size(k) for k in key[nb:])
+            size = np.prod(shape)
+            amplitudes[name].bb = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
 
         assert i0 == len(vector)
 
         return amplitudes
 
     def lambdas_to_vector(self, lambdas):
         vectors = []
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
             for spin in util.generate_spin_combinations(n, unique=True):
-                tn = getattr(lambdas["l%d" % n], spin)
+                tn = getattr(lambdas[lname], spin)
                 subscript = spin[:n] + spin[n:].upper()
                 vectors.append(util.compress_axes(subscript, tn).ravel())
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
-            vectors.append(lambdas["ls%d" % n].ravel())
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
+            vectors.append(lambdas["l" + name].ravel())
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                vectors.append(lambdas["lu%d%d" % (nf, nb)].aa.ravel())
-                vectors.append(lambdas["lu%d%d" % (nf, nb)].bb.ravel())
+            vectors.append(lambdas["l" + name].aa.ravel())
+            vectors.append(lambdas["l" + name].bb.ravel())
 
         return np.concatenate(vectors)
 
     def vector_to_lambdas(self, vector):
         lambdas = self.Amplitudes()
         i0 = 0
         spin_indices = {"a": 0, "b": 1}
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
-            lambdas["l%d" % n] = util.Namespace()
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            lname = name.replace("t", "l")
+            key = key[n:] + key[:n]
+            lambdas[lname] = util.Namespace()
             for spin in util.generate_spin_combinations(n, unique=True):
                 subscript = spin[:n] + spin[n:].upper()
+                # FIXME this will break for active space methods
                 size = util.get_compressed_size(
                     subscript,
                     a=self.space[0].ncvir,
                     b=self.space[1].ncvir,
                     A=self.space[0].ncocc,
                     B=self.space[1].ncocc,
                 )
-                shape = tuple(
-                    [
-                        *[self.space["ab".index(s)].ncvir for s in spin[:n]],
-                        *[self.space["ab".index(s)].ncocc for s in spin[n:]],
-                    ]
-                )
+                shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(spin, key))
                 tn_tril = vector[i0 : i0 + size]
                 tn = util.decompress_axes(subscript, tn_tril, shape=shape)
-                setattr(lambdas["l%d" % n], spin, tn)
+                setattr(lambdas[lname], spin, tn)
                 i0 += size
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             shape = (self.nbos,) * n
             size = np.prod(shape)
-            lambdas["ls%d" % n] = vector[i0 : i0 + size].reshape(shape)
+            lambdas["l" + name] = vector[i0 : i0 + size].reshape(shape)
             i0 += size
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
             if nf != 1:
                 raise util.ModelNotImplemented
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                lambdas["lu%d%d" % (nf, nb)] = util.Namespace()
-                shape = (self.nbos,) * nb + (self.space[0].ncvir, self.space[0].ncocc) * nf
-                size = np.prod(shape)
-                lambdas["lu%d%d" % (nf, nb)].aa = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
-                shape = (self.nbos,) * nb + (self.space[1].ncvir, self.space[1].ncocc) * nf
-                size = np.prod(shape)
-                lambdas["lu%d%d" % (nf, nb)].bb = vector[i0 : i0 + size].reshape(shape)
-                i0 += size
+            lname = "l" + name
+            key = key[:nb] + key[nb + nf :] + key[nb : nb + nf]
+            lambdas[lname] = util.Namespace()
+            shape = (self.nbos,) * nb + tuple(self.space[0].size(k) for k in key[nb:])
+            size = np.prod(shape)
+            lambdas[lname].aa = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
+            shape = (self.nbos,) * nb + tuple(self.space[1].size(k) for k in key[nb:])
+            size = np.prod(shape)
+            lambdas[lname].bb = vector[i0 : i0 + size].reshape(shape)
+            i0 += size
 
         assert i0 == len(vector)
 
         return lambdas
 
     def excitations_to_vector_ip(self, *excitations):
         vectors = []
         m = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             for spin in util.generate_spin_combinations(n, excited=True, unique=True):
                 vn = getattr(excitations[m], spin)
                 subscript = spin[:n] + spin[n:].upper()
                 vectors.append(util.compress_axes(subscript, vn).ravel())
             m += 1
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return np.concatenate(vectors)
 
     def excitations_to_vector_ee(self, *excitations):
         vectors = []
         m = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             for spin in util.generate_spin_combinations(n):
                 vn = getattr(excitations[m], spin)
                 subscript = spin[:n] + spin[n:].upper()
                 vectors.append(util.compress_axes(subscript, vn).ravel())
             m += 1
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         return np.concatenate(vectors)
 
     def vector_to_excitations_ip(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[:-1]
             amp = util.Namespace()
             for spin in util.generate_spin_combinations(n, excited=True, unique=True):
                 subscript = spin[:n] + spin[n:].upper()
+                # FIXME this will break for active space methods
                 size = util.get_compressed_size(
                     subscript,
                     a=self.space[0].ncocc,
                     b=self.space[1].ncocc,
                     A=self.space[0].ncvir,
                     B=self.space[1].ncvir,
                 )
-                shape = tuple(
-                    [
-                        *[self.space["ab".index(s)].ncocc for s in spin[:n]],
-                        *[self.space["ab".index(s)].ncvir for s in spin[n:]],
-                    ]
-                )
+                shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(spin, key))
                 vn_tril = vector[i0 : i0 + size]
                 factor = max(
                     spin[:n].count(s) for s in set(spin[:n])
                 )  # FIXME why? untested for n > 2
                 vn = util.decompress_axes(subscript, vn_tril, shape=shape) / factor
                 setattr(amp, spin, vn)
                 i0 += size
 
             excitations.append(amp)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         assert i0 == len(vector)
 
         return tuple(excitations)
 
     def vector_to_excitations_ea(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
+            key = key[n:] + key[: n - 1]
             amp = util.Namespace()
             for spin in util.generate_spin_combinations(n, excited=True, unique=True):
                 subscript = spin[:n] + spin[n:].upper()
+                # FIXME this will break for active space methods
                 size = util.get_compressed_size(
                     subscript,
                     a=self.space[0].ncvir,
                     b=self.space[1].ncvir,
                     A=self.space[0].ncocc,
                     B=self.space[1].ncocc,
                 )
-                shape = tuple(
-                    [
-                        *[self.space["ab".index(s)].ncvir for s in spin[:n]],
-                        *[self.space["ab".index(s)].ncocc for s in spin[n:]],
-                    ]
-                )
+                shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(spin, key))
                 vn_tril = vector[i0 : i0 + size]
                 factor = max(
                     spin[:n].count(s) for s in set(spin[:n])
                 )  # FIXME why? untested for n > 2
                 vn = util.decompress_axes(subscript, vn_tril, shape=shape) / factor
                 setattr(amp, spin, vn)
                 i0 += size
 
             excitations.append(amp)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         assert i0 == len(vector)
 
         return tuple(excitations)
 
     def vector_to_excitations_ee(self, vector):
         excitations = []
         i0 = 0
 
-        for n in self.ansatz.correlated_cluster_ranks[0]:
+        for name, key, n in self.ansatz.fermionic_cluster_ranks(spin_type=self.spin_type):
             amp = util.Namespace()
             for spin in util.generate_spin_combinations(n):
                 subscript = spin[:n] + spin[n:].upper()
+                # FIXME this will break for active space methods
                 size = util.get_compressed_size(
                     subscript,
                     a=self.space[0].ncocc,
                     b=self.space[1].ncocc,
                     A=self.space[0].ncvir,
                     B=self.space[1].ncvir,
                 )
-                shape = tuple(
-                    [
-                        *[self.space["ab".index(s)].ncocc for s in spin[:n]],
-                        *[self.space["ab".index(s)].ncvir for s in spin[n:]],
-                    ]
-                )
+                shape = tuple(self.space["ab".index(s)].size(k) for s, k in zip(spin, key))
                 vn_tril = vector[i0 : i0 + size]
                 factor = max(
                     spin[:n].count(s) for s in set(spin[:n])
                 )  # FIXME why? untested for n > 2
                 vn = util.decompress_axes(subscript, vn_tril, shape=shape) / factor
                 setattr(amp, spin, vn)
                 i0 += size
 
             excitations.append(amp)
 
-        for n in self.ansatz.correlated_cluster_ranks[1]:
+        for name, key, n in self.ansatz.bosonic_cluster_ranks(spin_type=self.spin_type):
             raise util.ModelNotImplemented
 
-        for nf in self.ansatz.correlated_cluster_ranks[2]:
-            for nb in self.ansatz.correlated_cluster_ranks[3]:
-                raise util.ModelNotImplemented
+        for name, key, nf, nb in self.ansatz.coupling_cluster_ranks(spin_type=self.spin_type):
+            raise util.ModelNotImplemented
 
         assert i0 == len(vector)
 
         return tuple(excitations)
 
     @property
     def spin_type(self):
@@ -863,7 +879,23 @@
     @property
     def ev(self):
         ev = util.Namespace(
             a=np.diag(self.fock.aa.vv),
             b=np.diag(self.fock.bb.vv),
         )
         return ev
+
+    @property
+    def eO(self):
+        eO = util.Namespace(
+            a=np.diag(self.fock.aa.OO),
+            b=np.diag(self.fock.bb.OO),
+        )
+        return eO
+
+    @property
+    def eV(self):
+        eV = util.Namespace(
+            a=np.diag(self.fock.aa.VV),
+            b=np.diag(self.fock.bb.VV),
+        )
+        return eV
```

### Comparing `ebcc-1.2.2/ebcc/util.py` & `ebcc-1.3.0/ebcc/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -316,14 +316,73 @@
     return v_as
 
 
 def is_mixed_spin(spin):
     return len(set(spin)) != 1
 
 
+def combine_subscripts(*subscripts, sizes=None):
+    """Combines subscripts into new unique subscripts for functions
+    such as `compress_axes`. For example, one may wish to compress an
+    amplitude according to both occupancy and spin signatures.
+
+    The output string of this function has the same length as the
+    input subscripts, where the `i`th character is an arbitrary
+    character chosen such that it is unique for a unique value of
+    `tuple(s[i] for s in subscripts)` among other values of `i`.
+
+    If `sizes` is passed, this function also returns a dictionary
+    indicating the size of each new character in the subscript
+    according to the size of the corresponding original character
+    in the dictionary `sizes`.
+
+    Parameters
+    ----------
+    subscripts : tuple of str
+        Subscripts to combine.  Each subscript must be a string of
+        the same length.
+    sizes : dict, optional
+        Dictionary of sizes for each index.  Keys should be
+        `tuple(s[i] for s in subscripts)`.  Default value is `None`.
+
+    Returns
+    -------
+    new_subscript : str
+        Output subscript.
+    new_sizes : dict, optional
+        Dictionary of the sizes of each new index.  Only returned if
+        the `sizes` keyword argument is provided.
+    """
+
+    if len(set(len(s) for s in subscripts)) != 1:
+        raise ValueError("Subscripts must be of the same length.")
+
+    char_map = {}
+    new_subscript = ""
+    new_sizes = {}
+    j = 0
+    for i in range(len(subscripts[0])):
+        key = tuple(s[i] for s in subscripts)
+        if key not in char_map:
+            if j == 91:
+                raise ValueError("Too many unique characters.")
+            char_map[key] = chr(97 + j)
+            j += 1
+            if j == 123:
+                j = 65
+        new_subscript += char_map[key]
+        if sizes is not None:
+            new_sizes[char_map[key]] = sizes[key]
+
+    if sizes is None:
+        return new_subscript
+    else:
+        return new_subscript, new_sizes
+
+
 def compress_axes(subscript, array, include_diagonal=False, out=None):
     """Compress an array into lower-triangular representations using
     an einsum-like input.
 
     >>> t2 = np.zeros((4, 4, 10, 10))
     >>> compress_axes("iiaa", t2).shape
     (6, 45)
@@ -678,15 +737,18 @@
             shape_ct.append(ranges[idx])
             inp_ct.append(idx)
         order_ct = [inp_ct.index(idx) for idx in out]
 
         # If any dimension has size zero, return here
         if a.size == 0 or b.size == 0:
             shape_c = [shape_ct[i] for i in order_ct]
-            return np.zeros(shape_c)
+            if buf is not None:
+                return buf.reshape(shape_c) * beta if beta != 1.0 else buf.reshape(shape_c)
+            else:
+                return np.zeros(shape_c)
 
         # Apply transposes
         at = a.transpose(order_a)
         bt = b.transpose(order_b)
 
         # Find the optimal memory alignment
         at = np.asarray(at.reshape(-1, inner_shape), order="F" if at.flags.f_contiguous else "C")
@@ -718,14 +780,21 @@
         tblis_dtype = tblis_einsum.tblis_dtype[dtype]
 
         # Get the shapes
         shape_a = a.shape
         shape_b = b.shape
         shape_c = tuple(ranges[x] for x in out)
 
+        # If any dimension has size zero, return here
+        if a.size == 0 or b.size == 0:
+            if buf is not None:
+                return buf.reshape(shape_c) * beta
+            else:
+                return np.zeros(shape_c)
+
         # Get the output buffer
         if buf is None:
             order = kwargs.get("order", "C")
             c = np.empty(shape_c, dtype=dtype, order=order)
         else:
             assert buf.dtype == dtype
             assert buf.size == np.prod(shape_c)
```

### Comparing `ebcc-1.2.2/ebcc.egg-info/PKG-INFO` & `ebcc-1.3.0/ebcc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcc
-Version: 1.2.2
+Version: 1.3.0
 Summary: Coupled cluster calculations on electron-boson systems
 Keywords: quantum,chemistry,electronic,structure,coupled,cluster,electron,boson,ccsd
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
```

### Comparing `ebcc-1.2.2/ebcc.egg-info/SOURCES.txt` & `ebcc-1.3.0/ebcc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,75 +24,81 @@
 ebcc/codegen/GCCD.py
 ebcc/codegen/GCCSD.py
 ebcc/codegen/GCCSDT.py
 ebcc/codegen/GCCSDTQ.py
 ebcc/codegen/GCCSD_SD_1_1.py
 ebcc/codegen/GCCSD_SD_1_2.py
 ebcc/codegen/GCCSD_S_1_1.py
+ebcc/codegen/GCCSDtp.py
 ebcc/codegen/GCCSDxTx.py
 ebcc/codegen/GMP2.py
 ebcc/codegen/GMP3.py
 ebcc/codegen/GQCISD.py
 ebcc/codegen/RCC2.py
 ebcc/codegen/RCC3.py
 ebcc/codegen/RCCD.py
 ebcc/codegen/RCCSD.py
 ebcc/codegen/RCCSDT.py
 ebcc/codegen/RCCSD_SD_1_1.py
 ebcc/codegen/RCCSD_SD_1_2.py
 ebcc/codegen/RCCSD_S_1_1.py
+ebcc/codegen/RCCSDtp.py
 ebcc/codegen/RCCSDxTx.py
 ebcc/codegen/RMP2.py
 ebcc/codegen/RMP3.py
 ebcc/codegen/RQCISD.py
 ebcc/codegen/UCC2.py
 ebcc/codegen/UCC3.py
 ebcc/codegen/UCCD.py
 ebcc/codegen/UCCSD.py
 ebcc/codegen/UCCSDT.py
 ebcc/codegen/UCCSD_SD_1_1.py
 ebcc/codegen/UCCSD_SD_1_2.py
 ebcc/codegen/UCCSD_S_1_1.py
+ebcc/codegen/UCCSDtp.py
 ebcc/codegen/UCCSDxTx.py
 ebcc/codegen/UMP2.py
 ebcc/codegen/UMP3.py
 ebcc/codegen/UQCISD.py
 ebcc/codegen/__init__.py
 tests/test_GCC2.py
 tests/test_GCC3.py
 tests/test_GCCD.py
 tests/test_GCCSD.py
 tests/test_GCCSDT.py
 tests/test_GCCSDTQ.py
 tests/test_GCCSD_SD_1_1.py
 tests/test_GCCSD_SD_1_2.py
 tests/test_GCCSD_S_1_1.py
+tests/test_GCCSDtp.py
 tests/test_GCCSDxTx.py
 tests/test_GMP2.py
 tests/test_GMP3.py
 tests/test_GQCISD.py
 tests/test_RCC2.py
 tests/test_RCC3.py
 tests/test_RCCD.py
 tests/test_RCCSD.py
 tests/test_RCCSDT.py
 tests/test_RCCSD_SD_1_1.py
 tests/test_RCCSD_SD_1_2.py
 tests/test_RCCSD_S_1_1.py
+tests/test_RCCSDtp.py
 tests/test_RCCSDxTx.py
 tests/test_RMP2.py
 tests/test_RMP3.py
 tests/test_RQCISD.py
 tests/test_UCC2.py
 tests/test_UCC3.py
 tests/test_UCCD.py
 tests/test_UCCSD.py
 tests/test_UCCSDT.py
 tests/test_UCCSD_SD_1_1.py
 tests/test_UCCSD_SD_1_2.py
 tests/test_UCCSD_S_1_1.py
+tests/test_UCCSDtp.py
 tests/test_UCCSDxTx.py
 tests/test_UMP2.py
 tests/test_UMP3.py
 tests/test_UQCISD.py
 tests/test_brueckner.py
 tests/test_util.py
```

### Comparing `ebcc-1.2.2/pyproject.toml` & `ebcc-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ebcc"
-version = "1.2.2"
+version = "1.3.0"
 description = "Coupled cluster calculations on electron-boson systems"
 keywords = [
     "quantum", "chemistry",
     "electronic", "structure",
     "coupled", "cluster",
     "electron", "boson",
     "ccsd",
```

### Comparing `ebcc-1.2.2/tests/test_GCC2.py` & `ebcc-1.3.0/tests/test_GCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCD.py` & `ebcc-1.3.0/tests/test_GCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCSD.py` & `ebcc-1.3.0/tests/test_GCCSD.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import pytest
 import scipy.linalg
 from types import SimpleNamespace
 from pyscf import cc, gto, lib, scf
 
-from ebcc import REBCC, UEBCC, GEBCC, NullLogger, util
+from ebcc import REBCC, UEBCC, GEBCC, Space, NullLogger, util
 
 # TODO test more excitations in EOM
 
 
 @pytest.mark.reference
 class GCCSD_Tests(unittest.TestCase):
     """Test GCCSD against the legacy GCCSD values.
@@ -179,14 +179,115 @@
                 log=NullLogger(),
         )
         uebcc.options.e_tol = 1e-12
         eris = uebcc.get_eris()
         uebcc.kernel(eris=eris)
         uebcc.solve_lambda(eris=eris)
         gebcc2 = GEBCC.from_uebcc(uebcc)
+
+        self.assertAlmostEqual(gebcc1.energy(), gebcc2.energy())
+        np.testing.assert_almost_equal(gebcc1.t1, gebcc2.t1, 6)
+        np.testing.assert_almost_equal(gebcc1.t2, gebcc2.t2, 6)
+        np.testing.assert_almost_equal(gebcc1.l1, gebcc2.l1, 5)
+        np.testing.assert_almost_equal(gebcc1.l2, gebcc2.l2, 5)
+        np.testing.assert_almost_equal(gebcc1.make_rdm1_f(), gebcc2.make_rdm1_f(), 6)
+        np.testing.assert_almost_equal(gebcc1.make_rdm2_f(), gebcc2.make_rdm2_f(), 6)
+
+    @pytest.mark.regression
+    def test_from_rebcc_frozen(self):
+        mf = self.mf
+        gmf = mf.to_uhf().to_ghf()
+
+        occupied = gmf.mo_occ > 0
+        frozen = np.zeros_like(gmf.mo_occ)
+        frozen[:2] = True
+        active = np.zeros_like(gmf.mo_occ)
+        space = Space(occupied, frozen, active)
+
+        gebcc1 = GEBCC(
+                gmf,
+                ansatz="CCSD",
+                space=space,
+                log=NullLogger(),
+        )
+        gebcc1.options.e_tol = 1e-12
+        eris = gebcc1.get_eris()
+        gebcc1.kernel(eris=eris)
+        gebcc1.solve_lambda(eris=eris)
+
+        occupied = mf.mo_occ > 0
+        frozen = np.zeros_like(mf.mo_occ)
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ)
+        space = Space(occupied, frozen, active)
+
+        rebcc = REBCC(
+                mf,
+                ansatz="CCSD",
+                space=space,
+                log=NullLogger(),
+        )
+        rebcc.options.e_tol = 1e-12
+        eris = rebcc.get_eris()
+        rebcc.kernel(eris=eris)
+        rebcc.solve_lambda(eris=eris)
+        gebcc2 = GEBCC.from_rebcc(rebcc)
+
+        self.assertAlmostEqual(gebcc1.energy(), gebcc2.energy())
+        np.testing.assert_almost_equal(gebcc1.t1, gebcc2.t1, 6)
+        np.testing.assert_almost_equal(gebcc1.t2, gebcc2.t2, 6)
+        np.testing.assert_almost_equal(gebcc1.l1, gebcc2.l1, 5)
+        np.testing.assert_almost_equal(gebcc1.l2, gebcc2.l2, 5)
+        np.testing.assert_almost_equal(gebcc1.make_rdm1_f(), gebcc2.make_rdm1_f(), 6)
+        np.testing.assert_almost_equal(gebcc1.make_rdm2_f(), gebcc2.make_rdm2_f(), 6)
+
+    @pytest.mark.regression
+    def test_from_uebcc_frozen(self):
+        mf = self.mf.to_uhf()
+        gmf = mf.to_ghf()
+
+        occupied = gmf.mo_occ > 0
+        frozen = np.zeros_like(gmf.mo_occ)
+        frozen[:2] = True
+        active = np.zeros_like(gmf.mo_occ)
+        space = Space(occupied, frozen, active)
+
+        gebcc1 = GEBCC(
+                mf,
+                ansatz="CCSD",
+                space=space,
+                log=NullLogger(),
+        )
+        gebcc1.options.e_tol = 1e-12
+        eris = gebcc1.get_eris()
+        gebcc1.kernel(eris=eris)
+        gebcc1.solve_lambda(eris=eris)
+
+        occupied = mf.mo_occ[0] > 0
+        frozen = np.zeros_like(mf.mo_occ[0])
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ[0])
+        space_a = Space(occupied, frozen, active)
+        occupied = mf.mo_occ[1] > 0
+        frozen = np.zeros_like(mf.mo_occ[1])
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ[1])
+        space_b = Space(occupied, frozen, active)
+
+        uebcc = UEBCC(
+                mf,
+                ansatz="CCSD",
+                space=(space_a, space_b),
+                log=NullLogger(),
+        )
+        uebcc.options.e_tol = 1e-12
+        eris = uebcc.get_eris()
+        uebcc.kernel(eris=eris)
+        uebcc.solve_lambda(eris=eris)
+        gebcc2 = GEBCC.from_uebcc(uebcc)
 
         self.assertAlmostEqual(gebcc1.energy(), gebcc2.energy())
         np.testing.assert_almost_equal(gebcc1.t1, gebcc2.t1, 6)
         np.testing.assert_almost_equal(gebcc1.t2, gebcc2.t2, 6)
         np.testing.assert_almost_equal(gebcc1.l1, gebcc2.l1, 5)
         np.testing.assert_almost_equal(gebcc1.l2, gebcc2.l2, 5)
         np.testing.assert_almost_equal(gebcc1.make_rdm1_f(), gebcc2.make_rdm1_f(), 6)
```

### Comparing `ebcc-1.2.2/tests/test_GCCSDT.py` & `ebcc-1.3.0/tests/test_GCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCSDTQ.py` & `ebcc-1.3.0/tests/test_GCCSDTQ.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pytest
 from pyscf import gto, lib, scf, fci
 
 from ebcc import GEBCC, NullLogger
 
 
 @pytest.mark.regression
-class GCCSDTQQ_Tests(unittest.TestCase):
+class GCCSDTQ_Tests(unittest.TestCase):
     """Test GCCSDTQ against regression.
     """
 
     def test_4_electron_exact(self):
         mol = gto.M(
                 atom=";".join(["H 0 0 %.10f" % (i*0.75) for i in range(4)]),
                 basis="sto3g",
```

### Comparing `ebcc-1.2.2/tests/test_GCCSD_SD_1_1.py` & `ebcc-1.3.0/tests/test_GCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCSD_SD_1_2.py` & `ebcc-1.3.0/tests/test_GCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCSD_S_1_1.py` & `ebcc-1.3.0/tests/test_GCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GCCSDxTx.py` & `ebcc-1.3.0/tests/test_GCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GMP2.py` & `ebcc-1.3.0/tests/test_GMP2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GMP3.py` & `ebcc-1.3.0/tests/test_GMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_GQCISD.py` & `ebcc-1.3.0/tests/test_GQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCC2.py` & `ebcc-1.3.0/tests/test_RCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCC3.py` & `ebcc-1.3.0/tests/test_RCC3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCD.py` & `ebcc-1.3.0/tests/test_RCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSD.py` & `ebcc-1.3.0/tests/test_RCCSD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSDT.py` & `ebcc-1.3.0/tests/test_RCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSD_SD_1_1.py` & `ebcc-1.3.0/tests/test_RCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSD_SD_1_2.py` & `ebcc-1.3.0/tests/test_RCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSD_S_1_1.py` & `ebcc-1.3.0/tests/test_RCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RCCSDxTx.py` & `ebcc-1.3.0/tests/test_RCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RMP2.py` & `ebcc-1.3.0/tests/test_RMP2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RMP3.py` & `ebcc-1.3.0/tests/test_RMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_RQCISD.py` & `ebcc-1.3.0/tests/test_RQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCC2.py` & `ebcc-1.3.0/tests/test_UCC2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCC3.py` & `ebcc-1.3.0/tests/test_UCC3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCD.py` & `ebcc-1.3.0/tests/test_UCCD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCSD.py` & `ebcc-1.3.0/tests/test_UCCSD.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,14 +103,68 @@
         np.testing.assert_almost_equal(self.ccsd.t2.bbbb, uebcc.t2.bbbb, 6)
         np.testing.assert_almost_equal(self.ccsd.l1.aa, uebcc.l1.aa, 5)
         np.testing.assert_almost_equal(self.ccsd.l1.bb, uebcc.l1.bb, 5)
         np.testing.assert_almost_equal(self.ccsd.l2.aaaa, uebcc.l2.aaaa, 5)
         np.testing.assert_almost_equal(self.ccsd.l2.abab, uebcc.l2.abab, 5)
         np.testing.assert_almost_equal(self.ccsd.l2.bbbb, uebcc.l2.bbbb, 5)
 
+    def test_from_rebcc_frozen(self):
+        mf = self.mf.to_rhf()
+        occupied = mf.mo_occ > 0
+        frozen = np.zeros_like(mf.mo_occ)
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ)
+        space = Space(occupied, frozen, active)
+
+        rebcc = REBCC(
+                mf,
+                ansatz="CCSD",
+                space=space,
+                log=NullLogger(),
+        )
+        rebcc.options.e_tol = 1e-12
+        rebcc.kernel()
+        rebcc.solve_lambda()
+
+        uebcc_1 = UEBCC.from_rebcc(rebcc)
+
+        mf = self.mf.to_uhf()
+        occupied = mf.mo_occ[0] > 0
+        frozen = np.zeros_like(mf.mo_occ[0])
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ[0])
+        space_a = Space(occupied, frozen, active)
+        occupied = mf.mo_occ[1] > 0
+        frozen = np.zeros_like(mf.mo_occ[1])
+        frozen[0] = True
+        active = np.zeros_like(mf.mo_occ[1])
+        space_b = Space(occupied, frozen, active)
+
+        uebcc_2 = UEBCC(
+                mf,
+                ansatz="CCSD",
+                space=(space_a, space_b),
+                log=NullLogger(),
+        )
+        uebcc_2.options.e_tol = 1e-12
+        uebcc_2.kernel()
+        uebcc_2.solve_lambda()
+
+        self.assertAlmostEqual(uebcc_2.energy(), uebcc_1.energy(), 8)
+        np.testing.assert_almost_equal(uebcc_2.t1.aa, uebcc_1.t1.aa, 6)
+        np.testing.assert_almost_equal(uebcc_2.t1.bb, uebcc_1.t1.bb, 6)
+        np.testing.assert_almost_equal(uebcc_2.t2.aaaa, uebcc_1.t2.aaaa, 6)
+        np.testing.assert_almost_equal(uebcc_2.t2.abab, uebcc_1.t2.abab, 6)
+        np.testing.assert_almost_equal(uebcc_2.t2.bbbb, uebcc_1.t2.bbbb, 6)
+        np.testing.assert_almost_equal(uebcc_2.l1.aa, uebcc_1.l1.aa, 5)
+        np.testing.assert_almost_equal(uebcc_2.l1.bb, uebcc_1.l1.bb, 5)
+        np.testing.assert_almost_equal(uebcc_2.l2.aaaa, uebcc_1.l2.aaaa, 5)
+        np.testing.assert_almost_equal(uebcc_2.l2.abab, uebcc_1.l2.abab, 5)
+        np.testing.assert_almost_equal(uebcc_2.l2.bbbb, uebcc_1.l2.bbbb, 5)
+
     def test_ip_moments(self):
         eom = self.ccsd.ip_eom()
         a = self.data[True]["ip_moms"].transpose(2, 0, 1)
         b = eom.moments(4)
         b = np.array([scipy.linalg.block_diag(x, y) for x, y in zip(b.aa, b.bb)])
         b = b[:, self.fsort][:, :, self.fsort]
         for i, (x, y) in enumerate(zip(a, b)):
```

### Comparing `ebcc-1.2.2/tests/test_UCCSDT.py` & `ebcc-1.3.0/tests/test_UCCSDT.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCSD_SD_1_1.py` & `ebcc-1.3.0/tests/test_UCCSD_SD_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCSD_SD_1_2.py` & `ebcc-1.3.0/tests/test_UCCSD_SD_1_2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCSD_S_1_1.py` & `ebcc-1.3.0/tests/test_UCCSD_S_1_1.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UCCSDxTx.py` & `ebcc-1.3.0/tests/test_UCCSDxTx.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UMP2.py` & `ebcc-1.3.0/tests/test_UMP2.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UMP3.py` & `ebcc-1.3.0/tests/test_UMP3.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_UQCISD.py` & `ebcc-1.3.0/tests/test_UQCISD.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_brueckner.py` & `ebcc-1.3.0/tests/test_brueckner.py`

 * *Files identical despite different names*

### Comparing `ebcc-1.2.2/tests/test_util.py` & `ebcc-1.3.0/tests/test_util.py`

 * *Files identical despite different names*

