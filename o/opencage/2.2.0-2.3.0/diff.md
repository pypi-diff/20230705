# Comparing `tmp/opencage-2.2.0.tar.gz` & `tmp/opencage-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mtm/dev/python-opencage-geocoder/dist/.tmp-r7fz0q9o/opencage-2.2.0.tar", last modified: Fri May  5 17:01:55 2023, max compression
+gzip compressed data, was "/home/vagrant/python-opencage-geocoder/dist/.tmp-h3h6njyo/opencage-2.3.0.tar", last modified: Tue Jul  4 22:15:04 2023, max compression
```

## Comparing `opencage-2.2.0.tar` & `opencage-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-05 17:01:55.789261 opencage-2.2.0/
--rw-r--r--   0 mtm        (501) staff       (20)     1513 2021-03-13 15:19:05.000000 opencage-2.2.0/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     5662 2023-05-05 17:01:55.789027 opencage-2.2.0/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     4604 2023-05-05 16:51:36.000000 opencage-2.2.0/README.md
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-05 17:01:55.780561 opencage-2.2.0/opencage/
--rw-r--r--   0 mtm        (501) staff       (20)      128 2021-03-13 15:18:50.000000 opencage-2.2.0/opencage/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)    11160 2023-05-05 16:29:01.000000 opencage-2.2.0/opencage/geocoder.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-05 17:01:55.782898 opencage-2.2.0/opencage.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     5662 2023-05-05 17:01:55.000000 opencage-2.2.0/opencage.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      542 2023-05-05 17:01:55.000000 opencage-2.2.0/opencage.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-05 17:01:55.000000 opencage-2.2.0/opencage.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2021-07-14 23:40:07.000000 opencage-2.2.0/opencage.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-05-05 17:01:55.000000 opencage-2.2.0/opencage.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       14 2023-05-05 17:01:55.000000 opencage-2.2.0/opencage.egg-info/top_level.txt
--rw-r--r--   0 mtm        (501) staff       (20)       38 2023-05-05 17:01:55.789335 opencage-2.2.0/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     2138 2023-05-05 16:56:23.000000 opencage-2.2.0/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-05 17:01:55.788572 opencage-2.2.0/test/
--rw-r--r--   0 mtm        (501) staff       (20)       34 2021-07-14 22:29:28.000000 opencage-2.2.0/test/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     2086 2023-05-05 16:29:01.000000 opencage-2.2.0/test/test_all.py
--rw-r--r--   0 mtm        (501) staff       (20)     1528 2023-01-07 15:46:16.000000 opencage-2.2.0/test/test_async.py
--rw-r--r--   0 mtm        (501) staff       (20)      675 2023-01-07 15:46:16.000000 opencage-2.2.0/test/test_error_blocked.py
--rw-r--r--   0 mtm        (501) staff       (20)     1096 2023-01-07 15:46:16.000000 opencage-2.2.0/test/test_error_invalid_input.py
--rw-r--r--   0 mtm        (501) staff       (20)      672 2023-01-07 15:46:16.000000 opencage-2.2.0/test/test_error_not_authorized.py
--rw-r--r--   0 mtm        (501) staff       (20)     1306 2023-01-16 20:52:14.000000 opencage-2.2.0/test/test_error_ratelimit_exceeded.py
--rw-r--r--   0 mtm        (501) staff       (20)     1314 2023-01-16 20:52:14.000000 opencage-2.2.0/test/test_error_unknown.py
--rw-r--r--   0 mtm        (501) staff       (20)      870 2021-07-14 22:29:28.000000 opencage-2.2.0/test/test_flotify_dict.py
--rw-r--r--   0 mtm        (501) staff       (20)      771 2021-07-14 22:29:28.000000 opencage-2.2.0/test/test_reverse.py
--rw-r--r--   0 mtm        (501) staff       (20)     1347 2023-01-16 20:52:14.000000 opencage-2.2.0/test/test_session.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-04 22:15:08.000000 opencage-2.3.0/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1513 2021-03-13 15:19:05.000000 opencage-2.3.0/LICENSE.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5706 2023-07-04 22:15:08.000000 opencage-2.3.0/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4648 2023-06-18 20:36:27.000000 opencage-2.3.0/README.md
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      131 2023-07-04 22:14:36.000000 opencage-2.3.0/opencage/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11160 2023-05-05 16:29:01.000000 opencage-2.3.0/opencage/geocoder.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5706 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      572 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2021-07-14 23:40:07.000000 opencage-2.3.0/opencage.egg-info/not-zip-safe
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       32 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2023-07-04 22:15:08.000000 opencage-2.3.0/opencage.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-07-04 22:15:08.000000 opencage-2.3.0/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2140 2023-07-04 22:14:36.000000 opencage-2.3.0/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-04 22:15:08.000000 opencage-2.3.0/test/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       34 2021-07-14 22:29:28.000000 opencage-2.3.0/test/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1931 2023-06-18 20:36:27.000000 opencage-2.3.0/test/test_all.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1528 2023-01-07 15:46:16.000000 opencage-2.3.0/test/test_async.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      675 2023-01-07 15:46:16.000000 opencage-2.3.0/test/test_error_blocked.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1096 2023-01-07 15:46:16.000000 opencage-2.3.0/test/test_error_invalid_input.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      672 2023-01-07 15:46:16.000000 opencage-2.3.0/test/test_error_not_authorized.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1306 2023-01-16 20:52:14.000000 opencage-2.3.0/test/test_error_ratelimit_exceeded.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1314 2023-01-16 20:52:14.000000 opencage-2.3.0/test/test_error_unknown.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      870 2021-07-14 22:29:28.000000 opencage-2.3.0/test/test_flotify_dict.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      771 2021-07-14 22:29:28.000000 opencage-2.3.0/test/test_reverse.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1347 2023-01-16 20:52:14.000000 opencage-2.3.0/test/test_session.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      211 2023-06-18 20:36:27.000000 opencage-2.3.0/test/test_setting_protocol.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `opencage-2.2.0/LICENSE.txt` & `opencage-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/PKG-INFO` & `opencage-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Wrapper module for the OpenCage Geocoder API
 Home-page: https://github.com/OpenCageData/python-opencage-geocoder/
 Download-URL: https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0
 Author: OpenCage GmbH
 Author-email: info@opencagedata.com
 License: BSD
 Keywords: geocoding,geocoder
@@ -20,26 +20,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-
 # OpenCage Geocoding Module for Python
 
 A Python module to access the [OpenCage Geocoding API](https://opencagedata.com/).
 
 ## Build Status / Code Quality / etc
 
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/py/opencage)
 [![Downloads](https://pepy.tech/badge/opencage/month)](https://pepy.tech/project/opencage)
 [![Versions](https://img.shields.io/pypi/pyversions/opencage)](https://pypi.org/project/opencage/)
 ![GitHub contributors](https://img.shields.io/github/contributors/opencagedata/python-opencage-geocoder)
-[![Build Status](https://travis-ci.com/OpenCageData/python-opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/python-opencage-geocoder)
+[![Build Status](https://github.com/OpenCageData/python-opencage-geocoder/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/OpenCageData/python-opencage-geocoder/actions/workflows/build.yml)
 ![Mastodon Follow](https://img.shields.io/mastodon/follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social)
 
 ## Tutorial
 
 You can find a [comprehensive tutorial for using this module on the OpenCage site](https://opencagedata.com/tutorials/geocode-in-python).
 
 ## Usage
@@ -83,18 +82,17 @@
 
 ```python
 results = geocoder.geocode('London', proximity='42.828576, -81.406643')
 print(results[0]['formatted'])
 # u'London, ON N6A 3M8, Canada'
 ```
 
-
 ### Reverse geocoding
 
-Turn a lat/long into an address with the ``reverse_geocode`` method:
+Turn a lat/long into an address with the `reverse_geocode` method:
 
 ```python
 result = geocoder.reverse_geocode(51.51024, -0.10303)
 ```
 
 ### Sessions
 
@@ -139,27 +137,26 @@
 
 <img src="batch-progress.gif"/>
 
 ### Exceptions
 
 If anything goes wrong, then an exception will be raised:
 
- * `InvalidInputError` for non-unicode query strings
- * `NotAuthorizedError` if API key is missing, invalid syntax or disabled
- * `ForbiddenError` API key is blocked or suspended
- * `RateLimitExceededError` if you go past your rate limit
- * `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
-
+- `InvalidInputError` for non-unicode query strings
+- `NotAuthorizedError` if API key is missing, invalid syntax or disabled
+- `ForbiddenError` API key is blocked or suspended
+- `RateLimitExceededError` if you go past your rate limit
+- `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
 
 ## Copyright & License
 
 This software is copyright OpenCage GmbH.
 Please see `LICENSE.txt`
 
 ### Who is OpenCage GmbH?
 
 <a href="https://opencagedata.com"><img src="opencage_logo_300_150.png"/></a>
 
-We run a worldwide [geocoding API](https://opencagedata.com/api) and [geosearch](https://opencagedata.com/geosearch) service based on open data. 
-Learn more [about us](https://opencagedata.com/about). 
+We run a worldwide [geocoding API](https://opencagedata.com/api) and [geosearch](https://opencagedata.com/geosearch) service based on open data.
+Learn more [about us](https://opencagedata.com/about).
 
 We also run [Geomob](https://thegeomob.com), a series of regular meetups for location based service creators, where we do our best to highlight geoinnovation. If you like geo stuff, you will probably enjoy [the Geomob podcast](https://thegeomob.com/podcast/).
```

### Comparing `opencage-2.2.0/README.md` & `opencage-2.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,288 +1,291 @@
-00000000: 0a23 204f 7065 6e43 6167 6520 4765 6f63  .# OpenCage Geoc
-00000010: 6f64 696e 6720 4d6f 6475 6c65 2066 6f72  oding Module for
-00000020: 2050 7974 686f 6e0a 0a41 2050 7974 686f   Python..A Pytho
-00000030: 6e20 6d6f 6475 6c65 2074 6f20 6163 6365  n module to acce
-00000040: 7373 2074 6865 205b 4f70 656e 4361 6765  ss the [OpenCage
-00000050: 2047 656f 636f 6469 6e67 2041 5049 5d28   Geocoding API](
-00000060: 6874 7470 733a 2f2f 6f70 656e 6361 6765  https://opencage
-00000070: 6461 7461 2e63 6f6d 2f29 2e0a 0a23 2320  data.com/)...## 
-00000080: 4275 696c 6420 5374 6174 7573 202f 2043  Build Status / C
-00000090: 6f64 6520 5175 616c 6974 7920 2f20 6574  ode Quality / et
-000000a0: 630a 0a5b 215b 5079 5049 2076 6572 7369  c..[![PyPI versi
-000000b0: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-000000c0: 652e 6675 7279 2e69 6f2f 7079 2f6f 7065  e.fury.io/py/ope
-000000d0: 6e63 6167 652e 7376 6729 5d28 6874 7470  ncage.svg)](http
-000000e0: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
-000000f0: 6f2f 7079 2f6f 7065 6e63 6167 6529 0a5b  o/py/opencage).[
-00000100: 215b 446f 776e 6c6f 6164 735d 2868 7474  ![Downloads](htt
-00000110: 7073 3a2f 2f70 6570 792e 7465 6368 2f62  ps://pepy.tech/b
-00000120: 6164 6765 2f6f 7065 6e63 6167 652f 6d6f  adge/opencage/mo
-00000130: 6e74 6829 5d28 6874 7470 733a 2f2f 7065  nth)](https://pe
-00000140: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-00000150: 6f70 656e 6361 6765 290a 5b21 5b56 6572  opencage).[![Ver
-00000160: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00000170: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000180: 7069 2f70 7976 6572 7369 6f6e 732f 6f70  pi/pyversions/op
-00000190: 656e 6361 6765 295d 2868 7474 7073 3a2f  encage)](https:/
-000001a0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000001b0: 742f 6f70 656e 6361 6765 2f29 0a21 5b47  t/opencage/).![G
-000001c0: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-000001d0: 7273 5d28 6874 7470 733a 2f2f 696d 672e  rs](https://img.
-000001e0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000001f0: 622f 636f 6e74 7269 6275 746f 7273 2f6f  b/contributors/o
-00000200: 7065 6e63 6167 6564 6174 612f 7079 7468  pencagedata/pyth
-00000210: 6f6e 2d6f 7065 6e63 6167 652d 6765 6f63  on-opencage-geoc
-00000220: 6f64 6572 290a 5b21 5b42 7569 6c64 2053  oder).[![Build S
-00000230: 7461 7475 735d 2868 7474 7073 3a2f 2f74  tatus](https://t
-00000240: 7261 7669 732d 6369 2e63 6f6d 2f4f 7065  ravis-ci.com/Ope
-00000250: 6e43 6167 6544 6174 612f 7079 7468 6f6e  nCageData/python
-00000260: 2d6f 7065 6e63 6167 652d 6765 6f63 6f64  -opencage-geocod
-00000270: 6572 2e73 7667 3f62 7261 6e63 683d 6d61  er.svg?branch=ma
-00000280: 7374 6572 295d 2868 7474 7073 3a2f 2f74  ster)](https://t
-00000290: 7261 7669 732d 6369 2e63 6f6d 2f4f 7065  ravis-ci.com/Ope
-000002a0: 6e43 6167 6544 6174 612f 7079 7468 6f6e  nCageData/python
-000002b0: 2d6f 7065 6e63 6167 652d 6765 6f63 6f64  -opencage-geocod
-000002c0: 6572 290a 215b 4d61 7374 6f64 6f6e 2046  er).![Mastodon F
-000002d0: 6f6c 6c6f 775d 2868 7474 7073 3a2f 2f69  ollow](https://i
-000002e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6d61  mg.shields.io/ma
-000002f0: 7374 6f64 6f6e 2f66 6f6c 6c6f 772f 3130  stodon/follow/10
-00000300: 3932 3837 3636 3334 3638 3530 3137 3639  9287663468501769
-00000310: 3f64 6f6d 6169 6e3d 6874 7470 7325 3341  ?domain=https%3A
-00000320: 2532 4625 3246 656e 2e6f 736d 2e74 6f77  %2F%2Fen.osm.tow
-00000330: 6e25 3246 2673 7479 6c65 3d73 6f63 6961  n%2F&style=socia
-00000340: 6c29 0a0a 2323 2054 7574 6f72 6961 6c0a  l)..## Tutorial.
-00000350: 0a59 6f75 2063 616e 2066 696e 6420 6120  .You can find a 
-00000360: 5b63 6f6d 7072 6568 656e 7369 7665 2074  [comprehensive t
-00000370: 7574 6f72 6961 6c20 666f 7220 7573 696e  utorial for usin
-00000380: 6720 7468 6973 206d 6f64 756c 6520 6f6e  g this module on
-00000390: 2074 6865 204f 7065 6e43 6167 6520 7369   the OpenCage si
-000003a0: 7465 5d28 6874 7470 733a 2f2f 6f70 656e  te](https://open
-000003b0: 6361 6765 6461 7461 2e63 6f6d 2f74 7574  cagedata.com/tut
-000003c0: 6f72 6961 6c73 2f67 656f 636f 6465 2d69  orials/geocode-i
-000003d0: 6e2d 7079 7468 6f6e 292e 0a0a 2323 2055  n-python)...## U
-000003e0: 7361 6765 0a0a 5375 7070 6f72 7473 2050  sage..Supports P
-000003f0: 7974 686f 6e20 332e 3720 6f72 206e 6577  ython 3.7 or new
-00000400: 6572 2e20 5573 6520 7468 6520 6f6c 6465  er. Use the olde
-00000410: 7220 6f70 656e 6361 6765 2031 2e78 2072  r opencage 1.x r
-00000420: 656c 6561 7365 7320 6966 2079 6f75 206e  eleases if you n
-00000430: 6565 6420 5079 7468 6f6e 2032 2e37 2073  eed Python 2.7 s
-00000440: 7570 706f 7274 2e0a 0a49 6e73 7461 6c6c  upport...Install
-00000450: 2074 6865 206d 6f64 756c 653a 0a0a 6060   the module:..``
-00000460: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
-00000470: 6c20 6f70 656e 6361 6765 0a60 6060 0a0a  l opencage.```..
-00000480: 4c6f 6164 2074 6865 206d 6f64 756c 653a  Load the module:
-00000490: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000004a0: 206f 7065 6e63 6167 652e 6765 6f63 6f64   opencage.geocod
-000004b0: 6572 2069 6d70 6f72 7420 4f70 656e 4361  er import OpenCa
-000004c0: 6765 4765 6f63 6f64 650a 6060 600a 0a43  geGeocode.```..C
-000004d0: 7265 6174 6520 616e 2069 6e73 7461 6e63  reate an instanc
-000004e0: 6520 6f66 2074 6865 2067 656f 636f 6465  e of the geocode
-000004f0: 7220 6d6f 6475 6c65 2c20 7061 7373 696e  r module, passin
-00000500: 6720 6120 7661 6c69 6420 4f70 656e 4361  g a valid OpenCa
-00000510: 6765 2044 6174 6120 4765 6f63 6f64 6572  ge Data Geocoder
-00000520: 2041 5049 206b 6579 0a61 7320 6120 7061   API key.as a pa
-00000530: 7261 6d65 7465 7220 746f 2074 6865 2067  rameter to the g
-00000540: 656f 636f 6465 7220 6d6f 6475 6c65 7327  eocoder modules'
-00000550: 7320 636f 6e73 7472 7563 746f 723a 0a0a  s constructor:..
-00000560: 6060 6070 7974 686f 6e0a 6b65 7920 3d20  ```python.key = 
-00000570: 2779 6f75 722d 6170 692d 6b65 792d 6865  'your-api-key-he
-00000580: 7265 270a 6765 6f63 6f64 6572 203d 204f  re'.geocoder = O
-00000590: 7065 6e43 6167 6547 656f 636f 6465 286b  penCageGeocode(k
-000005a0: 6579 290a 6060 600a 0a50 6173 7320 6120  ey).```..Pass a 
-000005b0: 7374 7269 6e67 2063 6f6e 7461 696e 696e  string containin
-000005c0: 6720 7468 6520 7175 6572 7920 6f72 2061  g the query or a
-000005d0: 6464 7265 7373 2074 6f20 6265 2067 656f  ddress to be geo
-000005e0: 636f 6465 6420 746f 2074 6865 206d 6f64  coded to the mod
-000005f0: 756c 6573 2720 6067 656f 636f 6465 6020  ules' `geocode` 
-00000600: 6d65 7468 6f64 3a0a 0a60 6060 7079 7468  method:..```pyth
-00000610: 6f6e 0a71 7565 7279 203d 2027 3832 2043  on.query = '82 C
-00000620: 6c65 726b 656e 7765 6c6c 2052 6f61 642c  lerkenwell Road,
-00000630: 204c 6f6e 646f 6e27 0a72 6573 756c 7473   London'.results
-00000640: 203d 2067 656f 636f 6465 722e 6765 6f63   = geocoder.geoc
-00000650: 6f64 6528 7175 6572 7929 0a60 6060 0a0a  ode(query).```..
-00000660: 596f 7520 6361 6e20 6164 6420 5b61 6464  You can add [add
-00000670: 6974 696f 6e61 6c20 7061 7261 6d65 7465  itional paramete
-00000680: 7273 5d28 6874 7470 733a 2f2f 6f70 656e  rs](https://open
-00000690: 6361 6765 6461 7461 2e63 6f6d 2f61 7069  cagedata.com/api
-000006a0: 2366 6f72 7761 7264 2d6f 7074 293a 0a0a  #forward-opt):..
-000006b0: 6060 6070 7974 686f 6e0a 7265 7375 6c74  ```python.result
-000006c0: 7320 3d20 6765 6f63 6f64 6572 2e67 656f  s = geocoder.geo
-000006d0: 636f 6465 2827 4c6f 6e64 6f6e 272c 206e  code('London', n
-000006e0: 6f5f 616e 6e6f 7461 7469 6f6e 733d 312c  o_annotations=1,
-000006f0: 206c 616e 6775 6167 653d 2765 7327 290a   language='es').
-00000700: 6060 600a 0a46 6f72 2065 7861 6d70 6c65  ```..For example
-00000710: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000720: 2070 726f 7869 6d69 7479 2070 6172 616d   proximity param
-00000730: 6574 6572 2074 6f20 7072 6f76 6964 6520  eter to provide 
-00000740: 7468 6520 6765 6f63 6f64 6572 2077 6974  the geocoder wit
-00000750: 6820 6120 6869 6e74 3a0a 0a60 6060 7079  h a hint:..```py
-00000760: 7468 6f6e 0a72 6573 756c 7473 203d 2067  thon.results = g
-00000770: 656f 636f 6465 722e 6765 6f63 6f64 6528  eocoder.geocode(
-00000780: 274c 6f6e 646f 6e27 2c20 7072 6f78 696d  'London', proxim
-00000790: 6974 793d 2734 322e 3832 3835 3736 2c20  ity='42.828576, 
-000007a0: 2d38 312e 3430 3636 3433 2729 0a70 7269  -81.406643').pri
-000007b0: 6e74 2872 6573 756c 7473 5b30 5d5b 2766  nt(results[0]['f
-000007c0: 6f72 6d61 7474 6564 275d 290a 2320 7527  ormatted']).# u'
-000007d0: 4c6f 6e64 6f6e 2c20 4f4e 204e 3641 2033  London, ON N6A 3
-000007e0: 4d38 2c20 4361 6e61 6461 270a 6060 600a  M8, Canada'.```.
-000007f0: 0a0a 2323 2320 5265 7665 7273 6520 6765  ..### Reverse ge
-00000800: 6f63 6f64 696e 670a 0a54 7572 6e20 6120  ocoding..Turn a 
-00000810: 6c61 742f 6c6f 6e67 2069 6e74 6f20 616e  lat/long into an
-00000820: 2061 6464 7265 7373 2077 6974 6820 7468   address with th
-00000830: 6520 6060 7265 7665 7273 655f 6765 6f63  e ``reverse_geoc
-00000840: 6f64 6560 6020 6d65 7468 6f64 3a0a 0a60  ode`` method:..`
-00000850: 6060 7079 7468 6f6e 0a72 6573 756c 7420  ``python.result 
-00000860: 3d20 6765 6f63 6f64 6572 2e72 6576 6572  = geocoder.rever
-00000870: 7365 5f67 656f 636f 6465 2835 312e 3531  se_geocode(51.51
-00000880: 3032 342c 202d 302e 3130 3330 3329 0a60  024, -0.10303).`
-00000890: 6060 0a0a 2323 2320 5365 7373 696f 6e73  ``..### Sessions
-000008a0: 0a0a 596f 7520 6361 6e20 7265 7573 6520  ..You can reuse 
-000008b0: 796f 7572 2048 5454 5020 636f 6e6e 6563  your HTTP connec
-000008c0: 7469 6f6e 2066 6f72 206d 756c 7469 706c  tion for multipl
-000008d0: 6520 7265 7175 6573 7473 2062 790a 7573  e requests by.us
-000008e0: 696e 6720 6120 6077 6974 6860 2062 6c6f  ing a `with` blo
-000008f0: 636b 2e20 5468 6973 2063 616e 2068 656c  ck. This can hel
-00000900: 7020 7065 7266 6f72 6d61 6e63 6520 7768  p performance wh
-00000910: 656e 206d 616b 696e 670a 6120 6c6f 7420  en making.a lot 
-00000920: 6f66 2072 6571 7565 7374 733a 0a0a 6060  of requests:..``
-00000930: 6070 7974 686f 6e0a 7175 6572 6965 7320  `python.queries 
-00000940: 3d20 5b27 3832 2043 6c65 726b 656e 7765  = ['82 Clerkenwe
-00000950: 6c6c 2052 6f61 642c 204c 6f6e 646f 6e27  ll Road, London'
-00000960: 2c20 2e2e 2e5d 0a77 6974 6820 4f70 656e  , ...].with Open
-00000970: 4361 6765 4765 6f63 6f64 6528 6b65 7929  CageGeocode(key)
-00000980: 2061 7320 6765 6f63 6f64 6572 3a0a 2020   as geocoder:.  
-00000990: 2020 2320 5175 6572 6965 7320 7265 7573    # Queries reus
-000009a0: 6520 7468 6520 7361 6d65 2048 5454 5020  e the same HTTP 
-000009b0: 636f 6e6e 6563 7469 6f6e 0a20 2020 2072  connection.    r
-000009c0: 6573 756c 7473 203d 205b 6765 6f63 6f64  esults = [geocod
-000009d0: 6572 2e67 656f 636f 6465 2871 7565 7279  er.geocode(query
-000009e0: 2920 666f 7220 7175 6572 7920 696e 2071  ) for query in q
-000009f0: 7565 7269 6573 5d0a 6060 600a 0a23 2323  ueries].```..###
-00000a00: 2041 7379 6e63 726f 6e6f 7573 2072 6571   Asyncronous req
-00000a10: 7565 7374 730a 0a59 6f75 2063 616e 2072  uests..You can r
-00000a20: 756e 2072 6571 7565 7374 7320 696e 2070  un requests in p
-00000a30: 6172 616c 6c65 6c20 7769 7468 2074 6865  arallel with the
-00000a40: 2060 6765 6f63 6f64 655f 6173 796e 6360   `geocode_async`
-00000a50: 2061 6e64 2060 7265 7665 7273 655f 6765   and `reverse_ge
-00000a60: 6f63 6f64 655f 6173 796e 6360 0a6d 6574  ocode_async`.met
-00000a70: 686f 6420 7768 6963 6820 6861 7665 2074  hod which have t
-00000a80: 6865 2073 616d 6520 7061 7261 6d65 7465  he same paramete
-00000a90: 7273 2061 6e64 2072 6573 706f 6e73 6520  rs and response 
-00000aa0: 6173 2074 6865 6972 2073 796e 726f 6e6f  as their synrono
-00000ab0: 7573 2063 6f75 6e74 6572 7061 7274 732e  us counterparts.
-00000ac0: 0a59 6f75 2077 696c 6c20 6e65 6564 2061  .You will need a
-00000ad0: 7420 6c65 6173 7420 5079 7468 6f6e 2033  t least Python 3
-00000ae0: 2e37 2061 6e64 2074 6865 2060 6173 796e  .7 and the `asyn
-00000af0: 6369 6f60 2061 6e64 2060 6169 6f68 7474  cio` and `aiohtt
-00000b00: 7060 2070 6163 6b61 6765 7320 696e 7374  p` packages inst
-00000b10: 616c 6c65 642e 0a0a 6060 6070 7974 686f  alled...```pytho
-00000b20: 6e0a 6173 796e 6320 7769 7468 204f 7065  n.async with Ope
-00000b30: 6e43 6167 6547 656f 636f 6465 286b 6579  nCageGeocode(key
-00000b40: 2920 6173 2067 656f 636f 6465 723a 0a20  ) as geocoder:. 
-00000b50: 2020 2072 6573 756c 7473 203d 2061 7761     results = awa
-00000b60: 6974 2067 656f 636f 6465 722e 6765 6f63  it geocoder.geoc
-00000b70: 6f64 655f 6173 796e 6328 6164 6472 6573  ode_async(addres
-00000b80: 7329 0a60 6060 0a0a 466f 7220 6120 6d6f  s).```..For a mo
-00000b90: 7265 2063 6f6d 706c 6574 6520 6578 616d  re complete exam
-00000ba0: 706c 6520 616e 6420 6c69 6e6b 7320 746f  ple and links to
-00000bb0: 2066 7574 6865 7220 7475 746f 7269 616c   futher tutorial
-00000bc0: 7320 6f6e 2061 7379 6e63 726f 6e6f 7573  s on asyncronous
-00000bd0: 2049 4f20 7365 650a 6062 6174 6368 2e70   IO see.`batch.p
-00000be0: 7960 2069 6e20 7468 6520 6065 7861 6d70  y` in the `examp
-00000bf0: 6c65 7360 2064 6972 6563 746f 7279 2e0a  les` directory..
-00000c00: 0a23 2323 204e 6f6e 2d53 534c 2041 5049  .### Non-SSL API
-00000c10: 2075 7365 0a0a 4966 2079 6f75 2068 6176   use..If you hav
-00000c20: 6520 7472 6f75 626c 6520 6163 6365 7369  e trouble accesi
-00000c30: 6e67 2074 6865 204f 7065 6e43 6167 6520  ng the OpenCage 
-00000c40: 4150 4920 7769 7468 2068 7474 7073 2c20  API with https, 
-00000c50: 652e 672e 2069 7373 7565 7320 7769 7468  e.g. issues with
-00000c60: 204f 7065 6e53 534c 0a6c 6962 7261 7269   OpenSSL.librari
-00000c70: 6573 2069 6e20 796f 7572 2065 6e76 6972  es in your envir
-00000c80: 6f6d 656e 742c 2074 6865 6e20 796f 7520  oment, then you 
-00000c90: 6361 6e20 7365 7420 7468 6520 2768 7474  can set the 'htt
-00000ca0: 7027 2070 726f 746f 636f 6c20 696e 7374  p' protocol inst
-00000cb0: 6561 642e 2050 6c65 6173 650a 756e 6465  ead. Please.unde
-00000cc0: 7273 7461 6e64 2074 6861 7420 7468 6520  rstand that the 
-00000cd0: 636f 6e6e 6563 7469 6f6e 2074 6f20 7468  connection to th
-00000ce0: 6520 4f70 656e 4361 6765 2041 5049 2077  e OpenCage API w
-00000cf0: 696c 6c20 6e6f 206c 6f6e 6765 7220 6265  ill no longer be
-00000d00: 2065 6e63 7279 7074 6564 2e0a 0a60 6060   encrypted...```
-00000d10: 7079 7468 6f6e 0a67 656f 636f 6465 7220  python.geocoder 
-00000d20: 3d20 4f70 656e 4361 6765 4765 6f63 6f64  = OpenCageGeocod
-00000d30: 6528 2779 6f75 722d 6170 692d 6b65 7927  e('your-api-key'
-00000d40: 2c20 2768 7474 7027 290a 6060 600a 0a23  , 'http').```..#
-00000d50: 2323 2043 6f6d 6d61 6e64 2d6c 696e 6520  ## Command-line 
-00000d60: 6261 7463 6820 6765 6f63 6f64 696e 670a  batch geocoding.
-00000d70: 0a53 6565 2060 6578 616d 706c 6573 2f62  .See `examples/b
-00000d80: 6174 6368 2e70 7960 2066 6f72 2061 6e20  atch.py` for an 
-00000d90: 6578 616d 706c 6520 746f 2067 656f 636f  example to geoco
-00000da0: 6465 2061 2043 5356 2066 696c 652e 0a0a  de a CSV file...
-00000db0: 3c69 6d67 2073 7263 3d22 6261 7463 682d  <img src="batch-
-00000dc0: 7072 6f67 7265 7373 2e67 6966 222f 3e0a  progress.gif"/>.
-00000dd0: 0a23 2323 2045 7863 6570 7469 6f6e 730a  .### Exceptions.
-00000de0: 0a49 6620 616e 7974 6869 6e67 2067 6f65  .If anything goe
-00000df0: 7320 7772 6f6e 672c 2074 6865 6e20 616e  s wrong, then an
-00000e00: 2065 7863 6570 7469 6f6e 2077 696c 6c20   exception will 
-00000e10: 6265 2072 6169 7365 643a 0a0a 202a 2060  be raised:.. * `
-00000e20: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
-00000e30: 7260 2066 6f72 206e 6f6e 2d75 6e69 636f  r` for non-unico
-00000e40: 6465 2071 7565 7279 2073 7472 696e 6773  de query strings
-00000e50: 0a20 2a20 604e 6f74 4175 7468 6f72 697a  . * `NotAuthoriz
-00000e60: 6564 4572 726f 7260 2069 6620 4150 4920  edError` if API 
-00000e70: 6b65 7920 6973 206d 6973 7369 6e67 2c20  key is missing, 
-00000e80: 696e 7661 6c69 6420 7379 6e74 6178 206f  invalid syntax o
-00000e90: 7220 6469 7361 626c 6564 0a20 2a20 6046  r disabled. * `F
-00000ea0: 6f72 6269 6464 656e 4572 726f 7260 2041  orbiddenError` A
-00000eb0: 5049 206b 6579 2069 7320 626c 6f63 6b65  PI key is blocke
-00000ec0: 6420 6f72 2073 7573 7065 6e64 6564 0a20  d or suspended. 
-00000ed0: 2a20 6052 6174 654c 696d 6974 4578 6365  * `RateLimitExce
-00000ee0: 6564 6564 4572 726f 7260 2069 6620 796f  ededError` if yo
-00000ef0: 7520 676f 2070 6173 7420 796f 7572 2072  u go past your r
-00000f00: 6174 6520 6c69 6d69 740a 202a 2060 556e  ate limit. * `Un
-00000f10: 6b6e 6f77 6e45 7272 6f72 6020 6966 2074  knownError` if t
-00000f20: 6865 7265 2773 2073 6f6d 6520 7072 6f62  here's some prob
-00000f30: 6c65 6d20 7769 7468 2074 6865 2041 5049  lem with the API
-00000f40: 2028 6261 6420 7265 7375 6c74 732c 2035   (bad results, 5
-00000f50: 3030 2073 7461 7475 7320 636f 6465 2c20  00 status code, 
-00000f60: 6574 6329 0a0a 0a23 2320 436f 7079 7269  etc)...## Copyri
-00000f70: 6768 7420 2620 4c69 6365 6e73 650a 0a54  ght & License..T
-00000f80: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
-00000f90: 636f 7079 7269 6768 7420 4f70 656e 4361  copyright OpenCa
-00000fa0: 6765 2047 6d62 482e 0a50 6c65 6173 6520  ge GmbH..Please 
-00000fb0: 7365 6520 604c 4943 454e 5345 2e74 7874  see `LICENSE.txt
-00000fc0: 600a 0a23 2323 2057 686f 2069 7320 4f70  `..### Who is Op
-00000fd0: 656e 4361 6765 2047 6d62 483f 0a0a 3c61  enCage GmbH?..<a
-00000fe0: 2068 7265 663d 2268 7474 7073 3a2f 2f6f   href="https://o
-00000ff0: 7065 6e63 6167 6564 6174 612e 636f 6d22  pencagedata.com"
-00001000: 3e3c 696d 6720 7372 633d 226f 7065 6e63  ><img src="openc
-00001010: 6167 655f 6c6f 676f 5f33 3030 5f31 3530  age_logo_300_150
-00001020: 2e70 6e67 222f 3e3c 2f61 3e0a 0a57 6520  .png"/></a>..We 
-00001030: 7275 6e20 6120 776f 726c 6477 6964 6520  run a worldwide 
-00001040: 5b67 656f 636f 6469 6e67 2041 5049 5d28  [geocoding API](
-00001050: 6874 7470 733a 2f2f 6f70 656e 6361 6765  https://opencage
-00001060: 6461 7461 2e63 6f6d 2f61 7069 2920 616e  data.com/api) an
-00001070: 6420 5b67 656f 7365 6172 6368 5d28 6874  d [geosearch](ht
+00000000: 2320 4f70 656e 4361 6765 2047 656f 636f  # OpenCage Geoco
+00000010: 6469 6e67 204d 6f64 756c 6520 666f 7220  ding Module for 
+00000020: 5079 7468 6f6e 0a0a 4120 5079 7468 6f6e  Python..A Python
+00000030: 206d 6f64 756c 6520 746f 2061 6363 6573   module to acces
+00000040: 7320 7468 6520 5b4f 7065 6e43 6167 6520  s the [OpenCage 
+00000050: 4765 6f63 6f64 696e 6720 4150 495d 2868  Geocoding API](h
+00000060: 7474 7073 3a2f 2f6f 7065 6e63 6167 6564  ttps://opencaged
+00000070: 6174 612e 636f 6d2f 292e 0a0a 2323 2042  ata.com/)...## B
+00000080: 7569 6c64 2053 7461 7475 7320 2f20 436f  uild Status / Co
+00000090: 6465 2051 7561 6c69 7479 202f 2065 7463  de Quality / etc
+000000a0: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
+000000b0: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+000000c0: 2e66 7572 792e 696f 2f70 792f 6f70 656e  .fury.io/py/open
+000000d0: 6361 6765 2e73 7667 295d 2868 7474 7073  cage.svg)](https
+000000e0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+000000f0: 2f70 792f 6f70 656e 6361 6765 290a 5b21  /py/opencage).[!
+00000100: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+00000110: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+00000120: 6467 652f 6f70 656e 6361 6765 2f6d 6f6e  dge/opencage/mon
+00000130: 7468 295d 2868 7474 7073 3a2f 2f70 6570  th)](https://pep
+00000140: 792e 7465 6368 2f70 726f 6a65 6374 2f6f  y.tech/project/o
+00000150: 7065 6e63 6167 6529 0a5b 215b 5665 7273  pencage).[![Vers
+00000160: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
+00000170: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000180: 692f 7079 7665 7273 696f 6e73 2f6f 7065  i/pyversions/ope
+00000190: 6e63 6167 6529 5d28 6874 7470 733a 2f2f  ncage)](https://
+000001a0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000001b0: 2f6f 7065 6e63 6167 652f 290a 215b 4769  /opencage/).![Gi
+000001c0: 7448 7562 2063 6f6e 7472 6962 7574 6f72  tHub contributor
+000001d0: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+000001e0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000001f0: 2f63 6f6e 7472 6962 7574 6f72 732f 6f70  /contributors/op
+00000200: 656e 6361 6765 6461 7461 2f70 7974 686f  encagedata/pytho
+00000210: 6e2d 6f70 656e 6361 6765 2d67 656f 636f  n-opencage-geoco
+00000220: 6465 7229 0a5b 215b 4275 696c 6420 5374  der).[![Build St
+00000230: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
+00000240: 7468 7562 2e63 6f6d 2f4f 7065 6e43 6167  thub.com/OpenCag
+00000250: 6544 6174 612f 7079 7468 6f6e 2d6f 7065  eData/python-ope
+00000260: 6e63 6167 652d 6765 6f63 6f64 6572 2f61  ncage-geocoder/a
+00000270: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000280: 2f62 7569 6c64 2e79 6d6c 2f62 6164 6765  /build.yml/badge
+00000290: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+000002a0: 6572 295d 2868 7474 7073 3a2f 2f67 6974  er)](https://git
+000002b0: 6875 622e 636f 6d2f 4f70 656e 4361 6765  hub.com/OpenCage
+000002c0: 4461 7461 2f70 7974 686f 6e2d 6f70 656e  Data/python-open
+000002d0: 6361 6765 2d67 656f 636f 6465 722f 6163  cage-geocoder/ac
+000002e0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000002f0: 6275 696c 642e 796d 6c29 0a21 5b4d 6173  build.yml).![Mas
+00000300: 746f 646f 6e20 466f 6c6c 6f77 5d28 6874  todon Follow](ht
+00000310: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000320: 732e 696f 2f6d 6173 746f 646f 6e2f 666f  s.io/mastodon/fo
+00000330: 6c6c 6f77 2f31 3039 3238 3736 3633 3436  llow/10928766346
+00000340: 3835 3031 3736 393f 646f 6d61 696e 3d68  8501769?domain=h
+00000350: 7474 7073 2533 4125 3246 2532 4665 6e2e  ttps%3A%2F%2Fen.
+00000360: 6f73 6d2e 746f 776e 2532 4626 7374 796c  osm.town%2F&styl
+00000370: 653d 736f 6369 616c 290a 0a23 2320 5475  e=social)..## Tu
+00000380: 746f 7269 616c 0a0a 596f 7520 6361 6e20  torial..You can 
+00000390: 6669 6e64 2061 205b 636f 6d70 7265 6865  find a [comprehe
+000003a0: 6e73 6976 6520 7475 746f 7269 616c 2066  nsive tutorial f
+000003b0: 6f72 2075 7369 6e67 2074 6869 7320 6d6f  or using this mo
+000003c0: 6475 6c65 206f 6e20 7468 6520 4f70 656e  dule on the Open
+000003d0: 4361 6765 2073 6974 655d 2868 7474 7073  Cage site](https
+000003e0: 3a2f 2f6f 7065 6e63 6167 6564 6174 612e  ://opencagedata.
+000003f0: 636f 6d2f 7475 746f 7269 616c 732f 6765  com/tutorials/ge
+00000400: 6f63 6f64 652d 696e 2d70 7974 686f 6e29  ocode-in-python)
+00000410: 2e0a 0a23 2320 5573 6167 650a 0a53 7570  ...## Usage..Sup
+00000420: 706f 7274 7320 5079 7468 6f6e 2033 2e37  ports Python 3.7
+00000430: 206f 7220 6e65 7765 722e 2055 7365 2074   or newer. Use t
+00000440: 6865 206f 6c64 6572 206f 7065 6e63 6167  he older opencag
+00000450: 6520 312e 7820 7265 6c65 6173 6573 2069  e 1.x releases i
+00000460: 6620 796f 7520 6e65 6564 2050 7974 686f  f you need Pytho
+00000470: 6e20 322e 3720 7375 7070 6f72 742e 0a0a  n 2.7 support...
+00000480: 496e 7374 616c 6c20 7468 6520 6d6f 6475  Install the modu
+00000490: 6c65 3a0a 0a60 6060 6261 7368 0a70 6970  le:..```bash.pip
+000004a0: 2069 6e73 7461 6c6c 206f 7065 6e63 6167   install opencag
+000004b0: 650a 6060 600a 0a4c 6f61 6420 7468 6520  e.```..Load the 
+000004c0: 6d6f 6475 6c65 3a0a 0a60 6060 7079 7468  module:..```pyth
+000004d0: 6f6e 0a66 726f 6d20 6f70 656e 6361 6765  on.from opencage
+000004e0: 2e67 656f 636f 6465 7220 696d 706f 7274  .geocoder import
+000004f0: 204f 7065 6e43 6167 6547 656f 636f 6465   OpenCageGeocode
+00000500: 0a60 6060 0a0a 4372 6561 7465 2061 6e20  .```..Create an 
+00000510: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+00000520: 6765 6f63 6f64 6572 206d 6f64 756c 652c  geocoder module,
+00000530: 2070 6173 7369 6e67 2061 2076 616c 6964   passing a valid
+00000540: 204f 7065 6e43 6167 6520 4461 7461 2047   OpenCage Data G
+00000550: 656f 636f 6465 7220 4150 4920 6b65 790a  eocoder API key.
+00000560: 6173 2061 2070 6172 616d 6574 6572 2074  as a parameter t
+00000570: 6f20 7468 6520 6765 6f63 6f64 6572 206d  o the geocoder m
+00000580: 6f64 756c 6573 2773 2063 6f6e 7374 7275  odules's constru
+00000590: 6374 6f72 3a0a 0a60 6060 7079 7468 6f6e  ctor:..```python
+000005a0: 0a6b 6579 203d 2027 796f 7572 2d61 7069  .key = 'your-api
+000005b0: 2d6b 6579 2d68 6572 6527 0a67 656f 636f  -key-here'.geoco
+000005c0: 6465 7220 3d20 4f70 656e 4361 6765 4765  der = OpenCageGe
+000005d0: 6f63 6f64 6528 6b65 7929 0a60 6060 0a0a  ocode(key).```..
+000005e0: 5061 7373 2061 2073 7472 696e 6720 636f  Pass a string co
+000005f0: 6e74 6169 6e69 6e67 2074 6865 2071 7565  ntaining the que
+00000600: 7279 206f 7220 6164 6472 6573 7320 746f  ry or address to
+00000610: 2062 6520 6765 6f63 6f64 6564 2074 6f20   be geocoded to 
+00000620: 7468 6520 6d6f 6475 6c65 7327 2060 6765  the modules' `ge
+00000630: 6f63 6f64 6560 206d 6574 686f 643a 0a0a  ocode` method:..
+00000640: 6060 6070 7974 686f 6e0a 7175 6572 7920  ```python.query 
+00000650: 3d20 2738 3220 436c 6572 6b65 6e77 656c  = '82 Clerkenwel
+00000660: 6c20 526f 6164 2c20 4c6f 6e64 6f6e 270a  l Road, London'.
+00000670: 7265 7375 6c74 7320 3d20 6765 6f63 6f64  results = geocod
+00000680: 6572 2e67 656f 636f 6465 2871 7565 7279  er.geocode(query
+00000690: 290a 6060 600a 0a59 6f75 2063 616e 2061  ).```..You can a
+000006a0: 6464 205b 6164 6469 7469 6f6e 616c 2070  dd [additional p
+000006b0: 6172 616d 6574 6572 735d 2868 7474 7073  arameters](https
+000006c0: 3a2f 2f6f 7065 6e63 6167 6564 6174 612e  ://opencagedata.
+000006d0: 636f 6d2f 6170 6923 666f 7277 6172 642d  com/api#forward-
+000006e0: 6f70 7429 3a0a 0a60 6060 7079 7468 6f6e  opt):..```python
+000006f0: 0a72 6573 756c 7473 203d 2067 656f 636f  .results = geoco
+00000700: 6465 722e 6765 6f63 6f64 6528 274c 6f6e  der.geocode('Lon
+00000710: 646f 6e27 2c20 6e6f 5f61 6e6e 6f74 6174  don', no_annotat
+00000720: 696f 6e73 3d31 2c20 6c61 6e67 7561 6765  ions=1, language
+00000730: 3d27 6573 2729 0a60 6060 0a0a 466f 7220  ='es').```..For 
+00000740: 6578 616d 706c 6520 796f 7520 6361 6e20  example you can 
+00000750: 7573 6520 7468 6520 7072 6f78 696d 6974  use the proximit
+00000760: 7920 7061 7261 6d65 7465 7220 746f 2070  y parameter to p
+00000770: 726f 7669 6465 2074 6865 2067 656f 636f  rovide the geoco
+00000780: 6465 7220 7769 7468 2061 2068 696e 743a  der with a hint:
+00000790: 0a0a 6060 6070 7974 686f 6e0a 7265 7375  ..```python.resu
+000007a0: 6c74 7320 3d20 6765 6f63 6f64 6572 2e67  lts = geocoder.g
+000007b0: 656f 636f 6465 2827 4c6f 6e64 6f6e 272c  eocode('London',
+000007c0: 2070 726f 7869 6d69 7479 3d27 3432 2e38   proximity='42.8
+000007d0: 3238 3537 362c 202d 3831 2e34 3036 3634  28576, -81.40664
+000007e0: 3327 290a 7072 696e 7428 7265 7375 6c74  3').print(result
+000007f0: 735b 305d 5b27 666f 726d 6174 7465 6427  s[0]['formatted'
+00000800: 5d29 0a23 2075 274c 6f6e 646f 6e2c 204f  ]).# u'London, O
+00000810: 4e20 4e36 4120 334d 382c 2043 616e 6164  N N6A 3M8, Canad
+00000820: 6127 0a60 6060 0a0a 2323 2320 5265 7665  a'.```..### Reve
+00000830: 7273 6520 6765 6f63 6f64 696e 670a 0a54  rse geocoding..T
+00000840: 7572 6e20 6120 6c61 742f 6c6f 6e67 2069  urn a lat/long i
+00000850: 6e74 6f20 616e 2061 6464 7265 7373 2077  nto an address w
+00000860: 6974 6820 7468 6520 6072 6576 6572 7365  ith the `reverse
+00000870: 5f67 656f 636f 6465 6020 6d65 7468 6f64  _geocode` method
+00000880: 3a0a 0a60 6060 7079 7468 6f6e 0a72 6573  :..```python.res
+00000890: 756c 7420 3d20 6765 6f63 6f64 6572 2e72  ult = geocoder.r
+000008a0: 6576 6572 7365 5f67 656f 636f 6465 2835  everse_geocode(5
+000008b0: 312e 3531 3032 342c 202d 302e 3130 3330  1.51024, -0.1030
+000008c0: 3329 0a60 6060 0a0a 2323 2320 5365 7373  3).```..### Sess
+000008d0: 696f 6e73 0a0a 596f 7520 6361 6e20 7265  ions..You can re
+000008e0: 7573 6520 796f 7572 2048 5454 5020 636f  use your HTTP co
+000008f0: 6e6e 6563 7469 6f6e 2066 6f72 206d 756c  nnection for mul
+00000900: 7469 706c 6520 7265 7175 6573 7473 2062  tiple requests b
+00000910: 790a 7573 696e 6720 6120 6077 6974 6860  y.using a `with`
+00000920: 2062 6c6f 636b 2e20 5468 6973 2063 616e   block. This can
+00000930: 2068 656c 7020 7065 7266 6f72 6d61 6e63   help performanc
+00000940: 6520 7768 656e 206d 616b 696e 670a 6120  e when making.a 
+00000950: 6c6f 7420 6f66 2072 6571 7565 7374 733a  lot of requests:
+00000960: 0a0a 6060 6070 7974 686f 6e0a 7175 6572  ..```python.quer
+00000970: 6965 7320 3d20 5b27 3832 2043 6c65 726b  ies = ['82 Clerk
+00000980: 656e 7765 6c6c 2052 6f61 642c 204c 6f6e  enwell Road, Lon
+00000990: 646f 6e27 2c20 2e2e 2e5d 0a77 6974 6820  don', ...].with 
+000009a0: 4f70 656e 4361 6765 4765 6f63 6f64 6528  OpenCageGeocode(
+000009b0: 6b65 7929 2061 7320 6765 6f63 6f64 6572  key) as geocoder
+000009c0: 3a0a 2020 2020 2320 5175 6572 6965 7320  :.    # Queries 
+000009d0: 7265 7573 6520 7468 6520 7361 6d65 2048  reuse the same H
+000009e0: 5454 5020 636f 6e6e 6563 7469 6f6e 0a20  TTP connection. 
+000009f0: 2020 2072 6573 756c 7473 203d 205b 6765     results = [ge
+00000a00: 6f63 6f64 6572 2e67 656f 636f 6465 2871  ocoder.geocode(q
+00000a10: 7565 7279 2920 666f 7220 7175 6572 7920  uery) for query 
+00000a20: 696e 2071 7565 7269 6573 5d0a 6060 600a  in queries].```.
+00000a30: 0a23 2323 2041 7379 6e63 726f 6e6f 7573  .### Asyncronous
+00000a40: 2072 6571 7565 7374 730a 0a59 6f75 2063   requests..You c
+00000a50: 616e 2072 756e 2072 6571 7565 7374 7320  an run requests 
+00000a60: 696e 2070 6172 616c 6c65 6c20 7769 7468  in parallel with
+00000a70: 2074 6865 2060 6765 6f63 6f64 655f 6173   the `geocode_as
+00000a80: 796e 6360 2061 6e64 2060 7265 7665 7273  ync` and `revers
+00000a90: 655f 6765 6f63 6f64 655f 6173 796e 6360  e_geocode_async`
+00000aa0: 0a6d 6574 686f 6420 7768 6963 6820 6861  .method which ha
+00000ab0: 7665 2074 6865 2073 616d 6520 7061 7261  ve the same para
+00000ac0: 6d65 7465 7273 2061 6e64 2072 6573 706f  meters and respo
+00000ad0: 6e73 6520 6173 2074 6865 6972 2073 796e  nse as their syn
+00000ae0: 726f 6e6f 7573 2063 6f75 6e74 6572 7061  ronous counterpa
+00000af0: 7274 732e 0a59 6f75 2077 696c 6c20 6e65  rts..You will ne
+00000b00: 6564 2061 7420 6c65 6173 7420 5079 7468  ed at least Pyth
+00000b10: 6f6e 2033 2e37 2061 6e64 2074 6865 2060  on 3.7 and the `
+00000b20: 6173 796e 6369 6f60 2061 6e64 2060 6169  asyncio` and `ai
+00000b30: 6f68 7474 7060 2070 6163 6b61 6765 7320  ohttp` packages 
+00000b40: 696e 7374 616c 6c65 642e 0a0a 6060 6070  installed...```p
+00000b50: 7974 686f 6e0a 6173 796e 6320 7769 7468  ython.async with
+00000b60: 204f 7065 6e43 6167 6547 656f 636f 6465   OpenCageGeocode
+00000b70: 286b 6579 2920 6173 2067 656f 636f 6465  (key) as geocode
+00000b80: 723a 0a20 2020 2072 6573 756c 7473 203d  r:.    results =
+00000b90: 2061 7761 6974 2067 656f 636f 6465 722e   await geocoder.
+00000ba0: 6765 6f63 6f64 655f 6173 796e 6328 6164  geocode_async(ad
+00000bb0: 6472 6573 7329 0a60 6060 0a0a 466f 7220  dress).```..For 
+00000bc0: 6120 6d6f 7265 2063 6f6d 706c 6574 6520  a more complete 
+00000bd0: 6578 616d 706c 6520 616e 6420 6c69 6e6b  example and link
+00000be0: 7320 746f 2066 7574 6865 7220 7475 746f  s to futher tuto
+00000bf0: 7269 616c 7320 6f6e 2061 7379 6e63 726f  rials on asyncro
+00000c00: 6e6f 7573 2049 4f20 7365 650a 6062 6174  nous IO see.`bat
+00000c10: 6368 2e70 7960 2069 6e20 7468 6520 6065  ch.py` in the `e
+00000c20: 7861 6d70 6c65 7360 2064 6972 6563 746f  xamples` directo
+00000c30: 7279 2e0a 0a23 2323 204e 6f6e 2d53 534c  ry...### Non-SSL
+00000c40: 2041 5049 2075 7365 0a0a 4966 2079 6f75   API use..If you
+00000c50: 2068 6176 6520 7472 6f75 626c 6520 6163   have trouble ac
+00000c60: 6365 7369 6e67 2074 6865 204f 7065 6e43  cesing the OpenC
+00000c70: 6167 6520 4150 4920 7769 7468 2068 7474  age API with htt
+00000c80: 7073 2c20 652e 672e 2069 7373 7565 7320  ps, e.g. issues 
+00000c90: 7769 7468 204f 7065 6e53 534c 0a6c 6962  with OpenSSL.lib
+00000ca0: 7261 7269 6573 2069 6e20 796f 7572 2065  raries in your e
+00000cb0: 6e76 6972 6f6d 656e 742c 2074 6865 6e20  nviroment, then 
+00000cc0: 796f 7520 6361 6e20 7365 7420 7468 6520  you can set the 
+00000cd0: 2768 7474 7027 2070 726f 746f 636f 6c20  'http' protocol 
+00000ce0: 696e 7374 6561 642e 2050 6c65 6173 650a  instead. Please.
+00000cf0: 756e 6465 7273 7461 6e64 2074 6861 7420  understand that 
+00000d00: 7468 6520 636f 6e6e 6563 7469 6f6e 2074  the connection t
+00000d10: 6f20 7468 6520 4f70 656e 4361 6765 2041  o the OpenCage A
+00000d20: 5049 2077 696c 6c20 6e6f 206c 6f6e 6765  PI will no longe
+00000d30: 7220 6265 2065 6e63 7279 7074 6564 2e0a  r be encrypted..
+00000d40: 0a60 6060 7079 7468 6f6e 0a67 656f 636f  .```python.geoco
+00000d50: 6465 7220 3d20 4f70 656e 4361 6765 4765  der = OpenCageGe
+00000d60: 6f63 6f64 6528 2779 6f75 722d 6170 692d  ocode('your-api-
+00000d70: 6b65 7927 2c20 2768 7474 7027 290a 6060  key', 'http').``
+00000d80: 600a 0a23 2323 2043 6f6d 6d61 6e64 2d6c  `..### Command-l
+00000d90: 696e 6520 6261 7463 6820 6765 6f63 6f64  ine batch geocod
+00000da0: 696e 670a 0a53 6565 2060 6578 616d 706c  ing..See `exampl
+00000db0: 6573 2f62 6174 6368 2e70 7960 2066 6f72  es/batch.py` for
+00000dc0: 2061 6e20 6578 616d 706c 6520 746f 2067   an example to g
+00000dd0: 656f 636f 6465 2061 2043 5356 2066 696c  eocode a CSV fil
+00000de0: 652e 0a0a 3c69 6d67 2073 7263 3d22 6261  e...<img src="ba
+00000df0: 7463 682d 7072 6f67 7265 7373 2e67 6966  tch-progress.gif
+00000e00: 222f 3e0a 0a23 2323 2045 7863 6570 7469  "/>..### Excepti
+00000e10: 6f6e 730a 0a49 6620 616e 7974 6869 6e67  ons..If anything
+00000e20: 2067 6f65 7320 7772 6f6e 672c 2074 6865   goes wrong, the
+00000e30: 6e20 616e 2065 7863 6570 7469 6f6e 2077  n an exception w
+00000e40: 696c 6c20 6265 2072 6169 7365 643a 0a0a  ill be raised:..
+00000e50: 2d20 6049 6e76 616c 6964 496e 7075 7445  - `InvalidInputE
+00000e60: 7272 6f72 6020 666f 7220 6e6f 6e2d 756e  rror` for non-un
+00000e70: 6963 6f64 6520 7175 6572 7920 7374 7269  icode query stri
+00000e80: 6e67 730a 2d20 604e 6f74 4175 7468 6f72  ngs.- `NotAuthor
+00000e90: 697a 6564 4572 726f 7260 2069 6620 4150  izedError` if AP
+00000ea0: 4920 6b65 7920 6973 206d 6973 7369 6e67  I key is missing
+00000eb0: 2c20 696e 7661 6c69 6420 7379 6e74 6178  , invalid syntax
+00000ec0: 206f 7220 6469 7361 626c 6564 0a2d 2060   or disabled.- `
+00000ed0: 466f 7262 6964 6465 6e45 7272 6f72 6020  ForbiddenError` 
+00000ee0: 4150 4920 6b65 7920 6973 2062 6c6f 636b  API key is block
+00000ef0: 6564 206f 7220 7375 7370 656e 6465 640a  ed or suspended.
+00000f00: 2d20 6052 6174 654c 696d 6974 4578 6365  - `RateLimitExce
+00000f10: 6564 6564 4572 726f 7260 2069 6620 796f  ededError` if yo
+00000f20: 7520 676f 2070 6173 7420 796f 7572 2072  u go past your r
+00000f30: 6174 6520 6c69 6d69 740a 2d20 6055 6e6b  ate limit.- `Unk
+00000f40: 6e6f 776e 4572 726f 7260 2069 6620 7468  nownError` if th
+00000f50: 6572 6527 7320 736f 6d65 2070 726f 626c  ere's some probl
+00000f60: 656d 2077 6974 6820 7468 6520 4150 4920  em with the API 
+00000f70: 2862 6164 2072 6573 756c 7473 2c20 3530  (bad results, 50
+00000f80: 3020 7374 6174 7573 2063 6f64 652c 2065  0 status code, e
+00000f90: 7463 290a 0a23 2320 436f 7079 7269 6768  tc)..## Copyrigh
+00000fa0: 7420 2620 4c69 6365 6e73 650a 0a54 6869  t & License..Thi
+00000fb0: 7320 736f 6674 7761 7265 2069 7320 636f  s software is co
+00000fc0: 7079 7269 6768 7420 4f70 656e 4361 6765  pyright OpenCage
+00000fd0: 2047 6d62 482e 0a50 6c65 6173 6520 7365   GmbH..Please se
+00000fe0: 6520 604c 4943 454e 5345 2e74 7874 600a  e `LICENSE.txt`.
+00000ff0: 0a23 2323 2057 686f 2069 7320 4f70 656e  .### Who is Open
+00001000: 4361 6765 2047 6d62 483f 0a0a 3c61 2068  Cage GmbH?..<a h
+00001010: 7265 663d 2268 7474 7073 3a2f 2f6f 7065  ref="https://ope
+00001020: 6e63 6167 6564 6174 612e 636f 6d22 3e3c  ncagedata.com"><
+00001030: 696d 6720 7372 633d 226f 7065 6e63 6167  img src="opencag
+00001040: 655f 6c6f 676f 5f33 3030 5f31 3530 2e70  e_logo_300_150.p
+00001050: 6e67 222f 3e3c 2f61 3e0a 0a57 6520 7275  ng"/></a>..We ru
+00001060: 6e20 6120 776f 726c 6477 6964 6520 5b67  n a worldwide [g
+00001070: 656f 636f 6469 6e67 2041 5049 5d28 6874  eocoding API](ht
 00001080: 7470 733a 2f2f 6f70 656e 6361 6765 6461  tps://opencageda
-00001090: 7461 2e63 6f6d 2f67 656f 7365 6172 6368  ta.com/geosearch
-000010a0: 2920 7365 7276 6963 6520 6261 7365 6420  ) service based 
-000010b0: 6f6e 206f 7065 6e20 6461 7461 2e20 0a4c  on open data. .L
-000010c0: 6561 726e 206d 6f72 6520 5b61 626f 7574  earn more [about
-000010d0: 2075 735d 2868 7474 7073 3a2f 2f6f 7065   us](https://ope
-000010e0: 6e63 6167 6564 6174 612e 636f 6d2f 6162  ncagedata.com/ab
-000010f0: 6f75 7429 2e20 0a0a 5765 2061 6c73 6f20  out). ..We also 
-00001100: 7275 6e20 5b47 656f 6d6f 625d 2868 7474  run [Geomob](htt
-00001110: 7073 3a2f 2f74 6865 6765 6f6d 6f62 2e63  ps://thegeomob.c
-00001120: 6f6d 292c 2061 2073 6572 6965 7320 6f66  om), a series of
-00001130: 2072 6567 756c 6172 206d 6565 7475 7073   regular meetups
-00001140: 2066 6f72 206c 6f63 6174 696f 6e20 6261   for location ba
-00001150: 7365 6420 7365 7276 6963 6520 6372 6561  sed service crea
-00001160: 746f 7273 2c20 7768 6572 6520 7765 2064  tors, where we d
-00001170: 6f20 6f75 7220 6265 7374 2074 6f20 6869  o our best to hi
-00001180: 6768 6c69 6768 7420 6765 6f69 6e6e 6f76  ghlight geoinnov
-00001190: 6174 696f 6e2e 2049 6620 796f 7520 6c69  ation. If you li
-000011a0: 6b65 2067 656f 2073 7475 6666 2c20 796f  ke geo stuff, yo
-000011b0: 7520 7769 6c6c 2070 726f 6261 626c 7920  u will probably 
-000011c0: 656e 6a6f 7920 5b74 6865 2047 656f 6d6f  enjoy [the Geomo
-000011d0: 6220 706f 6463 6173 745d 2868 7474 7073  b podcast](https
-000011e0: 3a2f 2f74 6865 6765 6f6d 6f62 2e63 6f6d  ://thegeomob.com
-000011f0: 2f70 6f64 6361 7374 2f29 2e0a            /podcast/)..
+00001090: 7461 2e63 6f6d 2f61 7069 2920 616e 6420  ta.com/api) and 
+000010a0: 5b67 656f 7365 6172 6368 5d28 6874 7470  [geosearch](http
+000010b0: 733a 2f2f 6f70 656e 6361 6765 6461 7461  s://opencagedata
+000010c0: 2e63 6f6d 2f67 656f 7365 6172 6368 2920  .com/geosearch) 
+000010d0: 7365 7276 6963 6520 6261 7365 6420 6f6e  service based on
+000010e0: 206f 7065 6e20 6461 7461 2e0a 4c65 6172   open data..Lear
+000010f0: 6e20 6d6f 7265 205b 6162 6f75 7420 7573  n more [about us
+00001100: 5d28 6874 7470 733a 2f2f 6f70 656e 6361  ](https://openca
+00001110: 6765 6461 7461 2e63 6f6d 2f61 626f 7574  gedata.com/about
+00001120: 292e 0a0a 5765 2061 6c73 6f20 7275 6e20  )...We also run 
+00001130: 5b47 656f 6d6f 625d 2868 7474 7073 3a2f  [Geomob](https:/
+00001140: 2f74 6865 6765 6f6d 6f62 2e63 6f6d 292c  /thegeomob.com),
+00001150: 2061 2073 6572 6965 7320 6f66 2072 6567   a series of reg
+00001160: 756c 6172 206d 6565 7475 7073 2066 6f72  ular meetups for
+00001170: 206c 6f63 6174 696f 6e20 6261 7365 6420   location based 
+00001180: 7365 7276 6963 6520 6372 6561 746f 7273  service creators
+00001190: 2c20 7768 6572 6520 7765 2064 6f20 6f75  , where we do ou
+000011a0: 7220 6265 7374 2074 6f20 6869 6768 6c69  r best to highli
+000011b0: 6768 7420 6765 6f69 6e6e 6f76 6174 696f  ght geoinnovatio
+000011c0: 6e2e 2049 6620 796f 7520 6c69 6b65 2067  n. If you like g
+000011d0: 656f 2073 7475 6666 2c20 796f 7520 7769  eo stuff, you wi
+000011e0: 6c6c 2070 726f 6261 626c 7920 656e 6a6f  ll probably enjo
+000011f0: 7920 5b74 6865 2047 656f 6d6f 6220 706f  y [the Geomob po
+00001200: 6463 6173 745d 2868 7474 7073 3a2f 2f74  dcast](https://t
+00001210: 6865 6765 6f6d 6f62 2e63 6f6d 2f70 6f64  hegeomob.com/pod
+00001220: 6361 7374 2f29 2e0a                      cast/)..
```

### Comparing `opencage-2.2.0/opencage/geocoder.py` & `opencage-2.3.0/opencage/geocoder.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/opencage.egg-info/PKG-INFO` & `opencage-2.3.0/opencage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Wrapper module for the OpenCage Geocoder API
 Home-page: https://github.com/OpenCageData/python-opencage-geocoder/
 Download-URL: https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0
 Author: OpenCage GmbH
 Author-email: info@opencagedata.com
 License: BSD
 Keywords: geocoding,geocoder
@@ -20,26 +20,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-
 # OpenCage Geocoding Module for Python
 
 A Python module to access the [OpenCage Geocoding API](https://opencagedata.com/).
 
 ## Build Status / Code Quality / etc
 
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/py/opencage)
 [![Downloads](https://pepy.tech/badge/opencage/month)](https://pepy.tech/project/opencage)
 [![Versions](https://img.shields.io/pypi/pyversions/opencage)](https://pypi.org/project/opencage/)
 ![GitHub contributors](https://img.shields.io/github/contributors/opencagedata/python-opencage-geocoder)
-[![Build Status](https://travis-ci.com/OpenCageData/python-opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/python-opencage-geocoder)
+[![Build Status](https://github.com/OpenCageData/python-opencage-geocoder/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/OpenCageData/python-opencage-geocoder/actions/workflows/build.yml)
 ![Mastodon Follow](https://img.shields.io/mastodon/follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social)
 
 ## Tutorial
 
 You can find a [comprehensive tutorial for using this module on the OpenCage site](https://opencagedata.com/tutorials/geocode-in-python).
 
 ## Usage
@@ -83,18 +82,17 @@
 
 ```python
 results = geocoder.geocode('London', proximity='42.828576, -81.406643')
 print(results[0]['formatted'])
 # u'London, ON N6A 3M8, Canada'
 ```
 
-
 ### Reverse geocoding
 
-Turn a lat/long into an address with the ``reverse_geocode`` method:
+Turn a lat/long into an address with the `reverse_geocode` method:
 
 ```python
 result = geocoder.reverse_geocode(51.51024, -0.10303)
 ```
 
 ### Sessions
 
@@ -139,27 +137,26 @@
 
 <img src="batch-progress.gif"/>
 
 ### Exceptions
 
 If anything goes wrong, then an exception will be raised:
 
- * `InvalidInputError` for non-unicode query strings
- * `NotAuthorizedError` if API key is missing, invalid syntax or disabled
- * `ForbiddenError` API key is blocked or suspended
- * `RateLimitExceededError` if you go past your rate limit
- * `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
-
+- `InvalidInputError` for non-unicode query strings
+- `NotAuthorizedError` if API key is missing, invalid syntax or disabled
+- `ForbiddenError` API key is blocked or suspended
+- `RateLimitExceededError` if you go past your rate limit
+- `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
 
 ## Copyright & License
 
 This software is copyright OpenCage GmbH.
 Please see `LICENSE.txt`
 
 ### Who is OpenCage GmbH?
 
 <a href="https://opencagedata.com"><img src="opencage_logo_300_150.png"/></a>
 
-We run a worldwide [geocoding API](https://opencagedata.com/api) and [geosearch](https://opencagedata.com/geosearch) service based on open data. 
-Learn more [about us](https://opencagedata.com/about). 
+We run a worldwide [geocoding API](https://opencagedata.com/api) and [geosearch](https://opencagedata.com/geosearch) service based on open data.
+Learn more [about us](https://opencagedata.com/about).
 
 We also run [Geomob](https://thegeomob.com), a series of regular meetups for location based service creators, where we do our best to highlight geoinnovation. If you like geo stuff, you will probably enjoy [the Geomob podcast](https://thegeomob.com/podcast/).
```

### Comparing `opencage-2.2.0/opencage.egg-info/SOURCES.txt` & `opencage-2.3.0/opencage.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 test/test_error_blocked.py
 test/test_error_invalid_input.py
 test/test_error_not_authorized.py
 test/test_error_ratelimit_exceeded.py
 test/test_error_unknown.py
 test/test_flotify_dict.py
 test/test_reverse.py
-test/test_session.py
+test/test_session.py
+test/test_setting_protocol.py
```

### Comparing `opencage-2.2.0/setup.py` & `opencage-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 if sys.version_info < (3, 6):
     raise RuntimeError(
         "opencage requires Python 3.7 or newer"
         "Use older opencage 1.x for Python 2.7 or 3.6"
     )
 
-# try for travis
+# try for testing
 try:
     with open(os.path.join(SOURCE_DIR, 'README.md'), encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
 
 setup(
     name="opencage",
-    version="2.2.0",
+    version="2.3.0",
     description="Wrapper module for the OpenCage Geocoder API",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author="OpenCage GmbH",
     author_email="info@opencagedata.com",
     url="https://github.com/OpenCageData/python-opencage-geocoder/",
     download_url="https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0",
@@ -53,17 +53,17 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: GIS',
         'Topic :: Utilities'
     ],
     install_requires=[
-        'Requests>=2.26.0',
-        'backoff>=1.10.0'
+        'Requests>=2.31.0',
+        'backoff>=2.2.1'
     ],
     test_suite='pytest',
     tests_require=[
-        'httpretty>=0.9.6',
-        'pylint==2.15.9',
-        'pytest>=6.0'
+        'httpretty>=1.1.4',
+        'pylint==2.17.4',
+        'pytest>=7.4.0'
     ],
 )
```

### Comparing `opencage-2.2.0/test/test_all.py` & `opencage-2.3.0/test/test_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 # reduce maximum backoff retry time from 120s to 1s
 os.environ['BACKOFF_MAX_TIME'] = '1'
 
 
 geocoder = OpenCageGeocode('abcde')
 
-# Check if protocol can be set
-geocoder_http = OpenCageGeocode('abcde', 'http')
-assert geocoder_http.url == 'http://api.opencagedata.com/geocode/v1/json'
-
 
 def _any_result_around(results, lat=None, lon=None):
     for result in results:
         if (abs(result['geometry']['lat'] - lat) < 0.05 and
             abs(result['geometry']['lng'] - lon) < 0.05):
             return True
     return False
```

### Comparing `opencage-2.2.0/test/test_async.py` & `opencage-2.3.0/test/test_async.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_error_blocked.py` & `opencage-2.3.0/test/test_error_blocked.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_error_invalid_input.py` & `opencage-2.3.0/test/test_error_invalid_input.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_error_not_authorized.py` & `opencage-2.3.0/test/test_error_not_authorized.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_error_ratelimit_exceeded.py` & `opencage-2.3.0/test/test_error_ratelimit_exceeded.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_error_unknown.py` & `opencage-2.3.0/test/test_error_unknown.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_flotify_dict.py` & `opencage-2.3.0/test/test_flotify_dict.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_reverse.py` & `opencage-2.3.0/test/test_reverse.py`

 * *Files identical despite different names*

### Comparing `opencage-2.2.0/test/test_session.py` & `opencage-2.3.0/test/test_session.py`

 * *Files identical despite different names*

