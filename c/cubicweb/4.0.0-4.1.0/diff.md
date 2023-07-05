# Comparing `tmp/cubicweb-4.0.0.tar.gz` & `tmp/cubicweb-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-4.0.0.tar", last modified: Tue May  9 16:03:59 2023, max compression
+gzip compressed data, was "cubicweb-4.1.0.tar", last modified: Wed Jul  5 08:55:37 2023, max compression
```

## Comparing `cubicweb-4.0.0.tar` & `cubicweb-4.1.0.tar`

### file list

```diff
@@ -1,1321 +1,1322 @@
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.237919 cubicweb-4.0.0/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17987 2023-04-06 12:54:03.000000 cubicweb-4.0.0/COPYING
--rw-r--r--   0 fferry    (1000) fferry    (1000)    26527 2023-04-06 13:14:49.000000 cubicweb-4.0.0/COPYING.LESSER
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4926 2023-04-17 13:13:13.000000 cubicweb-4.0.0/MANIFEST.in
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4231 2023-05-09 16:03:59.237919 cubicweb-4.0.0/PKG-INFO
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3819 2023-05-05 12:20:47.000000 cubicweb-4.0.0/README.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.969902 cubicweb-4.0.0/cubicweb/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7348 2023-04-06 12:54:34.000000 cubicweb-4.0.0/cubicweb/__init__.py
--rwxr-xr-x   0 fferry    (1000) fferry    (1000)       69 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/__main__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1665 2023-05-09 15:48:21.000000 cubicweb-4.0.0/cubicweb/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6885 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/_exceptions.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3860 2023-04-06 12:54:35.000000 cubicweb-4.0.0/cubicweb/_gcdebug.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5211 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/appobject.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1671 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/crypto.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    64585 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/cwconfig.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    32469 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/cwctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4899 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/cwgettext.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    25984 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/cwvreg.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.981902 cubicweb-4.0.0/cubicweb/dataimport/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1987 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3276 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/csv.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    21024 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/dataimport/importer.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    26724 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/dataimport/massive_store.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15511 2023-04-06 12:54:39.000000 cubicweb-4.0.0/cubicweb/dataimport/pgstore.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    18099 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/dataimport/stores.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.989902 cubicweb-4.0.0/cubicweb/dataimport/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.001902 cubicweb-4.0.0/cubicweb/dataimport/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)   474710 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/data/geonames.csv
--rw-r--r--   0 fferry    (1000) fferry    (1000)      113 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/data/people.csv
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1231 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12362 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/data/timeZones.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.013903 cubicweb-4.0.0/cubicweb/dataimport/test/data-massimport/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1987 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/data-massimport/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2513 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/test_csv.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    16178 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/dataimport/test/test_massive_store.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4179 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/dataimport/test/test_pgstore.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8221 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/dataimport/test/test_stores.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10720 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/dataimport/test/unittest_importer.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2677 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/debug.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.045903 cubicweb-4.0.0/cubicweb/devtools/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    27150 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/devtools/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4116 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/apptest_config.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.053903 cubicweb-4.0.0/cubicweb/devtools/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      266 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/data/cwmock.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5146 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/data/qunit.css
--rw-r--r--   0 fferry    (1000) fferry    (1000)   115758 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/data/qunit.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)    38090 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/devtools/devctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3702 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/fake.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    24604 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/devtools/fill.py
--rwxr-xr-x   0 fferry    (1000) fferry    (1000)     1011 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/fix_po_encoding
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10988 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/htmlparser.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5298 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/httptest.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9217 2023-04-06 12:54:43.000000 cubicweb-4.0.0/cubicweb/devtools/instrument.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2354 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/realdbtest.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10915 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/repotest.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6775 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/stresstester.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.057903 cubicweb-4.0.0/cubicweb/devtools/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.057903 cubicweb-4.0.0/cubicweb/devtools/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/bootstrap_cubes
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11311 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/firstnames.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.889901 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.065903 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      462 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.065903 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.065903 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2657 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.065903 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       13 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1720 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1679 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.889901 cubicweb-4.0.0/cubicweb/devtools/test/data/static/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.081904 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)       10 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      353 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      321 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      136 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      136 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      719 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/utils.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4354 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/devtools/test/unittest_dbfill.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6325 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/test/unittest_devctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2475 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/devtools/test/unittest_fill.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3225 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/test/unittest_i18n.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4687 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/devtools/test/unittest_testlib.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22045 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/devtools/testlib.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.085904 cubicweb-4.0.0/cubicweb/entities/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5330 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/entities/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    24573 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/entities/adapters.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6476 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/entities/authobjs.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4207 2023-04-06 12:54:45.000000 cubicweb-4.0.0/cubicweb/entities/lib.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6010 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/entities/schemaobjs.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4168 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/entities/sources.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.085904 cubicweb-4.0.0/cubicweb/entities/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.089904 cubicweb-4.0.0/cubicweb/entities/test/data/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.089904 cubicweb-4.0.0/cubicweb/entities/test/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      893 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/entities/test/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1307 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/entities/test/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9949 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/entities/test/unittest_base.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    36515 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/entities/test/unittest_wfobjs.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    23208 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/entities/wfobjs.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    59296 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/entity.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.093904 cubicweb-4.0.0/cubicweb/ext/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/ext/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5931 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/ext/html4zope.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1839 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/ext/markdown.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.093904 cubicweb-4.0.0/cubicweb/ext/test/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2013 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/ext/test/unittest_markdown.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.101904 cubicweb-4.0.0/cubicweb/hooks/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4593 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1544 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/bookmark.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3089 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/email.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13223 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/integrity.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5680 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/metadata.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9739 2023-04-06 12:54:47.000000 cubicweb-4.0.0/cubicweb/hooks/notification.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8112 2023-04-06 12:54:47.000000 cubicweb-4.0.0/cubicweb/hooks/security.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10642 2023-04-06 13:01:23.000000 cubicweb-4.0.0/cubicweb/hooks/synccomputed.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    60957 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/hooks/syncschema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4913 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/syncsession.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2952 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/syncsources.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.137904 cubicweb-4.0.0/cubicweb/hooks/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.141904 cubicweb-4.0.0/cubicweb/hooks/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      291 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/data/hooks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2728 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/data/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.141904 cubicweb-4.0.0/cubicweb/hooks/test/data-computed/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1700 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/data-computed/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1729 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_bookmarks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13100 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_hooks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8490 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_integrity.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1513 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_notificationhooks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2308 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_security.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_synccomputed.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    24444 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncschema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4778 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncsession.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2667 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncsources.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15886 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/hooks/workflow.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.149905 cubicweb-4.0.0/cubicweb/i18n/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    93082 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/i18n/de.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)    61668 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/i18n/en.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)   112148 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/i18n/es.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)   106920 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/i18n/fr.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3759 2023-04-06 12:59:38.000000 cubicweb-4.0.0/cubicweb/i18n.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5599 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/mail.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3352 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/md5crypt.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22103 2023-04-06 13:00:03.000000 cubicweb-4.0.0/cubicweb/migration.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.153905 cubicweb-4.0.0/cubicweb/misc/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.161905 cubicweb-4.0.0/cubicweb/misc/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      690 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.22.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      395 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.22.1_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      470 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.22.3_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3166 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.23.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      913 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.24.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1412 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.24.4_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      117 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.27.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      217 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.30.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.31.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      423 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.32.3_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       25 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/misc/migration/3.38.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    20222 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/misc/migration/bootstrapmigration_repository.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3370 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/migration/postcreate.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.165905 cubicweb-4.0.0/cubicweb/misc/scripts/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1448 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/scripts/chpasswd.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      395 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/scripts/detect_cycle.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5750 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/misc/scripts/fast_drop_entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      799 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/scripts/ldap_change_base_dn.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3474 2023-04-06 13:00:07.000000 cubicweb-4.0.0/cubicweb/misc/scripts/migration_helper.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1097 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/misc/source_highlight.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3270 2023-04-06 13:00:10.000000 cubicweb-4.0.0/cubicweb/mttransforms.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17407 2023-04-06 13:00:13.000000 cubicweb-4.0.0/cubicweb/multipart.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    50971 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/predicates.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4513 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pylintext.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.173905 cubicweb-4.0.0/cubicweb/pyramid/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9243 2023-05-09 15:47:46.000000 cubicweb-4.0.0/cubicweb/pyramid/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8851 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/pyramid/auth.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4572 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/config.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7548 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/core.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1483 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/csrf.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7081 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_source_code.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.181905 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1895 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1505 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3912 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1592 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4852 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2980 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8486 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/debugtoolbar_panels.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1837 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/development.ini.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3771 2023-05-09 15:47:46.000000 cubicweb-4.0.0/cubicweb/pyramid/predicates.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1632 2023-05-09 15:47:46.000000 cubicweb-4.0.0/cubicweb/pyramid/pyramid.ini.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13542 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/pyramid/pyramidctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5310 2023-05-09 15:47:46.000000 cubicweb-4.0.0/cubicweb/pyramid/resources.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6854 2023-05-09 15:47:46.000000 cubicweb-4.0.0/cubicweb/pyramid/rest_api.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9634 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/pyramid/session.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.181905 cubicweb-4.0.0/cubicweb/pyramid/test/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1862 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/pyramid/test/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.181905 cubicweb-4.0.0/cubicweb/pyramid/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        5 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/test/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.189905 cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      416 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1327 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3666 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/test/test_config.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6408 2023-05-02 08:49:36.000000 cubicweb-4.0.0/cubicweb/pyramid/test/test_content_negociation.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      782 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/pyramid/test/test_core.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      986 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/test/test_tools.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2065 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pyramid/tools.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1929 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/pytestconf.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1802 2023-04-06 13:00:49.000000 cubicweb-4.0.0/cubicweb/rdf.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2170 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/repoapi.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17499 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/req.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    41745 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/rqlrewrite.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11506 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/rqlsuggestions.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    27303 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/rset.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11717 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/rtags.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    57984 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6147 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schema_exporters.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.193905 cubicweb-4.0.0/cubicweb/schemas/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2279 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/Bookmark.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1696 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1662 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/_regproc.postgres.sql
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13898 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/base.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15024 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/bootstrap.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11853 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/schemas/workflow.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.221906 cubicweb-4.0.0/cubicweb/server/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14123 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3275 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/check_unused_index.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    23459 2023-04-06 12:58:21.000000 cubicweb-4.0.0/cubicweb/server/checkintegrity.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6110 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/edition.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    38611 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/hook.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    78083 2023-04-06 12:59:59.000000 cubicweb-4.0.0/cubicweb/server/migractions.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    35946 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/querier.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    47968 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/server/repository.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    19170 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/rqlannotation.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13967 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/server/schema2sql.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    28738 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/schemaserial.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3168 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/serverconfig.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    52134 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/serverctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    32452 2023-04-06 13:01:15.000000 cubicweb-4.0.0/cubicweb/server/session.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.225906 cubicweb-4.0.0/cubicweb/server/sources/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13281 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/sources/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    18201 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/sources/datafeed.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    16790 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/sources/ldapfeed.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    78435 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/sources/native.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    71413 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/server/sources/rql2sql.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11169 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/sources/storages.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22724 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/sqlutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22491 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/server/ssplanner.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.257906 cubicweb-4.0.0/cubicweb/server/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.277906 cubicweb-4.0.0/cubicweb/server/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.329907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.333907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.333907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.337907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.337907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.337907 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1087 2023-04-06 12:59:05.000000 cubicweb-4.0.0/cubicweb/server/test/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/hooks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1503 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/ldap_test.ldif
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.337907 cubicweb-4.0.0/cubicweb/server/test/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/site_cubicweb.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1585 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/slapd.conf.in
--rw-r--r--   0 fferry    (1000) fferry    (1000)       77 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/sources_extern
--rw-r--r--   0 fferry    (1000) fferry    (1000)       97 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data/sources_multi
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.277906 cubicweb-4.0.0/cubicweb/server/test/data-cwep002/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1299 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-cwep002/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.281906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.285906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.285906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.285906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.289906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1424 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      153 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      470 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.289906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1566 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2876 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.289906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.297906 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.301907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.301907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.309907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.309907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.313907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.313907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.313907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.321907 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8437 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9716 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-migractions/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.321907 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.325907 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2510 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/Company.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1242 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3298 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/State.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      980 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3778 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/toignore
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.329907 cubicweb-4.0.0/cubicweb/server/test/data-schemaserial/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1345 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schemaserial/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.341907 cubicweb-4.0.0/cubicweb/server/test/datacomputed/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.341907 cubicweb-4.0.0/cubicweb/server/test/datacomputed/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1893 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1851 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/datacomputed/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8829 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_datafeed.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2192 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_edition.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4881 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_hook.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    24724 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_ldapsource.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    96667 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_querier.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)   101035 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_rql2sql.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    23311 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_rqlannotation.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11087 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_schema2sql.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    28099 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_schemaserial.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    38100 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_server_security.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5431 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_server_utils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3908 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_serverctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2296 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_session.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1609 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_sources_native.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2449 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_sqlutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3285 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_ssplanner.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17471 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_storage.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1139 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_tools.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    21794 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_undo.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2619 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/test/unittest_utils.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.341907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.341907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.345907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.345907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.349907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.353907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.353907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.357907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.357907 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3596 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.357907 cubicweb-4.0.0/cubicweb/server/test_migractions/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.361907 cubicweb-4.0.0/cubicweb/server/test_migractions/data/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.405908 cubicweb-4.0.0/cubicweb/server/test_migractions/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.361907 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.365908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.365908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.365908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.369907 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1424 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      153 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      470 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.373908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1566 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2876 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.373908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.385908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.389908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.389908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.393908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.393908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.393908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.397908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.401908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.401908 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8437 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9716 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.409908 cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.409908 cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1893 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1851 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    47736 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions/unittest_migractions.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.409908 cubicweb-4.0.0/cubicweb/server/test_migractions2/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.413908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.441908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.453909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.453909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.453909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.453909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.457909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.473909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.413908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.413908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.413908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.413908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.421908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1424 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      153 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      470 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.425908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1566 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2876 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.425908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.425908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.429908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.429908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.429908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.429908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.437909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.437909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.437909 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.441908 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8437 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9716 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.477909 cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.477909 cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1893 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1851 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9732 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions2/unittest_migractions.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.477909 cubicweb-4.0.0/cubicweb/server/test_migractions3/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.489909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.541910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.545910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.545910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.545910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.493909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.497909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.497909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.505909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.509909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1424 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      153 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      470 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.509909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1566 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2876 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.509909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.513909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.513909 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.517910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.517910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.525910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.533910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.533910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.537910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.537910 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8437 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9716 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1893 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1851 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1972 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_migractions3/unittest_migractions.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.549910 cubicweb-4.0.0/cubicweb/server/test_postgres/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.553910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.553910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.561910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.561910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.561910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.561910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.561910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.565910 cubicweb-4.0.0/cubicweb/server/test_postgres/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1420 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/migration/postcreate.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/data/site_cubicweb.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10234 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_postgres/unittest_postgres.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.565910 cubicweb-4.0.0/cubicweb/server/test_repository/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.565910 cubicweb-4.0.0/cubicweb/server/test_repository/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       40 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.565910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_basket/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      774 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.569910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.569910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.573910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1277 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.577910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.577910 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      569 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1202 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/hooks.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10285 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.565910 cubicweb-4.0.0/cubicweb/server/test_repository/data-schemaserial/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1345 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data-schemaserial/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1121 2023-04-06 12:54:11.000000 cubicweb-4.0.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    37991 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/server/test_repository/unittest_repository.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5200 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/server/utils.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.581910 cubicweb-4.0.0/cubicweb/skeleton/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1112 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      262 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/.hgignore.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      109 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/.yamllint.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      249 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/Dockerfile.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      367 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/MANIFEST.in.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1484 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/skeleton/README.rst.tmpl
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.585910 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       97 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      618 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.589911 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       24 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
--rw-r--r--   0 fferry    (1000) fferry    (1000)      190 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      203 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.589911 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      248 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)      248 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)      248 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.593911 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      425 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      378 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      180 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      221 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      747 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)      215 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2030 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/setup.py.tmpl
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.593911 cubicweb-4.0.0/cubicweb/skeleton/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.593911 cubicweb-4.0.0/cubicweb/skeleton/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       13 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2001 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1039 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1330 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/skeleton/tox.ini.tmpl
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.593911 cubicweb-4.0.0/cubicweb/smoke_test/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1433 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1455 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.597911 cubicweb-4.0.0/cubicweb/sobjects/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1364 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/sobjects/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12952 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/ldapparser.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14620 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/sobjects/notification.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5869 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/sobjects/services.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8236 2023-04-06 13:01:22.000000 cubicweb-4.0.0/cubicweb/sobjects/supervising.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.609911 cubicweb-4.0.0/cubicweb/sobjects/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.609911 cubicweb-4.0.0/cubicweb/sobjects/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       13 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.613911 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      441 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.633911 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1030 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1052 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1154 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.633911 cubicweb-4.0.0/cubicweb/sobjects/test/data/sobjects/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1079 2023-04-06 12:57:18.000000 cubicweb-4.0.0/cubicweb/sobjects/test/data/sobjects/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4020 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/sobjects/test/unittest_email.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3061 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/sobjects/test/unittest_notification.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5404 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/sobjects/test/unittest_register_user.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5051 2023-04-06 13:02:01.000000 cubicweb-4.0.0/cubicweb/sobjects/test/unittest_supervising.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1996 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/tags.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.649911 cubicweb-4.0.0/cubicweb/test/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.657911 cubicweb-4.0.0/cubicweb/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       31 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/data/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.665912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      441 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.665912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1030 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1109 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.673912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1128 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/hooks.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.677912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/views/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/views/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.681912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1024 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.681912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/entities/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.681912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/hooks/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.681912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_forge/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      819 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_forge/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1153 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.685912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.685912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      845 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      875 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       51 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.685912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      857 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      887 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      657 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.689912 cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      157 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      622 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1565 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1555 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/erqlexpr_on_ertype.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       77 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/lowered_etype.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.693912 cubicweb-4.0.0/cubicweb/test/data/migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      835 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.0.3_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      835 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.0.4_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      835 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      855 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_common.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      847 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_repository.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      835 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/migration/0.1.2_Any.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      402 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/rqlexpr_on_computedrel.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1555 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1401 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/rrqlexpr_on_attr.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1182 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/rrqlexpr_on_eetype.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4319 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.697912 cubicweb-4.0.0/cubicweb/test/data/scripts/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      164 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/scripts/script1.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      168 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/scripts/script2.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      187 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/scripts/script3.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.697912 cubicweb-4.0.0/cubicweb/test/data/server_migration/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
--rw-r--r--   0 fferry    (1000) fferry    (1000)      882 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      131 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data/uppered_rtype.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.657911 cubicweb-4.0.0/cubicweb/test/data-rewrite/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       16 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/bootstrap_cubes
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.657911 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      441 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      664 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.661912 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_localperms/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       41 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1516 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3723 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data-rewrite/schema.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.697912 cubicweb-4.0.0/cubicweb/test/data_schemareader/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      732 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/data_schemareader/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2304 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_binary.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      404 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_crypto.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17528 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_cwconfig.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7427 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_cwctl.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    47978 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_entity.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4855 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_fast_drop_entities.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8359 2023-04-06 13:01:50.000000 cubicweb-4.0.0/cubicweb/test/unittest_mail.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7471 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_migration.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15441 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/test/unittest_predicates.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3879 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_repoapi.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5789 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_req.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    45868 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_rqlrewrite.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6509 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_rqlsuggestions.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    32593 2023-05-03 09:21:31.000000 cubicweb-4.0.0/cubicweb/test/unittest_rset.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6543 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_rtags.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    34435 2023-05-04 08:14:24.000000 cubicweb-4.0.0/cubicweb/test/unittest_schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4051 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_toolsutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9574 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_uilib.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3202 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/test/unittest_vregistry.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3998 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/test/unittest_wfutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15556 2023-05-05 12:20:47.000000 cubicweb-4.0.0/cubicweb/toolsutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3895 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/transaction.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    19495 2023-04-17 13:13:13.000000 cubicweb-4.0.0/cubicweb/uilib.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12358 2023-04-21 09:10:40.000000 cubicweb-4.0.0/cubicweb/utils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5113 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/wfutils.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1578 2023-04-06 13:14:49.000000 cubicweb-4.0.0/cubicweb/xy.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:57.973902 cubicweb-4.0.0/cubicweb.egg-info/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4231 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/PKG-INFO
--rw-r--r--   0 fferry    (1000) fferry    (1000)    51742 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/SOURCES.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/dependency_links.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      117 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/entry_points.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-04-19 08:52:40.000000 cubicweb-4.0.0/cubicweb.egg-info/not-zip-safe
--rw-r--r--   0 fferry    (1000) fferry    (1000)      435 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/requires.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        9 2023-05-09 16:03:57.000000 cubicweb-4.0.0/cubicweb.egg-info/top_level.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.701912 cubicweb-4.0.0/doc/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6608 2023-05-05 12:45:07.000000 cubicweb-4.0.0/doc/4.0.0_how_to_migrate.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2811 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/Makefile
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.701912 cubicweb-4.0.0/doc/_static/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    34494 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/_static/favicon.ico
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9202 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/_static/logo-cubicweb.svg
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1681 2023-04-06 12:57:29.000000 cubicweb-4.0.0/doc/announce.en.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1982 2023-04-06 12:57:31.000000 cubicweb-4.0.0/doc/announce.fr.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.709912 cubicweb-4.0.0/doc/api/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2251 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/__init__.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      181 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/appobject.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      830 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/cwvreg.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      491 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/dataimport.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)       87 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2536 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/predicates.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.713912 cubicweb-4.0.0/doc/api/pyramid/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      249 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/auth.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      370 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/bwcompat.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      480 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/core.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      296 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/login.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      259 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/profile.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      200 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/session.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      289 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid/url_redirection.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      234 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/pyramid.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      144 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/req.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      140 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/rset.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      781 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/urlpublishing.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      393 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/urlrewrite.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      520 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/api/web.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.713912 cubicweb-4.0.0/doc/book/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14655 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/MERGE_ME-tut-create-app.en.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7806 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.717912 cubicweb-4.0.0/doc/book/_maybe_to_integrate/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      225 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1286 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/_maybe_to_integrate/rss-xml.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      751 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/_maybe_to_integrate/template.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.717912 cubicweb-4.0.0/doc/book/additionnal_services/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      369 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/additionnal_services/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13562 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/additionnal_services/undo.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.757913 cubicweb-4.0.0/doc/book/admin/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2253 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/backups.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5658 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/config.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3879 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/book/admin/create-instance.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3396 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/book/admin/cubicweb-ctl.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4035 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/deploy.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      428 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5172 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/instance-config.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4825 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/ldap.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      130 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/multisources.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      366 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/rql-logs.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5401 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/setup.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3596 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/admin/site-config.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.761913 cubicweb-4.0.0/doc/book/annexes/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1893 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/depends.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3257 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/docstrings-conventions.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    16153 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/faq.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      234 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3481 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/mercurial.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.777913 cubicweb-4.0.0/doc/book/annexes/rql/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2115 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/Graph-ex.gif
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1167 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/debugging.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4697 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/implementation.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      267 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5570 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/intro.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    27490 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/annexes/rql/language.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2697 2023-05-02 08:49:43.000000 cubicweb-4.0.0/doc/book/annexes/rql/usecases.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.781913 cubicweb-4.0.0/doc/book/devrepo/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2147 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/connections_pooler.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.785913 cubicweb-4.0.0/doc/book/devrepo/cubes/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2645 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/cubes/available-cubes.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      932 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/cubes/cc-newcube.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      208 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/cubes/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6828 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/cubes/layout.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1967 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/cubes/what-is-a-cube.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4021 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/dataimport.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.793913 cubicweb-4.0.0/doc/book/devrepo/datamodel/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1389 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/datamodel/baseschema.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6178 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/datamodel/define-workflows.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    34880 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/datamodel/definition.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      248 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/datamodel/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1043 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/datamodel/metadata.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2940 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/debug_channels.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.797913 cubicweb-4.0.0/doc/book/devrepo/devcore/
--rw-r--r--   0 fferry    (1000) fferry    (1000)       67 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/devcore/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1129 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/devcore/reqbase.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.797913 cubicweb-4.0.0/doc/book/devrepo/entityclasses/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5159 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/entityclasses/adapters.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7268 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/entityclasses/application-logic.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5285 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/entityclasses/data-as-objects.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      303 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/entityclasses/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1719 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/entityclasses/load-sort.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4399 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/fti.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      504 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9399 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/migration.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2668 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/profiling.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.805914 cubicweb-4.0.0/doc/book/devrepo/repo/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9731 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/repo/hooks.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      155 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/repo/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1087 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/repo/notifications.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11467 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/repo/sessions.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)       75 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/repo/tasks.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    21316 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/testing.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    18285 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/devrepo/vreg.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.857914 cubicweb-4.0.0/doc/book/devweb/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      915 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/ajax.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3473 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/controllers.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      890 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/css.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.857914 cubicweb-4.0.0/doc/book/devweb/edition/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11979 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/edition/dissection.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3955 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/edition/editcontroller.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9905 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/edition/examples.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15502 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/edition/form.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      286 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/edition/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      698 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/facets.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      675 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/httpcaching.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      392 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10057 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/internationalization.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14107 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/js.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      265 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/property.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2017 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/publisher.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5119 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/request.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      709 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/resource.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      454 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/rtags.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1418 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/searchbar.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.877915 cubicweb-4.0.0/doc/book/devweb/views/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5889 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/basetemplates.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      701 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/baseviews.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1291 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/boxes.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2320 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/breadcrumbs.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      657 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/idownloadable.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      476 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10179 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/primary.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5991 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/reledit.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      521 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/startup.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5919 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/table.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5506 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/urlpublish.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4156 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/views.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      347 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/wdoc.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1703 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/views/xmlrss.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      947 2023-04-17 13:13:13.000000 cubicweb-4.0.0/doc/book/devweb/warning.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.885915 cubicweb-4.0.0/doc/book/intro/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    10427 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/intro/concepts.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1369 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/intro/history.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      385 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/intro/index.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.893915 cubicweb-4.0.0/doc/book/pyramid/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1377 2023-05-02 08:49:36.000000 cubicweb-4.0.0/doc/book/pyramid/auth.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1314 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/pyramid/ctl.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3819 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/book/pyramid/debug_toolbar.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      844 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/pyramid/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1795 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/book/pyramid/quickstart.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5419 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/book/pyramid/settings.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.893915 cubicweb-4.0.0/doc/book/security/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7880 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/security/csrf.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.893915 cubicweb-4.0.0/doc/book/src/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2930 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/src/archi_globale.dia
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1735 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/book/src/main_template_layout.dia
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.941915 cubicweb-4.0.0/doc/changes/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6619 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.14.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3904 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.15.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3647 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.16.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1815 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.17.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3632 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.18.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6757 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.19.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3165 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.20.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2991 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.21.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3689 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.22.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2799 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.23.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4033 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.24.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4655 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.25.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      434 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.26.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6870 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.27.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2656 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.28.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1249 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.29.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5588 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.30.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3683 2023-04-06 12:57:03.000000 cubicweb-4.0.0/doc/changes/3.31.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7979 2023-04-06 12:57:10.000000 cubicweb-4.0.0/doc/changes/3.32.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1728 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/3.32_reledit.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5634 2023-04-06 12:57:11.000000 cubicweb-4.0.0/doc/changes/3.33.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4522 2023-04-06 12:57:12.000000 cubicweb-4.0.0/doc/changes/3.34.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4835 2023-04-06 12:57:14.000000 cubicweb-4.0.0/doc/changes/3.35.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     4486 2023-04-06 13:23:29.000000 cubicweb-4.0.0/doc/changes/3.36.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5066 2023-04-06 13:23:29.000000 cubicweb-4.0.0/doc/changes/3.37.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7195 2023-04-06 13:23:29.000000 cubicweb-4.0.0/doc/changes/3.38.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6422 2023-05-09 15:49:54.000000 cubicweb-4.0.0/doc/changes/4.0.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      599 2023-05-05 12:20:48.000000 cubicweb-4.0.0/doc/changes/changelog.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)       99 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/changes/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7617 2023-05-05 12:20:49.000000 cubicweb-4.0.0/doc/conf.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:58.949916 cubicweb-4.0.0/doc/dev/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      708 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/coding_standards_css.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      768 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/coding_standards_js.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1037 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/continuous-integration.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1283 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/documenting.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)    24407 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/features_list.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      228 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1241 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/dev/refactoring-the-css-with-uiprops.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.205919 cubicweb-4.0.0/doc/images/
--rw-r--r--   0 fferry    (1000) fferry    (1000)    98393 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/03-transitions-view_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12650 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/breadcrumbs_header.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    85073 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_general_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   124385 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_registry_content_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   111325 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_registry_decisions_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   134505 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_rql_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   192629 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_rql_traceback_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   107766 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_show_source.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    55625 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_show_source_link.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   126845 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_sql_panel.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    97343 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/debugtoolbar_traceback_source_link.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    57300 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/example-card-with-rql-directive.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    55168 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/example-card-with-rql-table-directive.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2277 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/facet_date_range.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6013 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/facet_has_image.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22016 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/facet_overview.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1873 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/facet_range.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    21685 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_00-login_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    30326 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_01-start_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    35859 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_02-cookie-values_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    33922 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_02-create-blog_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    28123 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_03-list-one-blog_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    82897 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_03-site-config-panel_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   119813 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_03-state-submitted_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    98393 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_03-transitions-view_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    34771 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_04-detail-one-blog_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    28345 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_05-list-two-blog_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    49230 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_06-add-relation-entryof_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    96838 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_06-main-template-logo_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    40383 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_07-detail-one-blogentry_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    30591 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_08-schema_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    33091 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_09-new-view-blogentry_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    42230 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/lax-book_10-blog-with-two-entries_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17757 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/main_template.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8674 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/main_template.svg
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13842 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/main_template_layout.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    46411 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/primaryview_template.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14758 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/primaryview_template.svg
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22773 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/request_session.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7211 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/request_session.svg
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12030 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/server-class-diagram.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    62022 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_blog-form_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   105173 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    58500 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_blog-primary_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    42013 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_blogs-list_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   109769 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_form-generic-relations_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    65646 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_index_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    13605 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_index_gettext_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    88970 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_index_logged_in_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    11548 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_login-form_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   100347 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    63097 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    62431 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-community-default-primary_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    74856 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    79709 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-custom-footer_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   128406 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-schema_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    71500 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_myblog-siteinfo_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   104834 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_schema_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    22098 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_schema_graphviz_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   150520 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-base_siteconfig_en.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    60672 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_admin.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    61388 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_city_created.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    50694 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_city_creation.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    71561 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_data_model_schema.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    48896 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_empty_instance.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    55671 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_finished_import.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    57063 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_list_view.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    70893 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_museum_created.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    61656 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_museum_creation.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    74005 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_museum_with_city_name.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   225824 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_react_map.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    53544 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-museum_with_schema.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   354637 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_background-image.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    30437 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_boxes.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    54643 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_breadcrumbs.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   324086 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_facets.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    40520 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_grey-box.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    16843 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_index-after.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    26875 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_index-before.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17580 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_login-box.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    57814 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_prevnext.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    81362 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_ui1.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    93291 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_ui2.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)   290338 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/tutos-photowebsite_ui3.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    43051 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/undo_history-view_w600.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    26036 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/undo_mesage_w600.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    39625 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/undo_startup-link_w600.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17558 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/views-table-filter-shadow.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    14013 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/views-table-filter.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12375 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/views-table-shadow.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9676 2023-04-06 13:14:49.000000 cubicweb-4.0.0/doc/images/views-table.png
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7225 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2011 2023-04-06 12:54:03.000000 cubicweb-4.0.0/doc/plan_formation_python_cubicweb.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      139 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/stdlib.txt
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.217919 cubicweb-4.0.0/doc/tools/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1462 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tools/generate_modules.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1624 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tools/mode_plan.py
--rwxr-xr-x   0 fferry    (1000) fferry    (1000)     4944 2023-05-04 08:14:24.000000 cubicweb-4.0.0/doc/tools/pyjsrest.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.217919 cubicweb-4.0.0/doc/tutorials/
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.221919 cubicweb-4.0.0/doc/tutorials/advanced/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      604 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/advanced/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5486 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/advanced/part01_create-cube.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    17016 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/advanced/part02_security.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5614 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/advanced/part03_bfss.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15384 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/advanced/part04_ui-base.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    15114 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/advanced/part05_ui-advanced.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.225919 cubicweb-4.0.0/doc/tutorials/base/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3867 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/base/blog-in-five-minutes.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)      675 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/base/conclusion.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    20431 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/base/customizing-the-application.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7821 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/base/discovering-the-ui.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1340 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/base/index.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.229919 cubicweb-4.0.0/doc/tutorials/dataimport/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     9014 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/dataimport/diseasome_import.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3336 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/dataimport/diseasome_parser.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)    29917 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/dataimport/index.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6576 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/dataimport/schema.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      609 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/index.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.229919 cubicweb-4.0.0/doc/tutorials/museum/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5956 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/museum/data-management.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8836 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/museum/enhance-views.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)    12313 2023-05-05 12:20:47.000000 cubicweb-4.0.0/doc/tutorials/museum/getting-started.rst
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1156 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/museum/index.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.229919 cubicweb-4.0.0/doc/tutorials/textreports/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      440 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/textreports/index.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.233919 cubicweb-4.0.0/doc/tutorials/tools/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7241 2023-04-06 12:56:17.000000 cubicweb-4.0.0/doc/tutorials/tools/windmill.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.233919 cubicweb-4.0.0/extras/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3545 2023-04-19 08:40:28.000000 cubicweb-4.0.0/extras/cubicweb-ctl.bash_completion
--rw-r--r--   0 fferry    (1000) fferry    (1000)     7414 2023-04-06 12:56:17.000000 cubicweb-4.0.0/jshintrc
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.233919 cubicweb-4.0.0/man/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      651 2023-04-19 08:40:28.000000 cubicweb-4.0.0/man/cubicweb-ctl.1
--rw-r--r--   0 fferry    (1000) fferry    (1000)       56 2023-04-06 12:54:11.000000 cubicweb-4.0.0/mypy.ini
--rw-r--r--   0 fferry    (1000) fferry    (1000)      536 2023-04-06 12:54:03.000000 cubicweb-4.0.0/pylintrc
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-09 16:03:59.237919 cubicweb-4.0.0/requirements/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      174 2023-04-17 13:13:13.000000 cubicweb-4.0.0/requirements/dev.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       45 2023-04-17 13:13:13.000000 cubicweb-4.0.0/requirements/doc.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      377 2023-04-06 12:56:17.000000 cubicweb-4.0.0/requirements/from-forge.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      380 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-base.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       16 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-dataimport.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       15 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-devtools.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        9 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-ext.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       39 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-hooks.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      128 2023-04-06 12:54:11.000000 cubicweb-4.0.0/requirements/test-pyramid.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       35 2023-04-06 12:56:17.000000 cubicweb-4.0.0/requirements/test-server.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)      115 2023-05-09 16:03:59.241919 cubicweb-4.0.0/setup.cfg
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3325 2023-04-17 13:13:13.000000 cubicweb-4.0.0/setup.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8874 2023-05-09 16:03:40.000000 cubicweb-4.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.257017 cubicweb-4.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2023-07-05 08:55:06.000000 cubicweb-4.1.0/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2023-07-05 08:55:06.000000 cubicweb-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-05 08:55:37.257017 cubicweb-4.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.701010 cubicweb-4.1.0/cubicweb/
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       69 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6885 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/_gcdebug.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/appobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    64892 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    32469 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwgettext.py
+-rw-rw-rw-   0 root         (0) root         (0)    25984 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwvreg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.709010 cubicweb-4.1.0/cubicweb/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    21024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    26724 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    15511 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)    18099 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/stores.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.713010 cubicweb-4.1.0/cubicweb/dataimport/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.717010 cubicweb-4.1.0/cubicweb/dataimport/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)   474710 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/geonames.csv
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/people.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/timeZones.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.717010 cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    16178 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     4179 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8221 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/unittest_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.725010 cubicweb-4.1.0/cubicweb/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)    27150 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4116 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/apptest_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.725010 cubicweb-4.1.0/cubicweb/devtools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/cwmock.js
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/qunit.css
+-rw-rw-rw-   0 root         (0) root         (0)   115758 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/qunit.js
+-rw-rw-rw-   0 root         (0) root         (0)    38090 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fake.py
+-rw-rw-rw-   0 root         (0) root         (0)    24604 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fill.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fix_po_encoding
+-rw-rw-rw-   0 root         (0) root         (0)    10988 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/htmlparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5298 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9217 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/realdbtest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10915 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/repotest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/stresstester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.729010 cubicweb-4.1.0/cubicweb/devtools/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.729010 cubicweb-4.1.0/cubicweb/devtools/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/firstnames.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.605008 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.605008 cubicweb-4.1.0/cubicweb/devtools/test/data/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.737010 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_dbfill.py
+-rw-rw-rw-   0 root         (0) root         (0)     6325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_fill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    22045 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.741010 cubicweb-4.1.0/cubicweb/entities/
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24573 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/authobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     6010 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/schemaobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.741010 cubicweb-4.1.0/cubicweb/entities/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/entities/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/entities/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9992 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/unittest_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    36515 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/unittest_wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    23208 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    59296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/ext/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5931 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/html4zope.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/ext/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/test/unittest_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.753010 cubicweb-4.1.0/cubicweb/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/email.py
+-rw-rw-rw-   0 root         (0) root         (0)    13223 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5680 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     9739 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/security.py
+-rw-rw-rw-   0 root         (0) root         (0)    10642 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    60957 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncsources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.757010 cubicweb-4.1.0/cubicweb/hooks/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/hooks/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/hooks/test/data-computed/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data-computed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_bookmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)    13100 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_notificationhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24444 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    93082 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    61668 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)   112148 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)   106920 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/md5crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)    22103 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.765010 cubicweb-4.1.0/cubicweb/misc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.769011 cubicweb-4.1.0/cubicweb/misc/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.23.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.24.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.24.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.27.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.30.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.31.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.32.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.38.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)    20222 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.773011 cubicweb-4.1.0/cubicweb/misc/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/chpasswd.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/detect_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     5750 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/ldap_change_base_dn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/migration_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/source_highlight.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/mttransforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17407 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)    50971 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/predicates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.781011 cubicweb-4.1.0/cubicweb/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     9374 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4572 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7081 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_source_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.785011 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     8486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debugtoolbar_panels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/development.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/pyramid.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)    13542 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/pyramidctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9634 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6519 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_content_negociation.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    17499 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/req.py
+-rw-rw-rw-   0 root         (0) root         (0)    41745 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    11506 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27303 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rset.py
+-rw-rw-rw-   0 root         (0) root         (0)    11717 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    57984 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     6147 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schema_exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.793011 cubicweb-4.1.0/cubicweb/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/Bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/_regproc.postgres.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13898 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    11853 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.805011 cubicweb-4.1.0/cubicweb/server/
+-rw-rw-rw-   0 root         (0) root         (0)    14123 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/check_unused_index.py
+-rw-rw-rw-   0 root         (0) root         (0)    23459 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/checkintegrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/edition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38611 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    78083 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/migractions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/querier.py
+-rw-rw-rw-   0 root         (0) root         (0)    47968 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)    19170 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13967 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28738 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)     3168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/serverconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    52134 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.809011 cubicweb-4.1.0/cubicweb/server/sources/
+-rw-rw-rw-   0 root         (0) root         (0)    13281 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18201 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/ldapfeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    78435 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/native.py
+-rw-rw-rw-   0 root         (0) root         (0)    71413 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11169 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/storages.py
+-rw-rw-rw-   0 root         (0) root         (0)    22724 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22491 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/ssplanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.821011 cubicweb-4.1.0/cubicweb/server/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.825011 cubicweb-4.1.0/cubicweb/server/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.865012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.865012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/ldap_test.ldif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/slapd.conf.in
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/sources_extern
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/sources_multi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.825011 cubicweb-4.1.0/cubicweb/server/test/data-cwep002/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-cwep002/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.829011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.829011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.837011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.837011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.841012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.841012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.849012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.849012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.857012 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/toignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.857012 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_edition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4881 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    24766 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_ldapsource.py
+-rw-rw-rw-   0 root         (0) root         (0)    96667 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_querier.py
+-rw-rw-rw-   0 root         (0) root         (0)   101035 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    23311 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28099 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)    38100 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_server_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_sources_native.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_ssplanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    17471 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21794 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_undo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.873012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.873012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.877012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.877012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_migractions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_migractions/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.889012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.889012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.897012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.897012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.905012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.905012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.909012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.909012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    47736 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.925013 cubicweb-4.1.0/cubicweb/server/test_migractions2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.925013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.929013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.929013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.933013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.933013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.937013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.937013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.945013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.945013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.953013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.953013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.973013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.973013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.981013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.981013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_postgres/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.005014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.005014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    10234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/unittest_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.021014 cubicweb-4.1.0/cubicweb/server/test_repository/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.021014 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    37991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/unittest_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.033014 cubicweb-4.1.0/cubicweb/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.hgignore.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.yamllint.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/Dockerfile.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/MANIFEST.in.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/README.rst.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.037014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.045014 cubicweb-4.1.0/cubicweb/skeleton/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/tox.ini.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.045014 cubicweb-4.1.0/cubicweb/smoke_test/
+-rw-rw-rw-   0 root         (0) root         (0)     1433 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/ldapparser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14620 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5869 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     8236 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/supervising.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_register_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_supervising.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.065014 cubicweb-4.1.0/cubicweb/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.069015 cubicweb-4.1.0/cubicweb/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.077015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.077015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/views/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/entities/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.089015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.089015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/erqlexpr_on_ertype.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/lowered_etype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.093015 cubicweb-4.1.0/cubicweb/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.0.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.0.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_common.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_computedrel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_eetype.py
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.093015 cubicweb-4.1.0/cubicweb/test/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script1.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script2.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.097015 cubicweb-4.1.0/cubicweb/test/data/server_migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/uppered_rtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.069015 cubicweb-4.1.0/cubicweb/test/data-rewrite/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.073015 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.073015 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.097015 cubicweb-4.1.0/cubicweb/test/data_schemareader/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data_schemareader/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    17528 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     7427 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    48020 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8359 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)    15441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_req.py
+-rw-rw-rw-   0 root         (0) root         (0)    45868 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    32593 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     6543 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    34435 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9574 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15556 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3895 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    19495 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.705010 cubicweb-4.1.0/cubicweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51813 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.101015 cubicweb-4.1.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/4.0.0_how_to_migrate.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.101015 cubicweb-4.1.0/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/_static/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/announce.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/announce.fr.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.109015 cubicweb-4.1.0/doc/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/__init__.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/appobject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/cwvreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/dataimport.rst
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/predicates.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/api/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/bwcompat.rst
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/login.rst
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/profile.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/session.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/url_redirection.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/req.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/rset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/urlpublishing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/urlrewrite.rst
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/web.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/
+-rw-rw-rw-   0 root         (0) root         (0)    14655 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-app.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7806 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/_maybe_to_integrate/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/rss-xml.rst
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/additionnal_services/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/additionnal_services/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/additionnal_services/undo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.121015 cubicweb-4.1.0/doc/book/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/backups.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/create-instance.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/cubicweb-ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4034 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/deploy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5172 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/instance-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/ldap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/multisources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/rql-logs.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/site-config.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.121015 cubicweb-4.1.0/doc/book/annexes/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/depends.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/docstrings-conventions.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/mercurial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.125015 cubicweb-4.1.0/doc/book/annexes/rql/
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/Graph-ex.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/implementation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5570 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)    27490 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/language.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/usecases.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.129016 cubicweb-4.1.0/doc/book/devrepo/
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/connections_pooler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.133015 cubicweb-4.1.0/doc/book/devrepo/cubes/
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/available-cubes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/cc-newcube.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/what-is-a-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/dataimport.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.133015 cubicweb-4.1.0/doc/book/devrepo/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/baseschema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6178 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/define-workflows.rst
+-rw-rw-rw-   0 root         (0) root         (0)    34880 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/definition.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/debug_channels.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.137015 cubicweb-4.1.0/doc/book/devrepo/devcore/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/devcore/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/devcore/reqbase.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.137015 cubicweb-4.1.0/doc/book/devrepo/entityclasses/
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/adapters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7268 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/application-logic.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/data-as-objects.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/load-sort.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4399 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/fti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9399 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/profiling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.141016 cubicweb-4.1.0/doc/book/devrepo/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/hooks.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11467 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/sessions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/tasks.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21316 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/vreg.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.145016 cubicweb-4.1.0/doc/book/devweb/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/controllers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/css.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.149016 cubicweb-4.1.0/doc/book/devweb/edition/
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/dissection.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/editcontroller.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9905 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15502 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/facets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/httpcaching.rst
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10057 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/internationalization.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/js.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/property.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/publisher.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/request.rst
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/resource.rst
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/rtags.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/searchbar.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.157016 cubicweb-4.1.0/doc/book/devweb/views/
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/basetemplates.rst
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/baseviews.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/boxes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/breadcrumbs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/idownloadable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10179 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/startup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/urlpublish.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/views.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/wdoc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/xmlrss.rst
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/warning.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.157016 cubicweb-4.1.0/doc/book/intro/
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/concepts.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/debug_toolbar.rst
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/settings.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/security/
+-rw-rw-rw-   0 root         (0) root         (0)     7880 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/security/csrf.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/src/archi_globale.dia
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/src/main_template_layout.dia
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.173016 cubicweb-4.1.0/doc/changes/
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.14.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.15.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.16.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.17.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.18.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.19.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.20.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.21.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.22.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.23.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.24.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.25.rst
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.26.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6870 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.27.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.28.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.29.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.30.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.31.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.32.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.32_reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.33.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4522 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.34.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.35.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.36.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5213 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.37.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.38.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7617 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.177016 cubicweb-4.1.0/doc/dev/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/coding_standards_css.rst
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/coding_standards_js.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/continuous-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/documenting.txt
+-rw-rw-rw-   0 root         (0) root         (0)    24407 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/features_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/install_from_sources.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/refactoring-the-css-with-uiprops.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    12650 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/breadcrumbs_header.png
+-rw-rw-rw-   0 root         (0) root         (0)    85073 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_general_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   124385 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_registry_content_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   111325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_registry_decisions_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   134505 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_rql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   192629 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_rql_traceback_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   107766 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_show_source.png
+-rw-rw-rw-   0 root         (0) root         (0)    55625 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_show_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)   126845 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_sql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)    97343 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_traceback_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)    57300 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/example-card-with-rql-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)    55168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/example-card-with-rql-table-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_date_range.png
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_has_image.png
+-rw-rw-rw-   0 root         (0) root         (0)    22016 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_overview.png
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_range.png
+-rw-rw-rw-   0 root         (0) root         (0)    21685 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_00-login_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30326 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_01-start_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    35859 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_02-cookie-values_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33922 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_02-create-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28123 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-list-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    82897 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-site-config-panel_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   119813 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-state-submitted_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    34771 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_04-detail-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_05-list-two-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    49230 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_06-add-relation-entryof_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    96838 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_06-main-template-logo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    40383 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_07-detail-one-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30591 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_08-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33091 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_09-new-view-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42230 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_10-blog-with-two-entries_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    17757 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template.png
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13842 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template_layout.png
+-rw-rw-rw-   0 root         (0) root         (0)    46411 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/primaryview_template.png
+-rw-rw-rw-   0 root         (0) root         (0)    14758 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/primaryview_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22773 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/request_session.png
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/request_session.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/server-class-diagram.png
+-rw-rw-rw-   0 root         (0) root         (0)    62022 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   105173 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    58500 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blogs-list_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   109769 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_form-generic-relations_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    65646 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    13605 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_gettext_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    88970 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_logged_in_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_login-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   100347 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    63097 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    62431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-default-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    74856 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    79709 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-custom-footer_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   128406 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    71500 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-siteinfo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   104834 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    22098 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_schema_graphviz_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   150520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_siteconfig_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    60672 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_admin.png
+-rw-rw-rw-   0 root         (0) root         (0)    61388 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_city_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    50694 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_city_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    71561 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_data_model_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)    48896 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_empty_instance.png
+-rw-rw-rw-   0 root         (0) root         (0)    55671 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_finished_import.png
+-rw-rw-rw-   0 root         (0) root         (0)    57063 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_list_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    70893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    61656 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    74005 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_with_city_name.png
+-rw-rw-rw-   0 root         (0) root         (0)   225824 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_react_map.png
+-rw-rw-rw-   0 root         (0) root         (0)    53544 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_with_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)   354637 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_background-image.png
+-rw-rw-rw-   0 root         (0) root         (0)    30437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_boxes.png
+-rw-rw-rw-   0 root         (0) root         (0)    54643 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_breadcrumbs.png
+-rw-rw-rw-   0 root         (0) root         (0)   324086 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_facets.png
+-rw-rw-rw-   0 root         (0) root         (0)    40520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_grey-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    16843 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_index-after.png
+-rw-rw-rw-   0 root         (0) root         (0)    26875 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_index-before.png
+-rw-rw-rw-   0 root         (0) root         (0)    17580 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_login-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    57814 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_prevnext.png
+-rw-rw-rw-   0 root         (0) root         (0)    81362 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui1.png
+-rw-rw-rw-   0 root         (0) root         (0)    93291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui2.png
+-rw-rw-rw-   0 root         (0) root         (0)   290338 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui3.png
+-rw-rw-rw-   0 root         (0) root         (0)    43051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_history-view_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    26036 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_mesage_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    39625 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_startup-link_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    17558 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-filter-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-filter.png
+-rw-rw-rw-   0 root         (0) root         (0)    12375 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table.png
+-rw-rw-rw-   0 root         (0) root         (0)     7225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/plan_formation_python_cubicweb.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/stdlib.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/generate_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/mode_plan.py
+-rwxrwxrwx   0 root         (0) root         (0)     4944 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/pyjsrest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/tutorials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.245017 cubicweb-4.1.0/doc/tutorials/advanced/
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part01_create-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part02_security.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5614 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part03_bfss.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15384 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part04_ui-base.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15114 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part05_ui-advanced.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.245017 cubicweb-4.1.0/doc/tutorials/base/
+-rw-rw-rw-   0 root         (0) root         (0)     3867 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/blog-in-five-minutes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/conclusion.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/customizing-the-application.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/discovering-the-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.249017 cubicweb-4.1.0/doc/tutorials/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     9014 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    29917 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6576 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/doc/tutorials/museum/
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/data-management.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/develop-app.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/develop-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8840 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/enhance-views.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/doc/tutorials/textreports/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/textreports/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/extras/
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-05 08:55:06.000000 cubicweb-4.1.0/extras/cubicweb-ctl.bash_completion
+-rw-rw-rw-   0 root         (0) root         (0)     7414 2023-07-05 08:55:06.000000 cubicweb-4.1.0/jshintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/man/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-05 08:55:06.000000 cubicweb-4.1.0/man/cubicweb-ctl.1
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-05 08:55:06.000000 cubicweb-4.1.0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-05 08:55:06.000000 cubicweb-4.1.0/pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.257017 cubicweb-4.1.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/from-forge.txt
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-base.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-dataimport.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-devtools.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-ext.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-hooks.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-pyramid.txt
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-server.txt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-05 08:55:37.257017 cubicweb-4.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8874 2023-07-05 08:55:06.000000 cubicweb-4.1.0/tox.ini
```

### Comparing `cubicweb-4.0.0/COPYING` & `cubicweb-4.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/COPYING.LESSER` & `cubicweb-4.1.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/MANIFEST.in` & `cubicweb-4.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/PKG-INFO` & `cubicweb-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.0.0
+Version: 4.1.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 Provides-Extra: captcha
```

### Comparing `cubicweb-4.0.0/README.rst` & `cubicweb-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/__init__.py` & `cubicweb-4.1.0/cubicweb/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb global packaging information for the cubicweb knowledge management
 software
 """
 
 modname = distname = "cubicweb"
 
-numversion = (4, 0, 0)
+numversion = (4, 1, 0)
 version = ".".join(str(num) for num in numversion)
 
 description = "a repository of entities / relations for knowledge management"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = "https://www.cubicweb.org"
 license = "LGPL"
```

### Comparing `cubicweb-4.0.0/cubicweb/_exceptions.py` & `cubicweb-4.1.0/cubicweb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/_gcdebug.py` & `cubicweb-4.1.0/cubicweb/_gcdebug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/appobject.py` & `cubicweb-4.1.0/cubicweb/appobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/crypto.py` & `cubicweb-4.1.0/cubicweb/crypto.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/cwconfig.py` & `cubicweb-4.1.0/cubicweb/cwconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,24 @@
                 "default": None,
                 "help": "web server root url",
                 "group": "main",
                 "level": 1,
             },
         ),
         (
+            "receives-base-url-path",
+            {
+                "type": "yn",
+                "default": True,
+                "help": "will the instance receives and handle a sub path if present on its base-url",
+                "group": "main",
+                "level": 1,
+            },
+        ),
+        (
             "allow-email-login",
             {
                 "type": "yn",
                 "default": False,
                 "help": "allow users to login with their primary email if set",
                 "group": "main",
                 "level": 2,
@@ -1305,15 +1315,15 @@
     ):
         """return a configuration instance for the given instance identifier"""
         cls.load_available_configs()
         try:
             from cubicweb_web.webconfig import WebAllInOneConfiguration
 
             configcls = WebAllInOneConfiguration
-        except ModuleNotFoundError:
+        except ImportError:
             from cubicweb.pyramid.config import AllInOneConfiguration
 
             configcls = AllInOneConfiguration
 
         return configcls(appid, debugmode, creating, log_to_file=log_to_file)
 
     @classmethod
```

### Comparing `cubicweb-4.0.0/cubicweb/cwctl.py` & `cubicweb-4.1.0/cubicweb/cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/cwgettext.py` & `cubicweb-4.1.0/cubicweb/cwgettext.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/cwvreg.py` & `cubicweb-4.1.0/cubicweb/cwvreg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/__init__.py` & `cubicweb-4.1.0/cubicweb/dataimport/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/csv.py` & `cubicweb-4.1.0/cubicweb/dataimport/csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/importer.py` & `cubicweb-4.1.0/cubicweb/dataimport/importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/massive_store.py` & `cubicweb-4.1.0/cubicweb/dataimport/massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/pgstore.py` & `cubicweb-4.1.0/cubicweb/dataimport/pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/stores.py` & `cubicweb-4.1.0/cubicweb/dataimport/stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/data/geonames.csv` & `cubicweb-4.1.0/cubicweb/dataimport/test/data/geonames.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/data/timeZones.txt` & `cubicweb-4.1.0/cubicweb/dataimport/test/data/timeZones.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/data-massimport/schema.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/test_csv.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/test_massive_store.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/test_massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/test_pgstore.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/test_pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/test_stores.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/test_stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/dataimport/test/unittest_importer.py` & `cubicweb-4.1.0/cubicweb/dataimport/test/unittest_importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/debug.py` & `cubicweb-4.1.0/cubicweb/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/__init__.py` & `cubicweb-4.1.0/cubicweb/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/apptest_config.py` & `cubicweb-4.1.0/cubicweb/devtools/apptest_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/data/qunit.css` & `cubicweb-4.1.0/cubicweb/devtools/data/qunit.css`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/data/qunit.js` & `cubicweb-4.1.0/cubicweb/devtools/data/qunit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/devctl.py` & `cubicweb-4.1.0/cubicweb/devtools/devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/fake.py` & `cubicweb-4.1.0/cubicweb/devtools/fake.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/fill.py` & `cubicweb-4.1.0/cubicweb/devtools/fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/fix_po_encoding` & `cubicweb-4.1.0/cubicweb/devtools/fix_po_encoding`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/htmlparser.py` & `cubicweb-4.1.0/cubicweb/devtools/htmlparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/httptest.py` & `cubicweb-4.1.0/cubicweb/devtools/httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/instrument.py` & `cubicweb-4.1.0/cubicweb/devtools/instrument.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/realdbtest.py` & `cubicweb-4.1.0/cubicweb/devtools/realdbtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/repotest.py` & `cubicweb-4.1.0/cubicweb/devtools/repotest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/stresstester.py` & `cubicweb-4.1.0/cubicweb/devtools/stresstester.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/data/firstnames.txt` & `cubicweb-4.1.0/cubicweb/devtools/test/data/firstnames.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/devtools/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/data/static/js_examples/utils.js` & `cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/unittest_dbfill.py` & `cubicweb-4.1.0/cubicweb/devtools/test/unittest_dbfill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/unittest_devctl.py` & `cubicweb-4.1.0/cubicweb/devtools/test/unittest_devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/unittest_fill.py` & `cubicweb-4.1.0/cubicweb/devtools/test/unittest_fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/unittest_i18n.py` & `cubicweb-4.1.0/cubicweb/devtools/test/unittest_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/test/unittest_testlib.py` & `cubicweb-4.1.0/cubicweb/devtools/test/unittest_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/devtools/testlib.py` & `cubicweb-4.1.0/cubicweb/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/__init__.py` & `cubicweb-4.1.0/cubicweb/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/adapters.py` & `cubicweb-4.1.0/cubicweb/entities/adapters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/authobjs.py` & `cubicweb-4.1.0/cubicweb/entities/authobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/lib.py` & `cubicweb-4.1.0/cubicweb/entities/lib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/schemaobjs.py` & `cubicweb-4.1.0/cubicweb/entities/schemaobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/sources.py` & `cubicweb-4.1.0/cubicweb/entities/sources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/test/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/entities/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/entities/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/test/unittest_base.py` & `cubicweb-4.1.0/cubicweb/entities/test/unittest_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """unit tests for cubicweb.entities.base module
 """
 
+from urllib.parse import urljoin
+
 from logilab.common.decorators import clear_cache
 from logilab.common.testlib import unittest_main
 
 from cubicweb.devtools import BASE_URL
 from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.entities import AnyEntity
 
@@ -226,15 +228,15 @@
         with self.admin_access.repo_cnx() as cnx:
             entity = cnx.create_entity("CWGroup", name="tmp")
             cnx.commit()
             serializer = entity.cw_adapt_to("ISerializable")
             expected = {
                 "cw_etype": "CWGroup",
                 "eid": entity.eid,
-                "cwuri": f"{BASE_URL}{entity.eid}",
+                "cwuri": urljoin(BASE_URL, str(entity.eid)),
                 "creation_date": entity.creation_date,
                 "modification_date": entity.modification_date,
                 "name": "tmp",
             }
             self.assertEqual(serializer.serialize(), expected)
```

### Comparing `cubicweb-4.0.0/cubicweb/entities/test/unittest_wfobjs.py` & `cubicweb-4.1.0/cubicweb/entities/test/unittest_wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entities/wfobjs.py` & `cubicweb-4.1.0/cubicweb/entities/wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/entity.py` & `cubicweb-4.1.0/cubicweb/entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/ext/__init__.py` & `cubicweb-4.1.0/cubicweb/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/ext/html4zope.py` & `cubicweb-4.1.0/cubicweb/ext/html4zope.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/ext/markdown.py` & `cubicweb-4.1.0/cubicweb/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/ext/test/unittest_markdown.py` & `cubicweb-4.1.0/cubicweb/ext/test/unittest_markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/__init__.py` & `cubicweb-4.1.0/cubicweb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/bookmark.py` & `cubicweb-4.1.0/cubicweb/hooks/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/email.py` & `cubicweb-4.1.0/cubicweb/hooks/email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/integrity.py` & `cubicweb-4.1.0/cubicweb/hooks/integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/metadata.py` & `cubicweb-4.1.0/cubicweb/hooks/metadata.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/notification.py` & `cubicweb-4.1.0/cubicweb/hooks/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/security.py` & `cubicweb-4.1.0/cubicweb/hooks/security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/synccomputed.py` & `cubicweb-4.1.0/cubicweb/hooks/synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/syncschema.py` & `cubicweb-4.1.0/cubicweb/hooks/syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/syncsession.py` & `cubicweb-4.1.0/cubicweb/hooks/syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/syncsources.py` & `cubicweb-4.1.0/cubicweb/hooks/syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/hooks/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/data-computed/schema.py` & `cubicweb-4.1.0/cubicweb/hooks/test/data-computed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_bookmarks.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_hooks.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_integrity.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_notificationhooks.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_notificationhooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_security.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_synccomputed.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncschema.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncsession.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/test/unittest_syncsources.py` & `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/hooks/workflow.py` & `cubicweb-4.1.0/cubicweb/hooks/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/i18n/de.po` & `cubicweb-4.1.0/cubicweb/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/i18n/en.po` & `cubicweb-4.1.0/cubicweb/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/i18n/es.po` & `cubicweb-4.1.0/cubicweb/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/i18n/fr.po` & `cubicweb-4.1.0/cubicweb/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/i18n.py` & `cubicweb-4.1.0/cubicweb/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/mail.py` & `cubicweb-4.1.0/cubicweb/mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/md5crypt.py` & `cubicweb-4.1.0/cubicweb/md5crypt.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/migration.py` & `cubicweb-4.1.0/cubicweb/migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/3.22.0_Any.py` & `cubicweb-4.1.0/cubicweb/misc/migration/3.22.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/3.23.0_Any.py` & `cubicweb-4.1.0/cubicweb/misc/migration/3.23.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/3.24.0_Any.py` & `cubicweb-4.1.0/cubicweb/misc/migration/3.24.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/3.24.4_Any.py` & `cubicweb-4.1.0/cubicweb/misc/migration/3.24.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/bootstrapmigration_repository.py` & `cubicweb-4.1.0/cubicweb/misc/migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/misc/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/scripts/chpasswd.py` & `cubicweb-4.1.0/cubicweb/misc/scripts/chpasswd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/scripts/fast_drop_entities.py` & `cubicweb-4.1.0/cubicweb/misc/scripts/fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/scripts/ldap_change_base_dn.py` & `cubicweb-4.1.0/cubicweb/misc/scripts/ldap_change_base_dn.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/scripts/migration_helper.py` & `cubicweb-4.1.0/cubicweb/misc/scripts/migration_helper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/misc/source_highlight.py` & `cubicweb-4.1.0/cubicweb/misc/source_highlight.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/mttransforms.py` & `cubicweb-4.1.0/cubicweb/mttransforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/multipart.py` & `cubicweb-4.1.0/cubicweb/multipart.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/predicates.py` & `cubicweb-4.1.0/cubicweb/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/__init__.py` & `cubicweb-4.1.0/cubicweb/pyramid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 """Pyramid interface to CubicWeb"""
 
 import atexit
 import logging
 import os
 import sys
 from configparser import ConfigParser
+from urllib.parse import urlparse
 
 import wsgicors
 from pyramid.config import Configurator
 from pyramid.exceptions import ConfigurationError
 from pyramid.settings import asbool, aslist
 
 from cubicweb.cwconfig import CubicWebConfiguration as cwcfg
@@ -246,14 +247,16 @@
     config.registry["cubicweb.registry"] = repo.vreg
 
     base_url = cwconfig["base-url"]
     assert base_url is not None, (
         "base-url isn't properly set, it can be an issue in CubicWeb source code or in your configuration."
         "In normal case, 'base-url' is defined by cwconfig.repository()."
     )
+    if cwconfig["receives-base-url-path"]:
+        config.route_prefix = urlparse(base_url).path
 
     if cwconfig.mode != "test":
 
         @atexit.register
         def shutdown_repo():
             if repo.shutting_down:
                 return
```

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/auth.py` & `cubicweb-4.1.0/cubicweb/pyramid/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/config.py` & `cubicweb-4.1.0/cubicweb/pyramid/config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/core.py` & `cubicweb-4.1.0/cubicweb/pyramid/core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/csrf.py` & `cubicweb-4.1.0/cubicweb/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_source_code.py` & `cubicweb-4.1.0/cubicweb/pyramid/debug_source_code.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako` & `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/debugtoolbar_panels.py` & `cubicweb-4.1.0/cubicweb/pyramid/debugtoolbar_panels.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/development.ini.tmpl` & `cubicweb-4.1.0/cubicweb/pyramid/development.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/predicates.py` & `cubicweb-4.1.0/cubicweb/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/pyramid.ini.tmpl` & `cubicweb-4.1.0/cubicweb/pyramid/pyramid.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/pyramidctl.py` & `cubicweb-4.1.0/cubicweb/pyramid/pyramidctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/resources.py` & `cubicweb-4.1.0/cubicweb/pyramid/resources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/rest_api.py` & `cubicweb-4.1.0/cubicweb/pyramid/rest_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/session.py` & `cubicweb-4.1.0/cubicweb/pyramid/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py` & `cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/test/test_config.py` & `cubicweb-4.1.0/cubicweb/pyramid/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/test/test_content_negociation.py` & `cubicweb-4.1.0/cubicweb/pyramid/test/test_content_negociation.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         # the resource does not exist since a "rest_attr" is defined for PublicBlogEntry
         res = self.webapp.get(
             f"{BASE_URL}PublicBlogEntry/{self.blog_entry.eid}", status=404
         )
         assert "The resource could not be found." in res.body.decode("utf-8")
 
     def test_content_negociation_alternate_eid(self):
-        res = self.webapp.get(f"/{self.blog_entry.eid}", headers={"Accept": "text/n3"})
+        res = self.webapp.get(
+            f"{BASE_URL}{self.blog_entry.eid}", headers={"Accept": "text/n3"}
+        )
 
         g = Graph()
         g.parse(data=res.body.decode("utf-8"), format="text/n3")
         ask_res = g.query(
             f"""
             PREFIX owl: <http://www.w3.org/2002/07/owl#>
             ASK {{
@@ -94,15 +96,15 @@
         response = self.webapp.get(
             f"{BASE_URL}{self.blog_entry.eid}", headers={"Accept": "text/n4"}
         )
         assert response.html
 
     def test_content_negociation_rest_attr(self):
         res = self.webapp.get(
-            f"/PublicBlogEntry/{self.blog_entry.unique_id}",
+            f"{BASE_URL}PublicBlogEntry/{self.blog_entry.unique_id}",
             headers={"Accept": "text/n3"},
         )
         g = Graph()
         g.parse(data=res.body.decode("utf-8"), format="text/n3")
         ask_res = g.query(
             f"""
             PREFIX owl: <http://www.w3.org/2002/07/owl#>
@@ -113,15 +115,17 @@
                     <http://ns.cubicweb.org/cubicweb/0.0/title> "{self.blog_entry.title}";
                     <http://ns.cubicweb.org/cubicweb/0.0/content> "{self.blog_entry.content}".
             }}"""
         )
         assert ask_res.askAnswer
 
     def test_content_negociation_etype_eid(self):
-        res = self.webapp.get(f"/Blog/{self.blog.eid}", headers={"Accept": "text/n3"})
+        res = self.webapp.get(
+            f"{BASE_URL}Blog/{self.blog.eid}", headers={"Accept": "text/n3"}
+        )
         g = Graph()
         g.parse(data=res.body.decode("utf-8"), format="text/n3")
         ask_res = g.query(
             f"""
             PREFIX owl: <http://www.w3.org/2002/07/owl#>
             ASK {{
                 <{BASE_URL}{self.blog.eid}> ^owl:sameAs ?x.
@@ -129,30 +133,32 @@
                     a <http://ns.cubicweb.org/cubicweb/0.0/Blog>;
                     <http://ns.cubicweb.org/cubicweb/0.0/title> "{self.blog.title}".
             }}"""
         )
         assert ask_res.askAnswer, res.body.decode("Utf-8")
 
     def test_content_negociation_cwuri_sameas(self):
-        res = self.webapp.get(f"/Blog/{self.blog.eid}", headers={"Accept": "text/n3"})
+        res = self.webapp.get(
+            f"{BASE_URL}Blog/{self.blog.eid}", headers={"Accept": "text/n3"}
+        )
         g = Graph()
         g.parse(data=res.body.decode("utf-8"), format="text/n3")
         ask_res = g.query(
             f"""
             PREFIX owl: <http://www.w3.org/2002/07/owl#>
             ASK {{
             <{self.blog.absolute_url()}>
                 owl:sameAs <{BASE_URL}{self.blog.eid}>.
             }}"""
         )
         assert ask_res.askAnswer, res.body.decode("Utf-8")
 
     def test_content_negociation_jsonld_triples_content(self):
         res = self.webapp.get(
-            f"/PublicBlogEntry/{self.blog_entry.unique_id}",
+            f"{BASE_URL}PublicBlogEntry/{self.blog_entry.unique_id}",
             headers={"Accept": "application/ld+json"},
         )
         g = Graph()
         g.parse(data=res.body.decode("utf-8"), format="json-ld")
         ask_res = g.query(
             f"""
             PREFIX owl: <http://www.w3.org/2002/07/owl#>
```

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/test/test_core.py` & `cubicweb-4.1.0/cubicweb/pyramid/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/test/test_tools.py` & `cubicweb-4.1.0/cubicweb/pyramid/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pyramid/tools.py` & `cubicweb-4.1.0/cubicweb/pyramid/tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/pytestconf.py` & `cubicweb-4.1.0/cubicweb/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/rdf.py` & `cubicweb-4.1.0/cubicweb/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/repoapi.py` & `cubicweb-4.1.0/cubicweb/repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/req.py` & `cubicweb-4.1.0/cubicweb/req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/rqlrewrite.py` & `cubicweb-4.1.0/cubicweb/rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/rqlsuggestions.py` & `cubicweb-4.1.0/cubicweb/rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/rset.py` & `cubicweb-4.1.0/cubicweb/rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/rtags.py` & `cubicweb-4.1.0/cubicweb/rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schema.py` & `cubicweb-4.1.0/cubicweb/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schema_exporters.py` & `cubicweb-4.1.0/cubicweb/schema_exporters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/Bookmark.py` & `cubicweb-4.1.0/cubicweb/schemas/Bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/__init__.py` & `cubicweb-4.1.0/cubicweb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/_regproc.postgres.sql` & `cubicweb-4.1.0/cubicweb/schemas/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/base.py` & `cubicweb-4.1.0/cubicweb/schemas/base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/bootstrap.py` & `cubicweb-4.1.0/cubicweb/schemas/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/schemas/workflow.py` & `cubicweb-4.1.0/cubicweb/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/__init__.py` & `cubicweb-4.1.0/cubicweb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/check_unused_index.py` & `cubicweb-4.1.0/cubicweb/server/check_unused_index.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/checkintegrity.py` & `cubicweb-4.1.0/cubicweb/server/checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/edition.py` & `cubicweb-4.1.0/cubicweb/server/edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/hook.py` & `cubicweb-4.1.0/cubicweb/server/hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/migractions.py` & `cubicweb-4.1.0/cubicweb/server/migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/querier.py` & `cubicweb-4.1.0/cubicweb/server/querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/repository.py` & `cubicweb-4.1.0/cubicweb/server/repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/rqlannotation.py` & `cubicweb-4.1.0/cubicweb/server/rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/schema2sql.py` & `cubicweb-4.1.0/cubicweb/server/schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/schemaserial.py` & `cubicweb-4.1.0/cubicweb/server/schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/serverconfig.py` & `cubicweb-4.1.0/cubicweb/server/serverconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/serverctl.py` & `cubicweb-4.1.0/cubicweb/server/serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/session.py` & `cubicweb-4.1.0/cubicweb/server/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/__init__.py` & `cubicweb-4.1.0/cubicweb/server/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/datafeed.py` & `cubicweb-4.1.0/cubicweb/server/sources/datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/ldapfeed.py` & `cubicweb-4.1.0/cubicweb/server/sources/ldapfeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/native.py` & `cubicweb-4.1.0/cubicweb/server/sources/native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/rql2sql.py` & `cubicweb-4.1.0/cubicweb/server/sources/rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sources/storages.py` & `cubicweb-4.1.0/cubicweb/server/sources/storages.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/sqlutils.py` & `cubicweb-4.1.0/cubicweb/server/sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/ssplanner.py` & `cubicweb-4.1.0/cubicweb/server/ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/ldap_test.ldif` & `cubicweb-4.1.0/cubicweb/server/test/data/ldap_test.ldif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data/slapd.conf.in` & `cubicweb-4.1.0/cubicweb/server/test/data/slapd.conf.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-cwep002/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-cwep002/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-migractions/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/Company.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Company.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/Dates.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/State.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/State.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/__init__.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schema2sql/schema/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schemaserial/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/datacomputed/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/datacomputed/schema.py` & `cubicweb-4.1.0/cubicweb/server/test/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_datafeed.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_edition.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_hook.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_ldapsource.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_ldapsource.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import unittest
 from os.path import join
+from urllib.parse import urljoin
 
 from yams import ValidationError
 from cubicweb import AuthenticationError
 from cubicweb.devtools import BASE_URL
 from cubicweb.devtools.httptest import get_available_port
 from cubicweb.devtools.testlib import CubicWebTC
 
@@ -291,15 +292,15 @@
         is not modified.
         If EmailAddress are not modified, CWGroup are not.
         """
         with self.admin_access.cnx() as cnx:
             user = cnx.find("CWUser", login="syt").one()
             user.cw_set(cw_source=cnx.find("CWSource", name="system").one())
             with cnx.security_enabled(write=False):
-                user.cw_set(cwuri=f"{BASE_URL}{user.eid}")
+                user.cw_set(cwuri=urljoin(BASE_URL, str(user.eid)))
                 for mail in user.use_email:
                     mail.cw_set(address=mail.address[:-3] + ".net")
             cnx.commit()
             with self.assertLogs("cubicweb.appobject", level="ERROR") as cm:
                 self.pull(cnx)
                 self.assertEqual(
                     cm.output,
```

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_querier.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_rql2sql.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_rqlannotation.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_schema2sql.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_schemaserial.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_server_security.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_server_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_server_utils.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_server_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_serverctl.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_session.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_sources_native.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_sources_native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_sqlutils.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_ssplanner.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_storage.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_storage.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_tools.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_undo.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_undo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test/unittest_utils.py` & `cubicweb-4.1.0/cubicweb/server/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py` & `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/data-migractions/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/datacomputed/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions/unittest_migractions.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/data-migractions/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/datacomputed/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions2/unittest_migractions.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions2/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/data-migractions/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/datacomputed/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_migractions3/unittest_migractions.py` & `cubicweb-4.1.0/cubicweb/server/test_migractions3/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/migration/postcreate.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_postgres/unittest_postgres.py` & `cubicweb-4.1.0/cubicweb/server/test_postgres/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/entities.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/hooks.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data-schemaserial/schema.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/test_repository/unittest_repository.py` & `cubicweb-4.1.0/cubicweb/server/test_repository/unittest_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/server/utils.py` & `cubicweb-4.1.0/cubicweb/server/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/README.rst.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/README.rst.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/setup.py.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py` & `cubicweb-4.1.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/skeleton/tox.ini.tmpl` & `cubicweb-4.1.0/cubicweb/skeleton/tox.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py` & `cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py` & `cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/__init__.py` & `cubicweb-4.1.0/cubicweb/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/ldapparser.py` & `cubicweb-4.1.0/cubicweb/sobjects/ldapparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/notification.py` & `cubicweb-4.1.0/cubicweb/sobjects/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/services.py` & `cubicweb-4.1.0/cubicweb/sobjects/services.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/supervising.py` & `cubicweb-4.1.0/cubicweb/sobjects/supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/data/sobjects/__init__.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/unittest_email.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/unittest_notification.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/unittest_register_user.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_register_user.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/sobjects/test/unittest_supervising.py` & `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/tags.py` & `cubicweb-4.1.0/cubicweb/tags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_comment/schema.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_forge/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/__init__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/cubicweb_tag/schema.py` & `cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/entities.py` & `cubicweb-4.1.0/cubicweb/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/erqlexpr_on_ertype.py` & `cubicweb-4.1.0/cubicweb/test/data/erqlexpr_on_ertype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.0.3_Any.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.0.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.0.4_Any.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.0.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_Any.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_common.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_common.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.1.0_repository.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/migration/0.1.2_Any.py` & `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.2_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/rqlexpr_on_ertype_read.py` & `cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_ertype_read.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/rrqlexpr_on_attr.py` & `cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_attr.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/rrqlexpr_on_eetype.py` & `cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_eetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/schema.py` & `cubicweb-4.1.0/cubicweb/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py` & `cubicweb-4.1.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py` & `cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py` & `cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data-rewrite/schema.py` & `cubicweb-4.1.0/cubicweb/test/data-rewrite/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/data_schemareader/schema.py` & `cubicweb-4.1.0/cubicweb/test/data_schemareader/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_binary.py` & `cubicweb-4.1.0/cubicweb/test/unittest_binary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_cwconfig.py` & `cubicweb-4.1.0/cubicweb/test/unittest_cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_cwctl.py` & `cubicweb-4.1.0/cubicweb/test/unittest_cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_entity.py` & `cubicweb-4.1.0/cubicweb/test/unittest_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """unit tests for cubicweb.web.views.entities module"""
 
 from datetime import datetime
+from urllib.parse import urljoin
 
 from logilab.common import tempattr
 from logilab.common.decorators import clear_cache
 
 from cubicweb import Binary
 from cubicweb.devtools import BASE_URL
 from cubicweb.devtools.testlib import CubicWebTC
@@ -991,15 +992,15 @@
             note = cnx.create_entity("Note", type="y")
             note.cw_set(ecrit_par=person.eid)
             self.assertEqual(len(person.reverse_ecrit_par), 2)
 
     def test_absolute_url_empty_field(self):
         with self.admin_access.cnx() as cnx:
             card = cnx.create_entity("Card", wikiid="", title="test")
-            self.assertEqual(card.absolute_url(), f"{BASE_URL}{card.eid}")
+            self.assertEqual(card.absolute_url(), urljoin(BASE_URL, str(card.eid)))
 
     def test_create_and_compare_entity(self):
         access = self.admin_access
         with access.cnx() as cnx:
             p1 = cnx.create_entity("Personne", nom="fayolle", prenom="alexandre")
             p2 = cnx.create_entity("Personne", nom="campeas", prenom="aurelien")
             note = cnx.create_entity("Note", type="z")
```

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_fast_drop_entities.py` & `cubicweb-4.1.0/cubicweb/test/unittest_fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_mail.py` & `cubicweb-4.1.0/cubicweb/test/unittest_mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_migration.py` & `cubicweb-4.1.0/cubicweb/test/unittest_migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_predicates.py` & `cubicweb-4.1.0/cubicweb/test/unittest_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_repoapi.py` & `cubicweb-4.1.0/cubicweb/test/unittest_repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_req.py` & `cubicweb-4.1.0/cubicweb/test/unittest_req.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
+from urllib.parse import urljoin
+
 from logilab.common.testlib import TestCase, unittest_main
 
 from cubicweb import Unauthorized
 from cubicweb.devtools import BASE_URL
 from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.req import RequestSessionAndConnectionBase
 
@@ -41,18 +43,18 @@
         )
 
     def test_build_url(self):
         req = RequestSessionAndConnectionBase(None)
         req.from_controller = lambda: "view"
         req.relative_path = lambda includeparams=True: None
         req.base_url = lambda: BASE_URL
-        self.assertEqual(req.build_url(), f"{BASE_URL}view")
-        self.assertEqual(req.build_url(None), f"{BASE_URL}view")
-        self.assertEqual(req.build_url("one"), f"{BASE_URL}one")
-        self.assertEqual(req.build_url(param="ok"), f"{BASE_URL}view?param=ok")
+        self.assertEqual(req.build_url(), urljoin(BASE_URL, "view"))
+        self.assertEqual(req.build_url(None), urljoin(BASE_URL, "view"))
+        self.assertEqual(req.build_url("one"), urljoin(BASE_URL, "one"))
+        self.assertEqual(req.build_url(param="ok"), urljoin(BASE_URL, "view?param=ok"))
         self.assertRaises(AssertionError, req.build_url, "one", "two not allowed")
         self.assertRaises(AssertionError, req.build_url, "view", test=None)
 
     def test_ensure_no_rql(self):
         req = RequestSessionAndConnectionBase(None)
         self.assertEqual(req.ensure_ro_rql("Any X WHERE X is CWUser"), None)
         self.assertEqual(req.ensure_ro_rql("  Any X WHERE X is CWUser  "), None)
```

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_rqlrewrite.py` & `cubicweb-4.1.0/cubicweb/test/unittest_rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_rqlsuggestions.py` & `cubicweb-4.1.0/cubicweb/test/unittest_rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_rset.py` & `cubicweb-4.1.0/cubicweb/test/unittest_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_rtags.py` & `cubicweb-4.1.0/cubicweb/test/unittest_rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_schema.py` & `cubicweb-4.1.0/cubicweb/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_toolsutils.py` & `cubicweb-4.1.0/cubicweb/test/unittest_toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_uilib.py` & `cubicweb-4.1.0/cubicweb/test/unittest_uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_vregistry.py` & `cubicweb-4.1.0/cubicweb/test/unittest_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/test/unittest_wfutils.py` & `cubicweb-4.1.0/cubicweb/test/unittest_wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/toolsutils.py` & `cubicweb-4.1.0/cubicweb/toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/transaction.py` & `cubicweb-4.1.0/cubicweb/transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/uilib.py` & `cubicweb-4.1.0/cubicweb/uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/utils.py` & `cubicweb-4.1.0/cubicweb/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/wfutils.py` & `cubicweb-4.1.0/cubicweb/wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb/xy.py` & `cubicweb-4.1.0/cubicweb/xy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/cubicweb.egg-info/PKG-INFO` & `cubicweb-4.1.0/cubicweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.0.0
+Version: 4.1.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 Provides-Extra: captcha
```

### Comparing `cubicweb-4.0.0/cubicweb.egg-info/SOURCES.txt` & `cubicweb-4.1.0/cubicweb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 cubicweb/i18n.py
 cubicweb/mail.py
 cubicweb/md5crypt.py
 cubicweb/migration.py
 cubicweb/mttransforms.py
 cubicweb/multipart.py
 cubicweb/predicates.py
-cubicweb/pylintext.py
 cubicweb/pytestconf.py
 cubicweb/rdf.py
 cubicweb/repoapi.py
 cubicweb/req.py
 cubicweb/rqlrewrite.py
 cubicweb/rqlsuggestions.py
 cubicweb/rset.py
@@ -926,22 +925,24 @@
 doc/changes/3.33.rst
 doc/changes/3.34.rst
 doc/changes/3.35.rst
 doc/changes/3.36.rst
 doc/changes/3.37.rst
 doc/changes/3.38.rst
 doc/changes/4.0.rst
+doc/changes/4.1.rst
 doc/changes/changelog.rst
 doc/changes/index.rst
 doc/dev/coding_standards_css.rst
 doc/dev/coding_standards_js.rst
 doc/dev/continuous-integration.rst
 doc/dev/documenting.txt
 doc/dev/features_list.rst
 doc/dev/index.rst
+doc/dev/install_from_sources.rst
 doc/dev/refactoring-the-css-with-uiprops.rst
 doc/images/03-transitions-view_en.png
 doc/images/breadcrumbs_header.png
 doc/images/debugtoolbar_general_panel.png
 doc/images/debugtoolbar_registry_content_panel.png
 doc/images/debugtoolbar_registry_decisions_panel.png
 doc/images/debugtoolbar_rql_panel.png
@@ -1046,19 +1047,20 @@
 doc/tutorials/base/discovering-the-ui.rst
 doc/tutorials/base/index.rst
 doc/tutorials/dataimport/diseasome_import.py
 doc/tutorials/dataimport/diseasome_parser.py
 doc/tutorials/dataimport/index.rst
 doc/tutorials/dataimport/schema.py
 doc/tutorials/museum/data-management.rst
+doc/tutorials/museum/develop-app.rst
+doc/tutorials/museum/develop-ui.rst
 doc/tutorials/museum/enhance-views.rst
 doc/tutorials/museum/getting-started.rst
 doc/tutorials/museum/index.rst
 doc/tutorials/textreports/index.rst
-doc/tutorials/tools/windmill.rst
 extras/cubicweb-ctl.bash_completion
 man/cubicweb-ctl.1
 requirements/dev.txt
 requirements/doc.txt
 requirements/from-forge.txt
 requirements/test-base.txt
 requirements/test-dataimport.txt
```

### Comparing `cubicweb-4.0.0/doc/4.0.0_how_to_migrate.rst` & `cubicweb-4.1.0/doc/4.0.0_how_to_migrate.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/Makefile` & `cubicweb-4.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/_static/favicon.ico` & `cubicweb-4.1.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/_static/logo-cubicweb.svg` & `cubicweb-4.1.0/doc/_static/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/announce.en.txt` & `cubicweb-4.1.0/doc/announce.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/announce.fr.txt` & `cubicweb-4.1.0/doc/announce.fr.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/api/__init__.rst` & `cubicweb-4.1.0/doc/api/__init__.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/api/cwvreg.rst` & `cubicweb-4.1.0/doc/api/cwvreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/api/predicates.rst` & `cubicweb-4.1.0/doc/api/predicates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/api/urlpublishing.rst` & `cubicweb-4.1.0/doc/api/urlpublishing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/api/web.rst` & `cubicweb-4.1.0/doc/api/web.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/MERGE_ME-tut-create-app.en.txt` & `cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt` & `cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/_maybe_to_integrate/rss-xml.rst` & `cubicweb-4.1.0/doc/book/_maybe_to_integrate/rss-xml.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/_maybe_to_integrate/template.rst` & `cubicweb-4.1.0/doc/book/_maybe_to_integrate/template.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/additionnal_services/undo.rst` & `cubicweb-4.1.0/doc/book/additionnal_services/undo.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/backups.rst` & `cubicweb-4.1.0/doc/book/admin/backups.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/config.rst` & `cubicweb-4.1.0/doc/book/admin/config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/create-instance.rst` & `cubicweb-4.1.0/doc/book/admin/create-instance.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/cubicweb-ctl.rst` & `cubicweb-4.1.0/doc/book/admin/cubicweb-ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/deploy.rst` & `cubicweb-4.1.0/doc/book/admin/deploy.rst`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     threads = 8
     plugins = http,python3
     auto-procname = true
     lazy-apps = true
     log-master = true
     disable-logging = true
 
-You can run it manualliy with:
+You can run it manually with:
 
 .. sourcecode:: console
 
     uwsgi --ini /etc/uwsgi/apps-enabled/example.ini
 
 Apache configuration
 ````````````````````
```

### Comparing `cubicweb-4.0.0/doc/book/admin/instance-config.rst` & `cubicweb-4.1.0/doc/book/admin/instance-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/ldap.rst` & `cubicweb-4.1.0/doc/book/admin/ldap.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/admin/site-config.rst` & `cubicweb-4.1.0/doc/book/admin/site-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/depends.rst` & `cubicweb-4.1.0/doc/book/annexes/depends.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/docstrings-conventions.rst` & `cubicweb-4.1.0/doc/book/annexes/docstrings-conventions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/faq.rst` & `cubicweb-4.1.0/doc/book/annexes/faq.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/mercurial.rst` & `cubicweb-4.1.0/doc/book/annexes/mercurial.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/Graph-ex.gif` & `cubicweb-4.1.0/doc/book/annexes/rql/Graph-ex.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/debugging.rst` & `cubicweb-4.1.0/doc/book/annexes/rql/debugging.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/implementation.rst` & `cubicweb-4.1.0/doc/book/annexes/rql/implementation.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/intro.rst` & `cubicweb-4.1.0/doc/book/annexes/rql/intro.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/language.rst` & `cubicweb-4.1.0/doc/book/annexes/rql/language.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/annexes/rql/usecases.rst` & `cubicweb-4.1.0/doc/book/annexes/rql/usecases.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/connections_pooler.rst` & `cubicweb-4.1.0/doc/book/devrepo/connections_pooler.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/cubes/available-cubes.rst` & `cubicweb-4.1.0/doc/book/devrepo/cubes/available-cubes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/cubes/cc-newcube.rst` & `cubicweb-4.1.0/doc/book/devrepo/cubes/cc-newcube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/cubes/layout.rst` & `cubicweb-4.1.0/doc/book/devrepo/cubes/layout.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/cubes/what-is-a-cube.rst` & `cubicweb-4.1.0/doc/book/devrepo/cubes/what-is-a-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/dataimport.rst` & `cubicweb-4.1.0/doc/book/devrepo/dataimport.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/datamodel/baseschema.rst` & `cubicweb-4.1.0/doc/book/devrepo/datamodel/baseschema.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/datamodel/define-workflows.rst` & `cubicweb-4.1.0/doc/book/devrepo/datamodel/define-workflows.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/datamodel/definition.rst` & `cubicweb-4.1.0/doc/book/devrepo/datamodel/definition.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/datamodel/metadata.rst` & `cubicweb-4.1.0/doc/book/devrepo/datamodel/metadata.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/debug_channels.rst` & `cubicweb-4.1.0/doc/book/devrepo/debug_channels.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/devcore/reqbase.rst` & `cubicweb-4.1.0/doc/book/devrepo/devcore/reqbase.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/entityclasses/adapters.rst` & `cubicweb-4.1.0/doc/book/devrepo/entityclasses/adapters.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/entityclasses/application-logic.rst` & `cubicweb-4.1.0/doc/book/devrepo/entityclasses/application-logic.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/entityclasses/data-as-objects.rst` & `cubicweb-4.1.0/doc/book/devrepo/entityclasses/data-as-objects.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/entityclasses/load-sort.rst` & `cubicweb-4.1.0/doc/book/devrepo/entityclasses/load-sort.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/fti.rst` & `cubicweb-4.1.0/doc/book/devrepo/fti.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/migration.rst` & `cubicweb-4.1.0/doc/book/devrepo/migration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/profiling.rst` & `cubicweb-4.1.0/doc/book/devrepo/profiling.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/repo/hooks.rst` & `cubicweb-4.1.0/doc/book/devrepo/repo/hooks.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/repo/notifications.rst` & `cubicweb-4.1.0/doc/book/devrepo/repo/notifications.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/repo/sessions.rst` & `cubicweb-4.1.0/doc/book/devrepo/repo/sessions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/testing.rst` & `cubicweb-4.1.0/doc/book/devrepo/testing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devrepo/vreg.rst` & `cubicweb-4.1.0/doc/book/devrepo/vreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/ajax.rst` & `cubicweb-4.1.0/doc/book/devweb/ajax.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/controllers.rst` & `cubicweb-4.1.0/doc/book/devweb/controllers.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/css.rst` & `cubicweb-4.1.0/doc/book/devweb/css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/edition/dissection.rst` & `cubicweb-4.1.0/doc/book/devweb/edition/dissection.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/edition/editcontroller.rst` & `cubicweb-4.1.0/doc/book/devweb/edition/editcontroller.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/edition/examples.rst` & `cubicweb-4.1.0/doc/book/devweb/edition/examples.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/edition/form.rst` & `cubicweb-4.1.0/doc/book/devweb/edition/form.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/facets.rst` & `cubicweb-4.1.0/doc/book/devweb/facets.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/httpcaching.rst` & `cubicweb-4.1.0/doc/book/devweb/httpcaching.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/internationalization.rst` & `cubicweb-4.1.0/doc/book/devweb/internationalization.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/js.rst` & `cubicweb-4.1.0/doc/book/devweb/js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/publisher.rst` & `cubicweb-4.1.0/doc/book/devweb/publisher.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/request.rst` & `cubicweb-4.1.0/doc/book/devweb/request.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/resource.rst` & `cubicweb-4.1.0/doc/book/devweb/resource.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/searchbar.rst` & `cubicweb-4.1.0/doc/book/devweb/searchbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/basetemplates.rst` & `cubicweb-4.1.0/doc/book/devweb/views/basetemplates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/baseviews.rst` & `cubicweb-4.1.0/doc/book/devweb/views/baseviews.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/boxes.rst` & `cubicweb-4.1.0/doc/book/devweb/views/boxes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/breadcrumbs.rst` & `cubicweb-4.1.0/doc/book/devweb/views/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/idownloadable.rst` & `cubicweb-4.1.0/doc/book/devweb/views/idownloadable.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/primary.rst` & `cubicweb-4.1.0/doc/book/devweb/views/primary.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/reledit.rst` & `cubicweb-4.1.0/doc/book/devweb/views/reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/startup.rst` & `cubicweb-4.1.0/doc/book/devweb/views/startup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/table.rst` & `cubicweb-4.1.0/doc/book/devweb/views/table.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/urlpublish.rst` & `cubicweb-4.1.0/doc/book/devweb/views/urlpublish.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/views.rst` & `cubicweb-4.1.0/doc/book/devweb/views/views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/views/xmlrss.rst` & `cubicweb-4.1.0/doc/book/devweb/views/xmlrss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/devweb/warning.rst` & `cubicweb-4.1.0/doc/book/devweb/warning.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/intro/concepts.rst` & `cubicweb-4.1.0/doc/book/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/intro/history.rst` & `cubicweb-4.1.0/doc/book/intro/history.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/pyramid/auth.rst` & `cubicweb-4.1.0/doc/book/pyramid/auth.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Note that this module only provides an authentication policy, not the views
     that handle the login form. See :ref:`login_module`
 
 Customize
 ---------
 
 The default policies can be individually deactivated, as well as the default
-authentication callback that returns the current user groups as :term:`principals`.
+authentication callback that returns the current user groups as `principals`.
 
 The following settings can be set to `False`:
 
 -   :confval:`cubicweb.auth.update_login_time`. Activate the policy that update
     the user `login_time` when `remember` is called.
 -   :confval:`cubicweb.auth.authtkt` and all its subvalues.
 -   :confval:`cubicweb.auth.groups_principals`
```

### Comparing `cubicweb-4.0.0/doc/book/pyramid/ctl.rst` & `cubicweb-4.1.0/doc/book/pyramid/ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/pyramid/debug_toolbar.rst` & `cubicweb-4.1.0/doc/book/pyramid/debug_toolbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/pyramid/index.rst` & `cubicweb-4.1.0/doc/book/pyramid/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/pyramid/quickstart.rst` & `cubicweb-4.1.0/doc/book/pyramid/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/pyramid/settings.rst` & `cubicweb-4.1.0/doc/book/pyramid/settings.rst`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     :ref:`cubicweb-ctl_pyramid`.
 
 .. confval:: cubicweb.debug (bool)
 
     Enables the cubicweb debugmode. Works only if the instance is setup by
     :confval:`cubicweb.instance`.
 
-    Unlike when the debugmode is set by the :option:`cubicweb-ctl start --debug-mode`
+    Unlike when the debugmode is set by the `cubicweb-ctl start --debug-mode`
     command, the pyramid debug options are untouched.
 
 .. confval:: cubicweb.includes (list)
 
     Same as ``pyramid.includes``, but the includes are done after the cubicweb
     specific registry entries are initialized.
```

### Comparing `cubicweb-4.0.0/doc/book/security/csrf.rst` & `cubicweb-4.1.0/doc/book/security/csrf.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/src/archi_globale.dia` & `cubicweb-4.1.0/doc/book/src/archi_globale.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/book/src/main_template_layout.dia` & `cubicweb-4.1.0/doc/book/src/main_template_layout.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.14.rst` & `cubicweb-4.1.0/doc/changes/3.14.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.15.rst` & `cubicweb-4.1.0/doc/changes/3.15.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.16.rst` & `cubicweb-4.1.0/doc/changes/3.16.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.17.rst` & `cubicweb-4.1.0/doc/changes/3.17.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.18.rst` & `cubicweb-4.1.0/doc/changes/3.18.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.19.rst` & `cubicweb-4.1.0/doc/changes/3.19.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.20.rst` & `cubicweb-4.1.0/doc/changes/3.20.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.21.rst` & `cubicweb-4.1.0/doc/changes/3.21.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.22.rst` & `cubicweb-4.1.0/doc/changes/3.22.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.23.rst` & `cubicweb-4.1.0/doc/changes/3.23.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.24.rst` & `cubicweb-4.1.0/doc/changes/3.24.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.25.rst` & `cubicweb-4.1.0/doc/changes/3.25.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.27.rst` & `cubicweb-4.1.0/doc/changes/3.27.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.28.rst` & `cubicweb-4.1.0/doc/changes/3.28.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.29.rst` & `cubicweb-4.1.0/doc/changes/3.29.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.30.rst` & `cubicweb-4.1.0/doc/changes/3.30.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.31.rst` & `cubicweb-4.1.0/doc/changes/3.31.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.32.rst` & `cubicweb-4.1.0/doc/changes/3.32.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.32_reledit.rst` & `cubicweb-4.1.0/doc/changes/3.32_reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.33.rst` & `cubicweb-4.1.0/doc/changes/3.33.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.34.rst` & `cubicweb-4.1.0/doc/changes/3.34.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.35.rst` & `cubicweb-4.1.0/doc/changes/3.35.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.36.rst` & `cubicweb-4.1.0/doc/changes/3.36.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/changes/3.37.rst` & `cubicweb-4.1.0/doc/changes/3.37.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.37.16 (2023-06-07)
+====================
+👷 Bug fixes
+-----------
+
+- pyramid: allows to use None for timeout, max_age and reissue_time options
+
 3.37.15 (2023-03-24)
 ====================
 👷 Bug fixes
 -----------
 
 - testlib: define properly a generate_tzdatetime method with timezone (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/716)
```

### Comparing `cubicweb-4.0.0/doc/changes/3.38.rst` & `cubicweb-4.1.0/doc/changes/3.38.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.38.9 (2023-06-07)
+===================
+👷 Bug fixes
+-----------
+
+- pyramid: allows to use None for timeout, max_age and reissue_time options
+
 3.38.8 (2023-03-24)
 ===================
 👷 Bug fixes
 -----------
 
 - testlib: define properly a generate_tzdatetime method with timezone (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/716)
```

### Comparing `cubicweb-4.0.0/doc/changes/4.0.rst` & `cubicweb-4.1.0/doc/changes/4.0.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,33 @@
 - in RQL satements, :code:`NOW` and :code:`TODAY` are now evaluated differently depending on the entity type they represent (:code:`Datetime`, :code:`TZDateTime` or :code:`Date`), leading to more predictible behaviour
 
 Breaking changes
 ----------------
 
 - remove all :code:`cubicweb_web` retrocompatibility
 - content_negociation: use :code:`cubicweb.include` to include or not rdf/html views
-- autotest: move :code:`AutoPopulateTest` and :code:`AutomaticWebTest`to :code:`cubicweb_web.devtools.testlib`
+- autotest: move :code:`AutoPopulateTest` and :code:`AutomaticWebTest` to :code:`cubicweb_web.devtools.testlib`
 - bwcompat: move :code:`cubicweb.pyramid.bwcompat` to :code:`cubicweb_web.bwcompat`
 - move :code:`cubicweb.ext.rest` to :code:`cubicweb_web.ext.rest`
 - move :code:`cubicweb.predicates.paginated_rset` to :code:`cubicweb_web`
 - move :code:`cubicweb.pyramid.url_redirections` to :code:`cubicweb_web`
 - move :code:`CubicWebPyramidRequest` to :code:`cubicweb_web`
 - move :code:`has_cw_permission` pyramid predicates to :code:`cubicweb_web`
 - move :code:`ResultSet.limited_rql` to :code:`cubicweb_web.views.navigation.limited_rql`
 - move :code:`cubicweb.server.utils.HTMLHead` and :code:`cubicweb.server.utils.HTMLStream` to :code:`cubicweb_web.utils`
 - move :code:`cubicweb/pyramid/test/test_hooks.py` to :code:`cubicweb_web`
 - move :code:`test_sanitized_html` to :code:`cubicweb_web`
 - move back :code:`WebCreateHandler` from :code:`cubicweb_web` to :code:`cubicweb`
-- pyramid.ini: remove :code:`cubicweb.pyramid.defaults` and add specific option for auth and session (see :ref:`Migration guide  <migration-to-v4-pyramid>)
+- pyramid.ini: remove :code:`cubicweb.pyramid.defaults` and add specific option for auth and session (see :ref:`Migration guide <migration-to-v4-pyramid>`)
 - pyramid: include :code:`cubicweb.pyramid.core` after :code:`cubicweb.include` from pyramid.ini
-- config: :code:`BaseApptestConfiguration` now inherits from :code:`AllInOneConfiguration) (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/659)
+- config: :code:`BaseApptestConfiguration` now inherits from :code:`AllInOneConfiguration`) (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/659)
 - config: merge :code:`ApptestConfiguration` into :code:`BaseApptestConfiguration`,
   merge :code:`devtools.TestServerConfiguration` into :code:`devtools.apptest_config.BaseApptestConfiguration`,
   merge :code:`server.serverconfig.ServerConfiguration` into :code:`cwconfig.CubicWebConfiguration`,
-  drop :code:`devtools.RealDatabaseConfiguration` class `
-(https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/659)
+  drop :code:`devtools.RealDatabaseConfiguration` class (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/659)
 - services: remove :code:`CubicWebRequestBase` from :code:`repo_gc_stats`
 - testlib: move web related method from :code:`devtools.testlib.CubicWebTC` to :code:`cubicweb_web` (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/688)
 - remove all CSRF and login related code from :code:`cubicweb.pyramid.test` classes
 - remove :code:`WebConfiguration` from CubicWeb
 - rename :code:`cubicweb-ctl pyramid` command to :code:`cubicweb-ctl start`
 
 🎉 New features
```

### Comparing `cubicweb-4.0.0/doc/changes/changelog.rst` & `cubicweb-4.1.0/doc/changes/changelog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .. -*- coding: utf-8 -*-
 
+.. include:: 4.1.rst
 .. include:: 4.0.rst
 
 .. include:: 3.38.rst
 .. include:: 3.37.rst
 .. include:: 3.36.rst
 
 .. include:: 3.35.rst
```

### Comparing `cubicweb-4.0.0/doc/conf.py` & `cubicweb-4.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/coding_standards_css.rst` & `cubicweb-4.1.0/doc/dev/coding_standards_css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/coding_standards_js.rst` & `cubicweb-4.1.0/doc/dev/coding_standards_js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/continuous-integration.rst` & `cubicweb-4.1.0/doc/dev/continuous-integration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/documenting.txt` & `cubicweb-4.1.0/doc/dev/documenting.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/features_list.rst` & `cubicweb-4.1.0/doc/dev/features_list.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/dev/refactoring-the-css-with-uiprops.rst` & `cubicweb-4.1.0/doc/dev/refactoring-the-css-with-uiprops.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/03-transitions-view_en.png` & `cubicweb-4.1.0/doc/images/03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/breadcrumbs_header.png` & `cubicweb-4.1.0/doc/images/breadcrumbs_header.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_general_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_general_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_registry_content_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_registry_content_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_registry_decisions_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_registry_decisions_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_rql_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_rql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_rql_traceback_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_rql_traceback_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_show_source.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_show_source.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_show_source_link.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_show_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_sql_panel.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_sql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/debugtoolbar_traceback_source_link.png` & `cubicweb-4.1.0/doc/images/debugtoolbar_traceback_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/example-card-with-rql-directive.png` & `cubicweb-4.1.0/doc/images/example-card-with-rql-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/example-card-with-rql-table-directive.png` & `cubicweb-4.1.0/doc/images/example-card-with-rql-table-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/facet_date_range.png` & `cubicweb-4.1.0/doc/images/facet_date_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/facet_has_image.png` & `cubicweb-4.1.0/doc/images/facet_has_image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/facet_overview.png` & `cubicweb-4.1.0/doc/images/facet_overview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/facet_range.png` & `cubicweb-4.1.0/doc/images/facet_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_00-login_en.png` & `cubicweb-4.1.0/doc/images/lax-book_00-login_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_01-start_en.png` & `cubicweb-4.1.0/doc/images/lax-book_01-start_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_02-cookie-values_en.png` & `cubicweb-4.1.0/doc/images/lax-book_02-cookie-values_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_02-create-blog_en.png` & `cubicweb-4.1.0/doc/images/lax-book_02-create-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_03-list-one-blog_en.png` & `cubicweb-4.1.0/doc/images/lax-book_03-list-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_03-site-config-panel_en.png` & `cubicweb-4.1.0/doc/images/lax-book_03-site-config-panel_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_03-state-submitted_en.png` & `cubicweb-4.1.0/doc/images/lax-book_03-state-submitted_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_03-transitions-view_en.png` & `cubicweb-4.1.0/doc/images/lax-book_03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_04-detail-one-blog_en.png` & `cubicweb-4.1.0/doc/images/lax-book_04-detail-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_05-list-two-blog_en.png` & `cubicweb-4.1.0/doc/images/lax-book_05-list-two-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_06-add-relation-entryof_en.png` & `cubicweb-4.1.0/doc/images/lax-book_06-add-relation-entryof_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_06-main-template-logo_en.png` & `cubicweb-4.1.0/doc/images/lax-book_06-main-template-logo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_07-detail-one-blogentry_en.png` & `cubicweb-4.1.0/doc/images/lax-book_07-detail-one-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_08-schema_en.png` & `cubicweb-4.1.0/doc/images/lax-book_08-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_09-new-view-blogentry_en.png` & `cubicweb-4.1.0/doc/images/lax-book_09-new-view-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/lax-book_10-blog-with-two-entries_en.png` & `cubicweb-4.1.0/doc/images/lax-book_10-blog-with-two-entries_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/main_template.png` & `cubicweb-4.1.0/doc/images/main_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/main_template.svg` & `cubicweb-4.1.0/doc/images/main_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/main_template_layout.png` & `cubicweb-4.1.0/doc/images/main_template_layout.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/primaryview_template.png` & `cubicweb-4.1.0/doc/images/primaryview_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/primaryview_template.svg` & `cubicweb-4.1.0/doc/images/primaryview_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/request_session.png` & `cubicweb-4.1.0/doc/images/request_session.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/request_session.svg` & `cubicweb-4.1.0/doc/images/request_session.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/server-class-diagram.png` & `cubicweb-4.1.0/doc/images/server-class-diagram.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_blog-form_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_blog-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_blog-primary_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_blog-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_blogs-list_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_blogs-list_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_form-generic-relations_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_form-generic-relations_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_index_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_index_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_index_gettext_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_index_gettext_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_index_logged_in_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_index_logged_in_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_login-form_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_login-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-community-custom-primary_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-custom-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-community-default-primary_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-default-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-custom-footer_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-custom-footer_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-schema_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_myblog-siteinfo_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_myblog-siteinfo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_schema_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_schema_graphviz_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_schema_graphviz_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-base_siteconfig_en.png` & `cubicweb-4.1.0/doc/images/tutos-base_siteconfig_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_admin.png` & `cubicweb-4.1.0/doc/images/tutos-museum_admin.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_city_created.png` & `cubicweb-4.1.0/doc/images/tutos-museum_city_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_city_creation.png` & `cubicweb-4.1.0/doc/images/tutos-museum_city_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_data_model_schema.png` & `cubicweb-4.1.0/doc/images/tutos-museum_data_model_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_empty_instance.png` & `cubicweb-4.1.0/doc/images/tutos-museum_empty_instance.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_finished_import.png` & `cubicweb-4.1.0/doc/images/tutos-museum_finished_import.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_list_view.png` & `cubicweb-4.1.0/doc/images/tutos-museum_list_view.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_museum_created.png` & `cubicweb-4.1.0/doc/images/tutos-museum_museum_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_museum_creation.png` & `cubicweb-4.1.0/doc/images/tutos-museum_museum_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_museum_with_city_name.png` & `cubicweb-4.1.0/doc/images/tutos-museum_museum_with_city_name.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_react_map.png` & `cubicweb-4.1.0/doc/images/tutos-museum_react_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-museum_with_schema.png` & `cubicweb-4.1.0/doc/images/tutos-museum_with_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_background-image.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_background-image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_boxes.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_boxes.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_breadcrumbs.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_breadcrumbs.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_facets.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_facets.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_grey-box.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_grey-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_index-after.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_index-after.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_index-before.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_index-before.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_login-box.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_login-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_prevnext.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_prevnext.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_ui1.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui1.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_ui2.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui2.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/tutos-photowebsite_ui3.png` & `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui3.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/undo_history-view_w600.png` & `cubicweb-4.1.0/doc/images/undo_history-view_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/undo_mesage_w600.png` & `cubicweb-4.1.0/doc/images/undo_mesage_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/undo_startup-link_w600.png` & `cubicweb-4.1.0/doc/images/undo_startup-link_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/views-table-filter-shadow.png` & `cubicweb-4.1.0/doc/images/views-table-filter-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/views-table-filter.png` & `cubicweb-4.1.0/doc/images/views-table-filter.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/views-table-shadow.png` & `cubicweb-4.1.0/doc/images/views-table-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/images/views-table.png` & `cubicweb-4.1.0/doc/images/views-table.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/index.rst` & `cubicweb-4.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/plan_formation_python_cubicweb.txt` & `cubicweb-4.1.0/doc/plan_formation_python_cubicweb.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tools/generate_modules.py` & `cubicweb-4.1.0/doc/tools/generate_modules.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tools/mode_plan.py` & `cubicweb-4.1.0/doc/tools/mode_plan.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tools/pyjsrest.py` & `cubicweb-4.1.0/doc/tools/pyjsrest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/index.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/part01_create-cube.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/part01_create-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/part02_security.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/part02_security.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/part03_bfss.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/part03_bfss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/part04_ui-base.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/part04_ui-base.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/advanced/part05_ui-advanced.rst` & `cubicweb-4.1.0/doc/tutorials/advanced/part05_ui-advanced.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/base/blog-in-five-minutes.rst` & `cubicweb-4.1.0/doc/tutorials/base/blog-in-five-minutes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/base/conclusion.rst` & `cubicweb-4.1.0/doc/tutorials/base/conclusion.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/base/customizing-the-application.rst` & `cubicweb-4.1.0/doc/tutorials/base/customizing-the-application.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/base/discovering-the-ui.rst` & `cubicweb-4.1.0/doc/tutorials/base/discovering-the-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/base/index.rst` & `cubicweb-4.1.0/doc/tutorials/base/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/dataimport/diseasome_import.py` & `cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_import.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/dataimport/diseasome_parser.py` & `cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_parser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/dataimport/index.rst` & `cubicweb-4.1.0/doc/tutorials/dataimport/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/dataimport/schema.py` & `cubicweb-4.1.0/doc/tutorials/dataimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/doc/tutorials/index.rst` & `cubicweb-4.1.0/doc/tutorials/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -13,11 +13,10 @@
 The other tutorials cover specific topics you can learn about when you understand the basics.
 
 .. toctree::
     :maxdepth: 1
 
     base/index
     advanced/index
-    tools/windmill
     textreports/index
     dataimport/index
     museum/index
```

### Comparing `cubicweb-4.0.0/doc/tutorials/museum/data-management.rst` & `cubicweb-4.1.0/doc/tutorials/museum/data-management.rst`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 * ``with admincnx(appid) as cnx`` allows to have an admin access to our instance, and then
   be able to create new entities.
 
 Thus, to execute our import command, we just have to enter in our shell (within our virtual env):
 
 .. code-block:: console
 
-    cubicweb-ctl import-museums tuto_instance <path_to_the_csv>
+    cubicweb-ctl import-museums tutorial_instance <path_to_the_csv>
 
 After this script, we should be able to see that we have much more cities and museums by
 visiting the homepage of our CubicWeb instance:
 
 .. image:: ../../images/tutos-museum_finished_import.png
    :alt: A CubicWeb instance with several cities and museums.
 
@@ -150,8 +150,8 @@
 ~~~~~~~~~~~~~~~~~
 
 .. TODO complete documentation
 
 Content negotiation
 ~~~~~~~~~~~~~~~~~~~
 
-.. TODO complete documentation
+.. TODO complete documentation
```

### Comparing `cubicweb-4.0.0/doc/tutorials/museum/enhance-views.rst` & `cubicweb-4.1.0/doc/tutorials/museum/enhance-views.rst`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
     npm run build
 
 And then, run our application:
 
 .. code-block:: console
 
-    cubicweb-ctl start -D tuto_instance
+    cubicweb-ctl start -D tutorial_instance
 
 We now have a world map displaying the location of our museum on museum pages.
 A lot of things could be done to have a better result, like center the map on the museum,
 but it's out of the scope of this tutorial.
 
 .. image:: ../../images/tutos-museum_react_map.png
    :alt: Our application with a World Map.
```

### Comparing `cubicweb-4.0.0/doc/tutorials/museum/index.rst` & `cubicweb-4.1.0/doc/tutorials/museum/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 .. -*- coding: utf-8 -*-
 
 .. _TutosMuseums:
 
-Create a Website from scratch with CubicWeb
-===========================================
+Create a data-oriented web application CubicWeb 4
+=================================================
 
 Introduction
 ------------
 
-This tutorial aims to demonstrate how to create a website using CubicWeb. This website will
-present museums from French Ministry of Culture data, available here_.
+This tutorial aims to demonstrate how to create a data-oriented web application
+using CubicWeb 4. This application will be a catalog of museums using data_
+from the French Ministry of Culture.
 
-.. _here: https://data.culture.gouv.fr/explore/dataset/liste-et-localisation-des-musees-de-france/export/
+.. _data: https://data.culture.gouv.fr/explore/dataset/liste-et-localisation-des-musees-de-france/export/
 
-First, we will start with installation and creation of our website, and a short presentation of
-out of the box CubicWeb functionalities. Then, we will see how to enhance our views using Jinja2
-templates or React components to have a better looking site. Finally, we will see how to manage
-more data, and how to serialize them in RDF.
+To get started, we will setup a development environment for CubicWeb, then
+create an instance and check that it is accessible with a web browser.
 
-At the end of this tutorial, you will have a website giving information about all France's
-museums, describes them in RDF and present them on a map.
+As a second step, we will define the data model of the application, re-create
+the database of the instance with this new schema, then check that a generic
+admin interface provided by the `web` cube (server component) allows us to add
+and display cities and museums.
 
-You can find the code of the finished tutorial in our forge, look for the cube tuto_.
+.. _web: https://forge.extranet.logilab.fr/cubicweb/cubes/web
 
-.. _tuto: https://forge.extranet.logilab.fr/cubicweb/cubes/tuto/
+As a third step, we will quickly develop an independant user interface using
+NextJS and ReactJS, that will query the database using the RQL language and
+display the museums on a map.
+
+As a fourth and final step, we will load the data downloaded form the repository
+of the French Ministry of Culture, then expose that data using content
+negotiation and the RDF standard.
 
+You can find the code of the finished tutorial in our forge, by looking for the
+cube tuto_.
+
+.. _tuto: https://forge.extranet.logilab.fr/cubicweb/cubes/tuto/
 .. toctree::
    :maxdepth: 2
 
    getting-started
+   develop-app
+   develop-ui
    enhance-views
    data-management
```

### Comparing `cubicweb-4.0.0/extras/cubicweb-ctl.bash_completion` & `cubicweb-4.1.0/extras/cubicweb-ctl.bash_completion`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/jshintrc` & `cubicweb-4.1.0/jshintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/man/cubicweb-ctl.1` & `cubicweb-4.1.0/man/cubicweb-ctl.1`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/pylintrc` & `cubicweb-4.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/setup.py` & `cubicweb-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.0.0/tox.ini` & `cubicweb-4.1.0/tox.ini`

 * *Files identical despite different names*

