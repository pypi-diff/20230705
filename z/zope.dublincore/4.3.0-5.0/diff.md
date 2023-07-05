# Comparing `tmp/zope.dublincore-4.3.0.tar.gz` & `tmp/zope.dublincore-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zope.dublincore-4.3.0.tar", last modified: Wed Oct 14 06:10:21 2020, max compression
+gzip compressed data, was "zope.dublincore-5.0.tar", last modified: Wed Jul  5 07:16:14 2023, max compression
```

## Comparing `zope.dublincore-4.3.0.tar` & `zope.dublincore-5.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/
--rw-r--r--   0 mac        (513) staff       (20)      139 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)      669 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/.travis.yml
--rw-r--r--   0 mac        (513) staff       (20)     4220 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      281 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     8902 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1606 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      104 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6794 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      670 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)     8594 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     9042 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)      213 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     6717 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)     9435 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/docs/narrative.rst
--rw-r--r--   0 mac        (513) staff       (20)      228 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      172 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3291 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope/dublincore/
--rw-r--r--   0 mac        (513) staff       (20)       61 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     4358 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/annotatableadapter.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/
--rw-r--r--   0 mac        (513) staff       (20)       61 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      776 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/box.pt
--rw-r--r--   0 mac        (513) staff       (20)      655 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1778 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/edit.pt
--rw-r--r--   0 mac        (513) staff       (20)     2079 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/metadataedit.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/tests/
--rw-r--r--   0 mac        (513) staff       (20)        0 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1385 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/browser/tests/test_metadataedit.py
--rw-r--r--   0 mac        (513) staff       (20)     2004 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1927 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/creatorannotator.py
--rw-r--r--   0 mac        (513) staff       (20)     3988 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/dcsv.py
--rw-r--r--   0 mac        (513) staff       (20)     6385 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/dcterms.py
--rw-r--r--   0 mac        (513) staff       (20)    14196 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     3242 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/property.py
--rw-r--r--   0 mac        (513) staff       (20)      484 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/security.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1121 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/
--rw-r--r--   0 mac        (513) staff       (20)       61 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     8568 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_annotatableadapter.py
--rw-r--r--   0 mac        (513) staff       (20)     4307 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_creatorannotator.py
--rw-r--r--   0 mac        (513) staff       (20)     7382 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_dcsv.py
--rw-r--r--   0 mac        (513) staff       (20)    12710 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_xmlmetadata.py
--rw-r--r--   0 mac        (513) staff       (20)     1339 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zcml.py
--rw-r--r--   0 mac        (513) staff       (20)     1647 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zdcannotatableadapter.py
--rw-r--r--   0 mac        (513) staff       (20)     7313 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zopedublincore.py
--rw-r--r--   0 mac        (513) staff       (20)     1847 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/timeannotators.py
--rw-r--r--   0 mac        (513) staff       (20)     7827 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/xmlmetadata.py
--rw-r--r--   0 mac        (513) staff       (20)    10682 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/src/zope/dublincore/zopedublincore.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     8902 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1686 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      365 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2020-10-14 06:10:21.000000 zope.dublincore-4.3.0/src/zope.dublincore.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1051 2020-10-14 06:10:20.000000 zope.dublincore-4.3.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.644406 zope.dublincore-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4372 2023-07-05 07:16:14.000000 zope.dublincore-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-05 07:16:14.000000 zope.dublincore-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-05 07:16:14.000000 zope.dublincore-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-05 07:16:14.000000 zope.dublincore-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      400 2023-07-05 07:16:14.000000 zope.dublincore-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7234 2023-07-05 07:16:14.644509 zope.dublincore-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1648 2023-07-05 07:16:14.000000 zope.dublincore-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      104 2023-07-05 07:16:14.000000 zope.dublincore-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.638645 zope.dublincore-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6794 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      670 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8594 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9042 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      213 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6717 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9435 2023-07-05 07:16:14.000000 zope.dublincore-5.0/docs/narrative.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      228 2023-07-05 07:16:14.000000 zope.dublincore-5.0/rtd.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-07-05 07:16:14.644804 zope.dublincore-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3322 2023-07-05 07:16:14.000000 zope.dublincore-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.635253 zope.dublincore-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.638815 zope.dublincore-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.642127 zope.dublincore-5.0/src/zope/dublincore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4208 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/annotatableadapter.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.642857 zope.dublincore-5.0/src/zope/dublincore/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      776 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/box.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      655 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1778 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/edit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2064 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/metadataedit.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.643114 zope.dublincore-5.0/src/zope/dublincore/browser/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1364 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/browser/tests/test_metadataedit.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2004 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1835 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/creatorannotator.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3887 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/dcsv.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6368 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/dcterms.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14236 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3234 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/property.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      484 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/security.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      903 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.644261 zope.dublincore-5.0/src/zope/dublincore/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8253 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_annotatableadapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4268 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_creatorannotator.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7415 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_dcsv.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12581 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_xmlmetadata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1371 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1571 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_zdcannotatableadapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7218 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/tests/test_zopedublincore.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1851 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/timeannotators.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7792 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/xmlmetadata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10402 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope/dublincore/zopedublincore.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 07:16:14.640051 zope.dublincore-5.0/src/zope.dublincore.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7234 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1678 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      374 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-05 07:16:14.000000 zope.dublincore-5.0/src/zope.dublincore.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1827 2023-07-05 07:16:14.000000 zope.dublincore-5.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zope.dublincore-4.3.0/CHANGES.rst` & `zope.dublincore-5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+5.0 (2023-07-05)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add back support for Python 3.5.
+
+- Add support for Python 3.10, 3.11.
+
+
 4.3.0 (2020-10-14)
 ------------------
 
 - Port ``.browser`` sub-package to Python 3.
 
 - Add support for Python 3.7, 3.8 and 3.9.
```

### Comparing `zope.dublincore-4.3.0/LICENSE.txt` & `zope.dublincore-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/README.rst` & `zope.dublincore-5.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 00000000: 6060 7a6f 7065 2e64 7562 6c69 6e63 6f72  ``zope.dublincor
 00000010: 6560 600a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e``.============
 00000020: 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 696d 6167  =======.... imag
-00000030: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
-00000040: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000050: 762f 7a6f 7065 2e64 7562 6c69 6e63 6f72  v/zope.dublincor
-00000060: 652e 7376 670a 2020 203a 7461 7267 6574  e.svg.   :target
-00000070: 3a20 6874 7470 733a 2f2f 7079 7069 2e70  : https://pypi.p
-00000080: 7974 686f 6e2e 6f72 672f 7079 7069 2f7a  ython.org/pypi/z
-00000090: 6f70 652e 6475 626c 696e 636f 7265 2f0a  ope.dublincore/.
-000000a0: 2020 203a 616c 743a 204c 6174 6573 7420     :alt: Latest 
-000000b0: 7265 6c65 6173 650a 0a2e 2e20 696d 6167  release.... imag
-000000c0: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
-000000d0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000000e0: 7079 7665 7273 696f 6e73 2f7a 6f70 652e  pyversions/zope.
-000000f0: 6475 626c 696e 636f 7265 2e73 7667 0a20  dublincore.svg. 
-00000100: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
-00000110: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000120: 6563 742f 7a6f 7065 2e64 7562 6c69 6e63  ect/zope.dublinc
-00000130: 6f72 652f 0a20 2020 3a61 6c74 3a20 5375  ore/.   :alt: Su
-00000140: 7070 6f72 7465 6420 5079 7468 6f6e 2076  pported Python v
-00000150: 6572 7369 6f6e 730a 0a2e 2e20 696d 6167  ersions.... imag
-00000160: 653a 3a20 6874 7470 733a 2f2f 7472 6176  e:: https://trav
-00000170: 6973 2d63 692e 6f72 672f 7a6f 7065 666f  is-ci.org/zopefo
-00000180: 756e 6461 7469 6f6e 2f7a 6f70 652e 6475  undation/zope.du
-00000190: 626c 696e 636f 7265 2e73 7667 3f62 7261  blincore.svg?bra
-000001a0: 6e63 683d 6d61 7374 6572 0a20 2020 3a74  nch=master.   :t
-000001b0: 6172 6765 743a 2068 7474 7073 3a2f 2f74  arget: https://t
-000001c0: 7261 7669 732d 6369 2e6f 7267 2f7a 6f70  ravis-ci.org/zop
-000001d0: 6566 6f75 6e64 6174 696f 6e2f 7a6f 7065  efoundation/zope
-000001e0: 2e64 7562 6c69 6e63 6f72 650a 0a2e 2e20  .dublincore.... 
-000001f0: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000200: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
-00000210: 7072 6f6a 6563 7473 2f7a 6f70 6564 7562  projects/zopedub
-00000220: 6c69 6e63 6f72 652f 6261 6467 652f 3f76  lincore/badge/?v
-00000230: 6572 7369 6f6e 3d6c 6174 6573 740a 2020  ersion=latest.  
-00000240: 203a 7461 7267 6574 3a20 6874 7470 3a2f   :target: http:/
-00000250: 2f7a 6f70 6564 7562 6c69 6e63 6f72 652e  /zopedublincore.
-00000260: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
-00000270: 656e 2f6c 6174 6573 742f 0a20 2020 3a61  en/latest/.   :a
-00000280: 6c74 3a20 446f 6375 6d65 6e74 6174 696f  lt: Documentatio
-00000290: 6e20 5374 6174 7573 0a0a 2e2e 2069 6d61  n Status.... ima
-000002a0: 6765 3a3a 2068 7474 7073 3a2f 2f63 6f76  ge:: https://cov
-000002b0: 6572 616c 6c73 2e69 6f2f 7265 706f 732f  eralls.io/repos/
-000002c0: 6769 7468 7562 2f7a 6f70 6566 6f75 6e64  github/zopefound
-000002d0: 6174 696f 6e2f 7a6f 7065 2e64 7562 6c69  ation/zope.dubli
-000002e0: 6e63 6f72 652f 6261 6467 652e 7376 673f  ncore/badge.svg?
-000002f0: 6272 616e 6368 3d6d 6173 7465 720a 2020  branch=master.  
-00000300: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000310: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
-00000320: 6974 6875 622f 7a6f 7065 666f 756e 6461  ithub/zopefounda
-00000330: 7469 6f6e 2f7a 6f70 652e 6475 626c 696e  tion/zope.dublin
-00000340: 636f 7265 3f62 7261 6e63 683d 6d61 7374  core?branch=mast
-00000350: 6572 0a20 2020 3a61 6c74 3a20 436f 6465  er.   :alt: Code
-00000360: 2043 6f76 6572 6167 650a 0a0a 5468 6973   Coverage...This
-00000370: 2070 6163 6b61 6765 2070 726f 7669 6465   package provide
-00000380: 7320 6120 4475 626c 696e 2043 6f72 6520  s a Dublin Core 
-00000390: 7375 7070 6f72 7420 666f 7220 5a6f 7065  support for Zope
-000003a0: 2d62 6173 6564 2077 6562 0a61 7070 6c69  -based web.appli
-000003b0: 6361 7469 6f6e 732e 2020 5468 6973 2069  cations.  This i
-000003c0: 6e63 6c75 6465 733a 0a0a 2a20 616e 2060  ncludes:..* an `
-000003d0: 6049 5a6f 7065 4475 626c 696e 436f 7265  `IZopeDublinCore
-000003e0: 6060 2069 6e74 6572 6661 6365 2064 6566  `` interface def
-000003f0: 696e 6974 696f 6e20 7468 6174 2063 616e  inition that can
-00000400: 2062 6520 696d 706c 656d 656e 7465 640a   be implemented.
-00000410: 2020 6279 206f 626a 6563 7473 2064 6972    by objects dir
-00000420: 6563 746c 7920 6f72 2076 6961 2061 6e20  ectly or via an 
-00000430: 6164 6170 7465 7220 746f 2073 7570 706f  adapter to suppo
-00000440: 7274 2044 7562 6c69 6e43 6f72 650a 2020  rt DublinCore.  
-00000450: 6d65 7461 6461 7461 2e0a 0a2a 2061 6e20  metadata...* an 
-00000460: 6060 495a 6f70 6544 7562 6c69 6e43 6f72  ``IZopeDublinCor
-00000470: 6560 6020 6164 6170 7465 7220 666f 7220  e`` adapter for 
-00000480: 616e 6e6f 7461 7461 626c 6520 6f62 6a65  annotatable obje
-00000490: 6374 7320 286f 626a 6563 7473 0a20 2070  cts (objects.  p
-000004a0: 726f 7669 6469 6e67 2060 6049 416e 6e6f  roviding ``IAnno
-000004b0: 7461 7461 626c 6560 6020 6672 6f6d 2060  tatable`` from `
-000004c0: 607a 6f70 652e 616e 6e6f 7461 7469 6f6e  `zope.annotation
-000004d0: 6060 292e 0a0a 2a20 6120 7061 7274 6961  ``)...* a partia
-000004e0: 6c20 6164 6170 7465 7220 666f 7220 6f62  l adapter for ob
-000004f0: 6a65 6374 7320 7468 6174 2061 6c72 6561  jects that alrea
-00000500: 6479 2069 6d70 6c65 6d65 6e74 2073 6f6d  dy implement som
-00000510: 6520 6f66 2074 6865 0a20 2060 6049 5a6f  e of the.  ``IZo
-00000520: 7065 4475 626c 696e 436f 7265 6060 2041  peDublinCore`` A
-00000530: 5049 2c0a 0a2a 2061 2022 4d65 7461 6461  PI,..* a "Metada
-00000540: 7461 2220 6272 6f77 7365 7220 7061 6765  ta" browser page
-00000550: 2028 7768 6963 6820 6279 2064 6566 6175   (which by defau
-00000560: 6c74 2061 7070 6561 7273 2069 6e20 7468  lt appears in th
-00000570: 6520 5a4d 4929 2c0a 0a2a 2073 7562 7363  e ZMI),..* subsc
-00000580: 7269 6265 7273 2074 6f20 7661 7269 6f75  ribers to variou
-00000590: 7320 6f62 6a65 6374 206c 6966 6563 7963  s object lifecyc
-000005a0: 6c65 2065 7665 6e74 7320 7468 6174 2061  le events that a
-000005b0: 7574 6f6d 6174 6963 616c 6c79 0a20 2073  utomatically.  s
-000005c0: 6574 2074 6865 2063 7265 6174 6564 2061  et the created a
-000005d0: 6e64 206d 6f64 6966 6965 6420 6461 7465  nd modified date
-000005e0: 2061 6e64 2073 6f6d 6520 6f74 6865 7220   and some other 
-000005f0: 6d65 7461 6461 7461 2e0a 0a43 6f6d 706c  metadata...Compl
-00000600: 6574 6520 646f 6375 6d65 6e74 6174 696f  ete documentatio
-00000610: 6e20 6973 2068 6f73 7465 6420 6174 2068  n is hosted at h
-00000620: 7474 7073 3a2f 2f7a 6f70 6564 7562 6c69  ttps://zopedubli
-00000630: 6e63 6f72 652e 7265 6164 7468 6564 6f63  ncore.readthedoc
-00000640: 732e 696f 2f0a                           s.io/.
+00000030: 653a 3a20 6874 7470 733a 2f2f 6769 7468  e:: https://gith
+00000040: 7562 2e63 6f6d 2f7a 6f70 6566 6f75 6e64  ub.com/zopefound
+00000050: 6174 696f 6e2f 7a6f 7065 2e64 7562 6c69  ation/zope.dubli
+00000060: 6e63 6f72 652f 6163 7469 6f6e 732f 776f  ncore/actions/wo
+00000070: 726b 666c 6f77 732f 7465 7374 732e 796d  rkflows/tests.ym
+00000080: 6c2f 6261 6467 652e 7376 670a 2020 203a  l/badge.svg.   :
+00000090: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
+000000a0: 6769 7468 7562 2e63 6f6d 2f7a 6f70 6566  github.com/zopef
+000000b0: 6f75 6e64 6174 696f 6e2f 7a6f 7065 2e64  oundation/zope.d
+000000c0: 7562 6c69 6e63 6f72 652f 6163 7469 6f6e  ublincore/action
+000000d0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+000000e0: 732e 796d 6c0a 0a2e 2e20 696d 6167 653a  s.yml.... image:
+000000f0: 3a20 6874 7470 733a 2f2f 7265 6164 7468  : https://readth
+00000100: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000110: 7473 2f7a 6f70 6564 7562 6c69 6e63 6f72  ts/zopedublincor
+00000120: 652f 6261 6467 652f 3f76 6572 7369 6f6e  e/badge/?version
+00000130: 3d6c 6174 6573 740a 2020 203a 7461 7267  =latest.   :targ
+00000140: 6574 3a20 6874 7470 3a2f 2f7a 6f70 6564  et: http://zoped
+00000150: 7562 6c69 6e63 6f72 652e 7265 6164 7468  ublincore.readth
+00000160: 6564 6f63 732e 6f72 672f 656e 2f6c 6174  edocs.org/en/lat
+00000170: 6573 742f 0a20 2020 3a61 6c74 3a20 446f  est/.   :alt: Do
+00000180: 6375 6d65 6e74 6174 696f 6e20 5374 6174  cumentation Stat
+00000190: 7573 0a0a 2e2e 2069 6d61 6765 3a3a 2068  us.... image:: h
+000001a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000001b0: 6473 2e69 6f2f 7079 7069 2f76 2f7a 6f70  ds.io/pypi/v/zop
+000001c0: 652e 6475 626c 696e 636f 7265 2e73 7667  e.dublincore.svg
+000001d0: 0a20 2020 3a74 6172 6765 743a 2068 7474  .   :target: htt
+000001e0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+000001f0: 2e6f 7267 2f70 7970 692f 7a6f 7065 2e64  .org/pypi/zope.d
+00000200: 7562 6c69 6e63 6f72 652f 0a20 2020 3a61  ublincore/.   :a
+00000210: 6c74 3a20 4c61 7465 7374 2072 656c 6561  lt: Latest relea
+00000220: 7365 0a0a 2e2e 2069 6d61 6765 3a3a 2068  se.... image:: h
+00000230: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000240: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+00000250: 7369 6f6e 732f 7a6f 7065 2e64 7562 6c69  sions/zope.dubli
+00000260: 6e63 6f72 652e 7376 670a 2020 203a 7461  ncore.svg.   :ta
+00000270: 7267 6574 3a20 6874 7470 733a 2f2f 7079  rget: https://py
+00000280: 7069 2e6f 7267 2f70 726f 6a65 6374 2f7a  pi.org/project/z
+00000290: 6f70 652e 6475 626c 696e 636f 7265 2f0a  ope.dublincore/.
+000002a0: 2020 203a 616c 743a 2053 7570 706f 7274     :alt: Support
+000002b0: 6564 2050 7974 686f 6e20 7665 7273 696f  ed Python versio
+000002c0: 6e73 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ns.... image:: h
+000002d0: 7474 7073 3a2f 2f63 6f76 6572 616c 6c73  ttps://coveralls
+000002e0: 2e69 6f2f 7265 706f 732f 6769 7468 7562  .io/repos/github
+000002f0: 2f7a 6f70 6566 6f75 6e64 6174 696f 6e2f  /zopefoundation/
+00000300: 7a6f 7065 2e64 7562 6c69 6e63 6f72 652f  zope.dublincore/
+00000310: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000320: 3d6d 6173 7465 720a 2020 203a 7461 7267  =master.   :targ
+00000330: 6574 3a20 6874 7470 733a 2f2f 636f 7665  et: https://cove
+00000340: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
+00000350: 7a6f 7065 666f 756e 6461 7469 6f6e 2f7a  zopefoundation/z
+00000360: 6f70 652e 6475 626c 696e 636f 7265 3f62  ope.dublincore?b
+00000370: 7261 6e63 683d 6d61 7374 6572 0a20 2020  ranch=master.   
+00000380: 3a61 6c74 3a20 436f 6465 2043 6f76 6572  :alt: Code Cover
+00000390: 6167 650a 0a0a 5468 6973 2070 6163 6b61  age...This packa
+000003a0: 6765 2070 726f 7669 6465 7320 6120 4475  ge provides a Du
+000003b0: 626c 696e 2043 6f72 6520 7375 7070 6f72  blin Core suppor
+000003c0: 7420 666f 7220 5a6f 7065 2d62 6173 6564  t for Zope-based
+000003d0: 2077 6562 0a61 7070 6c69 6361 7469 6f6e   web.application
+000003e0: 732e 2020 5468 6973 2069 6e63 6c75 6465  s.  This include
+000003f0: 733a 0a0a 2a20 616e 2060 6049 5a6f 7065  s:..* an ``IZope
+00000400: 4475 626c 696e 436f 7265 6060 2069 6e74  DublinCore`` int
+00000410: 6572 6661 6365 2064 6566 696e 6974 696f  erface definitio
+00000420: 6e20 7468 6174 2063 616e 2062 6520 696d  n that can be im
+00000430: 706c 656d 656e 7465 640a 2020 6279 206f  plemented.  by o
+00000440: 626a 6563 7473 2064 6972 6563 746c 7920  bjects directly 
+00000450: 6f72 2076 6961 2061 6e20 6164 6170 7465  or via an adapte
+00000460: 7220 746f 2073 7570 706f 7274 2044 7562  r to support Dub
+00000470: 6c69 6e43 6f72 650a 2020 6d65 7461 6461  linCore.  metada
+00000480: 7461 2e0a 0a2a 2061 6e20 6060 495a 6f70  ta...* an ``IZop
+00000490: 6544 7562 6c69 6e43 6f72 6560 6020 6164  eDublinCore`` ad
+000004a0: 6170 7465 7220 666f 7220 616e 6e6f 7461  apter for annota
+000004b0: 7461 626c 6520 6f62 6a65 6374 7320 286f  table objects (o
+000004c0: 626a 6563 7473 0a20 2070 726f 7669 6469  bjects.  providi
+000004d0: 6e67 2060 6049 416e 6e6f 7461 7461 626c  ng ``IAnnotatabl
+000004e0: 6560 6020 6672 6f6d 2060 607a 6f70 652e  e`` from ``zope.
+000004f0: 616e 6e6f 7461 7469 6f6e 6060 292e 0a0a  annotation``)...
+00000500: 2a20 6120 7061 7274 6961 6c20 6164 6170  * a partial adap
+00000510: 7465 7220 666f 7220 6f62 6a65 6374 7320  ter for objects 
+00000520: 7468 6174 2061 6c72 6561 6479 2069 6d70  that already imp
+00000530: 6c65 6d65 6e74 2073 6f6d 6520 6f66 2074  lement some of t
+00000540: 6865 0a20 2060 6049 5a6f 7065 4475 626c  he.  ``IZopeDubl
+00000550: 696e 436f 7265 6060 2041 5049 2c0a 0a2a  inCore`` API,..*
+00000560: 2061 2022 4d65 7461 6461 7461 2220 6272   a "Metadata" br
+00000570: 6f77 7365 7220 7061 6765 2028 7768 6963  owser page (whic
+00000580: 6820 6279 2064 6566 6175 6c74 2061 7070  h by default app
+00000590: 6561 7273 2069 6e20 7468 6520 5a4d 4929  ears in the ZMI)
+000005a0: 2c0a 0a2a 2073 7562 7363 7269 6265 7273  ,..* subscribers
+000005b0: 2074 6f20 7661 7269 6f75 7320 6f62 6a65   to various obje
+000005c0: 6374 206c 6966 6563 7963 6c65 2065 7665  ct lifecycle eve
+000005d0: 6e74 7320 7468 6174 2061 7574 6f6d 6174  nts that automat
+000005e0: 6963 616c 6c79 0a20 2073 6574 2074 6865  ically.  set the
+000005f0: 2063 7265 6174 6564 2061 6e64 206d 6f64   created and mod
+00000600: 6966 6965 6420 6461 7465 2061 6e64 2073  ified date and s
+00000610: 6f6d 6520 6f74 6865 7220 6d65 7461 6461  ome other metada
+00000620: 7461 2e0a 0a43 6f6d 706c 6574 6520 646f  ta...Complete do
+00000630: 6375 6d65 6e74 6174 696f 6e20 6973 2068  cumentation is h
+00000640: 6f73 7465 6420 6174 2068 7474 7073 3a2f  osted at https:/
+00000650: 2f7a 6f70 6564 7562 6c69 6e63 6f72 652e  /zopedublincore.
+00000660: 7265 6164 7468 6564 6f63 732e 696f 2f0a  readthedocs.io/.
```

### Comparing `zope.dublincore-4.3.0/docs/Makefile` & `zope.dublincore-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/docs/api.rst` & `zope.dublincore-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/docs/conf.py` & `zope.dublincore-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/docs/hacking.rst` & `zope.dublincore-5.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/docs/make.bat` & `zope.dublincore-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/docs/narrative.rst` & `zope.dublincore-5.0/docs/narrative.rst`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/setup.py` & `zope.dublincore-5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.dublincore package
 """
-from setuptools import setup, find_packages
 import os.path
 
+from setuptools import find_packages
+from setuptools import setup
+
 
 def read(*path):
     with open(os.path.join(*path)) as f:
         return f.read() + '\n\n'
 
 
 long_description = '\n\n'.join([
@@ -36,66 +38,68 @@
     'zope.testing >= 3.8',
     'zope.testrunner',
     'zope.configuration',
     'BTrees',
 ]
 
 tests_require = testing_require + [
-    # 'zope.annotation',
     'zope.publisher',
 ]
 
 
 setup(
     name="zope.dublincore",
-    version='4.3.0',
+    version='5.0',
     url='http://github.com/zopefoundation/zope.dublincore',
     license='ZPL 2.1',
     description='Zope Dublin Core implementation',
     long_description=long_description,
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     keywords='metadata dublincore',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development',
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
     include_package_data=True,
+    python_requires='>=3.7',
     install_requires=[
         'persistent',
         'pytz',
         'setuptools',
-        'six',
         'zope.annotation',
         'zope.component[zcml]',
         'zope.datetime',
         'zope.interface',
         'zope.lifecycleevent',
         'zope.location',
         'zope.schema',
         'zope.security[zcml]>=3.8',
     ],
     extras_require={
         'testing': testing_require,
         'test': tests_require,
-        'docs': ['Sphinx', 'repoze.sphinx.autointerface'],
+        'docs': [
+            'Sphinx',
+            'repoze.sphinx.autointerface',
+            'zope.testing',
+        ],
     },
     zip_safe=False,
 )
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/annotatableadapter.py` & `zope.dublincore-5.0/src/zope/dublincore/annotatableadapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,33 +10,27 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Dublin Core Annotatable Adapter
 """
 from persistent.dict import PersistentDict
-
 from zope.annotation.interfaces import IAnnotatable
 from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
 from zope.interface import implementer
 from zope.location import Location
+
 from zope.dublincore.interfaces import IWriteZopeDublinCore
 from zope.dublincore.zopedublincore import DateProperty
 from zope.dublincore.zopedublincore import ScalarProperty
 from zope.dublincore.zopedublincore import ZopeDublinCore
-import six
 
-DCkey = "zope.app.dublincore.ZopeDublinCore"
 
-try:
-    unicode
-except NameError:
-    # Py3: Make unicode available.
-    unicode = str
+DCkey = "zope.app.dublincore.ZopeDublinCore"
 
 
 @implementer(IWriteZopeDublinCore)
 @adapter(IAnnotatable)
 class ZDCAnnotatableAdapter(ZopeDublinCore, Location):
     """Adapt annotatable objects to Zope Dublin Core."""
 
@@ -45,15 +39,15 @@
     def __init__(self, context):
         annotations = IAnnotations(context)
         dcdata = annotations.get(DCkey)
         if dcdata is None:
             self.annotations = annotations
             dcdata = ZDCAnnotationData()
 
-        super(ZDCAnnotatableAdapter, self).__init__(dcdata)
+        super().__init__(dcdata)
 
     def _changed(self):
         if self.annotations is not None:
             self.annotations[DCkey] = self._mapping
             self.annotations = None
 
 
@@ -68,29 +62,29 @@
 
 # Hybrid adapters.
 #
 # Adapter factories created using this support the Dublin Core using a
 # mixture of annotations and data on the context object.
 
 
-class DirectProperty(object):
+class DirectProperty:
 
     def __init__(self, name, attrname):
         self.__name__ = name
         self.__attrname = attrname
 
     def __get__(self, inst, klass):
         if inst is None:
             return self
         context = inst._ZDCPartialAnnotatableAdapter__context
-        return getattr(context, self.__attrname, u"")
+        return getattr(context, self.__attrname, "")
 
     def __set__(self, inst, value):
-        if not isinstance(value, unicode):
-            raise TypeError("Element must be unicode")
+        if not isinstance(value, str):
+            raise TypeError("Element must be str")
         context = inst._ZDCPartialAnnotatableAdapter__context
         oldvalue = getattr(context, self.__attrname, None)
         if oldvalue != value:
             setattr(context, self.__attrname, value)
 
 
 def partialAnnotatableAdapterFactory(direct_fields):
@@ -111,15 +105,15 @@
     class ZDCPartialAnnotatableAdapter(ZDCAnnotatableAdapter):
 
         def __init__(self, context):
             self.__context = context
             # can't use super() since this isn't a globally available class
             ZDCAnnotatableAdapter.__init__(self, context)
 
-    for dcname, attrname in six.iteritems(fieldmap):
+    for dcname, attrname in fieldmap.items():
         oldprop = ZopeDublinCore.__dict__.get(dcname)
         if oldprop is None:
             raise ValueError("%r is not a valid DC field" % dcname)
         if (isinstance(oldprop, DateProperty)
                 or not isinstance(oldprop, ScalarProperty)):
             raise ValueError("%r is not a supported DC field" % dcname)
         prop = DirectProperty(dcname, attrname)
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/browser/box.pt` & `zope.dublincore-5.0/src/zope/dublincore/browser/box.pt`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/browser/configure.zcml` & `zope.dublincore-5.0/src/zope/dublincore/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/browser/edit.pt` & `zope.dublincore-5.0/src/zope/dublincore/browser/edit.pt`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/browser/metadataedit.py` & `zope.dublincore-5.0/src/zope/dublincore/browser/metadataedit.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,39 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Dublin Core Meta Data View
 """
 from datetime import datetime
+
 from zope.event import notify
-from zope.dublincore.interfaces import IZopeDublinCore
-from zope.lifecycleevent import ObjectModifiedEvent, Attributes
 from zope.i18nmessageid import MessageFactory
+from zope.lifecycleevent import Attributes
+from zope.lifecycleevent import ObjectModifiedEvent
+
+from zope.dublincore.interfaces import IZopeDublinCore
+
 
 _ = MessageFactory('zope')
-text_type = type(u'')  # PY3
 
 
-class MetaDataEdit(object):
+class MetaDataEdit:
     """Provide view for editing basic dublin-core meta-data."""
 
     def edit(self):
         request = self.request
         formatter = self.request.locale.dates.getFormatter(
             'dateTime', 'medium')
         dc = IZopeDublinCore(self.context)
         message = ''
 
         if 'dctitle' in request:
-            dc.title = text_type(request['dctitle'])
-            dc.description = text_type(request['dcdescription'])
+            dc.title = str(request['dctitle'])
+            dc.description = str(request['dcdescription'])
             description = Attributes(IZopeDublinCore, 'title', 'description')
             notify(ObjectModifiedEvent(self.context, description))
             message = _(
                 "Changed data ${datetime}",
                 mapping={'datetime': formatter.format(datetime.utcnow())})
 
         return {
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/browser/tests/test_metadataedit.py` & `zope.dublincore-5.0/src/zope/dublincore/browser/tests/test_metadataedit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from zope.component.testing import PlacelessSetup
-from zope.dublincore.browser.metadataedit import MetaDataEdit
-from zope.publisher.browser import TestRequest
 import unittest
+
 import zope.annotation.interfaces
+from zope.component.testing import PlacelessSetup
+from zope.publisher.browser import TestRequest
+
 import zope.dublincore.testing
+from zope.dublincore.browser.metadataedit import MetaDataEdit
 
 
 @zope.interface.implementer(zope.annotation.interfaces.IAnnotations)
 class DummyContext(dict):
     """A dummy class which can store annotations."""
 
 
 class MetaDataEditTests(PlacelessSetup, unittest.TestCase):
     """Testing ..metadataedit.MetaDataEdit."""
 
     def setUp(self):
-        super(MetaDataEditTests, self).setUp()
+        super().setUp()
         zope.dublincore.testing.setUpDublinCore()
 
     def test_metadataedit__MetaDataEdit__edit__1(self):
         """It stores DC request values on the context."""
         view = MetaDataEdit()
         request = TestRequest(
             form={'dctitle': 'Test', 'dcdescription': 'Testing'})
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/configure.zcml` & `zope.dublincore-5.0/src/zope/dublincore/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/creatorannotator.py` & `zope.dublincore-5.0/src/zope/dublincore/creatorannotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,18 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Object that takes care of annotating the dublin core creator field.
 """
-from zope.dublincore.interfaces import IZopeDublinCore
 from zope.security.management import queryInteraction
 from zope.security.proxy import removeSecurityProxy
 
-try:
-    unicode
-except NameError:
-    # Py3: Make unicode available.
-    unicode = str
+from zope.dublincore.interfaces import IZopeDublinCore
 
 
 def CreatorAnnotator(object, event=None):
     """Update Dublin-Core creator property"""
     if event is None:
         # annotator was only called the event as only argument
         object = object.object
@@ -43,8 +38,8 @@
     interaction = queryInteraction()
     if interaction is not None:
         for participation in interaction.participations:
             if participation.principal is None:
                 continue
             principalid = participation.principal.id
             if principalid not in dc.creators:
-                dc.creators = dc.creators + (unicode(principalid), )
+                dc.creators = dc.creators + (str(principalid), )
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/dcterms.py` & `zope.dublincore-5.0/src/zope/dublincore/dcterms.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Support information for qualified Dublin Core Metadata.
 """
 from zope.dublincore import dcsv
-import six
+
 
 # useful namespace URIs
 DC_NS = "http://purl.org/dc/elements/1.1/"
 DCTERMS_NS = "http://purl.org/dc/terms/"
 XSI_NS = "http://www.w3.org/2001/XMLSchema-instance"
 
 W3CDTF = "W3CDTF"
@@ -192,12 +192,12 @@
 _prefix_to_ns = {
     "dc": DC_NS,
     "dcterms": DCTERMS_NS,
     # "xsi": XSI_NS,    dont' use this for element names, only attrs
 }
 
 element_to_name = {}
-for name, (qname, attrs) in six.iteritems(name_to_element):
+for name, (qname, attrs) in name_to_element.items():
     prefix, localname = qname.split(":")
     elem_name = _prefix_to_ns[prefix], localname
     element_to_name[elem_name] = name
     name_to_element[name] = (elem_name, attrs)
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/interfaces.py` & `zope.dublincore-5.0/src/zope/dublincore/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Dublin Core interfaces
 """
 from zope.interface import Interface
-from zope.schema import Text, TextLine, Datetime, Tuple
+from zope.schema import Datetime
+from zope.schema import Text
+from zope.schema import TextLine
+from zope.schema import Tuple
 
 
 class IDublinCoreElementItem(Interface):
     """A qualified dublin core element"""
 
     qualification = TextLine(
-        title=u"Qualification",
-        description=u"The element qualification"
+        title="Qualification",
+        description="The element qualification"
     )
 
     value = Text(
-        title=u"Value",
-        description=u"The element value",
+        title="Value",
+        description="The element value",
     )
 
 
 class IGeneralDublinCore(Interface):
     """Dublin-core data access interface
 
     The Dublin Core, http://dublincore.org/, is a meta data standard
@@ -197,85 +200,85 @@
         """
 
 
 class IDCDescriptiveProperties(Interface):
     """Basic descriptive meta-data properties"""
 
     title = TextLine(
-        title=u'Title',
-        description=u"The first unqualified Dublin Core 'Title' element value."
+        title='Title',
+        description="The first unqualified Dublin Core 'Title' element value."
     )
 
     description = Text(
-        title=u'Description',
+        title='Description',
         description=(
-            u"The first unqualified Dublin Core 'Description' element value.")
+            "The first unqualified Dublin Core 'Description' element value.")
     )
 
 
 class IDCTimes(Interface):
     """Time properties"""
 
     created = Datetime(
-        title=u'Creation Date',
-        description=u"The date and time that an object is created."
-                    u"\nThis is normally set automatically."
+        title='Creation Date',
+        description="The date and time that an object is created."
+                    "\nThis is normally set automatically."
     )
 
     modified = Datetime(
-        title=u'Modification Date',
-        description=u"The date and time that the object was last modified in a"
-                    u" meaningful way."
+        title='Modification Date',
+        description="The date and time that the object was last modified in a"
+                    " meaningful way."
     )
 
 
 class IDCPublishing(Interface):
     """Publishing properties"""
 
     effective = Datetime(
-        title=u'Effective Date',
-        description=u"The date and time that an object should be published."
+        title='Effective Date',
+        description="The date and time that an object should be published."
     )
 
     expires = Datetime(
-        title=u'Expiration Date',
-        description=u"The date and time that the object should become"
-                    u" unpublished."
+        title='Expiration Date',
+        description="The date and time that the object should become"
+                    " unpublished."
     )
 
 
 class IDCExtended(Interface):
     """Extended properties
 
     This is a mixed bag of properties we want but that we probably haven't
     quite figured out yet.
     """
 
     creators = Tuple(
-        title=u'Creators',
-        description=u"The unqualified Dublin Core 'Creator' element values",
+        title='Creators',
+        description="The unqualified Dublin Core 'Creator' element values",
         value_type=TextLine(),
     )
 
     subjects = Tuple(
-        title=u'Subjects',
-        description=u"The unqualified Dublin Core 'Subject' element values",
+        title='Subjects',
+        description="The unqualified Dublin Core 'Subject' element values",
         value_type=TextLine(),
     )
 
     publisher = Text(
-        title=u'Publisher',
-        description=u"The first unqualified Dublin Core 'Publisher' element"
-                    u" value.",
+        title='Publisher',
+        description="The first unqualified Dublin Core 'Publisher' element"
+                    " value.",
     )
 
     contributors = Tuple(
-        title=u'Contributors',
-        description=u"The unqualified Dublin Core 'Contributor' element"
-                    u" values",
+        title='Contributors',
+        description="The unqualified Dublin Core 'Contributor' element"
+                    " values",
         value_type=TextLine(),
     )
 
 
 class ICMFDublinCore(Interface):
     """This interface duplicates the CMF dublin core interface."""
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/property.py` & `zope.dublincore-5.0/src/zope/dublincore/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Base DublinCore property adapter.
 """
 from zope import schema
-
 from zope.dublincore.interfaces import IZopeDublinCore
 
+
 _marker = object()
 
 
-class DCProperty(object):
+class DCProperty:
     """Adapt to a dublin core property
 
     Handles DC list properties as scalar property.
     """
 
     def __init__(self, name):
         self.__name = name
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_annotatableadapter.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_annotatableadapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests annotatableadapter.
 """
 import unittest
 
+
 _marker = object()
 
 
 class ZDCAnnotatableAdapterTests(unittest.TestCase):
 
     _registered = False
 
@@ -31,17 +32,18 @@
         cleanUp()
 
     def _getTargetClass(self):
         from zope.dublincore.annotatableadapter import ZDCAnnotatableAdapter
         return ZDCAnnotatableAdapter
 
     def _registerAnnotations(self, dcdata=None):
+        from zope.annotation.interfaces import IAnnotations
         from zope.component import provideAdapter
         from zope.interface import Interface
-        from zope.annotation.interfaces import IAnnotations
+
         from zope.dublincore.annotatableadapter import DCkey
 
         class _Annotations(dict):
             pass
         instance = _Annotations({DCkey: dcdata})
 
         def _factory(context):
@@ -53,25 +55,27 @@
 
     def _makeOne(self, context=_marker):
         if context is _marker:
             context = self._makeContext()
         return self._getTargetClass()(context)
 
     def _makeContext(self):
-        class DummyContext(object):
+        class DummyContext:
             pass
         return DummyContext()
 
     def test_class_conforms_to_IWriteZopeDublinCore(self):
         from zope.interface.verify import verifyClass
+
         from zope.dublincore.interfaces import IWriteZopeDublinCore
         verifyClass(IWriteZopeDublinCore, self._getTargetClass())
 
     def test_instance_conforms_to_IWriteZopeDublinCore(self):
         from zope.interface.verify import verifyObject
+
         from zope.dublincore.interfaces import IWriteZopeDublinCore
         self._registerAnnotations()
         verifyObject(IWriteZopeDublinCore, self._makeOne())
 
     def test_ctor_wo_existing_DC_annotations(self):
         from zope.dublincore.annotatableadapter import DCkey
         self._registerAnnotations()
@@ -115,40 +119,40 @@
 
     def _makeOne(self, name, attrname):
         return self._getTargetClass()(name, attrname)
 
     def test___get___via_klass(self):
         prop = self._makeOne('title', 'headline')
 
-        class Testing(object):
+        class Testing:
             title = prop
         self.assertTrue(Testing.title is prop)
 
     def test___get___via_instance(self):
         prop = self._makeOne('title', 'headline')
 
-        class Context(object):
-            headline = u'HEADLINE'
+        class Context:
+            headline = 'HEADLINE'
 
-        class ZDCPartialAnnotatableAdapter(object):
+        class ZDCPartialAnnotatableAdapter:
             title = prop
 
             def __init__(self, context):
                 self.__context = context
         context = Context()
         testing = ZDCPartialAnnotatableAdapter(context)
-        self.assertEqual(testing.title, u'HEADLINE')
+        self.assertEqual(testing.title, 'HEADLINE')
 
     def test___set___non_unicode_raises(self):
         prop = self._makeOne('title', 'headline')
 
-        class Context(object):
-            headline = u'HEADLINE'
+        class Context:
+            headline = 'HEADLINE'
 
-        class ZDCPartialAnnotatableAdapter(object):
+        class ZDCPartialAnnotatableAdapter:
             title = prop
 
             def __init__(self, context):
                 self.__context = context
         context = Context()
         testing = ZDCPartialAnnotatableAdapter(context)
         try:
@@ -157,51 +161,51 @@
             pass
         else:
             self.fail("Didn't raise TypeError")
 
     def test___set___unchanged_doesnt_mutate(self):
         prop = self._makeOne('title', 'headline')
 
-        class Context(object):
-            headline = u'HEADLINE'
+        class Context:
+            headline = 'HEADLINE'
 
             def __setattr__(self, name, value):
                 assert 0
 
-        class ZDCPartialAnnotatableAdapter(object):
+        class ZDCPartialAnnotatableAdapter:
             title = prop
 
             def __init__(self, context):
                 self.__context = context
         context = Context()
         testing = ZDCPartialAnnotatableAdapter(context)
-        testing.title = u'HEADLINE'  # doesn't raise
+        testing.title = 'HEADLINE'  # doesn't raise
 
     def test___set___changed_mutates(self):
         prop = self._makeOne('title', 'headline')
 
-        class Context(object):
-            headline = u'HEADLINE1'
+        class Context:
+            headline = 'HEADLINE1'
 
-        class ZDCPartialAnnotatableAdapter(object):
+        class ZDCPartialAnnotatableAdapter:
             title = prop
 
             def __init__(self, context):
                 self.__context = context
         context = Context()
         testing = ZDCPartialAnnotatableAdapter(context)
-        testing.title = u'HEADLINE2'
-        self.assertEqual(context.headline, u'HEADLINE2')
+        testing.title = 'HEADLINE2'
+        self.assertEqual(context.headline, 'HEADLINE2')
 
 
 class Test_partialAnnotatableAdapterFactory(unittest.TestCase):
 
     def _callFUT(self, direct_fields):
-        from zope.dublincore.annotatableadapter \
-            import partialAnnotatableAdapterFactory
+        from zope.dublincore.annotatableadapter import \
+            partialAnnotatableAdapterFactory
         return partialAnnotatableAdapterFactory(direct_fields)
 
     def test_w_empty_list_raises(self):
         self.assertRaises(ValueError, self._callFUT, [])
 
     def test_w_empty_dict_raises(self):
         self.assertRaises(ValueError, self._callFUT, {})
@@ -231,15 +235,7 @@
     def test_w_scalar_prop_mapped(self):
         from zope.dublincore.annotatableadapter import DirectProperty
         klass = self._callFUT({'title': 'headline'})
         prop = klass.title
         self.assertTrue(isinstance(prop, DirectProperty))
         self.assertEqual(prop.__name__, 'title')
         self.assertEqual(prop._DirectProperty__attrname, 'headline')  # XXX
-
-
-def test_suite():
-    return unittest.TestSuite((
-        unittest.makeSuite(ZDCAnnotatableAdapterTests),
-        unittest.makeSuite(DirectPropertyTests),
-        unittest.makeSuite(Test_partialAnnotatableAdapterFactory),
-    ))
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_creatorannotator.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_creatorannotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def setUp(self):
         from zope.testing.cleanup import cleanUp
         cleanUp()
         self._makeInterface()
         self._registerAdapter()
 
     def tearDown(self):
-        from zope.testing.cleanup import cleanUp
         from zope.security.management import endInteraction
+        from zope.testing.cleanup import cleanUp
         endInteraction()
         cleanUp()
 
     def _callFUT(self, event):
         from zope.dublincore.creatorannotator import CreatorAnnotator
         return CreatorAnnotator(event)
 
@@ -40,37 +40,38 @@
         class IDummyContent(Interface):
             pass
 
         self._iface = IDummyContent
 
     def _registerAdapter(self):
         from zope.component import provideAdapter
+
         from zope.dublincore.interfaces import IZopeDublinCore
         provideAdapter(DummyDCAdapter, (self._iface, ), IZopeDublinCore)
 
     def _makeContextAndEvent(self):
 
         from zope.interface import implementer
 
         @implementer(self._iface)
-        class DummyDublinCore(object):
+        class DummyDublinCore:
             creators = ()
 
-        class DummyEvent(object):
+        class DummyEvent:
             def __init__(self, object):
                 self.object = object
 
         context = DummyDublinCore()
         event = DummyEvent(context)
         return context, event
 
     def _setPrincipal(self, id):
         from zope.security.management import newInteraction
 
-        class DummyPrincipal(object):
+        class DummyPrincipal:
             title = 'TITLE'
             description = 'DESCRIPTION'
 
             def __init__(self, id):
                 self.id = id
         if id is None:
             newInteraction(DummyRequest(None))
@@ -113,25 +114,25 @@
 class CreatorAnnotatorObjectEventTests(CreatorAnnotatorTests):
 
     def _callFUT(self, event):
         from zope.dublincore.creatorannotator import CreatorAnnotator
         return CreatorAnnotator(event.object, event)
 
 
-class DummyDCAdapter(object):
+class DummyDCAdapter:
 
     def _getcreator(self):
         return self.context.creators
 
     def _setcreator(self, value):
         self.context.creators = value
     creators = property(_getcreator, _setcreator, None, "Adapted Creators")
 
     def __init__(self, context):
         self.context = context
 
 
-class DummyRequest(object):
+class DummyRequest:
 
     def __init__(self, principal):
         self.principal = principal
         self.interaction = None
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_dcsv.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_dcsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test the Dublin Core Structured Value support functions.
 """
 from doctest import DocTestSuite
+
 # Imports needed inside the doctests:
-from zope.dublincore.dcsv import encode, decode
+from zope.dublincore.dcsv import decode
+from zope.dublincore.dcsv import encode
 
 
 # TODO still need tests for errors, and createMapping()
 
 
 def test_decode_empty():
     """
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_xmlmetadata.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_xmlmetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 #
 ##############################################################################
 """Test loading of Dublin Core metadata from the XML representation.
 """
 import unittest
 
 from zope.dublincore import dcterms
-from zope.dublincore.xmlmetadata import dumpString, parseString
+from zope.dublincore.xmlmetadata import dumpString
+from zope.dublincore.xmlmetadata import parseString
 
 
 class XMLDublinCoreLoadingTests(unittest.TestCase):
 
     # Note: We're not using the 'traditional' namespace prefixes in
     # the tests since we want to make sure we're doing the right thing
     # in the content handler.  Also, we should use something we're not
@@ -29,50 +30,50 @@
                "<metadata xmlns:d='%s'\n"
                "          xmlns:t='%s'\n"
                "          xmlns:s='%s'>\n"
                % (dcterms.DC_NS, dcterms.DCTERMS_NS, dcterms.XSI_NS))
     _suffix = "\n</metadata>"
 
     def parse(self, text):
-        return parseString("%s%s%s" % (self._prefix, text, self._suffix))
+        return parseString("{}{}{}".format(self._prefix, text, self._suffix))
 
     def check1(self, text, name, value, generic=None):
         expected = {name: (value,)}
         m = self.parse(text)
         self.assertEqual(m, expected)
         m = self.parse("<wrap>%s</wrap>" % text)
         self.assertEqual(m, expected)
         if generic:
-            m = self.parse("<%s>%s</%s>" % (generic, text, generic))
+            m = self.parse("<{}>{}</{}>".format(generic, text, generic))
             self.assertEqual(m, expected)
             m = self.parse("<%s><wrap>%s</wrap></%s>"
                            % (generic, text, generic))
             self.assertEqual(m, expected)
 
     # tests with acceptable input
 
     def test_empty(self):
         m = parseString("<metadata/>")
         self.assertEqual(m, {})
 
     # core elements and related refinements
 
     def test_simple_title(self):
-        self.check1("<d:title>Foo</d:title>", "Title", u"Foo")
+        self.check1("<d:title>Foo</d:title>", "Title", "Foo")
 
     def test_two_titles(self):
         m = self.parse("<d:title>Foo</d:title>"
                        "<d:title>Bar</d:title>")
-        self.assertEqual(m, {"Title": (u"Foo", u"Bar")})
+        self.assertEqual(m, {"Title": ("Foo", "Bar")})
 
     def test_alternative_title(self):
         m = self.parse("<d:title>Foo</d:title>"
                        "<t:alternative>Bar</t:alternative>")
-        self.assertEqual(m, {"Title": (u"Foo",),
-                             "Title.Alternative": (u"Bar",)})
+        self.assertEqual(m, {"Title": ("Foo",),
+                             "Title.Alternative": ("Bar",)})
 
     def test_creator(self):
         self.check1("<d:creator>somebody</d:creator>",
                     "Creator", "somebody")
 
     def test_subject(self):
         self.check1("<d:subject>something</d:subject>",
@@ -233,20 +234,20 @@
                     "Audience.Mediator", "people", generic="t:audience")
 
     def test_nested_refinement(self):
         # direct nesting
         self.check1(("<d:title>"
                      "<t:alternative>Foo</t:alternative>"
                      "</d:title>"),
-                    "Title.Alternative", u"Foo")
+                    "Title.Alternative", "Foo")
         # nesting with an intermediate element
         self.check1(("<d:title>"
                      "<x><t:alternative>Foo</t:alternative></x>"
                      "</d:title>"),
-                    "Title.Alternative", u"Foo")
+                    "Title.Alternative", "Foo")
 
     # tests with errors in the input
 
     def test_invalid_nested_refinement(self):
         self.assertRaises(ValueError, self.parse,
                           ("<d:format>"
                            "<t:alternative>Title</t:alternative>"
@@ -272,17 +273,11 @@
         parsed = parseString(text)
         self.assertEqual(parsed, mapping)
 
     def test_serialize_empty(self):
         self.roundtrip({})
 
     def test_single_entry(self):
-        self.roundtrip({"Title.Alternative": (u"Foo",)})
+        self.roundtrip({"Title.Alternative": ("Foo",)})
 
     def test_two_titles(self):
-        self.roundtrip({"Title": (u"Foo", u"Bar")})
-
-
-def test_suite():
-    suite = unittest.makeSuite(XMLDublinCoreLoadingTests)
-    suite.addTest(unittest.makeSuite(XMLDublinCoreSerializationTests))
-    return suite
+        self.roundtrip({"Title": ("Foo", "Bar")})
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zcml.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_zcml.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Tests that ZCML can be loaded.
 """
 import unittest
+
 import zope.component.testing
 
 
 class ZCMLTests(unittest.TestCase):
 
     setUp = zope.component.testing.setUp
     tearDown = zope.component.testing.tearDown
 
     def test_loadable(self):
         # N.B.:  this test deliberately avoids any "ftesting" / layers
         #        support:  its purpose is to ensure that the package's
         #        ZCML file is loadable *without* loading any other ZCML.
         from zope.configuration.xmlconfig import file
+
         import zope.dublincore
         return file('configure.zcml', package=zope.dublincore)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ZCMLTests),
+        unittest.defaultTestLoader.loadTestsFromTestCase(ZCMLTests),
     ))
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zdcannotatableadapter.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_zdcannotatableadapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,14 @@
 
     def testZDCAnnotatableAdapter(self):
         from zope.dublincore.annotatableadapter import ZDCAnnotatableAdapter
         annotations = TestAnnotations()
         dc = ZDCAnnotatableAdapter(annotations)
 
         self.assertFalse(annotations, "There shouldn't be any data yet")
-        self.assertEqual(dc.title, u'')
+        self.assertEqual(dc.title, '')
         self.assertFalse(annotations, "There shouldn't be any data yet")
-        dc.title = u"Test title"
+        dc.title = "Test title"
         self.assertTrue(annotations, "There should be data now!")
 
         dc = ZDCAnnotatableAdapter(annotations)
-        self.assertEqual(dc.title, u'Test title')
-
-
-def test_suite():
-    return unittest.makeSuite(DublinCoreAdapterTest)
+        self.assertEqual(dc.title, 'Test title')
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/tests/test_zopedublincore.py` & `zope.dublincore-5.0/src/zope/dublincore/tests/test_zopedublincore.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from unittest import TestCase
 
 
 class Test(TestCase):
 
     def testImplementa(self):
         from zope.interface.verify import verifyObject
+
         from zope.dublincore.interfaces import IZopeDublinCore
         verifyObject(IZopeDublinCore, self.dc)
 
     def _Test__new(self):
         from zope.dublincore.zopedublincore import ZopeDublinCore
         return ZopeDublinCore()
 
@@ -38,18 +39,18 @@
         ivalues.sort()
         ovalues = list(ovalues)
         ovalues.sort()
         self.assertEqual(ovalues, ivalues)
 
     def __testQualified(self, name,
                         values=[
-                            (u'', u'blah blah'),
-                            (u'old', u'bleep bleep'),
-                            (u'old', u'bleep bleep \u1111'),
-                            (u'foo\u1111', u'bleep bleep'),
+                            ('', 'blah blah'),
+                            ('old', 'bleep bleep'),
+                            ('old', 'bleep bleep \u1111'),
+                            ('foo\u1111', 'bleep bleep'),
                         ]):
         getattr(self.dc, 'setQualified' + name)(values)
         self.__testGetQualified(name, values)
 
     def testOtherQualified(self):
         for name in ('Sources', 'Relations', 'Coverages'):
             self.__testQualified(name)
@@ -63,122 +64,122 @@
                 ('Formats', 'Format', 'format'),
                 ('Identifiers', 'Identifier', 'identifier'),
                 ('Languages', 'Language', 'language'),
                 ('Rights', 'Rights', 'rights'),
         ):
             self.__testQualified(qname)
             dc = self.dc
-            self.assertEqual(getattr(dc, pname), u'blah blah')
-            self.assertEqual(getattr(dc, mname)(), u'blah blah')
+            self.assertEqual(getattr(dc, pname), 'blah blah')
+            self.assertEqual(getattr(dc, mname)(), 'blah blah')
 
             self.assertRaises(Exception, setattr, dc, pname, b'foo')
-            setattr(dc, pname, u'foo')
-            self.assertEqual(getattr(dc, pname), u'foo')
-            self.assertEqual(getattr(dc, mname)(), u'foo')
+            setattr(dc, pname, 'foo')
+            self.assertEqual(getattr(dc, pname), 'foo')
+            self.assertEqual(getattr(dc, mname)(), 'foo')
             self.__testGetQualified(qname,
-                                    [(u'', u'foo'),
-                                     (u'old', u'bleep bleep'),
-                                     (u'old', u'bleep bleep \u1111'),
-                                     (u'foo\u1111', u'bleep bleep'),
+                                    [('', 'foo'),
+                                     ('old', 'bleep bleep'),
+                                     ('old', 'bleep bleep \u1111'),
+                                     ('foo\u1111', 'bleep bleep'),
                                      ]
                                     )
 
     def testSequences(self):
         for qname, mname, pname in (
             ('Creators', 'Creator', 'creators'),
             ('Subjects', 'Subject', 'subjects'),
             ('Contributors', 'Contributors', 'contributors'),
         ):
-            self.__testQualified(qname, [(u'', u'foo'),
-                                         (u'', u'bar'),
-                                         (u'', u'baz'),
-                                         (u'', u'baz\u1111'),
-                                         (u'old', u'bleep bleep'),
-                                         (u'old', u'bleep bleep \u1111'),
-                                         (u'foo\u1111', u'bleep bleep'),
+            self.__testQualified(qname, [('', 'foo'),
+                                         ('', 'bar'),
+                                         ('', 'baz'),
+                                         ('', 'baz\u1111'),
+                                         ('old', 'bleep bleep'),
+                                         ('old', 'bleep bleep \u1111'),
+                                         ('foo\u1111', 'bleep bleep'),
                                          ]
                                  )
             dc = self.dc
 
             v = getattr(dc, pname)
             v = list(v)
             v.sort()
-            self.assertEqual(v, [u'bar', u'baz', u'baz\u1111', u'foo'])
+            self.assertEqual(v, ['bar', 'baz', 'baz\u1111', 'foo'])
 
             v = getattr(dc, mname)()
             v = list(v)
             v.sort()
-            self.assertEqual(v, [u'bar', u'baz', u'baz\u1111', u'foo'])
+            self.assertEqual(v, ['bar', 'baz', 'baz\u1111', 'foo'])
 
             self.assertRaises(Exception, setattr, dc, pname, b'foo')
             self.assertRaises(Exception, setattr, dc, pname, [b'foo'])
 
-            setattr(dc, pname, [u'high', u'low', u'spam', u'eggs', u'ham', ])
+            setattr(dc, pname, ['high', 'low', 'spam', 'eggs', 'ham', ])
 
             v = getattr(dc, pname)
             v = list(v)
             v.sort()
-            self.assertEqual(v, [u'eggs', u'ham', u'high', u'low', u'spam'])
+            self.assertEqual(v, ['eggs', 'ham', 'high', 'low', 'spam'])
 
             v = getattr(dc, mname)()
             v = list(v)
             v.sort()
-            self.assertEqual(v, [u'eggs', u'ham', u'high', u'low', u'spam'])
+            self.assertEqual(v, ['eggs', 'ham', 'high', 'low', 'spam'])
 
             self.__testGetQualified(qname,
-                                    [(u'', u'high'),
-                                     (u'', u'low'),
-                                     (u'', u'spam'),
-                                     (u'', u'eggs'),
-                                     (u'', u'ham'),
-                                     (u'old', u'bleep bleep'),
-                                     (u'old', u'bleep bleep \u1111'),
-                                     (u'foo\u1111', u'bleep bleep'),
+                                    [('', 'high'),
+                                     ('', 'low'),
+                                     ('', 'spam'),
+                                     ('', 'eggs'),
+                                     ('', 'ham'),
+                                     ('old', 'bleep bleep'),
+                                     ('old', 'bleep bleep \u1111'),
+                                     ('foo\u1111', 'bleep bleep'),
                                      ]
                                     )
 
     def testDates(self):
         self.__testQualified('Dates', [
-            (u'', u'1990-01-01'),
-            (u'Created', u'1980-10-01T23:11:10-04:00'),
-            (u'Modified', u'2002-10-01T12:09:22-04:00'),
-            (u'Effective', u'2002-10-09T00:00:00-04:00'),
-            (u'Expires', u'2002-10-16T00:00:00-04:00'),
-            (u'xxx', u'2000-07-04'),
-            (u'xxx', u'2001-12-31'),
-            (u'foo \u1111', u'2001-12-31'),
+            ('', '1990-01-01'),
+            ('Created', '1980-10-01T23:11:10-04:00'),
+            ('Modified', '2002-10-01T12:09:22-04:00'),
+            ('Effective', '2002-10-09T00:00:00-04:00'),
+            ('Expires', '2002-10-16T00:00:00-04:00'),
+            ('xxx', '2000-07-04'),
+            ('xxx', '2001-12-31'),
+            ('foo \u1111', '2001-12-31'),
         ])
 
         from zope.datetime import parseDatetimetz
 
         dc = self.dc
         self.assertEqual(dc.created,
                          parseDatetimetz('1980-10-01T23:11:10-04:00'))
         self.assertEqual(dc.modified,
                          parseDatetimetz('2002-10-01T12:09:22-04:00'))
         self.assertEqual(dc.effective,
                          parseDatetimetz('2002-10-09T00:00:00-04:00'))
         self.assertEqual(dc.expires,
                          parseDatetimetz('2002-10-16T00:00:00-04:00'))
 
-        self.assertEqual(dc.Date(), u'1990-01-01')
-        self.assertEqual(dc.CreationDate(), u'1980-10-01T23:11:10-04:00')
-        self.assertEqual(dc.ModificationDate(), u'2002-10-01T12:09:22-04:00')
-        self.assertEqual(dc.EffectiveDate(), u'2002-10-09T00:00:00-04:00')
-        self.assertEqual(dc.ExpirationDate(), u'2002-10-16T00:00:00-04:00')
+        self.assertEqual(dc.Date(), '1990-01-01')
+        self.assertEqual(dc.CreationDate(), '1980-10-01T23:11:10-04:00')
+        self.assertEqual(dc.ModificationDate(), '2002-10-01T12:09:22-04:00')
+        self.assertEqual(dc.EffectiveDate(), '2002-10-09T00:00:00-04:00')
+        self.assertEqual(dc.ExpirationDate(), '2002-10-16T00:00:00-04:00')
 
         dt = parseDatetimetz('2002-10-03T14:51:55-04:00')
 
         dc.modified = dt
 
         self.assertRaises(Exception, setattr, dc, 'modified', 'foo')
 
         modified = [qv[1]
                     for qv in dc.getQualifiedDates()
-                    if qv[0] == u'Modified']
+                    if qv[0] == 'Modified']
 
         self.assertFalse(len(modified) != 1,
                          "should be only one: %r" % modified)
 
         self.assertEqual(parseDatetimetz(modified[0]), dt)
 
         modified = dc.ModificationDate()
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/timeannotators.py` & `zope.dublincore-5.0/src/zope/dublincore/timeannotators.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Objects that take care of annotating dublin core meta data times
 """
 from datetime import datetime
+
 import pytz
-from zope.dublincore.interfaces import IZopeDublinCore
+
 from zope.security.proxy import removeSecurityProxy
 
+from zope.dublincore.interfaces import IZopeDublinCore
+
+
 _NOW = None
 
 
 def _now():
     if _NOW is None:
         return datetime.now(pytz.utc)
     return _NOW
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/xmlmetadata.py` & `zope.dublincore-5.0/src/zope/dublincore/xmlmetadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,39 +11,35 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Dublin Core XML data parser and writer
 """
 import xml.sax
 import xml.sax.handler
-
-from xml.sax.saxutils import escape, quoteattr
+from io import StringIO
+from xml.sax.saxutils import escape
+from xml.sax.saxutils import quoteattr
 
 from zope.dublincore import dcterms
 
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from io import StringIO
-
 
 XSI_TYPE = (dcterms.XSI_NS, "type")
 
 dublin_core_namespaces = dcterms.DC_NS, dcterms.DCTERMS_NS
 
 
 DEFAULT_NAMESPACE_PREFIXES = {
     # uri:              prefix,
     dcterms.DC_NS: "dc",
     dcterms.DCTERMS_NS: "dcterms",
     dcterms.XSI_NS: "xsi",
 }
 
 
-class NamespaceTracker(object):
+class NamespaceTracker:
     def __init__(self, mapping=None):
         self._mapping = {}
         self._used = {}
         if mapping:
             self._mapping.update(mapping)
         self._counter = 0
 
@@ -57,15 +53,15 @@
             self._mapping[uri] = prefix
             self._used[prefix] = uri
         else:
             prefix = self._mapping[uri]
             if prefix not in self._used:
                 self._used[prefix] = uri
         if prefix:
-            return "%s:%s" % (prefix, localname)
+            return "{}:{}".format(prefix, localname)
         else:
             return localname
 
     def getPrefixMappings(self):
         return self._used.items()
 
 
@@ -82,28 +78,28 @@
             prev = group
         if name in dcterms.name_to_element:
             element, t = dcterms.name_to_element[name]
             qname = nsmap.encode(element)
             if not type:
                 type = t
             if type:
-                type = " %s=%s" % (nsmap.encode((dcterms.XSI_NS, "type")),
-                                   quoteattr(type))
+                type = " {}={}".format(nsmap.encode((dcterms.XSI_NS, "type")),
+                                       quoteattr(type))
             for value in values:
                 sio.write("  <%s%s>\n    %s\n  </%s>\n"
                           % (qname, type, _encode_string(value), qname))
         else:
             raise RuntimeError("could not serialize %r metadata element"
                                % name)
     content = sio.getvalue()
     sio = StringIO()
     sio.write("<?xml version='1.0' encoding='utf-8'?>\n"
               "<metadata")
     for prefix, uri in nsmap.getPrefixMappings():
-        sio.write("\n  xmlns:%s=%s" % (prefix, quoteattr(uri)))
+        sio.write("\n  xmlns:{}={}".format(prefix, quoteattr(uri)))
     sio.write(">\n")
     sio.write(content)
     sio.write("</metadata>\n")
     return sio.getvalue()
 
 
 try:
@@ -136,15 +132,15 @@
     parser.setFeature(xml.sax.handler.feature_namespaces, True)
     parser.setContentHandler(ch)
     if error_handler is not None:
         parser.setErrorHandler(error_handler)
     return parser, ch
 
 
-class PrefixManager(object):
+class PrefixManager:
     # We don't use this other than in the DublinCoreHandler, but it's
     # entirely general so we'll separate it out for now.
 
     """General handler for namespace prefixes.
 
     This should be used as a mix-in when creating a ContentHandler.
     """
@@ -188,15 +184,15 @@
         if name in dcterms.element_to_name:
             # dcelem contains type info, so go back to the mapping
             return dcterms.element_to_name[name]
         else:
             return None
 
     def startElementNS(self, name, qname, attrs):
-        self.buffer = u""
+        self.buffer = ""
         # TODO: need convert element to metadata element name
         dcelem = validator = None
         if name in dcterms.element_to_name:
             dcelem = dcterms.element_to_name[name]
         type = attrs.get(XSI_TYPE)
         if type:
             if not dcelem:
@@ -216,15 +212,15 @@
             for elem in allowed_in:
                 elem_split = elem.split(".")
                 if dcelem_split[:len(elem_split)] == elem_split:
                     break
             else:
                 raise ValueError("%s values are not allowed for %r"
                                  % (type, dcelem))
-            dcelem = "%s.%s" % (dcelem, type)
+            dcelem = "{}.{}".format(dcelem, type)
         if dcelem:
             cont = self.get_dc_container()
             if cont and cont != dcelem:
                 prefix = cont + "."
                 if not dcelem.startswith(prefix):
                     raise ValueError("%s is not a valid refinement for %s"
                                      % (dcelem, cont))
```

### Comparing `zope.dublincore-4.3.0/src/zope/dublincore/zopedublincore.py` & `zope.dublincore-5.0/src/zope/dublincore/zopedublincore.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,58 +11,52 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Zope's Dublin Core Implementation
 """
 from datetime import datetime
 
-from zope.interface import implementer
 from zope.datetime import parseDatetimetz
-from zope.dublincore.interfaces import IZopeDublinCore
-import six
+from zope.interface import implementer
 
-try:
-    unicode
-except NameError:
-    # Py3: Make unicode available.
-    unicode = str
+from zope.dublincore.interfaces import IZopeDublinCore
 
 
-class SimpleProperty(object):
+class SimpleProperty:
 
     def __init__(self, name):
         self.__name__ = name
 
 
 class ScalarProperty(SimpleProperty):
 
     def __get__(self, inst, klass):
         if inst is None:
             return self
         data = inst._mapping.get(self.__name__, ())
         if data:
             return data[0]
         else:
-            return u''
+            return ''
 
     def __set__(self, inst, value):
-        if not isinstance(value, unicode):
-            raise TypeError("Element must be unicode")
+        if not isinstance(value, str):
+            raise TypeError("Element must be str")
         dict = inst._mapping
         __name__ = self.__name__
         inst._changed()
         dict[__name__] = (value, ) + dict.get(__name__, ())[1:]
 
 
 def _scalar_get(inst, name):
     data = inst._mapping.get(name, ())
     if data:
         return data[0]
     else:
-        return u''
+        return ''
 
 
 class DateProperty(ScalarProperty):
 
     def __get__(self, inst, klass):
         if inst is None:
             return self
@@ -73,40 +67,39 @@
             return None
 
     def __set__(self, inst, value):
         if not isinstance(value, datetime):
             raise TypeError("Element must be %s", datetime)
 
         value = value.isoformat('T')
-        # Py3: Python 2 support, where isformat returned bytes.
         if isinstance(value, bytes):
             value = value.decode('ascii')
 
-        super(DateProperty, self).__set__(inst, value)
+        super().__set__(inst, value)
 
 
 class SequenceProperty(SimpleProperty):
 
     def __get__(self, inst, klass):
         if inst is None:
             return self
 
         return inst._mapping.get(self.__name__, ())
 
     def __set__(self, inst, value):
         value = tuple(value)
         for v in value:
-            if not isinstance(v, unicode):
-                raise TypeError("Elements must be unicode")
+            if not isinstance(v, str):
+                raise TypeError("Elements must be str")
         inst._changed()
         inst._mapping[self.__name__] = value
 
 
 @implementer(IZopeDublinCore)
-class ZopeDublinCore(object):
+class ZopeDublinCore:
     """Zope Dublin Core Mixin
 
     Subclasses should define either `_changed()` or `_p_changed`.
 
     Just mix with `Persistence` to get a persistent version.
     """
 
@@ -114,248 +107,248 @@
         if mapping is None:
             mapping = {}
         self._mapping = mapping
 
     def _changed(self):
         self._p_changed = True
 
-    title = ScalarProperty(u'Title')
+    title = ScalarProperty('Title')
 
     def Title(self):
         """See `IZopeDublinCore`"""
         return self.title
 
-    creators = SequenceProperty(u'Creator')
+    creators = SequenceProperty('Creator')
 
     def Creator(self):
         """See `IZopeDublinCore`"""
         return self.creators
 
-    subjects = SequenceProperty(u'Subject')
+    subjects = SequenceProperty('Subject')
 
     def Subject(self):
         """See `IZopeDublinCore`"""
         return self.subjects
 
-    description = ScalarProperty(u'Description')
+    description = ScalarProperty('Description')
 
     def Description(self):
         """See `IZopeDublinCore`"""
         return self.description
 
-    publisher = ScalarProperty(u'Publisher')
+    publisher = ScalarProperty('Publisher')
 
     def Publisher(self):
         """See IZopeDublinCore"""
         return self.publisher
 
-    contributors = SequenceProperty(u'Contributor')
+    contributors = SequenceProperty('Contributor')
 
     def Contributors(self):
         """See `IZopeDublinCore`"""
         return self.contributors
 
     def Date(self):
         """See IZopeDublinCore"""
-        return _scalar_get(self, u'Date')
+        return _scalar_get(self, 'Date')
 
-    created = DateProperty(u'Date.Created')
+    created = DateProperty('Date.Created')
 
     def CreationDate(self):
         """See `IZopeDublinCore`"""
-        return _scalar_get(self, u'Date.Created')
+        return _scalar_get(self, 'Date.Created')
 
-    effective = DateProperty(u'Date.Effective')
+    effective = DateProperty('Date.Effective')
 
     def EffectiveDate(self):
         """See `IZopeDublinCore`"""
-        return _scalar_get(self, u'Date.Effective')
+        return _scalar_get(self, 'Date.Effective')
 
-    expires = DateProperty(u'Date.Expires')
+    expires = DateProperty('Date.Expires')
 
     def ExpirationDate(self):
         """See `IZopeDublinCore`"""
-        return _scalar_get(self, u'Date.Expires')
+        return _scalar_get(self, 'Date.Expires')
 
-    modified = DateProperty(u'Date.Modified')
+    modified = DateProperty('Date.Modified')
 
     def ModificationDate(self):
         """See `IZopeDublinCore`"""
-        return _scalar_get(self, u'Date.Modified')
+        return _scalar_get(self, 'Date.Modified')
 
-    type = ScalarProperty(u'Type')
+    type = ScalarProperty('Type')
 
     def Type(self):
         """See `IZopeDublinCore`"""
         return self.type
 
-    format = ScalarProperty(u'Format')
+    format = ScalarProperty('Format')
 
     def Format(self):
         """See `IZopeDublinCore`"""
         return self.format
 
-    identifier = ScalarProperty(u'Identifier')
+    identifier = ScalarProperty('Identifier')
 
     def Identifier(self):
         """See `IZopeDublinCore`"""
         return self.identifier
 
-    language = ScalarProperty(u'Language')
+    language = ScalarProperty('Language')
 
     def Language(self):
         """See `IZopeDublinCore`"""
         return self.language
 
-    rights = ScalarProperty(u'Rights')
+    rights = ScalarProperty('Rights')
 
     def Rights(self):
         """See `IZopeDublinCore`"""
         return self.rights
 
     def setQualifiedTitles(self, qualified_titles):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Title', qualified_titles)
+        return _set_qualified(self, 'Title', qualified_titles)
 
     def setQualifiedCreators(self, qualified_creators):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Creator', qualified_creators)
+        return _set_qualified(self, 'Creator', qualified_creators)
 
     def setQualifiedSubjects(self, qualified_subjects):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Subject', qualified_subjects)
+        return _set_qualified(self, 'Subject', qualified_subjects)
 
     def setQualifiedDescriptions(self, qualified_descriptions):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Description', qualified_descriptions)
+        return _set_qualified(self, 'Description', qualified_descriptions)
 
     def setQualifiedPublishers(self, qualified_publishers):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Publisher', qualified_publishers)
+        return _set_qualified(self, 'Publisher', qualified_publishers)
 
     def setQualifiedContributors(self, qualified_contributors):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Contributor', qualified_contributors)
+        return _set_qualified(self, 'Contributor', qualified_contributors)
 
     def setQualifiedDates(self, qualified_dates):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Date', qualified_dates)
+        return _set_qualified(self, 'Date', qualified_dates)
 
     def setQualifiedTypes(self, qualified_types):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Type', qualified_types)
+        return _set_qualified(self, 'Type', qualified_types)
 
     def setQualifiedFormats(self, qualified_formats):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Format', qualified_formats)
+        return _set_qualified(self, 'Format', qualified_formats)
 
     def setQualifiedIdentifiers(self, qualified_identifiers):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Identifier', qualified_identifiers)
+        return _set_qualified(self, 'Identifier', qualified_identifiers)
 
     def setQualifiedSources(self, qualified_sources):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Source', qualified_sources)
+        return _set_qualified(self, 'Source', qualified_sources)
 
     def setQualifiedLanguages(self, qualified_languages):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Language', qualified_languages)
+        return _set_qualified(self, 'Language', qualified_languages)
 
     def setQualifiedRelations(self, qualified_relations):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Relation', qualified_relations)
+        return _set_qualified(self, 'Relation', qualified_relations)
 
     def setQualifiedCoverages(self, qualified_coverages):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Coverage', qualified_coverages)
+        return _set_qualified(self, 'Coverage', qualified_coverages)
 
     def setQualifiedRights(self, qualified_rights):
         """See `IWritableDublinCore`"""
-        return _set_qualified(self, u'Rights', qualified_rights)
+        return _set_qualified(self, 'Rights', qualified_rights)
 
     def getQualifiedTitles(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Title')
+        return _get_qualified(self, 'Title')
 
     def getQualifiedCreators(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Creator')
+        return _get_qualified(self, 'Creator')
 
     def getQualifiedSubjects(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Subject')
+        return _get_qualified(self, 'Subject')
 
     def getQualifiedDescriptions(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Description')
+        return _get_qualified(self, 'Description')
 
     def getQualifiedPublishers(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Publisher')
+        return _get_qualified(self, 'Publisher')
 
     def getQualifiedContributors(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Contributor')
+        return _get_qualified(self, 'Contributor')
 
     def getQualifiedDates(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Date')
+        return _get_qualified(self, 'Date')
 
     def getQualifiedTypes(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Type')
+        return _get_qualified(self, 'Type')
 
     def getQualifiedFormats(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Format')
+        return _get_qualified(self, 'Format')
 
     def getQualifiedIdentifiers(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Identifier')
+        return _get_qualified(self, 'Identifier')
 
     def getQualifiedSources(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Source')
+        return _get_qualified(self, 'Source')
 
     def getQualifiedLanguages(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Language')
+        return _get_qualified(self, 'Language')
 
     def getQualifiedRelations(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Relation')
+        return _get_qualified(self, 'Relation')
 
     def getQualifiedCoverages(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Coverage')
+        return _get_qualified(self, 'Coverage')
 
     def getQualifiedRights(self):
         """See `IStandardDublinCore`"""
-        return _get_qualified(self, u'Rights')
+        return _get_qualified(self, 'Rights')
 
 
 def _set_qualified(self, name, qvalue):
     data = {}
     dict = self._mapping
 
     for qualification, value in qvalue:
         data[qualification] = data.get(qualification, ()) + (value, )
 
     self._changed()
-    for qualification, values in six.iteritems(data):
+    for qualification, values in data.items():
         qname = qualification and (name + '.' + qualification) or name
         dict[qname] = values
 
 
 def _get_qualified(self, name):
     result = []
-    for aname, avalue in six.iteritems(self._mapping):
+    for aname, avalue in self._mapping.items():
 
         if aname == name:
-            qualification = u''
+            qualification = ''
             for value in avalue:
                 result.append((qualification, value))
 
         elif aname.startswith(name):
             qualification = aname[len(name) + 1:]
             for value in avalue:
                 result.append((qualification, value))
```

### Comparing `zope.dublincore-4.3.0/src/zope.dublincore.egg-info/SOURCES.txt` & `zope.dublincore-5.0/src/zope.dublincore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-.coveragerc
-.travis.yml
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 rtd.txt
 setup.cfg
```

