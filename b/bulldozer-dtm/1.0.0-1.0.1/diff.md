# Comparing `tmp/bulldozer-dtm-1.0.0.tar.gz` & `tmp/bulldozer-dtm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/scratch/lallemd/bulldozer/master/bulldozer/dist/.tmp-jk986l_9/bulldozer-dtm-1.0.0.tar", last modified: Fri Mar 10 13:59:36 2023, max compression
+gzip compressed data, was "/work/scratch/lallemd/bulldozer/v1.0.1/bulldozer/dist/.tmp-q83o8jh_/bulldozer-dtm-1.0.1.tar", last modified: Wed Jul  5 15:49:48 2023, max compression
```

## Comparing `bulldozer-dtm-1.0.0.tar` & `bulldozer-dtm-1.0.1.tar`

### file list

```diff
@@ -1,229 +1,57 @@
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.320652 bulldozer-dtm-1.0.0/
--rw-------   0 lallemd   (9005) eolab     (8316)    11371 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/LICENSE
--rw-------   0 lallemd   (9005) eolab     (8316)       85 2023-03-10 13:22:56.000000 bulldozer-dtm-1.0.0/MANIFEST.in
--rw-------   0 lallemd   (9005) eolab     (8316)     7210 2023-03-10 13:59:36.320978 bulldozer-dtm-1.0.0/PKG-INFO
--rw-------   0 lallemd   (9005) eolab     (8316)     6189 2023-03-10 13:51:35.000000 bulldozer-dtm-1.0.0/README.md
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.646816 bulldozer-dtm-1.0.0/TMP/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.650698 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.651140 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.651561 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.652566 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.660971 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.691217 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/
--rw-------   0 lallemd   (9005) eolab     (8316)     3354 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/Code.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2918 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/FlowControl.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2468 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/ParseTreeTransforms.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     8984 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/Parsing.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2113 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/Scanning.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1792 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Compiler/Visitor.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.692462 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.762446 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/
--rw-------   0 lallemd   (9005) eolab     (8316)       61 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       66 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_bool.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_buffer.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       67 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_bytes.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_cobject.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_complex.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       66 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_dict.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_exc.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       67 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_float.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       70 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_function.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_getargs.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       70 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_instance.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_int.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       70 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_iterator.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       66 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_list.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       66 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_long.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_mapping.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_mem.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_method.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_module.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_number.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_object.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       71 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_oldbuffer.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       71 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_pycapsule.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_ref.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       70 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_sequence.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_set.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       68 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_string.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       67 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_tuple.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       66 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_type.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_unicode.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_version.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       69 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/python_weakref.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       64 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/stdio.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       65 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/stdlib.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2187 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/Deprecated/stl.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.881100 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/
--rw-------   0 lallemd   (9005) eolab     (8316)     8254 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/__init__.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     6056 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/array.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1359 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/bool.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     4870 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/buffer.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1443 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/bytearray.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     9906 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/bytes.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1390 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/cellobject.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      236 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/ceval.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1524 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/cobject.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     5084 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/codecs.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1777 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/complex.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1696 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/conversion.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     6776 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/datetime.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     6877 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/dict.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)    13606 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/exc.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1424 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/float.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2671 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/function.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1052 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/genobject.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      775 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/getargs.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      985 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/instance.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     4131 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/int.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1319 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/iterator.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1036 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/iterobject.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     4084 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/list.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     7051 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/long.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      480 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/longintrepr.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2693 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/mapping.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     5386 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/mem.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2504 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/memoryview.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2196 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/method.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     9226 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/module.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)    11922 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/number.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)    18366 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/object.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2916 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/oldbuffer.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     5692 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/pycapsule.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2000 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/pylifecycle.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3683 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/pystate.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1946 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/pythread.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2557 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/ref.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     6008 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/sequence.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     5383 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/set.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3111 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/slice.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     9944 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/string.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3206 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/tuple.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1831 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/type.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)    27009 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/unicode.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      847 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/version.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1984 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/cpython/weakref.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.909922 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/
--rw-------   0 lallemd   (9005) eolab     (8316)       13 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/__init__.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2050 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/errno.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      966 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/float.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      621 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/limits.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1140 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/locale.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2948 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/math.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      297 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/setjmp.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1170 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/signal.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      164 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/stddef.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3449 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/stdint.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2476 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/stdio.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2444 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/stdlib.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2038 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/string.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1317 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libc/time.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.178843 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/
--rw-------   0 lallemd   (9005) eolab     (8316)       94 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/__init__.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1770 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/algorithm.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      501 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/cast.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3012 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/complex.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3106 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/deque.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2392 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/forward_list.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      381 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/functional.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1432 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/iterator.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1661 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/limits.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2658 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/list.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2551 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/map.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3600 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/memory.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       27 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/pair.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      649 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/queue.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2170 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/set.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      292 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/stack.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     8731 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/string.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      524 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/typeindex.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      304 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/typeinfo.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2867 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/unordered_map.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     2622 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/unordered_set.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1040 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/utility.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3350 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/libcpp/vector.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.180833 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/numpy/
--rw-------   0 lallemd   (9005) eolab     (8316)    38138 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     5807 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/numpy/math.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1713 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/openmp.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.420299 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/
--rw-------   0 lallemd   (9005) eolab     (8316)       13 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/__init__.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      355 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/dlfcn.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1194 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/fcntl.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)       99 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/ioctl.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     3362 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/mman.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1254 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/resource.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      546 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/select.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1876 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/signal.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1734 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/stat.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1054 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/stdio.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      934 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/stdlib.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)      374 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/strings.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1980 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/time.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1162 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/types.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     8061 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/unistd.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1244 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Includes/posix/wait.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.423052 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Plex/
--rw-------   0 lallemd   (9005) eolab     (8316)      585 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Plex/Actions.pxd
--rw-------   0 lallemd   (9005) eolab     (8316)     1481 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Plex/Scanners.pxd
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.424054 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Runtime/
--rw-------   0 lallemd   (9005) eolab     (8316)     6279 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Runtime/refnanny.pyx
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.432451 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/
--rw-------   0 lallemd   (9005) eolab     (8316)     4338 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/CConvert.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)     1893 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/CpdefEnums.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)     6098 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/CppConvert.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)    49749 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/MemoryView.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)      152 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/TestCyUtilityLoader.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)     1595 2023-03-10 13:59:26.000000 bulldozer-dtm-1.0.0/TMP/build-env-3a07l0qb/lib64/python3.8/site-packages/Cython/Utility/TestCythonScope.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)       59 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/pyproject.toml
--rw-------   0 lallemd   (9005) eolab     (8316)     1322 2023-03-10 13:59:36.322204 bulldozer-dtm-1.0.0/setup.cfg
--rw-------   0 lallemd   (9005) eolab     (8316)     1724 2023-03-09 13:44:58.000000 bulldozer-dtm-1.0.0/setup.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:34.669846 bulldozer-dtm-1.0.0/src/
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.436030 bulldozer-dtm-1.0.0/src/bulldozer/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/__init__.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:35.438121 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)    16493 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/dtm_extraction.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.248418 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)     2855 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/c_springforce.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)     1327 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/c_springforce.h
--rw-------   0 lallemd   (9005) eolab     (8316)   817119 2023-02-28 09:59:27.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/springforce.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)     1074 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/springforce.pyx
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.250170 bulldozer-dtm-1.0.0/src/bulldozer/pipeline/
--rw-------   0 lallemd   (9005) eolab     (8316)        1 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/pipeline/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)    10330 2023-03-07 17:07:59.000000 bulldozer-dtm-1.0.0/src/bulldozer/pipeline/bulldozer_pipeline.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.254846 bulldozer-dtm-1.0.0/src/bulldozer/postprocessing/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/postprocessing/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)    16485 2023-03-09 12:52:21.000000 bulldozer-dtm-1.0.0/src/bulldozer/postprocessing/dtm_postprocess.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.256635 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/__init__.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.300938 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)   835701 2023-02-28 09:59:28.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/bordernodata.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)     2817 2023-02-21 13:20:46.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/bordernodata.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)     1198 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/c_bordernodata.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)      983 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/c_bordernodata.h
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.307282 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)     6249 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)     2810 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.h
--rw-------   0 lallemd   (9005) eolab     (8316)   838436 2023-03-10 13:59:33.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/disturbedareas.cpp
--rw-------   0 lallemd   (9005) eolab     (8316)     3156 2023-02-21 13:19:07.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/disturbedareas.pyx
--rw-------   0 lallemd   (9005) eolab     (8316)    13617 2023-03-10 13:56:57.000000 bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/dsm_preprocess.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.310223 bulldozer-dtm-1.0.0/src/bulldozer/scale/
--rw-------   0 lallemd   (9005) eolab     (8316)     6803 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/scale/Shared.py
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/scale/__init__.py
--rw-------   0 lallemd   (9005) eolab     (8316)     8155 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/scale/tools.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.314341 bulldozer-dtm-1.0.0/src/bulldozer/utils/
--rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/utils/__init__.py
--rwx------   0 lallemd   (9005) eolab     (8316)     3098 2023-02-21 09:52:24.000000 bulldozer-dtm-1.0.0/src/bulldozer/utils/config_parser.py
--rw-------   0 lallemd   (9005) eolab     (8316)     6390 2023-03-09 12:41:26.000000 bulldozer-dtm-1.0.0/src/bulldozer/utils/helper.py
--rw-------   0 lallemd   (9005) eolab     (8316)     5063 2023-03-02 15:14:36.000000 bulldozer-dtm-1.0.0/src/bulldozer/utils/logging_helper.py
-drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-03-10 13:59:36.319954 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/
--rw-------   0 lallemd   (9005) eolab     (8316)     7210 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/PKG-INFO
--rw-------   0 lallemd   (9005) eolab     (8316)    15600 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/SOURCES.txt
--rw-------   0 lallemd   (9005) eolab     (8316)        1 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/dependency_links.txt
--rw-------   0 lallemd   (9005) eolab     (8316)       82 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/entry_points.txt
--rw-------   0 lallemd   (9005) eolab     (8316)      101 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/requires.txt
--rw-------   0 lallemd   (9005) eolab     (8316)       10 2023-03-10 13:59:34.000000 bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/top_level.txt
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.572465 bulldozer-dtm-1.0.1/
+-rw-------   0 lallemd   (9005) eolab     (8316)    11371 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/LICENSE
+-rw-------   0 lallemd   (9005) eolab     (8316)       85 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/MANIFEST.in
+-rw-------   0 lallemd   (9005) eolab     (8316)     7268 2023-07-05 15:49:48.572684 bulldozer-dtm-1.0.1/PKG-INFO
+-rw-------   0 lallemd   (9005) eolab     (8316)     6247 2023-07-05 09:44:46.000000 bulldozer-dtm-1.0.1/README.md
+-rw-------   0 lallemd   (9005) eolab     (8316)       59 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/pyproject.toml
+-rw-------   0 lallemd   (9005) eolab     (8316)     1322 2023-07-05 15:49:48.573698 bulldozer-dtm-1.0.1/setup.cfg
+-rw-------   0 lallemd   (9005) eolab     (8316)     1724 2023-06-25 06:46:24.000000 bulldozer-dtm-1.0.1/setup.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.511468 bulldozer-dtm-1.0.1/src/
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.516368 bulldozer-dtm-1.0.1/src/bulldozer/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/__init__.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.517779 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)    17307 2023-07-05 09:53:49.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/dtm_extraction.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.544885 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     2855 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/c_springforce.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)     1327 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/c_springforce.h
+-rw-------   0 lallemd   (9005) eolab     (8316)   817119 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/springforce.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)     1074 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/springforce.pyx
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.546334 bulldozer-dtm-1.0.1/src/bulldozer/pipeline/
+-rw-------   0 lallemd   (9005) eolab     (8316)        1 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/pipeline/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     9799 2023-07-05 09:55:24.000000 bulldozer-dtm-1.0.1/src/bulldozer/pipeline/bulldozer_pipeline.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.547800 bulldozer-dtm-1.0.1/src/bulldozer/postprocessing/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/postprocessing/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)    16820 2023-07-05 09:44:46.000000 bulldozer-dtm-1.0.1/src/bulldozer/postprocessing/dtm_postprocess.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.549856 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/__init__.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.556442 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)   837392 2023-07-05 15:49:43.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/bordernodata.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)     2817 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/bordernodata.pyx
+-rw-------   0 lallemd   (9005) eolab     (8316)     1198 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/c_bordernodata.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)      983 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/c_bordernodata.h
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.562422 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     6253 2023-07-05 09:44:40.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)     2810 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.h
+-rw-------   0 lallemd   (9005) eolab     (8316)   840127 2023-07-05 15:49:45.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/disturbedareas.cpp
+-rw-------   0 lallemd   (9005) eolab     (8316)     3156 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/disturbedareas.pyx
+-rw-------   0 lallemd   (9005) eolab     (8316)    15598 2023-07-05 09:44:46.000000 bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/dsm_preprocess.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.564442 bulldozer-dtm-1.0.1/src/bulldozer/scale/
+-rw-------   0 lallemd   (9005) eolab     (8316)    10559 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/scale/Shared.py
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/scale/__init__.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     8419 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/scale/tools.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.567673 bulldozer-dtm-1.0.1/src/bulldozer/utils/
+-rw-------   0 lallemd   (9005) eolab     (8316)        0 2023-06-25 06:39:59.000000 bulldozer-dtm-1.0.1/src/bulldozer/utils/__init__.py
+-rwx------   0 lallemd   (9005) eolab     (8316)     3098 2023-06-25 06:58:08.000000 bulldozer-dtm-1.0.1/src/bulldozer/utils/config_parser.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     7125 2023-07-05 09:50:18.000000 bulldozer-dtm-1.0.1/src/bulldozer/utils/helper.py
+-rw-------   0 lallemd   (9005) eolab     (8316)     5421 2023-07-05 09:44:46.000000 bulldozer-dtm-1.0.1/src/bulldozer/utils/logging_helper.py
+drwx------   0 lallemd   (9005) eolab     (8316)        0 2023-07-05 15:49:48.571968 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/
+-rw-------   0 lallemd   (9005) eolab     (8316)     7268 2023-07-05 15:49:48.568606 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/PKG-INFO
+-rw-------   0 lallemd   (9005) eolab     (8316)     1783 2023-07-05 15:49:48.569224 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/SOURCES.txt
+-rw-------   0 lallemd   (9005) eolab     (8316)        1 2023-07-05 15:49:48.569920 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/dependency_links.txt
+-rw-------   0 lallemd   (9005) eolab     (8316)       82 2023-07-05 15:49:48.570641 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/entry_points.txt
+-rw-------   0 lallemd   (9005) eolab     (8316)      101 2023-07-05 15:49:48.571330 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/requires.txt
+-rw-------   0 lallemd   (9005) eolab     (8316)       10 2023-07-05 15:49:48.572057 bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/top_level.txt
```

### Comparing `bulldozer-dtm-1.0.0/LICENSE` & `bulldozer-dtm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/PKG-INFO` & `bulldozer-dtm-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulldozer-dtm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bulldozer is a DTM extraction tool requiring only a DSM as input
 Home-page: https://github.com/CNES/bulldozer
 Author: CNES
 Author-email: pierre.lassalle@cnes.fr,dimitri.lallement@cnes.fr,yannick.ott@thalesgroup.com
 License: Apache V2.0
 Keywords: bulldozer,DTM,DSM,3D,Photogrammetry,Remote Sensing,LiDar,CARS
 Classifier: Development Status :: 4 - Beta
@@ -19,23 +19,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-    <img src="docs/source/images/bulldozer_logo.png" width=256
-    >
+    <img src="https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/bulldozer_logo.png" width=256>
 
 **Bulldozer, a DTM extraction tool requiring only a DSM as input.**
 
 [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)](CONTRIBUTING.md)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer/)
+[![PyPI Version](https://img.shields.io/pypi/v/bulldozer-dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-dtm/)
 
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#installation">Installation</a> •  
   <a href="#quick-start">Quick Start</a> •
   <a href="#documentation">Documentation</a> •
@@ -47,15 +46,15 @@
 </div>
 
 ---
 
 ## Key features
 
 <div align="center">
-<img src="docs/source/images/result_overview.gif" alt="drawing" width="400"/>
+<img src="docs/source/images/result_overview.gif" alt="demo" width="400"/>
 </div>
 
 **Bulldozer** is designed as a pipeline of standalone functions that aims to extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).  
 But you can also use one of the following function without running the full pipeline:
 * **DSM preprocessing**
     * **Nodata extraction:** a group of methods to differentiate and extract nodata related to failed correlations during the DSM computation and those of the image border
     * **Disturbed areas detection:** a method to locate disturbed areas. These noisy areas are mainly related to areas in which the correlator has incorrectly estimated the elevation (water or shadow areas).
@@ -94,17 +93,17 @@
 pip install .
 ```
 ## Quick Start
 
 1. First you have to create a configuration file or edit the `configuration_template.yaml` available in the `conf` directory. You have to update at least the following parameters:
 ```yaml
 # Input DSM path (expected format: "<folder_1>/<folder_2>/<file>.<[tif/tiff]>")
-dsmPath : "<input_dsm.tif>"
+dsm_path : "<input_dsm.tif>"
 # Output directory path (if the directory doesn't exist, create it)
-outputDir : "<output_dir>"
+output_dir : "<output_dir>"
 ```
 2. Run the pipeline:
    * Through CLI *(Command Line Interface)*
    ```console
    bulldozer --conf conf/configuration_template.yaml
    ```
    * Through Python API using the config file
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: bulldozer-dtm Version: 1.0.0 Summary: Bulldozer is
+Metadata-Version: 2.1 Name: bulldozer-dtm Version: 1.0.1 Summary: Bulldozer is
 a DTM extraction tool requiring only a DSM as input Home-page: https://
 github.com/CNES/bulldozer Author: CNES Author-email:
 pierre.lassalle@cnes.fr,dimitri.lallement@cnes.fr,yannick.ott@thalesgroup.com
 License: Apache V2.0 Keywords: bulldozer,DTM,DSM,3D,Photogrammetry,Remote
 Sensing,LiDar,CARS Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE
-  [docs/source/images/bulldozer_logo.png] **Bulldozer, a DTM extraction tool
-   requiring only a DSM as input.** [![Python](https://img.shields.io/badge/
-python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
- [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-
-orange.svg)](CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
+ [https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/
+bulldozer_logo.png] **Bulldozer, a DTM extraction tool requiring only a DSM as
+input.** [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https:
+   //www.python.org/downloads/release/python-380/) [![Contributions welcome]
+       (https://img.shields.io/badge/contributions-welcome-orange.svg)]
+      (CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
   Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![PyPI
-                    Version](https://img.shields.io/pypi/v/
-  bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/
-                                  bulldozer/)
+               Version](https://img.shields.io/pypi/v/bulldozer-
+dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-
+                                     dtm/)
 Key_Features â¢ Installation â¢ Quick_Start â¢ Documentation â¢ Contribute
                            â¢ Licence â¢ Reference
 --- ## Key features
-                                   [drawing]
+                                    [demo]
 **Bulldozer** is designed as a pipeline of standalone functions that aims to
 extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).
 But you can also use one of the following function without running the full
 pipeline: * **DSM preprocessing** * **Nodata extraction:** a group of methods
 to differentiate and extract nodata related to failed correlations during the
 DSM computation and those of the image border * **Disturbed areas detection:**
 a method to locate disturbed areas. These noisy areas are mainly related to
@@ -46,17 +47,17 @@
 docs.conda.io/en/latest/) or [virtualenv](https://virtualenv.pypa.io/en/latest/
 ). * Installation with `virtualenv`: ```sh # Clone the project git clone https:
 //github.com/CNES/bulldozer.git cd bulldozer/ # Create the environment python -
 m venv bulldozer_venv source bulldozer_venv/bin/activate # Install the library
 pip install . ``` ## Quick Start 1. First you have to create a configuration
 file or edit the `configuration_template.yaml` available in the `conf`
 directory. You have to update at least the following parameters: ```yaml #
-Input DSM path (expected format: "//.<[tif/tiff]>") dsmPath : "
+Input DSM path (expected format: "//.<[tif/tiff]>") dsm_path : "
 tif>" # Output directory path (if the directory doesn't exist, create it)
-outputDir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
+output_dir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
 Interface)* ```console bulldozer --conf conf/configuration_template.yaml ``` *
 Through Python API using the config file ```python from
 bulldozer.pipeline.bulldozer_pipeline import dsm_to_dtm dsm_to_dtm
 (config_path="conf/configuration_template.yaml") ``` * Through Python API
 providing directly the input parameters (missing parameters will be replaced by
 default values) ```python from bulldozer.pipeline.bulldozer_pipeline import
 dsm_to_dtm # Example with a specific number of workers dsm_to_dtm(dsm_path="
```

### Comparing `bulldozer-dtm-1.0.0/README.md` & `bulldozer-dtm-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 <div align="center">
-    <img src="docs/source/images/bulldozer_logo.png" width=256
-    >
+    <img src="https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/bulldozer_logo.png" width=256>
 
 **Bulldozer, a DTM extraction tool requiring only a DSM as input.**
 
 [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)](CONTRIBUTING.md)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer/)
+[![PyPI Version](https://img.shields.io/pypi/v/bulldozer-dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-dtm/)
 
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#installation">Installation</a> •  
   <a href="#quick-start">Quick Start</a> •
   <a href="#documentation">Documentation</a> •
@@ -23,15 +22,15 @@
 </div>
 
 ---
 
 ## Key features
 
 <div align="center">
-<img src="docs/source/images/result_overview.gif" alt="drawing" width="400"/>
+<img src="docs/source/images/result_overview.gif" alt="demo" width="400"/>
 </div>
 
 **Bulldozer** is designed as a pipeline of standalone functions that aims to extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).  
 But you can also use one of the following function without running the full pipeline:
 * **DSM preprocessing**
     * **Nodata extraction:** a group of methods to differentiate and extract nodata related to failed correlations during the DSM computation and those of the image border
     * **Disturbed areas detection:** a method to locate disturbed areas. These noisy areas are mainly related to areas in which the correlator has incorrectly estimated the elevation (water or shadow areas).
@@ -70,17 +69,17 @@
 pip install .
 ```
 ## Quick Start
 
 1. First you have to create a configuration file or edit the `configuration_template.yaml` available in the `conf` directory. You have to update at least the following parameters:
 ```yaml
 # Input DSM path (expected format: "<folder_1>/<folder_2>/<file>.<[tif/tiff]>")
-dsmPath : "<input_dsm.tif>"
+dsm_path : "<input_dsm.tif>"
 # Output directory path (if the directory doesn't exist, create it)
-outputDir : "<output_dir>"
+output_dir : "<output_dir>"
 ```
 2. Run the pipeline:
    * Through CLI *(Command Line Interface)*
    ```console
    bulldozer --conf conf/configuration_template.yaml
    ```
    * Through Python API using the config file
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-  [docs/source/images/bulldozer_logo.png] **Bulldozer, a DTM extraction tool
-   requiring only a DSM as input.** [![Python](https://img.shields.io/badge/
-python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
- [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-
-orange.svg)](CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
+ [https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/
+bulldozer_logo.png] **Bulldozer, a DTM extraction tool requiring only a DSM as
+input.** [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https:
+   //www.python.org/downloads/release/python-380/) [![Contributions welcome]
+       (https://img.shields.io/badge/contributions-welcome-orange.svg)]
+      (CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
   Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![PyPI
-                    Version](https://img.shields.io/pypi/v/
-  bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/
-                                  bulldozer/)
+               Version](https://img.shields.io/pypi/v/bulldozer-
+dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-
+                                     dtm/)
 Key_Features â¢ Installation â¢ Quick_Start â¢ Documentation â¢ Contribute
                            â¢ Licence â¢ Reference
 --- ## Key features
-                                   [drawing]
+                                    [demo]
 **Bulldozer** is designed as a pipeline of standalone functions that aims to
 extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).
 But you can also use one of the following function without running the full
 pipeline: * **DSM preprocessing** * **Nodata extraction:** a group of methods
 to differentiate and extract nodata related to failed correlations during the
 DSM computation and those of the image border * **Disturbed areas detection:**
 a method to locate disturbed areas. These noisy areas are mainly related to
@@ -32,17 +33,17 @@
 docs.conda.io/en/latest/) or [virtualenv](https://virtualenv.pypa.io/en/latest/
 ). * Installation with `virtualenv`: ```sh # Clone the project git clone https:
 //github.com/CNES/bulldozer.git cd bulldozer/ # Create the environment python -
 m venv bulldozer_venv source bulldozer_venv/bin/activate # Install the library
 pip install . ``` ## Quick Start 1. First you have to create a configuration
 file or edit the `configuration_template.yaml` available in the `conf`
 directory. You have to update at least the following parameters: ```yaml #
-Input DSM path (expected format: "//.<[tif/tiff]>") dsmPath : "
+Input DSM path (expected format: "//.<[tif/tiff]>") dsm_path : "
 tif>" # Output directory path (if the directory doesn't exist, create it)
-outputDir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
+output_dir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
 Interface)* ```console bulldozer --conf conf/configuration_template.yaml ``` *
 Through Python API using the config file ```python from
 bulldozer.pipeline.bulldozer_pipeline import dsm_to_dtm dsm_to_dtm
 (config_path="conf/configuration_template.yaml") ``` * Through Python API
 providing directly the input parameters (missing parameters will be replaced by
 default values) ```python from bulldozer.pipeline.bulldozer_pipeline import
 dsm_to_dtm # Example with a specific number of workers dsm_to_dtm(dsm_path="
```

### Comparing `bulldozer-dtm-1.0.0/setup.cfg` & `bulldozer-dtm-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bulldozer-dtm
-version = 1.0.0
+version = 1.0.1
 description = Bulldozer is a DTM extraction tool requiring only a DSM as input
 url = https://github.com/CNES/bulldozer
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache V2.0
 license_files = LICENSE
 keywords = bulldozer,DTM,DSM,3D,Photogrammetry,Remote Sensing,LiDar,CARS
```

### Comparing `bulldozer-dtm-1.0.0/setup.py` & `bulldozer-dtm-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/dtm_extraction.py` & `bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/dtm_extraction.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import os
 import math
 import logging
 import rasterio
 import numpy as np
 from tqdm import tqdm
 import concurrent.futures
+import scipy.ndimage as ndimage
 from collections import namedtuple
 import bulldozer.springforce as sf
 from bulldozer.utils.logging_helper import BulldozerLogger
 from bulldozer.utils.helper import downsample_profile, retrieve_raster_resolution, Pyramid, write_tiles
 
 Tile = namedtuple('Tile', ['start_y', 'start_x', 'end_y', 'end_x', 'margin_top', 'margin_right', 'margin_bottom', 'margin_left', 'path'])
 
@@ -38,24 +39,27 @@
                  max_object_size: int = 16,
                  uniform_filter_size: int = 3,
                  prevent_unhook_iter: int = 100,
                  num_outer_iterations: int = 100,
                  num_inner_iterations: int= 10,
                  mp_tile_size: int = 1500,
                  output_resolution : float = -1.,
-                 mp_nb_procs: int = 16):
+                 mp_nb_procs: int = 16,
+                 keep_inter_dtm: bool = False):
         """ """
         self.max_object_size: int = max_object_size
         self.uniform_filter_size: int = uniform_filter_size
         self.prevent_unhook_iter: int = prevent_unhook_iter
         self.num_outer_iterations: int = num_outer_iterations
         self.num_inner_iterations: int= num_inner_iterations
         self.mp_tile_size: int = mp_tile_size
         self.output_resolution = output_resolution
         self.mp_nb_procs: int = mp_nb_procs
+        self.keep_inter_dtm: bool = keep_inter_dtm
+
 
     def next_power_of_2(self, x : int) -> int:
         """
         This function returns the smallest power of 2 that is greater than or equal to a given non-negative integer x.
 
         Args:
             x : non negative integer.
@@ -207,18 +211,15 @@
             
             for j in range(self.num_inner_iterations):
 
                 # handle DSM intersections, snap back to below DSM
                 np.minimum(dtm, dsm, out=dtm, where=valid)
 
                 # apply spring tension forces (blur the DTM)
-                nb_rows = dtm.shape[0]
-                nb_cols = dtm.shape[1]
-                dtm = bfilters.run(dtm, nb_rows, nb_cols, self.uniform_filter_size, nodata_val)
-                dtm = dtm.reshape((nb_rows, nb_cols))
+                dtm = ndimage.uniform_filter(dtm, size=self.uniform_filter_size)
                 
         # One final intersection check
         np.minimum(dtm, dsm, out=dtm, where=valid)
         valid = None
         return dtm
 
     def tiled_drape_cloth(self,
@@ -279,18 +280,15 @@
         # Initialize the dtm at this current dsm.
         dsm = dsm_pyramid.getArrayAtLevel(level=nb_levels-1)
         dtm = dsm.copy()
 
         # Prevent unhook from hills
         bfilters = sf.PyBulldozerFilters()
         for i in tqdm(range(self.prevent_unhook_iter), desc="Prevent unhook from hills..."):
-            nb_rows = dtm.shape[0]
-            nb_cols = dtm.shape[1]
-            dtm = bfilters.run(dtm, nb_rows, nb_cols, self.uniform_filter_size, nodata_val)
-            dtm = dtm.reshape((nb_rows, nb_cols))
+            dtm = ndimage.uniform_filter(dtm, size=self.uniform_filter_size)
         
         
         # Get min and max valid height from dsm
         
         valid_data = dsm[dsm != nodata_val]
         min_alt = np.min(valid_data)
         max_alt = np.max(valid_data)
@@ -300,14 +298,23 @@
         step = (max_alt - min_alt) / self.num_outer_iterations
 
         # Init classical parameters of drap cloth
         level = nb_levels - 1
         max_level = nb_levels - 1
         current_num_outer_iterations = self.num_outer_iterations
 
+        start_res = self.output_resolution if self.output_resolution is not None and self.output_resolution > dsm_res else dsm_res
+        resolutions = [ start_res ]
+        i: int = 1
+        for l in range(min_level + 1, nb_levels):
+            resolutions.append( resolutions[i-1] * 2.0 )
+            i += 1
+        
+        i = len(resolutions) - 1
+
         while level >= min_level:
 
             BulldozerLogger.log("Process level " + str(level) + "...", logging.INFO)
 
             if level < max_level:
                 
                 next_shape : tuple = dsm_pyramid.shape(level=level)
@@ -382,16 +389,27 @@
             else:
                 dtm = self.sequential_drape_cloth(dtm = dtm,
                                                   dsm = dsm,
                                                   num_outer_iterations = current_num_outer_iterations,
                                                   step = step,
                                                   nodata_val = nodata_val)
 
+            # flush this intermediate dtm to disk
+            if level > min_level and self.keep_inter_dtm:
+                inter_dtm_profile = downsample_profile(in_dsm_profile, 2**level)
+                inter_dtm_profile['nodata'] = nodata_val
+                inter_dtm_path = os.path.join(output_dir, "raw_DTM_" + str(resolutions[i]).replace(".", "_") + ".tif")
+                write_tiles(tile_buffer= dtm, 
+                            tile_path = inter_dtm_path,
+                            original_profile = inter_dtm_profile,
+                            tagLevel=level)
+            
             # Decrease level
             level -= 1
+            i -= 1
             dsm = None
 
             # Decrease step and number of outer iterations
             step = step / (2 * 2 ** (max_level - level))
             current_num_outer_iterations = max(1, int(self.num_outer_iterations / 2**(max_level - level)))
         
         dtm_profile = downsample_profile(in_dsm_profile, 2**min_level)
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/c_springforce.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/c_springforce.cpp`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/c_springforce.h` & `bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/c_springforce.h`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/springforce.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/springforce.cpp`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/dtm_extraction/springforce/springforce.pyx` & `bulldozer-dtm-1.0.1/src/bulldozer/dtm_extraction/springforce/springforce.pyx`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/pipeline/bulldozer_pipeline.py` & `bulldozer-dtm-1.0.1/src/bulldozer/pipeline/bulldozer_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,65 +19,96 @@
 # limitations under the License.
 
 """
     This module is used to postprocess the DTM in order to improve its quality. It required a DTM generated from Bulldozer.
 """
 import os
 import sys
+import logging
 from shutil import copy
 from datetime import datetime
 from sys import stdout
 import argparse
 import multiprocessing
 import argcomplete
 from bulldozer.dtm_extraction.dtm_extraction import ClothSimulation
 from bulldozer.preprocessing.dsm_preprocess import preprocess_pipeline
 from bulldozer.postprocessing.dtm_postprocess import postprocess_pipeline
 from bulldozer.utils.config_parser import ConfigParser
 from bulldozer.utils.logging_helper import BulldozerLogger
-from bulldozer.utils.helper import Runtime, retrieve_nodata
+from bulldozer.utils.helper import Runtime, retrieve_nodata, DefaultValues
 
-#import threading
-import time
+__version__ = "1.0.1"
 
-__version__ = "1.0.0"
+@Runtime
+def dsm_to_dtm(config_path : str = None, **kwargs) -> None:
+    """
+        Main pipeline orchestrator.
+        
+        Args:
+            config_path: path to the config file (YAML file expected, refers to the provided template in /conf).
+            **kwargs: bulldozer parameters (used if the user don't provide a configuration file).
 
+    """
+    # Retrieves Bulldozer settings from the config file, the CLI parameters or the Python API parameters
+    params = retrieve_params(config_path, **kwargs) 
 
-# import psutil
-
-# stop_thread = False
-
-# def memory() :
-#     t0 = time.time()
-#     with open('memory.txt', 'w') as out :
-#         process = psutil.Process(os.getpid())
-#         while    :
-#             t = time.time()True
-#             mem = process.memory_info()
-#             print("%.2f" % (t - t0), "%.2f" %  (mem.rss / 1024 / 1024), end='', file=out)
-            
-#             children = process.children()
-#             for child in children:
-#                 print('\t', "%.2f" %  (child.memory_info().rss / 1024 / 1024), end='', file=out) 
-        
-#             print('', file=out)
-#             time.sleep(0.5)
-#             global stop_thread
-#             if stop_thread:
-#                 out.close()
-#                 break
+    # If the target output directory does not exist, creates it
+    if not os.path.isdir(params['output_dir']):
+            os.makedirs(params['output_dir']) 
 
-@Runtime
-def dsm_to_dtm(config_path : str = None, **kwargs) -> None:
+    logger = BulldozerLogger.getInstance(logger_file_path=os.path.join(params['output_dir'], "trace_" + datetime.now().strftime("%d.%m.%Y_%H:%M:%S") +".log"))
+
+    BulldozerLogger.log("Bulldozer input parameters: \n" + "".join("\t- " + str(key) +": " + str(value) + "\n" for key, value in params.items()), logging.DEBUG)
+
+    preprocessed_dsm_path, quality_mask_path = preprocess_pipeline(dsm_path = params['dsm_path'], 
+                                                                   output_dir = params['output_dir'], 
+                                                                   nb_max_workers = params['nb_max_workers'], 
+                                                                   nodata = params['nodata'], 
+                                                                   slope_threshold = params['slope_threshold'], 
+                                                                   is_four_connexity = params['four_connexity'],
+                                                                   minValidHeight = params['min_valid_height'])
+
+    clothSimu = ClothSimulation(params['max_object_width'], 
+                                params['uniform_filter_size'], 
+                                params['prevent_unhook_iter'],
+                                params['num_outer_iter'], 
+                                params['num_inner_iter'], 
+                                params['mp_tile_size'],
+                                params['output_resolution'], 
+                                params['nb_max_workers'],
+                                params['keep_inter_dtm'])
+
+    raw_dtm_path: str = clothSimu.run(preprocessed_dsm_path, 
+                                      params['output_dir'], 
+                                      params['nodata'])
+
+    postprocess_pipeline(raw_dtm_path =  raw_dtm_path, 
+                         output_dir = params['output_dir'],
+                         nb_max_workers = params['nb_max_workers'],
+                         quality_mask_path =  quality_mask_path, 
+                         generate_dhm = params['generate_dhm'], 
+                         dsm_path = params['dsm_path'],
+                         check_intersection = params['check_intersection'],
+                         nodata = params['nodata'])
+    
+    if not params['developper_mode']:
+        # Remove the raw DTM since the postprocess pipeline generates a refined DTM
+        preprocessed_dsm_path = os.path.join(params['output_dir'], 'preprocessed_DSM.tif')
+        os.remove(raw_dtm_path)
+        os.remove(preprocessed_dsm_path)
+
+def retrieve_params(config_path : str = None, **kwargs):
     """
-        Pipeline orchestrator.
+        Defines the input parameters based on the provided configuration file (if provided), or the kwargs (CLI or Python API).
+        For the missing parameters the Bullodzer default values are set.
         
         Args:
             config_path: path to the config file (YAML file expected, refers to the provided template in /conf).
-            **kwargs: you can directly provide the parameters but we expect the following parameters name :
+            **kwargs: list of expected arguments if the urser don't provide a configuration file:
                 - dsm_path: str (required)
                 - output_dir: str (required)
                 - nodata: float (optionnal)
                 - nb_max_workers: int (optionnal)
                 - slope_threshold: float (optionnal)
                 - four_connexit: bool (optionnal)
                 - min_valid_heigh: float (optionnal)
@@ -87,128 +118,67 @@
                 - num_outer_iter: int (optionnal)
                 - num_inner_iter: int (optionnal)
                 - mp_tile_size: int (optionnal)
                 - output_resolution: float (optionnal)
                 - generate_dhm: bool (optionnal)
                 - check_intersection: bool (optionnal)
                 - developper_mode : bool (optionnal)
-                refers to the config file template to understand the use of each parameter.
-
+                refers to the documentation to understand the use of each parameter.
     """
+    bulldozer_params = dict()
     # Config path provided case
+
+    input_params = dict()
+
     if config_path:
         # Configuration file format check
         if not (config_path.endswith('.yaml') or config_path.endswith('.yml')) :
             raise ValueError('Expected yaml configuration file: \'config_path\' argument should be a path to a Yaml file (here: {})'.format(config_path))
 
         # Configuration file existence check
         if not os.path.isfile(config_path):
             raise FileNotFoundError('The input configuration file \'{}\' doesn\'t exist'.format(config_path))
         
         # Retrieves all the settings
         parser = ConfigParser(False)
-        cfg = parser.read(config_path)
-        dsm_path = cfg['dsmPath']
-        output_dir = cfg['outputDir']
-        nodata = cfg['noData']
-        nb_max_workers = cfg['nbMaxWorkers']
-        slope_threshold = cfg['slopeThreshold']
-        four_connexity = cfg['fourConnexity']
-        min_valid_height = cfg['minValidHeight']
-        max_object_width = cfg['maxObjectWidth']
-        uniform_filter_size = cfg['uniformFilterSize']
-        prevent_unhook_iter = cfg['preventUnhookIter']
-        num_outer_iter = cfg['numOuterIter']
-        num_inner_iter = cfg['numInnerIter']
-        mp_tile_size = cfg['mpTileSize']
-        output_resolution = cfg['outputResolution']
-        generate_dhm = cfg['generateDhm']
-        check_intersection = cfg['checkIntersection']
-        developper_mode = cfg['developperMode']
-    # User directly provide the configuration as dsm_to_dtm parameters case
+        input_params = parser.read(config_path)
+        if 'dsm_path' not in input_params.keys():
+            raise ValueError('No DSM path provided or invalid YAML key syntax. Expected: dsm_path="<path>/<dsm_file>.<[tif/tiff]>"')
+        else:
+            bulldozer_params['dsm_path'] = input_params['dsm_path']
+
+        if 'output_dir' not in input_params.keys():
+            raise ValueError('No output diectory path provided or invalid YAML key syntax. Expected: output_dir="<path>")')
+        else:
+            bulldozer_params['output_dir'] = input_params['output_dir']
     else :
-        if not 'dsm_path' in kwargs:
-            raise ValueError('No DSM path provided or invalid argument syntax. Expected dsm_to_dtm(dsm_path="<path>")')
-        dsm_path = kwargs['dsm_path']
-        if not 'output_dir' in kwargs:
-            raise ValueError('No output diectory path provided or invalid argument syntax. Expected dsm_to_dtm(dsm_path="<path>, output_dir="<path>")')
-        output_dir = kwargs['output_dir']
-        nodata = kwargs['nodata'] if 'nodata' in kwargs else None
-        nb_max_workers = kwargs['nb_max_workers'] if 'nb_max_workers' in kwargs else None
-        slope_threshold = kwargs['slope_threshold'] if 'slope_threshold' in kwargs else None
-        four_connexity = kwargs['four_connexity'] if 'four_connexity' in kwargs else None
-        min_valid_height = kwargs['min_valid_height'] if 'min_valid_height' in kwargs else None
-        max_object_width = kwargs['max_object_width'] if 'max_object_width' in kwargs else None
-        uniform_filter_size = kwargs['uniform_filter_size'] if 'uniform_filter_size' in kwargs else None
-        prevent_unhook_iter = kwargs['prevent_unhook_iter'] if 'prevent_unhook_iter' in kwargs else None
-        num_outer_iter = kwargs['num_outer_iter'] if 'num_outer_iter' in kwargs else None
-        num_inner_iter = kwargs['num_inner_iter'] if 'num_inner_iter' in kwargs else None
-        mp_tile_size = kwargs['mp_tile_size'] if 'mp_tile_size' in kwargs else None
-        output_resolution = kwargs['output_resolution'] if 'output_resolution' in kwargs else None
-        generate_dhm = kwargs['generate_dhm'] if 'generate_dhm' in kwargs else None
-        check_intersection = kwargs['check_intersection'] if 'check_intersection' in kwargs else None
-        developper_mode = kwargs['developper_mode'] if 'developper_mode' in kwargs else None
-    
-    # If the target output directory does not exist, creates it
-    if not os.path.isdir(output_dir):
-            os.mkdir(output_dir) 
-
-    logger = BulldozerLogger.getInstance(logger_file_path=os.path.join(output_dir, "trace_" + datetime.now().strftime("%d.%m.%Y_%H:%M:%S") +".log"))
-   
-    # x = threading.Thread(target=memory)
-    # x.start()
-
-    # Retrieves the nodata value from the config file or the DSM metadata
-    nodata = retrieve_nodata(dsm_path, nodata)
+        # User directly provides the input parameters (kwargs)
+        input_params = kwargs
+        if not 'dsm_path' in input_params:
+            raise ValueError('No DSM path provided or invalid argument syntax. Expected: \n\t-Python API: dsm_to_dtm(dsm_path="<path>")\n\t-CLI: bulldozer -in <path>')
+        bulldozer_params['dsm_path'] = input_params['dsm_path']
+        if not 'output_dir' in input_params:
+            raise ValueError('No output diectory path provided or invalid argument syntax. Expected: \n\t-Python API:  dsm_to_dtm(dsm_path="<path>, output_dir="<path>")\n\t-CLI: bulldozer -in <path> -out path')
+        bulldozer_params['output_dir'] = input_params['output_dir']
+
+    # For each optional parameters of Bulldozer check if the user provide a specific value, otherwise retrieve the default value from DefaultValues enum
+    for key, value in DefaultValues.items():
+        bulldozer_params[key.lower()] = input_params[key.lower()] if key.lower() in input_params.keys() else value  
+        
+    # Retrieves the nodata value from input DSM metadata if the user didn't provides a specific value
+    if bulldozer_params['nodata'] is None:
+        bulldozer_params['nodata'] = retrieve_nodata(bulldozer_params['dsm_path'])
     
-    # Retrieves the number of CPU if the number of available workers is not set
-    if not nb_max_workers:
-        nb_max_workers = multiprocessing.cpu_count()
+    # Retrieves the number of CPU if the number of available workers if the user didn't provides a specific value
+    if bulldozer_params['nb_max_workers'] is None:
+        bulldozer_params['nb_max_workers'] = multiprocessing.cpu_count()
     
-    preprocessed_dsm_path, quality_mask_path = preprocess_pipeline(dsm_path = dsm_path, 
-                                                                   output_dir = output_dir, 
-                                                                   nb_max_workers = nb_max_workers, 
-                                                                   nodata = nodata, 
-                                                                   slope_threshold = slope_threshold, 
-                                                                   is_four_connexity = four_connexity,
-                                                                   minValidHeight = min_valid_height)
+    return bulldozer_params
     
 
-    clothSimu = ClothSimulation(max_object_width, 
-                                uniform_filter_size, 
-                                prevent_unhook_iter,
-                                num_outer_iter, 
-                                num_inner_iter, 
-                                mp_tile_size,
-                                output_resolution, 
-                                nb_max_workers)
-
-    raw_dtm_path: str = clothSimu.run(preprocessed_dsm_path, 
-                                      output_dir, 
-                                      nodata)
-
-    postprocess_pipeline(raw_dtm_path =  raw_dtm_path, 
-                         output_dir = output_dir,
-                         nb_max_workers = nb_max_workers,
-                         quality_mask_path =  quality_mask_path, 
-                         generate_dhm = generate_dhm, 
-                         dsm_path = dsm_path,
-                         check_intersection = check_intersection,
-                         nodata = nodata)
-    
-    if not developper_mode:
-        # Remove the raw DTM since the postprocess pipeline generates a refined DTM
-        preprocessed_dsm_path = os.path.join(output_dir, 'preprocessed_DSM.tif')
-        os.remove(raw_dtm_path)
-        os.remove(preprocessed_dsm_path)
-        
-    # global stop_thread
-    # stop_thread = True
-    # x.join()
-
 def get_parser():
     """
     Argument parser for Bulldozer (CLI).
 
     Returns:
         the parser.
     """
@@ -220,14 +190,16 @@
 
     parser.add_argument(
         "--version",
         "-v",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
     )
+    
+    #TODO add all the parameters
     return parser
 
 
 def bulldozer_cli() -> None:
     """
         Call bulldozer main pipeline.
     """
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/postprocessing/dtm_postprocess.py` & `bulldozer-dtm-1.0.1/src/bulldozer/postprocessing/dtm_postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,16 @@
                                 dst_nodata=full_mask_dataset.nodata,
                             )
                         
                         os.rename(src=decimated_quality_mask_path, 
                                 dst=quality_mask_path)
 
                 return decimated_dsm_path
+            else:
+                return dsm_path
         else:
             return dsm_path
 
 @Runtime
 def postprocess_pipeline(raw_dtm_path : str, 
                          output_dir : str,
                          nb_max_workers : int = 1,
@@ -372,18 +374,19 @@
         output_CRS: if a CRS (different from the input DSM) is provided, reproject the DTM to the new CRS.
     """
     BulldozerLogger.log("Starting postprocess", logging.DEBUG)
 
     # We need to retrieve the resolution factor from the dtm
     # in the case the user gives an output resolution greater than the full
     # resolution
-    dsm_path: str = adaptToTargetResolution(raw_dtm_path = raw_dtm_path,
-                                            dsm_path = dsm_path,
-                                            output_dir = output_dir,
-                                            quality_mask_path = quality_mask_path)
+    if dsm_path is not None:
+        dsm_path: str = adaptToTargetResolution(raw_dtm_path = raw_dtm_path,
+                                                dsm_path = dsm_path,
+                                                output_dir = output_dir,
+                                                quality_mask_path = quality_mask_path)
 
 
     # Fill DTM nodata for future pits detection
     # To apply uniform filter you need to fill nodata value of the raw dtm
     # then detect pits on the filled dtm and use raw dtm to put back nodata value
     filled_dtm_path : str = os.path.join(output_dir, "filled_dtm.tif")
     buildIntermediateFilledDtm(dtm_path = raw_dtm_path,
@@ -406,24 +409,30 @@
         # check the interstion after the filling
         checkIntersection(dtm_path = filled_dtm_path,
                         dsm_path = dsm_path, 
                         out_dtm_path = dtm_path, 
                         nb_max_workers = nb_max_workers,
                         nodata = nodata)
 
+    os.remove(filled_dtm_path)
+
     with rasterio.open(dtm_path, 'r') as dtm_dataset:
         # Updates the quality mask if it's provided
         if quality_mask_path:
             # Add a new band for the pits mask
+            concat_mask = np.zeros((2, dtm_dataset.height, dtm_dataset.width), dtype=np.uint8)
+            concat_profile = None
             with rasterio.open(quality_mask_path, 'r') as q_mask_dataset:
                 with rasterio.open(pits_mask_path, "r") as pits_mask_dataset:
-                    pits_mask = pits_mask_dataset.read(indexes=1)
-                    q_mask_profile = q_mask_dataset.profile
-                    q_mask_profile['count'] = q_mask_profile['count'] + 1
-                    write_dataset(quality_mask_path, pits_mask, q_mask_profile, band=q_mask_profile['count'])
+                    concat_mask[1,:,:] = pits_mask_dataset.read(indexes=1)
+                    concat_mask[0,:,:] = q_mask_dataset.read(indexes=1)
+                    concat_profile = q_mask_dataset.profile
                     os.remove(pits_mask_path)
+            concat_profile['count'] = 2
+            with rasterio.open(quality_mask_path, 'w', **concat_profile) as q_mask_dataset:
+                q_mask_dataset.write(concat_mask)
         else:
             BulldozerLogger.log("No quality mask provided", logging.WARNING)
         # Generates the DHM (DSM - DTM) if the option is activated
         if generate_dhm and dsm_path:
             dhm_path = os.path.join(output_dir, "DHM.tif")
             build_dhm(dsm_path, dtm_path, dhm_path, nb_max_workers, nodata)
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/bordernodata.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/bordernodata.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/bulldozer/preprocessing/bordernodata/c_bordernodata.cpp",
             "src/bulldozer/preprocessing/bordernodata/c_bordernodata.h"
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -94,18 +94,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -219,15 +223,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -258,15 +262,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -395,17 +399,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -475,14 +476,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1721,14 +1727,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -10252,15 +10275,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -15976,15 +15999,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_9bulldozer_12bordernodata_PyBorderNodata(PyObject *o) {
   struct __pyx_obj_9bulldozer_12bordernodata_PyBorderNodata *p = (struct __pyx_obj_9bulldozer_12bordernodata_PyBorderNodata *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->border_nodata);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -16058,15 +16081,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -16087,15 +16110,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -16250,15 +16273,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -16272,15 +16295,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -16372,15 +16395,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -16403,15 +16426,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16636,15 +16659,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -16656,15 +16679,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16785,15 +16808,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -17244,14 +17267,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -18763,28 +18791,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21104,15 +21132,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21338,15 +21366,15 @@
                         } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
                             return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21534,15 +21562,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21730,15 +21758,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21964,15 +21992,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/bordernodata.pyx` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/bordernodata.pyx`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/c_bordernodata.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/c_bordernodata.cpp`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/bordernodata/c_bordernodata.h` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/bordernodata/c_bordernodata.h`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,27 @@
                                                 unsigned char * disturbance_mask,
                                                 unsigned int nb_rows,
                                                 unsigned int nb_cols,
                                                 float thresh,
                                                 float nodata_value) {
 
         if(m_IsFourConnexity) {
-            for(unsigned int r = 1; r < nb_rows -2; r++) {
-                for(unsigned int c = 1; c < nb_cols -2; c++) {
+            for(unsigned int r = 1; r < nb_rows - 1; r++) {
+                for(unsigned int c = 1; c < nb_cols - 1; c++) {
                     const unsigned int coords = r * nb_cols + c;
                     if(dsm[coords] != nodata_value){
                         disturbance_mask[coords] = isVerticalDisturbed(dsm, coords, nb_cols, thresh, nodata_value) 
                                                     && isHorizontalDisturbed(dsm, coords, thresh, nodata_value);
                     }
                 }
             }
         }
         else {
-            for(unsigned int r = 1; r < nb_rows -2; r++) {
-                for(unsigned int c = 1; c < nb_cols -2; c++) {
+            for(unsigned int r = 1; r < nb_rows - 1; r++) {
+                for(unsigned int c = 1; c < nb_cols - 1; c++) {
                     const unsigned int coords = r * nb_cols + c;
                     if(dsm[coords] != nodata_value){
                         disturbance_mask[coords] = isVerticalDisturbed(dsm, coords, nb_cols, thresh, nodata_value) && 
                                                 isHorizontalDisturbed(dsm, coords, thresh, nodata_value) &&
                                                 isDiag1Disturbed(dsm, coords, nb_cols, thresh, nodata_value) &&
                                                 isDiag2Disturbed(dsm, coords, nb_cols, thresh, nodata_value);
                     }
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.h` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.h`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/disturbedareas.cpp` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/disturbedareas.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.cpp",
             "src/bulldozer/preprocessing/disturbedareas/c_disturbedareas.h"
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -94,18 +94,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -219,15 +223,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -258,15 +262,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -395,17 +399,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -475,14 +476,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1718,14 +1724,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -10311,15 +10334,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -16035,15 +16058,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_9bulldozer_14disturbedareas_PyDisturbedAreas(PyObject *o) {
   struct __pyx_obj_9bulldozer_14disturbedareas_PyDisturbedAreas *p = (struct __pyx_obj_9bulldozer_14disturbedareas_PyDisturbedAreas *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->disturbed_areas);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -16117,15 +16140,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -16146,15 +16169,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -16309,15 +16332,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -16331,15 +16354,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -16431,15 +16454,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -16462,15 +16485,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16695,15 +16718,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -16715,15 +16738,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16844,15 +16867,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -17305,14 +17328,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -18784,28 +18812,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21125,15 +21153,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21359,15 +21387,15 @@
                         } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
                             return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21555,15 +21583,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21751,15 +21779,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21985,15 +22013,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/disturbedareas/disturbedareas.pyx` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/disturbedareas/disturbedareas.pyx`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/preprocessing/dsm_preprocess.py` & `bulldozer-dtm-1.0.1/src/bulldozer/preprocessing/dsm_preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 # limitations under the License.
 
 """
     This module is used to preprocess the DSM in order to improve the DTM computation.
 """
 
 import rasterio
+from rasterio.fill import fillnodata
 import os
 import numpy as np
 import logging
 import bulldozer.bordernodata as bn
 import bulldozer.disturbedareas as da
 from bulldozer.utils.helper import write_dataset
 from bulldozer.utils.logging_helper import BulldozerLogger
 from bulldozer.scale.tools import scaleRun
 from bulldozer.scale.Shared import Shared
-from bulldozer.utils.helper import Runtime, retrieve_nodata
+from bulldozer.utils.helper import Runtime, retrieve_nodata, DefaultValues
 
-# No data value constant used in bulldozer
-NO_DATA_VALUE = -32768
+
+def generate_identical_profile(input_profile: rasterio.DatasetReader.profile) -> dict:
+    return input_profile
 
 def generate_output_profile_for_mask(input_profile: rasterio.DatasetReader.profile) -> dict:
     output_profile = input_profile
     output_profile['dtype'] = np.ubyte
     return output_profile
 
 def border_nodata_computer( inputBuffers: list,
@@ -55,16 +57,16 @@
     Returns:
         mask flagging the border nodata areas
     """
     dsm = inputBuffers[0]
     nodata = params['nodata']
 
     if np.isnan(nodata):
-        dsm = np.nan_to_num(dsm, False, nan=NO_DATA_VALUE)
-        nodata = NO_DATA_VALUE
+        dsm = np.nan_to_num(dsm, False, nan=DefaultValues['NODATA'])
+        nodata = DefaultValues['NODATA']
     
     # We're using our C++ implementation to perform this computation
     border_nodata = bn.PyBorderNodata()
 
     if params["doTranspose"]:
         return border_nodata.build_border_nodata_mask(dsm, nodata).astype(np.ubyte)
     else:
@@ -142,16 +144,16 @@
         Returns:
             mask flagging the disturbed areas. 
     """
 
     nodata = params["nodata"]
 
     if np.isnan(nodata):
-        dsm = np.nan_to_num(dsm, False, nan=NO_DATA_VALUE)
-        nodata = NO_DATA_VALUE
+        dsm = np.nan_to_num(dsm, False, nan=DefaultValues['NODATA'])
+        nodata = DefaultValues['NODATA']
 
     disturbed_areas = da.PyDisturbedAreas(params["is_four_connexity"])
     disturbance_mask = disturbed_areas.build_disturbance_mask(inputBuffers[0], 
                                                               params["slope_threshold"],
                                                               params["nodata"]).astype(np.ubyte)
     return disturbance_mask
 
@@ -174,14 +176,15 @@
 
     Returns:
         masks containing the disturbed areas.
     """
     if nodata is None:
         nodata = retrieve_nodata(dsm_path)
 
+    #TODO assert not none c++ param raise Value Error (missing value for parameters)
     disturbanceParams = {
         "is_four_connexity": is_four_connexity,
         "slope_threshold": slope_threshold,
         "nodata": nodata,
         "desc": "Build Disturbance Mask"
     }
 
@@ -191,14 +194,38 @@
                                 algoParams = disturbanceParams, 
                                 generateOutputProfileComputer = generate_output_profile_for_mask, 
                                 nbWorkers = nb_max_workers,
                                 stableMargin = 1,
                                 inMemory=True)
     return disturbance_mask != 0
     
+def fillNoDataComputer(inputBuffers: list,
+                       params: dict) -> np.ndarray:
+    
+    return fillnodata(inputBuffers[0], mask=inputBuffers[1], max_search_distance=100.0, smoothing_iterations=0)
+
+
+def multiProcsFillNoData(inputImagePaths: list,
+                         outputPath: str,
+                         nb_max_workers: int = 1) -> None:
+    
+    fillNoDataParams = {
+        "desc": "Filling DSM nodata..."
+    }
+
+    filledDSM = scaleRun(inputImagePaths = inputImagePaths, 
+                         outputImagePath = outputPath, 
+                         algoComputer = fillNoDataComputer, 
+                         algoParams = fillNoDataParams, 
+                         generateOutputProfileComputer = generate_identical_profile, 
+                         nbWorkers = nb_max_workers, 
+                         stableMargin = 100,
+                         inMemory=False)
+
+    
 def write_quality_mask(border_nodata_mask: np.ndarray,
                        inner_nodata_mask : np.ndarray, 
                        disturbed_area_mask : np.ndarray,
                        quality_mask_path: str,
                        profile : rasterio.profiles.Profile) -> None:
     """
     This method merges the nodata masks generated during the DSM preprocessing into a single quality mask.
@@ -207,29 +234,25 @@
 
     Args:
         inner_nodata_mask: nodata areas in the input DSM.
         disturbed_area_mask: areas flagged as nodata due to their aspect (mainly correlation issue).
         output_dir: bulldozer output directory. The quality mask will be written in this folder.
         profile: DSM profile (TIF metadata).
     """     
-    quality_mask = np.zeros(np.shape(inner_nodata_mask), dtype=np.uint8)
-
-    maskProfile = profile.copy()
+    quality_mask_profile = profile.copy()
 
     # Metadata update
-    maskProfile['dtype'] = np.uint8
-    maskProfile['count'] = 1
+    quality_mask_profile['dtype'] = np.uint8
+    quality_mask_profile['count'] = 3
     # We don't except nodata value in this mask
-    maskProfile['nodata'] = None
-    quality_mask[disturbed_area_mask] = 2
-    quality_mask[inner_nodata_mask] = 1
-    quality_mask[border_nodata_mask] = 3
-    write_dataset(quality_mask_path, quality_mask, maskProfile)
-
-
+    quality_mask_profile['nodata'] = None
+    buffer = np.stack([inner_nodata_mask, disturbed_area_mask, border_nodata_mask], axis=0)
+    with rasterio.open(quality_mask_path, 'w', nbits=1, **quality_mask_profile) as dst_dataset:
+        dst_dataset.write(buffer)
+        dst_dataset.close()
 
 def preprocess_pipeline(dsm_path : str, 
                         output_dir : str,
                         nb_max_workers : int = 1,
                         nodata : float = None,
                         slope_threshold : float = 2.0, 
                         is_four_connexity : bool = True,
@@ -247,64 +270,77 @@
         slope_treshold: if the slope is greater than this threshold then we consider it as disturbed variation.
         is_four_connexity: number of evaluated axis. 
                         Vertical and horizontal if true else vertical, horizontal and diagonals.
         minValidHeight: DSM minimum valid elevation. All the points lower this threshold will be consider as nodata.             
     """ 
 
     BulldozerLogger.log("Starting preprocess", logging.DEBUG)
+    outputFilledDsmPath = os.path.join(output_dir, 'preprocessed_DSM.tif')
 
     # The value is already retrieved before calling the preprocess method
     # If it is none, it is set automatically to -32768
     if nodata is None:
-        BulldozerLogger.log("No data value is set to " + str(NO_DATA_VALUE), logging.INFO)
-        nodata = NO_DATA_VALUE
+        nodata = retrieve_nodata(dsm_path)
 
     with rasterio.open(dsm_path) as dsm_dataset:
         preprocessedDsmProfile = dsm_dataset.profile
         preprocessedDsmProfile['nodata'] = nodata
         
 
     # Read the buffer in shared memory
     with Shared.make_shared_from_rasterio(dsm_path) as shared_dsm:
         dsm = shared_dsm.getArray()
         dsm_memory_path = shared_dsm.get_memory_path()
         
+        # Get the maximum height value
+        maxValidHeight: float = np.amax(dsm)
         
         # handle the case where there are dynamic nodata values (MicMac DSM for example)
-        if minValidHeight:
+        if minValidHeight is not None:
             BulldozerLogger.log("Min valid height set by the user" + str(minValidHeight), logging.INFO)
             dsm[:] = np.where( dsm < minValidHeight, nodata, dsm)[:]
+        else:
+            BulldozerLogger.log("Min valid height is not set by the user, this may be dangerous if there are aberrant low height values !", logging.DEBUG)
 
         # Retrieves the disturbed area mask (mainly correlation issues: occlusion, water, etc.)
         BulldozerLogger.log("Compute disturbance mask", logging.DEBUG)
         disturbed_area_mask = build_disturbance_mask(dsm_memory_path, nb_max_workers, slope_threshold, is_four_connexity, nodata)
         BulldozerLogger.log("disturbance mask: Done", logging.INFO)
 
 
         with Shared.make_shared_from_numpy(disturbed_area_mask) as shared_disturbed_area_mask:
+
+            # Can be unset since it became a shared resource
             disturbed_area_mask = None
             
             # Generates inner nodata mask
             BulldozerLogger.log("Starting inner_nodata_mask and border_nodata_mask building", logging.DEBUG)
             border_nodata_mask = build_border_nodata_mask(dsm_memory_path, nb_max_workers, nodata)
             inner_nodata_mask = np.logical_and(np.logical_not(border_nodata_mask), dsm == nodata)
             BulldozerLogger.log("inner_nodata_mask and border_nodata_mask generation: Done", logging.INFO)
         
+            # Replace border nodata by maximum valid height
+            dsm[border_nodata_mask] = maxValidHeight
+
             # Merges and writes the quality mask
             quality_mask_path = os.path.join(output_dir, "quality_mask.tif")
             write_quality_mask(border_nodata_mask, inner_nodata_mask, shared_disturbed_area_mask.getArray(), quality_mask_path, preprocessedDsmProfile)
+
+            # Merge inner nodata and disturbed areas into a mask indicating all the pixels to interpolate by idw
+            pixelsToInterpolate = np.invert(np.logical_or(inner_nodata_mask, shared_disturbed_area_mask.getArray()))
             
             border_nodata_mask = None
             inner_nodata_mask = None
             
-            dsm[shared_disturbed_area_mask.getArray()] = nodata
+            with Shared.make_shared_from_numpy(pixelsToInterpolate) as shared_pixels_to_interpolate_mask:
     
+                pixelsToInterpolate = None
 
-        # Creates the preprocessed DSM. This DSM is only intended for bulldozer DTM extraction function.
-        BulldozerLogger.log("Write preprocessed dsm", logging.DEBUG)
-        preprocessed_dsm_path = os.path.join(output_dir, 'preprocessed_DSM.tif')
+                pixels_to_interpolate_mem_path = shared_pixels_to_interpolate_mask.get_memory_path()
 
-        write_dataset(preprocessed_dsm_path, dsm, preprocessedDsmProfile)
+                multiProcsFillNoData( inputImagePaths= [dsm_memory_path, pixels_to_interpolate_mem_path], 
+                                      outputPath = outputFilledDsmPath,
+                                      nb_max_workers= nb_max_workers)
 
+    # The input dsm for dtm extraction must be filled !
     BulldozerLogger.log("Preprocess done", logging.INFO)
-
-    return preprocessed_dsm_path, quality_mask_path
+    return outputFilledDsmPath, quality_mask_path
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/scale/tools.py` & `bulldozer-dtm-1.0.1/src/bulldozer/scale/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 from typing import Callable
 import numpy as np
 import rasterio
 import concurrent.futures
 from tqdm import tqdm
-from bulldozer.scale.Shared import Shared
+from bulldozer.scale.Shared import Shared, dictToRasterioProfile, getNumpyArrayShapeFromProfile
 
 Tile = namedtuple('Tile', ["startX", "startY", "endX", "endY", "topM", "rightM", "bottomM", "leftM"])
 
 def computeTiles(rasterHeight: float,
                  rasterWidth: float,
                  stableMargin: int,
                  nbProcs: int):
@@ -148,28 +148,31 @@
         Memory aware multiprocessing execution
     """
 
         
     if Shared.is_shared_memory_path(inputImagePaths[0]) :
         sh = Shared()
         sh.open(inputImagePaths[0])
-        shape = sh.metadata['shape']
-        dtype = sh.metadata['dtype']
-        if 'profile' in sh.metadata :
-            inputProfile = sh.metadata['profile']
+        inputProfile = sh.metadata['profile']
+        shape = getNumpyArrayShapeFromProfile(inputProfile)
+        dtype = inputProfile['dtype']
+        inputProfile = dictToRasterioProfile(inputProfile)
     
     else : 
         with rasterio.open(inputImagePaths[0], "r") as inputImgDataset:
             shape = (inputImgDataset.height, inputImgDataset.width)
+            if inputImgDataset.count > 1:
+                shape = (inputImgDataset.count, inputImgDataset.height, inputImgDataset.width)
             dtype = inputImgDataset.dtypes[0]
             inputProfile = inputImgDataset.profile.copy()
+    
 
     # Generate the tiles
-    tiles = computeTiles(rasterHeight = shape[0],
-                        rasterWidth = shape[1],
+    tiles = computeTiles(rasterHeight = inputProfile['height'],
+                        rasterWidth = inputProfile['width'],
                         stableMargin = stableMargin,
                         nbProcs = nbWorkers)
 
 
     if inMemory:
         wholeOutputArray = np.zeros(shape, dtype=dtype)
         with concurrent.futures.ProcessPoolExecutor(max_workers = nbWorkers) as executor:
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/utils/config_parser.py` & `bulldozer-dtm-1.0.1/src/bulldozer/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/utils/helper.py` & `bulldozer-dtm-1.0.1/src/bulldozer/utils/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,26 +17,45 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
     This module groups different generic methods used in Bulldozer.
 """
-import platform
-import psutil
 import time
 import os
-import getpass
 import rasterio
 import logging
 import numpy as np
 from git import Repo
 from rasterio import Affine
 from bulldozer.utils.logging_helper import BulldozerLogger
 
+# This dict store all the Bulldozer default parameters
+DefaultValues = {
+    # Basic parameters
+    'GENERATE_DHM' : True,
+    'MAX_OBJECT_WIDTH' : 16,
+    # Advanced settings
+    'OUTPUT_RESOLUTION' : None,
+    'NODATA' : -32768.0,
+    'MIN_VALID_HEIGHT' : None,
+    'NB_MAX_WORKERS' : None,
+    'CHECK_INTERSECTION' : False,
+    'DEVELOPPER_MODE' : False,
+    # Bulldozer core settings
+    'FOUR_CONNEXITY' : True,
+    'UNIFORM_FILTER_SIZE': 1,
+    'PREVENT_UNHOOK_ITER' : 10,
+    'NUM_OUTER_ITER' : 50,
+    'NUM_INNER_ITER' : 10,
+    'MP_TILE_SIZE' : 1500,
+    'SLOPE_THRESHOLD' : 2,
+    'KEEP_INTER_DTM' : False
+}
 
 def write_dataset(buffer_path : str, 
                   buffer : np.ndarray, 
                   profile : rasterio.profiles.Profile,
                   window : rasterio.windows.Window = None,
                   band : int = 1) -> None:
     """
@@ -84,18 +103,20 @@
     """
     if cfg_nodata is not None :
         return float(cfg_nodata)
     
     # If nodata is not specified in the config file, retrieve the value from the DSM metadata
     with rasterio.open(dsm_path) as dsm_dataset:
         nodata = dsm_dataset.nodata
-        return nodata
+        if nodata is not None :
+            return nodata
     
-    # By default, if no value is set for nodata, return None
-    return None
+    BulldozerLogger.log("No data value is set to " + str(DefaultValues.NODATA.value), logging.INFO)
+    # By default, if no value is set for nodata, return -32768.0
+    return DefaultValues.NODATA.value
 
 def downsample_profile(profile, factor : float) :
     
     transform= profile['transform']
 
     newprofile = profile.copy()
     dst_transform = Affine.translation(transform[2], transform[5]) * Affine.scale(transform[0]*factor, transform[4]*factor)
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer/utils/logging_helper.py` & `bulldozer-dtm-1.0.1/src/bulldozer/utils/logging_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # limitations under the License.
 
 """
 This module aims to centralize the use of the logger in Bullodzer.
 """
 import sys
 import os
+import getpass
+import platform
+import psutil
+import multiprocessing
 import logging
 import logging.config
 from git import Repo
 from git.exc import InvalidGitRepositoryError
 
 class BulldozerLogger:
     """
@@ -112,27 +116,34 @@
                 info['commit_sha'] = repo.head.object.hexsha
                 info['branch'] = repo.active_branch
             except InvalidGitRepositoryError as e:
                 info['commit_sha'] = "No git repo found ({})".format(e)
                 info['branch'] = "No git repo found ({})".format(e)
                 
             # Node info
-            info['user']=getpass.getuser()
-            info['node']=platform.node()
-            info['processor']=platform.processor()
-            info['ram']=str(round(psutil.virtual_memory().total / (1024 **3)))+" GB"
-
+            try:
+                info['user'] = getpass.getuser()
+            except:
+                info['user'] = 'unknown'
+            try:
+                info['node'] = platform.node()
+            except:
+                info['node'] = 'unknown'
+            info['processor'] = platform.processor()
+            info['cpu_count'] = multiprocessing.cpu_count()
+            info['ram'] = str(round(psutil.virtual_memory().total / (1024 **3)))+" GB"
+            
             # OS info
-            info['system']=platform.system()
-            info['release']=platform.release()
-            info['os_version']=platform.version()
+            info['system'] = platform.system()
+            info['release'] = platform.release()
+            info['os_version'] = platform.version()
             
             # Message format
             init = ("\n"+"#"*17+"\n#   BULLDOZER   #\n"+"#"*17+"\n# <Git info>\n#\t- branch: {}\n#\t- commit SHA: {}"
-                    "\n#\n# <Node info>\n#\t - user: {}\n#\t - node: {}\n#\t - processor: {}\n#\t - RAM: {}"
+                    "\n#\n# <Node info>\n#\t - user: {}\n#\t - node: {}\n#\t - processor: {}\n#\t - CPU count: {}\n#\t - RAM: {}"
                     "\n#\n# <OS info>\n#\t - system: {}\n#\t - release: {}\n#\t - version: {}\n"
                     +"#"*17).format(info['branch'], info['commit_sha'], info['user'], info['node'], 
-                                    info['processor'], info['ram'], info['system'], info['release'], info['os_version'])
+                                    info['processor'], info['cpu_count'], info['ram'], info['system'], info['release'], info['os_version'])
             BulldozerLogger.log(init, logging.DEBUG)
 
         except Exception as e:
             BulldozerLogger.log("Error occured during logger init: \n" + str(e), logging.DEBUG)
```

### Comparing `bulldozer-dtm-1.0.0/src/bulldozer_dtm.egg-info/PKG-INFO` & `bulldozer-dtm-1.0.1/src/bulldozer_dtm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulldozer-dtm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bulldozer is a DTM extraction tool requiring only a DSM as input
 Home-page: https://github.com/CNES/bulldozer
 Author: CNES
 Author-email: pierre.lassalle@cnes.fr,dimitri.lallement@cnes.fr,yannick.ott@thalesgroup.com
 License: Apache V2.0
 Keywords: bulldozer,DTM,DSM,3D,Photogrammetry,Remote Sensing,LiDar,CARS
 Classifier: Development Status :: 4 - Beta
@@ -19,23 +19,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-    <img src="docs/source/images/bulldozer_logo.png" width=256
-    >
+    <img src="https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/bulldozer_logo.png" width=256>
 
 **Bulldozer, a DTM extraction tool requiring only a DSM as input.**
 
 [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)](CONTRIBUTING.md)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer/)
+[![PyPI Version](https://img.shields.io/pypi/v/bulldozer-dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-dtm/)
 
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#installation">Installation</a> •  
   <a href="#quick-start">Quick Start</a> •
   <a href="#documentation">Documentation</a> •
@@ -47,15 +46,15 @@
 </div>
 
 ---
 
 ## Key features
 
 <div align="center">
-<img src="docs/source/images/result_overview.gif" alt="drawing" width="400"/>
+<img src="docs/source/images/result_overview.gif" alt="demo" width="400"/>
 </div>
 
 **Bulldozer** is designed as a pipeline of standalone functions that aims to extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).  
 But you can also use one of the following function without running the full pipeline:
 * **DSM preprocessing**
     * **Nodata extraction:** a group of methods to differentiate and extract nodata related to failed correlations during the DSM computation and those of the image border
     * **Disturbed areas detection:** a method to locate disturbed areas. These noisy areas are mainly related to areas in which the correlator has incorrectly estimated the elevation (water or shadow areas).
@@ -94,17 +93,17 @@
 pip install .
 ```
 ## Quick Start
 
 1. First you have to create a configuration file or edit the `configuration_template.yaml` available in the `conf` directory. You have to update at least the following parameters:
 ```yaml
 # Input DSM path (expected format: "<folder_1>/<folder_2>/<file>.<[tif/tiff]>")
-dsmPath : "<input_dsm.tif>"
+dsm_path : "<input_dsm.tif>"
 # Output directory path (if the directory doesn't exist, create it)
-outputDir : "<output_dir>"
+output_dir : "<output_dir>"
 ```
 2. Run the pipeline:
    * Through CLI *(Command Line Interface)*
    ```console
    bulldozer --conf conf/configuration_template.yaml
    ```
    * Through Python API using the config file
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: bulldozer-dtm Version: 1.0.0 Summary: Bulldozer is
+Metadata-Version: 2.1 Name: bulldozer-dtm Version: 1.0.1 Summary: Bulldozer is
 a DTM extraction tool requiring only a DSM as input Home-page: https://
 github.com/CNES/bulldozer Author: CNES Author-email:
 pierre.lassalle@cnes.fr,dimitri.lallement@cnes.fr,yannick.ott@thalesgroup.com
 License: Apache V2.0 Keywords: bulldozer,DTM,DSM,3D,Photogrammetry,Remote
 Sensing,LiDar,CARS Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE
-  [docs/source/images/bulldozer_logo.png] **Bulldozer, a DTM extraction tool
-   requiring only a DSM as input.** [![Python](https://img.shields.io/badge/
-python-v3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
- [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-
-orange.svg)](CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
+ [https://raw.githubusercontent.com/CNES/bulldozer/master/docs/source/images/
+bulldozer_logo.png] **Bulldozer, a DTM extraction tool requiring only a DSM as
+input.** [![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https:
+   //www.python.org/downloads/release/python-380/) [![Contributions welcome]
+       (https://img.shields.io/badge/contributions-welcome-orange.svg)]
+      (CONTRIBUTING.md) [![License](https://img.shields.io/badge/License-
   Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![PyPI
-                    Version](https://img.shields.io/pypi/v/
-  bulldozer?color=%2334D058&label=pypi%20package)](https://pypi.org/project/
-                                  bulldozer/)
+               Version](https://img.shields.io/pypi/v/bulldozer-
+dtm?color=%2334D058&label=pypi%20package)](https://pypi.org/project/bulldozer-
+                                     dtm/)
 Key_Features â¢ Installation â¢ Quick_Start â¢ Documentation â¢ Contribute
                            â¢ Licence â¢ Reference
 --- ## Key features
-                                   [drawing]
+                                    [demo]
 **Bulldozer** is designed as a pipeline of standalone functions that aims to
 extract a *Digital Terrain Model* (DTM) from a *Digital Surface Model* (DSM).
 But you can also use one of the following function without running the full
 pipeline: * **DSM preprocessing** * **Nodata extraction:** a group of methods
 to differentiate and extract nodata related to failed correlations during the
 DSM computation and those of the image border * **Disturbed areas detection:**
 a method to locate disturbed areas. These noisy areas are mainly related to
@@ -46,17 +47,17 @@
 docs.conda.io/en/latest/) or [virtualenv](https://virtualenv.pypa.io/en/latest/
 ). * Installation with `virtualenv`: ```sh # Clone the project git clone https:
 //github.com/CNES/bulldozer.git cd bulldozer/ # Create the environment python -
 m venv bulldozer_venv source bulldozer_venv/bin/activate # Install the library
 pip install . ``` ## Quick Start 1. First you have to create a configuration
 file or edit the `configuration_template.yaml` available in the `conf`
 directory. You have to update at least the following parameters: ```yaml #
-Input DSM path (expected format: "//.<[tif/tiff]>") dsmPath : "
+Input DSM path (expected format: "//.<[tif/tiff]>") dsm_path : "
 tif>" # Output directory path (if the directory doesn't exist, create it)
-outputDir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
+output_dir : "" ``` 2. Run the pipeline: * Through CLI *(Command Line
 Interface)* ```console bulldozer --conf conf/configuration_template.yaml ``` *
 Through Python API using the config file ```python from
 bulldozer.pipeline.bulldozer_pipeline import dsm_to_dtm dsm_to_dtm
 (config_path="conf/configuration_template.yaml") ``` * Through Python API
 providing directly the input parameters (missing parameters will be replaced by
 default values) ```python from bulldozer.pipeline.bulldozer_pipeline import
 dsm_to_dtm # Example with a specific number of workers dsm_to_dtm(dsm_path="
```

