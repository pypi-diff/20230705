# Comparing `tmp/ai-aside-2.0.1.tar.gz` & `tmp/ai-aside-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-aside-2.0.1.tar", last modified: Thu Jun 29 16:16:40 2023, max compression
+gzip compressed data, was "ai-aside-2.0.2.tar", last modified: Wed Jul  5 13:47:52 2023, max compression
```

## Comparing `ai-aside-2.0.1.tar` & `ai-aside-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-29 16:16:35.000000 ai-aside-2.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-29 16:16:35.000000 ai-aside-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-29 16:16:35.000000 ai-aside-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7691 2023-06-29 16:16:40.246649 ai-aside-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-06-29 16:16:35.000000 ai-aside-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/summaryhook_aside/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7691 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-06-29 16:16:35.000000 ai-aside-2.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-29 16:16:35.000000 ai-aside-2.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-29 16:16:40.246649 ai-aside-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5399 2023-06-29 16:16:35.000000 ai-aside-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-29 16:16:35.000000 ai-aside-2.0.1/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-07-05 13:47:44.000000 ai-aside-2.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-05 13:47:44.000000 ai-aside-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-05 13:47:44.000000 ai-aside-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-07-05 13:47:52.948860 ai-aside-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-07-05 13:47:44.000000 ai-aside-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/ai_aside/summaryhook_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-05 13:47:44.000000 ai-aside-2.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-05 13:47:44.000000 ai-aside-2.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-05 13:47:52.948860 ai-aside-2.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5399 2023-07-05 13:47:44.000000 ai-aside-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-05 13:47:44.000000 ai-aside-2.0.2/tests/test_placeholder.py
```

### Comparing `ai-aside-2.0.1/CHANGELOG.rst` & `ai-aside-2.0.2/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -23,46 +23,58 @@
 00000160: 3a2f 2f73 656d 7665 722e 6f72 672f 292e  ://semver.org/).
 00000170: 0a0a 2e2e 2054 6865 7265 2073 686f 756c  .... There shoul
 00000180: 6420 616c 7761 7973 2062 6520 616e 2022  d always be an "
 00000190: 556e 7265 6c65 6173 6564 2220 7365 6374  Unreleased" sect
 000001a0: 696f 6e20 666f 7220 6368 616e 6765 7320  ion for changes 
 000001b0: 7065 6e64 696e 6720 7265 6c65 6173 652e  pending release.
 000001c0: 0a0a 556e 7265 6c65 6173 6564 0a2a 2a2a  ..Unreleased.***
-000001d0: 2a2a 2a2a 2a2a 2a0a 0a32 2e30 2e31 20e2  *******..2.0.1 .
-000001e0: 8093 2032 3032 332d 3036 2d32 390a 2a2a  .. 2023-06-29.**
+000001d0: 2a2a 2a2a 2a2a 2a0a 0a32 2e30 2e32 20e2  *******..2.0.2 .
+000001e0: 8093 2032 3032 332d 3037 2d30 350a 2a2a  .. 2023-07-05.**
 000001f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00000200: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00000210: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 4669  ************..Fi
-00000220: 780a 3d3d 3d3d 3d0a 0a2a 2046 6978 2074  x.=====..* Fix t
-00000230: 7261 6e73 6372 6970 7420 666f 726d 6174  ranscript format
-00000240: 2072 6571 7565 7374 2061 6e64 2063 6f6e   request and con
-00000250: 7665 7273 696f 6e0a 0a0a 322e 302e 3020  version...2.0.0 
-00000260: e280 9320 3230 3233 2d30 362d 3238 0a2a  ... 2023-06-28.*
-00000270: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000280: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000290: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 0a41  *************..A
-000002a0: 6464 6564 0a3d 3d3d 3d3d 0a0a 2a20 4164  dded.=====..* Ad
-000002b0: 6473 2061 2068 616e 646c 6572 2065 6e64  ds a handler end
-000002c0: 706f 696e 7420 746f 2070 726f 7669 6465  point to provide
-000002d0: 2073 756d 6d61 7269 7a61 626c 6520 636f   summarizable co
-000002e0: 6e74 656e 740a 2a20 496d 7072 6f76 6573  ntent.* Improves
-000002f0: 2063 6f6e 7465 6e74 206c 656e 6774 6820   content length 
-00000300: 6368 6563 6b69 6e67 2075 7369 6e67 2074  checking using t
-00000310: 6861 7420 7375 6d6d 6172 697a 6162 6c65  hat summarizable
-00000320: 2063 6f6e 7465 6e74 0a0a 0a31 2e32 2e31   content...1.2.1
-00000330: 20e2 8093 2032 3032 332d 3035 2d31 390a   ... 2023-05-19.
+00000220: 780a 3d3d 3d3d 3d0a 0a2a 2055 7064 6174  x.=====..* Updat
+00000230: 6564 2048 544d 4c20 7061 7273 6572 2074  ed HTML parser t
+00000240: 6f20 7265 6d6f 7665 2074 6167 7320 7769  o remove tags wi
+00000250: 7468 2074 6865 6972 2063 6f6e 7465 6e74  th their content
+00000260: 2066 6f72 2073 7065 6369 6669 6320 6361   for specific ca
+00000270: 7365 7320 6c69 6b65 2060 3c73 6372 6970  ses like `<scrip
+00000280: 743e 6020 6f72 2060 3c73 7479 6c65 3e60  t>` or `<style>`
+00000290: 2e0a 0a0a 322e 302e 3120 e280 9320 3230  ....2.0.1 ... 20
+000002a0: 3233 2d30 362d 3239 0a2a 2a2a 2a2a 2a2a  23-06-29.*******
+000002b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000002c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000002d0: 2a2a 2a2a 2a2a 2a0a 0a46 6978 0a3d 3d3d  *******..Fix.===
+000002e0: 3d3d 0a0a 2a20 4669 7820 7472 616e 7363  ==..* Fix transc
+000002f0: 7269 7074 2066 6f72 6d61 7420 7265 7175  ript format requ
+00000300: 6573 7420 616e 6420 636f 6e76 6572 7369  est and conversi
+00000310: 6f6e 0a0a 0a32 2e30 2e30 20e2 8093 2032  on...2.0.0 ... 2
+00000320: 3032 332d 3036 2d32 380a 2a2a 2a2a 2a2a  023-06-28.******
+00000330: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00000340: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000350: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000360: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a  **************..
-00000370: 4669 7865 730a 3d3d 3d3d 3d0a 0a2a 2046  Fixes.=====..* F
-00000380: 6978 2073 756d 6d61 7279 2d61 7369 6465  ix summary-aside
-00000390: 2073 6574 7469 6e67 7320 7061 636b 6167   settings packag
-000003a0: 650a 0a31 2e32 2e30 20e2 8093 2032 3032  e..1.2.0 ... 202
-000003b0: 332d 3035 2d31 310a 2a2a 2a2a 2a2a 2a2a  3-05-11.********
-000003c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000003d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000003e0: 2a2a 2a2a 2a2a 0a0a 4164 6465 640a 3d3d  ******..Added.==
-000003f0: 3d3d 3d0a 0a2a 2050 6f72 7469 6e67 206f  ===..* Porting o
-00000400: 7665 7220 7375 6d6d 6172 792d 6173 6964  ver summary-asid
-00000410: 6520 6672 6f6d 2065 6478 2d61 7263 682d  e from edx-arch-
-00000420: 6578 7065 7269 6d65 6e74 7320 7665 7273  experiments vers
-00000430: 696f 6e20 312e 322e 300a                 ion 1.2.0.
+00000350: 2a2a 2a2a 2a2a 2a2a 0a0a 4164 6465 640a  ********..Added.
+00000360: 3d3d 3d3d 3d0a 0a2a 2041 6464 7320 6120  =====..* Adds a 
+00000370: 6861 6e64 6c65 7220 656e 6470 6f69 6e74  handler endpoint
+00000380: 2074 6f20 7072 6f76 6964 6520 7375 6d6d   to provide summ
+00000390: 6172 697a 6162 6c65 2063 6f6e 7465 6e74  arizable content
+000003a0: 0a2a 2049 6d70 726f 7665 7320 636f 6e74  .* Improves cont
+000003b0: 656e 7420 6c65 6e67 7468 2063 6865 636b  ent length check
+000003c0: 696e 6720 7573 696e 6720 7468 6174 2073  ing using that s
+000003d0: 756d 6d61 7269 7a61 626c 6520 636f 6e74  ummarizable cont
+000003e0: 656e 740a 0a0a 312e 322e 3120 e280 9320  ent...1.2.1 ... 
+000003f0: 3230 3233 2d30 352d 3139 0a2a 2a2a 2a2a  2023-05-19.*****
+00000400: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000410: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000420: 2a2a 2a2a 2a2a 2a2a 2a0a 0a46 6978 6573  *********..Fixes
+00000430: 0a3d 3d3d 3d3d 0a0a 2a20 4669 7820 7375  .=====..* Fix su
+00000440: 6d6d 6172 792d 6173 6964 6520 7365 7474  mmary-aside sett
+00000450: 696e 6773 2070 6163 6b61 6765 0a0a 312e  ings package..1.
+00000460: 322e 3020 e280 9320 3230 3233 2d30 352d  2.0 ... 2023-05-
+00000470: 3131 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  11.*************
+00000480: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000490: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000004a0: 2a0a 0a41 6464 6564 0a3d 3d3d 3d3d 0a0a  *..Added.=====..
+000004b0: 2a20 506f 7274 696e 6720 6f76 6572 2073  * Porting over s
+000004c0: 756d 6d61 7279 2d61 7369 6465 2066 726f  ummary-aside fro
+000004d0: 6d20 6564 782d 6172 6368 2d65 7870 6572  m edx-arch-exper
+000004e0: 696d 656e 7473 2076 6572 7369 6f6e 2031  iments version 1
+000004f0: 2e32 2e30 0a                             .2.0.
```

### Comparing `ai-aside-2.0.1/LICENSE.txt` & `ai-aside-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/PKG-INFO` & `ai-aside-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.1
+Version: 2.0.2
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -196,14 +196,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+2.0.2 – 2023-07-05
+**********************************************
+
+Fix
+=====
+
+* Updated HTML parser to remove tags with their content for specific cases like `<script>` or `<style>`.
+
+
 2.0.1 – 2023-06-29
 **********************************************
 
 Fix
 =====
 
 * Fix transcript format request and conversion
```

### Comparing `ai-aside-2.0.1/README.rst` & `ai-aside-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside/apps.py` & `ai-aside-2.0.2/ai_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside/summaryhook_aside/apps.py` & `ai-aside-2.0.2/ai_aside/summaryhook_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside/summaryhook_aside/block.py` & `ai-aside-2.0.2/ai_aside/summaryhook_aside/block.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/devstack.py` & `ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside/summaryhook_aside/text_utils.py` & `ai-aside-2.0.2/ai_aside/summaryhook_aside/text_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Text manipulation utils.
 """
 
 from html.parser import HTMLParser
 from re import sub
 
+from django.conf import settings
+
 
 def cleanup_text(text):
     """
     Removes litter from replacing or manipulating text
     """
     stripped = sub(r'[^\S\r\n]+', ' ', text)  # Removing extra spaces
     stripped = sub(r'\n{2,}', '\n', stripped)  # Removing extra new lines
@@ -18,27 +20,35 @@
     return stripped
 
 
 class _HTMLToTextHelper(HTMLParser):  # lint-amnesty, pylint: disable=abstract-method
     """
     Helper function for html_to_text below
     """
+    _is_content = True
 
     def __init__(self):
         HTMLParser.__init__(self)
         self.reset()
         self.fed = []
 
+    def handle_starttag(self, tag, _):
+        """This runs when a new tag is found. We use this to exclude unwanted content."""
+        tags_to_filter = getattr(settings, 'HTML_TAGS_TO_REMOVE', None)
+        self._is_content = not (tags_to_filter and tag in tags_to_filter)
+
     def handle_data(self, data):
         """takes the data in separate chunks"""
-        self.fed.append(data)
+        if self._is_content:
+            self.fed.append(data)
 
     def handle_entityref(self, name):
         """appends the reference to the body"""
-        self.fed.append('&%s;' % name)
+        if self._is_content:
+            self.fed.append('&%s;' % name)
 
     def get_data(self):
         """joins together the seperate chunks into one cohesive string"""
         return ''.join(self.fed)
 
 
 def html_to_text(html):
```

### Comparing `ai-aside-2.0.1/ai_aside/summaryhook_aside/waffle.py` & `ai-aside-2.0.2/ai_aside/summaryhook_aside/waffle.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/ai_aside.egg-info/PKG-INFO` & `ai-aside-2.0.2/ai_aside.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.1
+Version: 2.0.2
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -196,14 +196,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+2.0.2 – 2023-07-05
+**********************************************
+
+Fix
+=====
+
+* Updated HTML parser to remove tags with their content for specific cases like `<script>` or `<style>`.
+
+
 2.0.1 – 2023-06-29
 **********************************************
 
 Fix
 =====
 
 * Fix transcript format request and conversion
```

### Comparing `ai-aside-2.0.1/ai_aside.egg-info/SOURCES.txt` & `ai-aside-2.0.2/ai_aside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/requirements/constraints.txt` & `ai-aside-2.0.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.1/setup.py` & `ai-aside-2.0.2/setup.py`

 * *Files identical despite different names*

