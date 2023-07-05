# Comparing `tmp/ZEO-5.4.0.tar.gz` & `tmp/ZEO-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZEO-5.4.0.tar", last modified: Wed Jan 18 17:12:13 2023, max compression
+gzip compressed data, was "ZEO-5.4.1.tar", last modified: Wed Jul  5 15:30:49 2023, max compression
```

## Comparing `ZEO-5.4.0.tar` & `ZEO-5.4.1.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.604331 ZEO-5.4.0/
--rw-r--r--   0 jens       (501) staff       (20)    14880 2023-01-18 17:11:23.000000 ZEO-5.4.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2022-05-12 07:25:22.000000 ZEO-5.4.0/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       91 2021-11-02 08:52:31.000000 ZEO-5.4.0/COPYING
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:31.000000 ZEO-5.4.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:31.000000 ZEO-5.4.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      557 2023-01-18 15:11:08.000000 ZEO-5.4.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    17294 2023-01-18 17:12:13.604410 ZEO-5.4.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      949 2021-11-02 08:52:31.000000 ZEO-5.4.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      458 2021-11-02 08:52:31.000000 ZEO-5.4.0/buildout.cfg
--rw-r--r--   0 jens       (501) staff       (20)        8 2021-11-02 08:52:31.000000 ZEO-5.4.0/doc-requirements.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.590522 ZEO-5.4.0/docs/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.586826 ZEO-5.4.0/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.586867 ZEO-5.4.0/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.591838 ZEO-5.4.0/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)     2856 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/blob-nfs.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/changelog.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     7734 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/client-cache-tracing.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1882 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/client-cache.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10099 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/clients.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1257 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5470 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/introduction.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       35 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/nagios.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9961 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/ordering.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2374 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/protocol.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      326 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/reference.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     8178 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/_build/html/_sources/server.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2856 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/blob-nfs.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/changelog.rst
--rw-r--r--   0 jens       (501) staff       (20)     7734 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/client-cache-tracing.rst
--rw-r--r--   0 jens       (501) staff       (20)     1882 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/client-cache.rst
--rw-r--r--   0 jens       (501) staff       (20)    10099 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/clients.rst
--rw-r--r--   0 jens       (501) staff       (20)     8406 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)     1257 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5470 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/introduction.rst
--rw-r--r--   0 jens       (501) staff       (20)       35 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/nagios.rst
--rw-r--r--   0 jens       (501) staff       (20)     9961 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/ordering.rst
--rw-r--r--   0 jens       (501) staff       (20)     2374 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/protocol.rst
--rw-r--r--   0 jens       (501) staff       (20)      326 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/reference.rst
--rw-r--r--   0 jens       (501) staff       (20)     8178 2022-05-12 07:25:22.000000 ZEO-5.4.0/docs/server.rst
--rw-r--r--   0 jens       (501) staff       (20)      586 2022-10-07 12:31:26.000000 ZEO-5.4.0/log.ini
--rw-r--r--   0 jens       (501) staff       (20)     8965 2021-11-02 08:52:31.000000 ZEO-5.4.0/perf.py
--rw-r--r--   0 jens       (501) staff       (20)     2355 2022-05-12 07:25:22.000000 ZEO-5.4.0/release.py
--rw-r--r--   0 jens       (501) staff       (20)      446 2023-01-18 17:12:13.604724 ZEO-5.4.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     3552 2023-01-18 16:43:40.000000 ZEO-5.4.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.587028 ZEO-5.4.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.594927 ZEO-5.4.0/src/ZEO/
--rw-r--r--   0 jens       (501) staff       (20)    49792 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/ClientStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     1417 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/Exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)    46609 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/StorageServer.py
--rw-r--r--   0 jens       (501) staff       (20)     3358 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/TransactionBuffer.py
--rw-r--r--   0 jens       (501) staff       (20)     3170 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2327 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)     9472 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/_forker.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.597582 ZEO-5.4.0/src/ZEO/asyncio/
--rw-r--r--   0 jens       (501) staff       (20)     3800 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/README.rst
--rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/asyncio/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    15265 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/_futures.pyx
--rw-r--r--   0 jens       (501) staff       (20)     5107 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/_smp.pyx
--rw-r--r--   0 jens       (501) staff       (20)     6978 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/base.py
--rw-r--r--   0 jens       (501) staff       (20)    42485 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/client.py
--rw-r--r--   0 jens       (501) staff       (20)      304 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/asyncio/compat.py
--rw-r--r--   0 jens       (501) staff       (20)    16128 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/futures.py
--rw-r--r--   0 jens       (501) staff       (20)     4943 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/asyncio/marshal.py
--rw-r--r--   0 jens       (501) staff       (20)     9698 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/server.py
--rw-r--r--   0 jens       (501) staff       (20)     7054 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/smp.py
--rw-r--r--   0 jens       (501) staff       (20)     8839 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/testing.py
--rw-r--r--   0 jens       (501) staff       (20)    63889 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/asyncio/tests.py
--rw-r--r--   0 jens       (501) staff       (20)    31311 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/cache.py
--rw-r--r--   0 jens       (501) staff       (20)     5915 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/component.xml
--rw-r--r--   0 jens       (501) staff       (20)      964 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/hash.py
--rw-r--r--   0 jens       (501) staff       (20)     3342 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     4047 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/monitor.py
--rw-r--r--   0 jens       (501) staff       (20)     4861 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/nagios.py
--rw-r--r--   0 jens       (501) staff       (20)     3870 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/nagios.rst
--rw-r--r--   0 jens       (501) staff       (20)    14179 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/runzeo.py
--rw-r--r--   0 jens       (501) staff       (20)     1196 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/schema.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.599260 ZEO-5.4.0/src/ZEO/scripts/
--rw-r--r--   0 jens       (501) staff       (20)     1931 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/scripts/README.txt
--rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/scripts/__init__.py
--rwxr-xr-x   0 jens       (501) staff       (20)    19311 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/scripts/cache_simul.py
--rwxr-xr-x   0 jens       (501) staff       (20)    13622 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/scripts/cache_stats.py
--rw-r--r--   0 jens       (501) staff       (20)     3628 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/parsezeolog.py
--rw-r--r--   0 jens       (501) staff       (20)     1148 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/tests.py
--rwxr-xr-x   0 jens       (501) staff       (20)     1897 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/timeout.py
--rwxr-xr-x   0 jens       (501) staff       (20)     5338 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/scripts/zeopack.py
--rw-r--r--   0 jens       (501) staff       (20)     8904 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/scripts/zeopack.test
--rwxr-xr-x   0 jens       (501) staff       (20)    11102 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/zeoqueue.py
--rw-r--r--   0 jens       (501) staff       (20)     9000 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/zeoreplay.py
--rw-r--r--   0 jens       (501) staff       (20)    15834 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/scripts/zeoserverlog.py
--rwxr-xr-x   0 jens       (501) staff       (20)     4340 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/scripts/zeoup.py
--rw-r--r--   0 jens       (501) staff       (20)     4768 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/server.xml
--rw-r--r--   0 jens       (501) staff       (20)     1980 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/shortrepr.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.604236 ZEO-5.4.0/src/ZEO/tests/
--rw-r--r--   0 jens       (501) staff       (20)     1872 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/Cache.py
--rw-r--r--   0 jens       (501) staff       (20)     5571 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/CommitLockTests.py
--rw-r--r--   0 jens       (501) staff       (20)    42615 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/ConnectionTests.py
--rw-r--r--   0 jens       (501) staff       (20)    16874 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/InvalidationTests.py
--rw-r--r--   0 jens       (501) staff       (20)     8698 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/IterationTests.py
--rw-r--r--   0 jens       (501) staff       (20)     2326 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/TestThread.py
--rw-r--r--   0 jens       (501) staff       (20)     5109 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/ThreadTests.py
--rw-r--r--   0 jens       (501) staff       (20)      641 2022-10-12 08:54:06.000000 ZEO-5.4.0/src/ZEO/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2902 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/client-config.test
--rw-r--r--   0 jens       (501) staff       (20)     1233 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/client.pem
--rw-r--r--   0 jens       (501) staff       (20)     1675 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/client_key.pem
--rw-r--r--   0 jens       (501) staff       (20)      286 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/component.xml
--rw-r--r--   0 jens       (501) staff       (20)     4641 2022-03-16 11:02:29.000000 ZEO-5.4.0/src/ZEO/tests/drop_cache_rather_than_verify.txt
--rw-r--r--   0 jens       (501) staff       (20)     2139 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/dynamic_server_ports.test
--rw-r--r--   0 jens       (501) staff       (20)     5450 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/forker.py
--rw-r--r--   0 jens       (501) staff       (20)     4200 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/invalidation-age.txt
--rw-r--r--   0 jens       (501) staff       (20)     1039 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/new_addr.test
--rw-r--r--   0 jens       (501) staff       (20)     1164 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/protocols.test
--rw-r--r--   0 jens       (501) staff       (20)     2299 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/racetest.py
--rw-r--r--   0 jens       (501) staff       (20)     1342 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/server.pem
--rw-r--r--   0 jens       (501) staff       (20)     1013 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/server.pem.csr
--rw-r--r--   0 jens       (501) staff       (20)     1675 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/server_key.pem
--rw-r--r--   0 jens       (501) staff       (20)     1285 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/serverpw.pem
--rw-r--r--   0 jens       (501) staff       (20)     1751 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/serverpw_key.pem
--rw-r--r--   0 jens       (501) staff       (20)     3113 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/servertesting.py
--rw-r--r--   0 jens       (501) staff       (20)     6554 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/speed.py
--rw-r--r--   0 jens       (501) staff       (20)     3813 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/stress.py
--rw-r--r--   0 jens       (501) staff       (20)     4671 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/testConfig.py
--rw-r--r--   0 jens       (501) staff       (20)     8320 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/testConnection.py
--rw-r--r--   0 jens       (501) staff       (20)     3839 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/testConversionSupport.py
--rw-r--r--   0 jens       (501) staff       (20)     1878 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/testTransactionBuffer.py
--rw-r--r--   0 jens       (501) staff       (20)    60271 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/testZEO.py
--rw-r--r--   0 jens       (501) staff       (20)    16834 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/testZEO2.py
--rw-r--r--   0 jens       (501) staff       (20)     3664 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/testZEOOptions.py
--rw-r--r--   0 jens       (501) staff       (20)     5324 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/testZEOServer.py
--rw-r--r--   0 jens       (501) staff       (20)    47992 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/test_cache.py
--rw-r--r--   0 jens       (501) staff       (20)     1643 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/test_client_credentials.py
--rw-r--r--   0 jens       (501) staff       (20)     5190 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/test_client_side_conflict_resolution.py
--rw-r--r--   0 jens       (501) staff       (20)     1022 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/test_marshal.py
--rw-r--r--   0 jens       (501) staff       (20)     1039 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/test_sync.py
--rw-r--r--   0 jens       (501) staff       (20)    13846 2022-12-17 11:33:31.000000 ZEO-5.4.0/src/ZEO/tests/testssl.py
--rw-r--r--   0 jens       (501) staff       (20)      384 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/threaded.py
--rw-r--r--   0 jens       (501) staff       (20)     1917 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/tests/utils.py
--rw-r--r--   0 jens       (501) staff       (20)     3708 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/zdoptions.test
--rw-r--r--   0 jens       (501) staff       (20)     4221 2023-01-18 15:11:08.000000 ZEO-5.4.0/src/ZEO/tests/zeo-fan-out.test
--rw-r--r--   0 jens       (501) staff       (20)     5331 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/tests/zeo_blob_cache.test
--rw-r--r--   0 jens       (501) staff       (20)     1872 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/util.py
--rw-r--r--   0 jens       (501) staff       (20)        8 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/version.txt
--rw-r--r--   0 jens       (501) staff       (20)     2826 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/zconfig.py
--rw-r--r--   0 jens       (501) staff       (20)     1028 2022-05-12 07:25:22.000000 ZEO-5.4.0/src/ZEO/zeoctl.py
--rw-r--r--   0 jens       (501) staff       (20)      856 2021-11-02 08:52:31.000000 ZEO-5.4.0/src/ZEO/zeoctl.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 17:12:13.595861 ZEO-5.4.0/src/ZEO.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    17294 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3737 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)      132 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2021-11-24 08:34:14.000000 ZEO-5.4.0/src/ZEO.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      359 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        4 2023-01-18 17:12:13.000000 ZEO-5.4.0/src/ZEO.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1908 2022-12-17 11:33:38.000000 ZEO-5.4.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.813332 ZEO-5.4.1/
+-rw-r--r--   0 jens       (501) staff       (20)    15264 2023-07-05 14:51:31.000000 ZEO-5.4.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2023-07-05 14:54:11.000000 ZEO-5.4.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       91 2021-11-02 08:52:31.000000 ZEO-5.4.1/COPYING
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:31.000000 ZEO-5.4.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:31.000000 ZEO-5.4.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      557 2023-07-05 14:54:11.000000 ZEO-5.4.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    17678 2023-07-05 15:30:49.813418 ZEO-5.4.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      949 2021-11-02 08:52:31.000000 ZEO-5.4.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      458 2021-11-02 08:52:31.000000 ZEO-5.4.1/buildout.cfg
+-rw-r--r--   0 jens       (501) staff       (20)        8 2021-11-02 08:52:31.000000 ZEO-5.4.1/doc-requirements.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.801143 ZEO-5.4.1/docs/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.797353 ZEO-5.4.1/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.797408 ZEO-5.4.1/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.802913 ZEO-5.4.1/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)     2856 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/blob-nfs.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     7734 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/client-cache-tracing.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1882 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/client-cache.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10099 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/clients.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1257 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5470 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/introduction.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       35 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/nagios.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9961 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/ordering.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2374 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/protocol.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      326 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/reference.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8178 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/_build/html/_sources/server.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2856 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/blob-nfs.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/changelog.rst
+-rw-r--r--   0 jens       (501) staff       (20)     7734 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/client-cache-tracing.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1882 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/client-cache.rst
+-rw-r--r--   0 jens       (501) staff       (20)    10099 2023-07-05 14:49:05.000000 ZEO-5.4.1/docs/clients.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8406 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)     1257 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5470 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/introduction.rst
+-rw-r--r--   0 jens       (501) staff       (20)       35 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/nagios.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9961 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/ordering.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2374 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/protocol.rst
+-rw-r--r--   0 jens       (501) staff       (20)      326 2022-05-12 07:25:22.000000 ZEO-5.4.1/docs/reference.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8178 2023-07-05 14:49:05.000000 ZEO-5.4.1/docs/server.rst
+-rw-r--r--   0 jens       (501) staff       (20)      586 2022-10-07 12:31:26.000000 ZEO-5.4.1/log.ini
+-rw-r--r--   0 jens       (501) staff       (20)     8965 2021-11-02 08:52:31.000000 ZEO-5.4.1/perf.py
+-rw-r--r--   0 jens       (501) staff       (20)     2355 2022-05-12 07:25:22.000000 ZEO-5.4.1/release.py
+-rw-r--r--   0 jens       (501) staff       (20)      446 2023-07-05 15:30:49.813692 ZEO-5.4.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3538 2023-07-05 14:51:37.000000 ZEO-5.4.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.797622 ZEO-5.4.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.805208 ZEO-5.4.1/src/ZEO/
+-rw-r--r--   0 jens       (501) staff       (20)    49790 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/ClientStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     1417 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/Exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    46587 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/StorageServer.py
+-rw-r--r--   0 jens       (501) staff       (20)     3358 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/TransactionBuffer.py
+-rw-r--r--   0 jens       (501) staff       (20)     3170 2022-05-12 07:25:22.000000 ZEO-5.4.1/src/ZEO/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     2327 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)     9465 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/_forker.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.807513 ZEO-5.4.1/src/ZEO/asyncio/
+-rw-r--r--   0 jens       (501) staff       (20)     3800 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/asyncio/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/asyncio/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    15356 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/_futures.pyx
+-rw-r--r--   0 jens       (501) staff       (20)     5107 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/asyncio/_smp.pyx
+-rw-r--r--   0 jens       (501) staff       (20)     6978 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/asyncio/base.py
+-rw-r--r--   0 jens       (501) staff       (20)    42300 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/client.py
+-rw-r--r--   0 jens       (501) staff       (20)      304 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/asyncio/compat.py
+-rw-r--r--   0 jens       (501) staff       (20)      600 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/connectco_2.py
+-rw-r--r--   0 jens       (501) staff       (20)      575 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/connectco_3.py
+-rw-r--r--   0 jens       (501) staff       (20)    16353 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/futures.py
+-rw-r--r--   0 jens       (501) staff       (20)     4943 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/asyncio/marshal.py
+-rw-r--r--   0 jens       (501) staff       (20)     9691 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/server.py
+-rw-r--r--   0 jens       (501) staff       (20)     7054 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/asyncio/smp.py
+-rw-r--r--   0 jens       (501) staff       (20)     8839 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/asyncio/testing.py
+-rw-r--r--   0 jens       (501) staff       (20)    64617 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/asyncio/tests.py
+-rw-r--r--   0 jens       (501) staff       (20)    31311 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/cache.py
+-rw-r--r--   0 jens       (501) staff       (20)     5915 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)     3342 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     4047 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/monitor.py
+-rw-r--r--   0 jens       (501) staff       (20)     4861 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/nagios.py
+-rw-r--r--   0 jens       (501) staff       (20)     3870 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/nagios.rst
+-rw-r--r--   0 jens       (501) staff       (20)    14179 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/runzeo.py
+-rw-r--r--   0 jens       (501) staff       (20)     1196 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/schema.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.808792 ZEO-5.4.1/src/ZEO/scripts/
+-rw-r--r--   0 jens       (501) staff       (20)     1931 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/scripts/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/scripts/__init__.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    19311 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/cache_simul.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    13622 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/cache_stats.py
+-rw-r--r--   0 jens       (501) staff       (20)     3628 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/parsezeolog.py
+-rw-r--r--   0 jens       (501) staff       (20)     1148 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/tests.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     1897 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/timeout.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     5338 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/zeopack.py
+-rw-r--r--   0 jens       (501) staff       (20)     8904 2022-12-17 11:33:31.000000 ZEO-5.4.1/src/ZEO/scripts/zeopack.test
+-rwxr-xr-x   0 jens       (501) staff       (20)    11102 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/zeoqueue.py
+-rw-r--r--   0 jens       (501) staff       (20)     9000 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/zeoreplay.py
+-rw-r--r--   0 jens       (501) staff       (20)    15834 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/zeoserverlog.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     4340 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/scripts/zeoup.py
+-rw-r--r--   0 jens       (501) staff       (20)     4768 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/server.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1980 2022-05-12 07:25:22.000000 ZEO-5.4.1/src/ZEO/shortrepr.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.813239 ZEO-5.4.1/src/ZEO/tests/
+-rw-r--r--   0 jens       (501) staff       (20)     1872 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/Cache.py
+-rw-r--r--   0 jens       (501) staff       (20)     5571 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/CommitLockTests.py
+-rw-r--r--   0 jens       (501) staff       (20)    42615 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/ConnectionTests.py
+-rw-r--r--   0 jens       (501) staff       (20)    16876 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/InvalidationTests.py
+-rw-r--r--   0 jens       (501) staff       (20)     8698 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/IterationTests.py
+-rw-r--r--   0 jens       (501) staff       (20)     2327 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/TestThread.py
+-rw-r--r--   0 jens       (501) staff       (20)     5110 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/ThreadTests.py
+-rw-r--r--   0 jens       (501) staff       (20)      641 2022-10-12 08:54:06.000000 ZEO-5.4.1/src/ZEO/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     3137 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/client-config.test
+-rw-r--r--   0 jens       (501) staff       (20)     1233 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/client.pem
+-rw-r--r--   0 jens       (501) staff       (20)     1675 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/client_key.pem
+-rw-r--r--   0 jens       (501) staff       (20)      286 2022-12-17 11:33:31.000000 ZEO-5.4.1/src/ZEO/tests/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)     4641 2022-03-16 11:02:29.000000 ZEO-5.4.1/src/ZEO/tests/drop_cache_rather_than_verify.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2139 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/dynamic_server_ports.test
+-rw-r--r--   0 jens       (501) staff       (20)     5450 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/forker.py
+-rw-r--r--   0 jens       (501) staff       (20)     4200 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/invalidation-age.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1039 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/new_addr.test
+-rw-r--r--   0 jens       (501) staff       (20)     1164 2022-12-17 11:33:31.000000 ZEO-5.4.1/src/ZEO/tests/protocols.test
+-rw-r--r--   0 jens       (501) staff       (20)     2299 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/racetest.py
+-rw-r--r--   0 jens       (501) staff       (20)     1342 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/server.pem
+-rw-r--r--   0 jens       (501) staff       (20)     1013 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/server.pem.csr
+-rw-r--r--   0 jens       (501) staff       (20)     1675 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/server_key.pem
+-rw-r--r--   0 jens       (501) staff       (20)     1285 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/serverpw.pem
+-rw-r--r--   0 jens       (501) staff       (20)     1751 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/tests/serverpw_key.pem
+-rw-r--r--   0 jens       (501) staff       (20)     3113 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/servertesting.py
+-rw-r--r--   0 jens       (501) staff       (20)     6554 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/speed.py
+-rw-r--r--   0 jens       (501) staff       (20)     3813 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/stress.py
+-rw-r--r--   0 jens       (501) staff       (20)     4701 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/testConfig.py
+-rw-r--r--   0 jens       (501) staff       (20)     8415 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/testConnection.py
+-rw-r--r--   0 jens       (501) staff       (20)     3839 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/testConversionSupport.py
+-rw-r--r--   0 jens       (501) staff       (20)     1967 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/testTransactionBuffer.py
+-rw-r--r--   0 jens       (501) staff       (20)    60676 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/testZEO.py
+-rw-r--r--   0 jens       (501) staff       (20)    16834 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/testZEO2.py
+-rw-r--r--   0 jens       (501) staff       (20)     3664 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/tests/testZEOOptions.py
+-rw-r--r--   0 jens       (501) staff       (20)     5324 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/testZEOServer.py
+-rw-r--r--   0 jens       (501) staff       (20)    47988 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/test_cache.py
+-rw-r--r--   0 jens       (501) staff       (20)     1673 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/test_client_credentials.py
+-rw-r--r--   0 jens       (501) staff       (20)     5190 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/test_client_side_conflict_resolution.py
+-rw-r--r--   0 jens       (501) staff       (20)     1022 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/tests/test_marshal.py
+-rw-r--r--   0 jens       (501) staff       (20)     1039 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/tests/test_sync.py
+-rw-r--r--   0 jens       (501) staff       (20)    13919 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/testssl.py
+-rw-r--r--   0 jens       (501) staff       (20)      384 2022-05-12 07:25:22.000000 ZEO-5.4.1/src/ZEO/tests/threaded.py
+-rw-r--r--   0 jens       (501) staff       (20)     1917 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     3708 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/tests/zdoptions.test
+-rw-r--r--   0 jens       (501) staff       (20)     4221 2023-01-18 15:11:08.000000 ZEO-5.4.1/src/ZEO/tests/zeo-fan-out.test
+-rw-r--r--   0 jens       (501) staff       (20)     5329 2023-07-05 14:49:13.000000 ZEO-5.4.1/src/ZEO/tests/zeo_blob_cache.test
+-rw-r--r--   0 jens       (501) staff       (20)     1872 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/util.py
+-rw-r--r--   0 jens       (501) staff       (20)        8 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/version.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2826 2023-07-05 14:49:05.000000 ZEO-5.4.1/src/ZEO/zconfig.py
+-rw-r--r--   0 jens       (501) staff       (20)     1028 2022-05-12 07:25:22.000000 ZEO-5.4.1/src/ZEO/zeoctl.py
+-rw-r--r--   0 jens       (501) staff       (20)      856 2021-11-02 08:52:31.000000 ZEO-5.4.1/src/ZEO/zeoctl.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-05 15:30:49.805945 ZEO-5.4.1/src/ZEO.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    17678 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3783 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)      132 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2021-11-24 08:34:14.000000 ZEO-5.4.1/src/ZEO.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      352 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        4 2023-07-05 15:30:49.000000 ZEO-5.4.1/src/ZEO.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1852 2023-07-05 14:55:54.000000 ZEO-5.4.1/tox.ini
```

### Comparing `ZEO-5.4.0/CHANGES.rst` & `ZEO-5.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+5.4.1 (2023-07-05)
+------------------
+
+- Fix `#226 <https://github.com/zopefoundation/ZEO/issues/226>`_
+  using an ``asyncio.Task`` (rather than a proprietary,
+  specially ZEO optimized task) for the connection process.
+  This is advisable because the connection process is not
+  implemented by ZEO but by foreign code which may
+  have problems with the limitations of ZEO tasks.
+
+
 5.4.0 (2023-01-18)
 ------------------
 
 - Reimplement and streamline the ``asyncio`` part of the ``ClientStorage``
   implementation:
 
    - switch from futures with explicit callbacks to `async/await`-like style
@@ -20,25 +31,25 @@
 - Remove support for interoperability with ZEO4 server. It turned out that ZEO5
   client, contrary to interoperability with ZEO5 server, implements support for
   interoperability with ZEO4 server incorrectly with concurrency bugs that lead
   to data corruption. The fix is not trivial and we believe that in 2022 noone
   actually uses ZEO5.client-ZEO4.server configuration. That's why support for
   ZEO4 server was dropped rather than fixed.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - If the ``zeopack`` script cannot connect to a server it sets exit status 1
   See `#214 <https://github.com/zopefoundation/ZEO/issues/214>`_.
 
 - Remove ``asyncio/mtacceptor`` module. It turned out that multi-threaded ZEO5
   server has concurrency issues that lead to data corruption. Multi-threaded
   server mode was already deprecated and scheduled for removal, so the fix is
   to finally remove it. From now on ZEO server is always single-threaded.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - Test ZEO only with the following storages
   ``FileStorage`` with server side blobs,
   ``FileStorage`` with shared blob directory,
   ``MappingStorage`` (without blobs).
 
   Those tests cover all storage features with impact on ZEO:
```

### Comparing `ZEO-5.4.0/CONTRIBUTING.md` & `ZEO-5.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/LICENSE.txt` & `ZEO-5.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/MANIFEST.in` & `ZEO-5.4.1/MANIFEST.in`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 
 recursive-include src *.py
-recursive-include src *.pyx
 include *.py
 include COPYING
 include log.ini
 recursive-include src *.csr
 recursive-include src *.pem
+recursive-include src *.pyx
 recursive-include src *.rst
 recursive-include src *.test
 recursive-include src *.txt
 recursive-include src *.xml
```

### Comparing `ZEO-5.4.0/PKG-INFO` & `ZEO-5.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZEO
-Version: 5.4.0
+Version: 5.4.1
 Summary: ZEO - Single-server client-server database server for ZODB
 Home-page: https://github.com/zopefoundation/ZEO
 Author: Zope Foundation and Contributors
 Author-email: zodb@googlegroups.com
 License: ZPL 2.1
 Keywords: database,zodb
 Platform: any
@@ -56,14 +56,25 @@
   leverages the RDBMS servers to provide a client-server storage.
 
 The documentation is available on `readthedocs <http://zeo.readthedocs.io/en/latest/>`_.
 
 Changelog
 =========
 
+5.4.1 (2023-07-05)
+------------------
+
+- Fix `#226 <https://github.com/zopefoundation/ZEO/issues/226>`_
+  using an ``asyncio.Task`` (rather than a proprietary,
+  specially ZEO optimized task) for the connection process.
+  This is advisable because the connection process is not
+  implemented by ZEO but by foreign code which may
+  have problems with the limitations of ZEO tasks.
+
+
 5.4.0 (2023-01-18)
 ------------------
 
 - Reimplement and streamline the ``asyncio`` part of the ``ClientStorage``
   implementation:
 
    - switch from futures with explicit callbacks to `async/await`-like style
@@ -79,25 +90,25 @@
 - Remove support for interoperability with ZEO4 server. It turned out that ZEO5
   client, contrary to interoperability with ZEO5 server, implements support for
   interoperability with ZEO4 server incorrectly with concurrency bugs that lead
   to data corruption. The fix is not trivial and we believe that in 2022 noone
   actually uses ZEO5.client-ZEO4.server configuration. That's why support for
   ZEO4 server was dropped rather than fixed.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - If the ``zeopack`` script cannot connect to a server it sets exit status 1
   See `#214 <https://github.com/zopefoundation/ZEO/issues/214>`_.
 
 - Remove ``asyncio/mtacceptor`` module. It turned out that multi-threaded ZEO5
   server has concurrency issues that lead to data corruption. Multi-threaded
   server mode was already deprecated and scheduled for removal, so the fix is
   to finally remove it. From now on ZEO server is always single-threaded.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - Test ZEO only with the following storages
   ``FileStorage`` with server side blobs,
   ``FileStorage`` with shared blob directory,
   ``MappingStorage`` (without blobs).
 
   Those tests cover all storage features with impact on ZEO:
```

### Comparing `ZEO-5.4.0/README.rst` & `ZEO-5.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/blob-nfs.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/blob-nfs.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/client-cache-tracing.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/client-cache-tracing.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/client-cache.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/client-cache.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/clients.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/clients.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/index.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/introduction.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/ordering.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/ordering.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/protocol.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/protocol.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/_build/html/_sources/server.rst.txt` & `ZEO-5.4.1/docs/_build/html/_sources/server.rst.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/blob-nfs.rst` & `ZEO-5.4.1/docs/blob-nfs.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/client-cache-tracing.rst` & `ZEO-5.4.1/docs/client-cache-tracing.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/client-cache.rst` & `ZEO-5.4.1/docs/client-cache.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/clients.rst` & `ZEO-5.4.1/docs/clients.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/conf.py` & `ZEO-5.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/index.rst` & `ZEO-5.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/introduction.rst` & `ZEO-5.4.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/ordering.rst` & `ZEO-5.4.1/docs/ordering.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/protocol.rst` & `ZEO-5.4.1/docs/protocol.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/docs/server.rst` & `ZEO-5.4.1/docs/server.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/log.ini` & `ZEO-5.4.1/log.ini`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/perf.py` & `ZEO-5.4.1/perf.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/release.py` & `ZEO-5.4.1/release.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/setup.py` & `ZEO-5.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 from setuptools import setup, find_packages
 
-version = '5.4.0'
+version = '5.4.1'
 
 install_requires = [
     'ZODB >= 5.1.1',
     'six',
     'transaction >= 2.0.3',
     'persistent >= 4.1.0',
     'zc.lockfile',
@@ -30,15 +30,14 @@
 tests_require = [
     # We rely on implementation details of
     # test mocks. See https://github.com/zopefoundation/ZODB/pull/222
     'ZConfig',
     'ZODB >= 5.5.1',
     'ZopeUndo',
     'zope.testing',
-    'manuel',
     'transaction',
     'mock',
     'msgpack < 1',
     'zdaemon',
     'zope.testrunner',
 ]
```

### Comparing `ZEO-5.4.0/src/ZEO/ClientStorage.py` & `ZEO-5.4.1/src/ZEO/ClientStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         target = max(self._blob_cache_size - self._blob_cache_size_check, 0)
 
         check_blob_size_thread = threading.Thread(
             target=_check_blob_cache_size,
             args=(self.blob_dir, target),
             name="%s zeo client check blob size thread" % self.__name__,
             )
-        check_blob_size_thread.setDaemon(True)
+        check_blob_size_thread.daemon = True
         check_blob_size_thread.start()
         self._check_blob_size_thread = check_blob_size_thread
 
     def registerDB(self, db):
         """Storage API: register a database for invalidation messages.
 
         This is called by ZODB.DB (and by some tests).
```

### Comparing `ZEO-5.4.0/src/ZEO/Exceptions.py` & `ZEO-5.4.1/src/ZEO/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/StorageServer.py` & `ZEO-5.4.1/src/ZEO/StorageServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,24 +65,24 @@
     logger.log(level, message, exc_info=exc_info)
 
 
 class StorageServerError(StorageError):
     """Error reported when an unpicklable exception is raised."""
 
 
-registered_methods = set(
-    ('get_info', 'lastTransaction',
+registered_methods = {
+    'get_info', 'lastTransaction',
      'getInvalidations', 'new_oids', 'pack', 'loadBefore', 'storea',
      'checkCurrentSerialInTransaction', 'restorea', 'storeBlobStart',
      'storeBlobChunk', 'storeBlobEnd', 'storeBlobShared',
      'deleteObject', 'tpc_begin', 'vote', 'tpc_finish', 'tpc_abort',
      'history', 'record_iternext', 'sendBlob', 'getTid', 'loadSerial',
      'new_oid', 'undoa', 'undoLog', 'undoInfo', 'iterator_start',
      'iterator_next', 'iterator_record_start', 'iterator_record_next',
-     'iterator_gc', 'server_status', 'set_client_label', 'ping'))
+     'iterator_gc', 'server_status', 'set_client_label', 'ping'}
 
 
 class ZEOStorage(object):
     """Proxy to underlying storage for a single remote client."""
 
     connected = connection = stats = storage = storage_id = transaction = None
     blob_tempfile = None
@@ -276,15 +276,15 @@
         # Yes, you can pack a read-only server or storage!
         if wait:
             return run_in_thread(self._pack_impl, time)
         else:
             # If the client isn't waiting for a reply, start a thread
             # and forget about it.
             t = threading.Thread(target=self._pack_impl, args=(time,))
-            t.setName("zeo storage packing thread")
+            t.name = "zeo storage packing thread"
             t.start()
             return None
 
     def _pack_impl(self, time):
         self.log("pack(time=%s) started..." % repr(time))
         self.storage.pack(time, referencesf)
         self.log("pack(time=%s) complete" % repr(time))
@@ -761,15 +761,15 @@
             self.stats[name] = stats = StorageStats(
                 self.zeo_storages_by_storage_id[name])
             if transaction_timeout is None:
                 # An object with no-op methods
                 timeout = StubTimeoutThread()
             else:
                 timeout = TimeoutThread(transaction_timeout)
-                timeout.setName("TimeoutThread for %s" % name)
+                timeout.name = "TimeoutThread for %s" % name
                 timeout.start()
             self.lock_managers[name] = LockManager(name, stats, timeout)
 
         self.invalidation_age = invalidation_age
         self.client_conflict_resolution = client_conflict_resolution
 
         if addr is not None:
@@ -905,16 +905,16 @@
 
         return latest_tid, list(oids)
 
     __thread = None
 
     def start_thread(self, daemon=True):
         self.__thread = thread = threading.Thread(target=self.loop)
-        thread.setName("StorageServer(%s)" % _addr_label(self.addr))
-        thread.setDaemon(daemon)
+        thread.name = "StorageServer(%s)" % _addr_label(self.addr)
+        thread.daemon = daemon
         thread.start()
 
     __closed = False
 
     def close(self, join_timeout=1):
         """Close the dispatcher so that there are no new connections.
 
@@ -967,16 +967,16 @@
         if PY3:
             # doctests and maybe clients expect a str, not bytes
             last_transaction_hex = str(last_transaction_hex, 'ascii')
         status['last-transaction'] = last_transaction_hex
         return status
 
     def ruok(self):
-        return dict((storage_id, self.server_status(storage_id))
-                    for storage_id in self.storages)
+        return {storage_id: self.server_status(storage_id)
+                    for storage_id in self.storages}
 
 
 class StubTimeoutThread(object):
 
     def begin(self, client):
         pass
 
@@ -991,16 +991,16 @@
     """Monitors transaction progress and generates timeouts."""
 
     # There is one TimeoutThread per storage, because there's one
     # transaction lock per storage.
 
     def __init__(self, timeout):
         threading.Thread.__init__(self)
-        self.setName("TimeoutThread")
-        self.setDaemon(1)
+        self.name = "TimeoutThread"
+        self.daemon = True
         self._timeout = timeout
         self._client = None
         self._deadline = None
         self._cond = threading.Condition()  # Protects _client and _deadline
 
     def begin(self, client):
         # Called from the restart code the "main" thread, whenever the
@@ -1062,15 +1062,15 @@
     # run these methods in response to an I/O event, they
     # will block all other server activity until they complete.  To
     # avoid blocking, we spawn a separate thread, return an MTDelay()
     # object, and have the thread reply() when it finishes.
 
     def __init__(self, method, args):
         threading.Thread.__init__(self)
-        self.setName("SlowMethodThread for %s" % method.__name__)
+        self.name = "SlowMethodThread for %s" % method.__name__
         self._method = method
         self._args = args
         self.delay = MTDelay()
 
     def run(self):
         try:
             result = self._method(*self._args)
```

### Comparing `ZEO-5.4.0/src/ZEO/TransactionBuffer.py` & `ZEO-5.4.1/src/ZEO/TransactionBuffer.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/__init__.py` & `ZEO-5.4.1/src/ZEO/__init__.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/_compat.py` & `ZEO-5.4.1/src/ZEO/_compat.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/_forker.py` & `ZEO-5.4.1/src/ZEO/_forker.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     old_protocol = None
     if protocol:
         import ZEO.asyncio.server
         old_protocol = ZEO.asyncio.server.best_protocol_version
         ZEO.asyncio.server.best_protocol_version = protocol
         old_protocols = ZEO.asyncio.server.ServerProtocol.protocols
         ZEO.asyncio.server.ServerProtocol.protocols = tuple(sorted(
-            set(old_protocols) | set([protocol])
+            set(old_protocols) | {protocol}
             ))
 
     try:
         import threading
         from . import runzeo
 
         options = runzeo.ZEOOptions()
@@ -124,15 +124,15 @@
         logger.debug('SERVER CREATED')
         qout.put(server.server.acceptor.addr)
         logger.debug('ADDRESS SENT')
         thread = threading.Thread(
             target=server.server.loop, kwargs=dict(timeout=.2),
             name=(None if name is None else name + '-server'),
             )
-        thread.setDaemon(True)
+        thread.daemon = True
         thread.start()
         os.remove(config)
 
         try:
             qin.get(timeout=timeout)  # wait for shutdown
         except Empty:
             pass
```

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/README.rst` & `ZEO-5.4.1/src/ZEO/asyncio/README.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/_futures.pyx` & `ZEO-5.4.1/src/ZEO/asyncio/_futures.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # cython: language_level=3
+"""``cython`` implementation of ``futures.py``.
+
+Please see its docstring for details.
+"""
 
 from .compat import asyncio
 cdef object CancelledError = asyncio.CancelledError
 cdef object InvalidStateError = asyncio.InvalidStateError
 cdef object get_event_loop = asyncio.get_event_loop
 import inspect
 from threading import Event
```

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/_smp.pyx` & `ZEO-5.4.1/src/ZEO/asyncio/_smp.pyx`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/base.py` & `ZEO-5.4.1/src/ZEO/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/client.py` & `ZEO-5.4.1/src/ZEO/asyncio/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 from . import base
 from .base import loop_run_forever, loop_run_until_complete
 from .compat import asyncio, new_event_loop
 from .marshal import encoder, decoder
 from .futures import Future, AsyncTask as Task, \
      coroutine, return_, run_coroutine_threadsafe, switch_thread
 
+if sys.version_info[0] == 2:
+    from .connectco_2 import connect_coroutine
+else:
+    from .connectco_3 import connect_coroutine
+
 logger = logging.getLogger(__name__)
 
 Fallback = object()
 
 local_random = random.Random()  # use separate generator to facilitate tests
 
 uvloop_used = "uvloop" in sys.modules
@@ -150,30 +155,20 @@
             cr = lambda: self.loop.create_connection(  # noqa: E731
                 self.protocol_factory, host or '127.0.0.1', port,
                 ssl=self.ssl, server_hostname=self.ssl_server_hostname)
         else:
             cr = lambda: self.loop.create_unix_connection(  # noqa: E731
                 self.protocol_factory, self.addr, ssl=self.ssl)
 
-        @coroutine
-        def connect():
-            while not self.closed:
-                try:
-                    yield cr()
-                    return
-                except asyncio.CancelledError:
-                    logger.info("Connection to %r cancelled", self.addr)
-                    raise
-                except Exception as exc:
-                    logger.info("Connection to %r failed, %s",
-                                self.addr, exc)
-                yield asyncio.sleep(self.connect_poll + local_random.random())
-                logger.info("retry connecting %r", self.addr)
-
-        self._connecting = Task(connect(), self.loop)
+        # Usually, we use our optimized but feature limited tasks
+        # to run coroutines. Here we use a standard task
+        # because we do not know which task features the connect
+        # coroutine needs.
+        self._connecting = self.loop.create_task(
+            connect_coroutine(cr, self, logger, local_random.random))
 
     def connection_made(self, transport):
         logger.debug('connection_made %s', self)
         super(Protocol, self).connection_made(transport)
         self.heartbeat(write=False)
 
     def connection_lost(self, exc):
```

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/futures.py` & `ZEO-5.4.1/src/ZEO/asyncio/futures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Optimized variants of ``asyncio``'s ``Future`` and ``Task``.
 
 ``asyncio`` schedules callbacks to be executed in the next
 loop run. This increases the number of loop runs necessary to
 obtain the result of a ZEO server request and adds significant
 latency (+ 27% in some benchmarks).
-This module defines variants which run callbacks immediately.
+This module defines variants which run callbacks immediately
+and ignore a context.
+
+The tasks defined by this module build on those futures
+and in addition do not implement a task context. If you do not
+know the coroutine run by the task, it is safer to use
+a standard ``asyncio.Task``.
 """
 
 from .compat import asyncio
 import functools
 import six
 CancelledError = asyncio.CancelledError
 InvalidStateError = asyncio.InvalidStateError
```

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/marshal.py` & `ZEO-5.4.1/src/ZEO/asyncio/marshal.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/server.py` & `ZEO-5.4.1/src/ZEO/asyncio/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class ServerProtocol(base.ZEOBaseProtocol):
     """asyncio low-level ZEO server interface
     """
 
     protocols = (b'5', )
 
-    methods = set(('register', ))
+    methods = {'register'}
 
     unlogged_exception_types = (
         ZODB.POSException.POSKeyError,
         ZODB.POSException.ConflictError,
         ZODB.POSException.ReadConflictError,
         )
```

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/smp.py` & `ZEO-5.4.1/src/ZEO/asyncio/smp.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/testing.py` & `ZEO-5.4.1/src/ZEO/asyncio/testing.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/asyncio/tests.py` & `ZEO-5.4.1/src/ZEO/asyncio/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,18 @@
         # object and a cache.
 
         wrapper = mock.Mock(__name__="__name__")
         self.target = wrapper
         cache = MemoryCache()
         # We can also provide an event loop.  We'll use a testing loop
         # so we don't have to actually make any network connection.
-        self.loop = loop = FaithfulLoop(
-            addrs if loop_addrs is None else loop_addrs)
+        if self.loop is None:
+            self.loop = FaithfulLoop(
+                addrs if loop_addrs is None else loop_addrs)
+        loop = self.loop
         ClientThread.__init__(self,
                               addrs, wrapper, cache, 'TEST',
                               read_only, timeout=1)
         loop.run_until_inactive()
         self.assertFalse(wrapper.notify_disconnected.called)
         protocol = loop.protocol
         transport = loop.transport
@@ -501,14 +503,29 @@
         self.assertTrue(client.connected.done() and not transport.data)
         self.assertEqual(cache.getLastTid(), b'e'*8)
 
         # But the cache is now empty and we invalidated the database cache
         self.assertFalse(cache)
         wrapper.invalidateCache.assert_called_with()
 
+    def test_reconnect_trial(self):
+        """test for "https://github.com/zopefoundation/ZEO/issues/226"."""
+        # we use a unix connection (to be in line with #226)
+        addrs = ["__nonexisting_unix_socket__"]
+        loop = self.loop = FaithfulLoop(addrs)
+        # we override the loop's ``create_unix_connection`` to let it
+        # fail immediately
+        loop.create_unix_connection = lambda *args: 1/0
+        wrapper, cache, loop, client, protocol, transport = self.start(
+            addrs, ())
+
+        # The failed connection is attempted in the future:
+        delay, func, args, handle = loop.later.pop(0)
+        self.assertTrue(1 <= delay <= 2)
+
     def test_multiple_addresses(self):
         # We can pass multiple addresses to client constructor
         addrs = [('1.2.3.4', 8200), ('2.2.3.4', 8200)]
         wrapper, cache, loop, client, protocol, transport = self.start(
             addrs, ())
 
         # We haven't connected yet
```

### Comparing `ZEO-5.4.0/src/ZEO/cache.py` & `ZEO-5.4.1/src/ZEO/cache.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/component.xml` & `ZEO-5.4.1/src/ZEO/component.xml`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/interfaces.py` & `ZEO-5.4.1/src/ZEO/interfaces.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/monitor.py` & `ZEO-5.4.1/src/ZEO/monitor.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/nagios.py` & `ZEO-5.4.1/src/ZEO/nagios.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/nagios.rst` & `ZEO-5.4.1/src/ZEO/nagios.rst`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/runzeo.py` & `ZEO-5.4.1/src/ZEO/runzeo.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/schema.xml` & `ZEO-5.4.1/src/ZEO/schema.xml`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/README.txt` & `ZEO-5.4.1/src/ZEO/scripts/README.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/cache_simul.py` & `ZEO-5.4.1/src/ZEO/scripts/cache_simul.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/cache_stats.py` & `ZEO-5.4.1/src/ZEO/scripts/cache_stats.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/parsezeolog.py` & `ZEO-5.4.1/src/ZEO/scripts/parsezeolog.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/tests.py` & `ZEO-5.4.1/src/ZEO/scripts/tests.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/timeout.py` & `ZEO-5.4.1/src/ZEO/scripts/timeout.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeopack.py` & `ZEO-5.4.1/src/ZEO/scripts/zeopack.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeopack.test` & `ZEO-5.4.1/src/ZEO/scripts/zeopack.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeoqueue.py` & `ZEO-5.4.1/src/ZEO/scripts/zeoqueue.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeoreplay.py` & `ZEO-5.4.1/src/ZEO/scripts/zeoreplay.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeoserverlog.py` & `ZEO-5.4.1/src/ZEO/scripts/zeoserverlog.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/scripts/zeoup.py` & `ZEO-5.4.1/src/ZEO/scripts/zeoup.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/server.xml` & `ZEO-5.4.1/src/ZEO/server.xml`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/shortrepr.py` & `ZEO-5.4.1/src/ZEO/shortrepr.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/Cache.py` & `ZEO-5.4.1/src/ZEO/tests/Cache.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/CommitLockTests.py` & `ZEO-5.4.1/src/ZEO/tests/CommitLockTests.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/ConnectionTests.py` & `ZEO-5.4.1/src/ZEO/tests/ConnectionTests.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/InvalidationTests.py` & `ZEO-5.4.1/src/ZEO/tests/InvalidationTests.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,22 @@
         self.sleep = sleep
         self.added_keys = []
         self.commitdict = commitdict
 
     def _testrun(self):
         tm = transaction.TransactionManager()
         cn = self.db.open(transaction_manager=tm)
-        while not self.stop.isSet():
+        while not self.stop.is_set():
             try:
                 tree = cn.root()["tree"]
                 break
             except (ConflictError, KeyError):
                 tm.abort()
         key = self.startnum
-        while not self.stop.isSet():
+        while not self.stop.is_set():
             try:
                 tree[key] = self.threadnum
                 tm.get().note(u"add key %s" % key)
                 tm.commit()
                 self.commitdict[self] = 1
                 if self.sleep:
                     time.sleep(self.sleep)
@@ -187,25 +187,25 @@
         self.step = step
         self.sleep = sleep
         self.added_keys = []
         self.commitdict = commitdict
 
     def _testrun(self):
         cn = self.db.open()
-        while not self.stop.isSet():
+        while not self.stop.is_set():
             try:
                 tree = cn.root()["tree"]
                 break
             except (ConflictError, KeyError):
                 # print("%d getting tree abort" % self.threadnum)
                 transaction.abort()
 
         keys_added = {}  # set of keys we commit
         tkeys = []
-        while not self.stop.isSet():
+        while not self.stop.is_set():
 
             # The test picks 50 keys spread across many buckets.
             # self.startnum and self.step ensure that all threads use
             # disjoint key sets, to minimize conflict errors.
 
             nkeys = len(tkeys)
             if nkeys < 50:
@@ -305,15 +305,15 @@
         # Run the threads
         for t in threads:
             t.start()
         delay = self.MINTIME
         start = time.time()
         while time.time() - start <= self.MAXTIME:
             stop.wait(delay)
-            if stop.isSet():
+            if stop.is_set():
                 # Some thread failed.  Stop right now.
                 break
             delay = 2.0
             if len(commitdict) >= len(threads):
                 break
             # Some thread still hasn't managed to commit anything.
         stop.set()
@@ -396,15 +396,15 @@
 
         # Run threads that update the BTree
         cd = {}
         threads = [self.StressThread(self, dbs[i], stop, i, cd, i, n)
                    for i in range(n)]
         self.go(stop, cd, *threads)
 
-        while len(set(db.lastTransaction() for db in dbs)) > 1:
+        while len({db.lastTransaction() for db in dbs}) > 1:
             _ = [db._storage.sync() for db in dbs]
 
         cn = dbs[0].open()
         tree = cn.root()["tree"]
         self._check_tree(cn, tree)
         self._check_threads(tree, *threads)
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/IterationTests.py` & `ZEO-5.4.1/src/ZEO/tests/IterationTests.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/TestThread.py` & `ZEO-5.4.1/src/ZEO/tests/TestThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     period, then the test is made to fail with a "Thread still alive"
     message.
     """
 
     def __init__(self, testcase):
         threading.Thread.__init__(self)
         # In case this thread hangs, don't stop Python from exiting.
-        self.setDaemon(1)
+        self.daemon = True
         self._exc_info = None
         self._testcase = testcase
 
     def run(self):
         try:
             self.testrun()
         except:  # NOQA: E722 blank except
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/ThreadTests.py` & `ZEO-5.4.1/src/ZEO/tests/ThreadTests.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.storage = storage
         self.trans = TransactionMetaData()
         self.doNextEvent = doNextEvent
         self.threadStartedEvent = threadStartedEvent
         self.gotValueError = 0
         self.gotDisconnected = 0
         threading.Thread.__init__(self)
-        self.setDaemon(1)
+        self.daemon = True
 
     def join(self):
         threading.Thread.join(self, 10)
         assert not self.is_alive()
 
 
 class GetsThroughVoteThread(BasicThread):
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/__init__.py` & `ZEO-5.4.1/src/ZEO/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/client-config.test` & `ZEO-5.4.1/src/ZEO/tests/client-config.test`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,19 @@
     1048576000
 
     >>> print(storage._blob_cache_size_check)
     104857600
 
 In isolated runs, the ``close`` below failed with a timeout.
 Set up a log handler to get at the associated log message.
+Note that we are interested only in this specific log message
+(from `ZEO.asyncio.client.ClientIO.close_co`).
+Occasionally (when the server response for the access to the
+non existing storage `2` is processed sufficiently fast),
+there will we other error log entries; we ignore them.
 
 Note: ``InstalledHandler`` changes the logger's level.
 Therefore, we cannot set ``level`` to ``ERROR`` even though
 we are only interested in error messages for this test (it would discard
 other log messages important for the timeout analysis).
 Instead, we initially request the ``DEBUG`` level
 and later set the handler's level to ``ERROR``.
@@ -92,16 +97,14 @@
 
     >>> storage.close()
 
 Check log records
 
     >>> def check_log_records(records):
     ...     records = [r.message for r in records]
-    ...     if len(records) != 1:
-    ...	        return records
-    ...     return records if "bug" in records[0] else []
+    ...     return any("as a bug" in r for r in records) and records or []
     >>> check_log_records(handler.records)
     []
 
 Cleanup
 
     >>> handler.uninstall()
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/client.pem` & `ZEO-5.4.1/src/ZEO/tests/client.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/client_key.pem` & `ZEO-5.4.1/src/ZEO/tests/client_key.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/drop_cache_rather_than_verify.txt` & `ZEO-5.4.1/src/ZEO/tests/drop_cache_rather_than_verify.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/dynamic_server_ports.test` & `ZEO-5.4.1/src/ZEO/tests/dynamic_server_ports.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/forker.py` & `ZEO-5.4.1/src/ZEO/tests/forker.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/invalidation-age.txt` & `ZEO-5.4.1/src/ZEO/tests/invalidation-age.txt`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/new_addr.test` & `ZEO-5.4.1/src/ZEO/tests/new_addr.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/protocols.test` & `ZEO-5.4.1/src/ZEO/tests/protocols.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/racetest.py` & `ZEO-5.4.1/src/ZEO/tests/racetest.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/server.pem` & `ZEO-5.4.1/src/ZEO/tests/server.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/server.pem.csr` & `ZEO-5.4.1/src/ZEO/tests/server.pem.csr`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/server_key.pem` & `ZEO-5.4.1/src/ZEO/tests/server_key.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/serverpw.pem` & `ZEO-5.4.1/src/ZEO/tests/serverpw.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/serverpw_key.pem` & `ZEO-5.4.1/src/ZEO/tests/serverpw_key.pem`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/servertesting.py` & `ZEO-5.4.1/src/ZEO/tests/servertesting.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/speed.py` & `ZEO-5.4.1/src/ZEO/tests/speed.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/stress.py` & `ZEO-5.4.1/src/ZEO/tests/stress.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/testConfig.py` & `ZEO-5.4.1/src/ZEO/tests/testConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,10 +117,10 @@
 
     def test_blob_cache_size_check(self):
         self.test_default_zeo_config(blob_cache_size=424242,
                                      blob_cache_size_check=50)
 
 
 def test_suite():
-    suite = unittest.makeSuite(ZEOConfigTest)
+    suite = unittest.defaultTestLoader.loadTestsFromTestCase(ZEOConfigTest)
     suite.layer = threaded_server_tests
     return suite
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/testConnection.py` & `ZEO-5.4.1/src/ZEO/tests/testConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     ...             i = random.randint(0, nobs-1)
     ...             conn2.root()[i].value += 1
     ...             tm.commit()
     ...             #logging.getLogger('ZEO').debug(
     ...             #   'COMMIT %s %s %r' % (
     ...             #   i, conn2.root()[i].value, conn2.root()[i]._p_serial))
     >>> thread = threading.Thread(target=run)
-    >>> thread.setDaemon(True)
+    >>> thread.daemon = True
     >>> thread.start()
 
 - restarting the first client, and
 - testing for cache validity.
 
     >>> bad = False
     >>> try:
@@ -237,15 +237,17 @@
     """
 
 
 def test_suite():
     suite = unittest.TestSuite()
 
     for klass in test_classes:
-        sub = unittest.makeSuite(klass, 'check')
+        test_loader = unittest.TestLoader()
+        test_loader.testMethodPrefix = 'check'
+        sub = test_loader.loadTestsFromTestCase(klass)
         sub.layer = ZODB.tests.util.MininalTestLayer(
             klass.__name__ + ' ZEO Connection Tests')
         suite.addTest(sub)
 
     sub = doctest.DocTestSuite(
         setUp=forker.setUp, tearDown=setupstack.tearDown,
         )
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/testConversionSupport.py` & `ZEO-5.4.1/src/ZEO/tests/testConversionSupport.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/testTransactionBuffer.py` & `ZEO-5.4.1/src/ZEO/tests/testTransactionBuffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,8 +56,10 @@
         for i, (oid, d, resolved) in enumerate(tbuf):
             self.assertEqual((oid, d), data[i][0])
             self.assertEqual(resolved, data[i][1])
         tbuf.close()
 
 
 def test_suite():
-    return unittest.makeSuite(TransBufTests, 'check')
+    test_loader = unittest.TestLoader()
+    test_loader.testMethodPrefix = 'check'
+    return test_loader.loadTestsFromTestCase(TransBufTests)
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/testZEO.py` & `ZEO-5.4.1/src/ZEO/tests/testZEO.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,15 +343,15 @@
                 store.tpc_finish(t)
             except Exception as v:
                 self.exception = v
             finally:
                 store.close()
 
         thread = threading.Thread(name='T2', target=do_store)
-        thread.setDaemon(True)
+        thread.daemon = True
         thread.start()
         thread.join(voted and .1 or 9)
         if self.exception is not None:
             six.reraise(type(self.exception), self.exception)
         return thread
 
 
@@ -1250,15 +1250,15 @@
 
 
 def client_asyncore_thread_has_name():
     """
     >>> addr, _ = start_server()  # NOQA: F821 undefined
     >>> db = ZEO.DB(addr)
     >>> any(t for t in threading.enumerate()
-    ...     if ' zeo client networking thread' in t.getName())
+    ...     if ' zeo client networking thread' in t.name)
     True
     >>> db.close()
     """
 
 
 def runzeo_without_configfile():
     r"""
@@ -1305,21 +1305,21 @@
 
     >>> addr, _ = start_server()  # NOQA: F821 undefined
     >>> writing = threading.Event()
     >>> def mad_write_thread():
     ...     global writing
     ...     conn = ZEO.connection(addr)
     ...     writing.set()
-    ...     while writing.isSet():
+    ...     while writing.is_set():
     ...         conn.root.x = 1
     ...         transaction.commit()
     ...     conn.close()
 
     >>> thread = threading.Thread(target=mad_write_thread)
-    >>> thread.setDaemon(True)
+    >>> thread.daemon = True
     >>> thread.start()
     >>> _ = writing.wait()
     >>> time.sleep(.01)
     >>> for i in range(10):
     ...     conn = ZEO.connection(addr)
     ...     _ = conn._storage.load(b'\0'*8)
     ...     conn.close()
@@ -1831,19 +1831,21 @@
         # so we'll clear the caches.
         self._cache.clear()
         ZEO.ClientStorage._check_blob_cache_size(self.blob_dir, 0)
 
 
 def test_suite():
     suite = unittest.TestSuite((
-        unittest.makeSuite(Test_convenience_functions),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            Test_convenience_functions),
     ))
 
     zeo = unittest.TestSuite()
-    zeo.addTest(unittest.makeSuite(ZODB.tests.util.AAAA_Test_Runner_Hack))
+    zeo.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(
+        ZODB.tests.util.AAAA_Test_Runner_Hack))
     patterns = [
         (re.compile(r"u?'start': u?'[^\n]+'"), 'start'),
         (re.compile(r"u?'last-transaction': u?'[0-9a-f]+'"),
          'last-transaction'),
         (re.compile("ZODB.POSException.ConflictError"), "ConflictError"),
         (re.compile("ZODB.POSException.POSKeyError"), "POSKeyError"),
         (re.compile("ZEO.Exceptions.ClientStorageError"),
@@ -1868,15 +1870,18 @@
             ZEO.tests.IterationTests,
             setUp=forker.setUp, tearDown=zope.testing.setupstack.tearDown,
             checker=renormalizing.RENormalizing((
                     (re.compile("ZEO.Exceptions.ClientDisconnected"),
                      "ClientDisconnected"),
                     )),
             ))
-    zeo.addTest(unittest.makeSuite(ClientConflictResolutionTests, 'check'))
+    test_loader = unittest.TestLoader()
+    test_loader.testMethodPrefix = 'check'
+    zeo.addTest(test_loader.loadTestsFromTestCase(
+        ClientConflictResolutionTests))
     zeo.layer = ZODB.tests.util.MininalTestLayer('testZeo-misc')
     suite.addTest(zeo)
 
     zeo = unittest.TestSuite()
     zeo.addTest(
         doctest.DocFileSuite(
             'zdoptions.test',
@@ -1890,15 +1895,17 @@
         )
     zeo.addTest(PackableStorage.IExternalGC_suite(
         lambda:
         ServerManagingClientStorageForIExternalGCTest(
             'data.fs', 'blobs', extrafsoptions='pack-gc false')
         ))
     for klass in quick_test_classes:
-        zeo.addTest(unittest.makeSuite(klass, "check"))
+        test_loader = unittest.TestLoader()
+        test_loader.testMethodPrefix = 'check'
+        zeo.addTest(test_loader.loadTestsFromTestCase(klass))
     zeo.layer = ZODB.tests.util.MininalTestLayer('testZeo-misc2')
     suite.addTest(zeo)
 
     # tests that often fail, maybe if they have their own layers
     for name in 'zeo-fan-out.test', 'new_addr.test':
         zeo = unittest.TestSuite()
         zeo.addTest(
@@ -1908,19 +1915,22 @@
                 checker=renormalizing.RENormalizing(patterns),
                 globs={'print_function': print_function},
                 ),
             )
         zeo.layer = ZODB.tests.util.MininalTestLayer('testZeo-' + name)
         suite.addTest(zeo)
 
-    suite.addTest(unittest.makeSuite(MultiprocessingTests))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(
+        MultiprocessingTests))
 
     # Put the heavyweights in their own layers
     for klass in slow_test_classes:
-        sub = unittest.makeSuite(klass, "check")
+        test_loader = unittest.TestLoader()
+        test_loader.testMethodPrefix = 'check'
+        sub = test_loader.loadTestsFromTestCase(klass)
         sub.layer = ZODB.tests.util.MininalTestLayer(klass.__name__)
         suite.addTest(sub)
 
     suite.addTest(ZODB.tests.testblob.storage_reusable_suite(
         'ClientStorageNonSharedBlobs', ServerManagingClientStorage))
     suite.addTest(ZODB.tests.testblob.storage_reusable_suite(
         'ClientStorageSharedBlobs', create_storage_shared))
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/testZEO2.py` & `ZEO-5.4.1/src/ZEO/tests/testZEO2.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/testZEOOptions.py` & `ZEO-5.4.1/src/ZEO/tests/testZEOOptions.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/testZEOServer.py` & `ZEO-5.4.1/src/ZEO/tests/testZEOServer.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/test_cache.py` & `ZEO-5.4.1/src/ZEO/tests/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
 
         # Verify that internals of both objects are the same.
         # Could also test that external API produces the same results.
         eq = self.assertEqual
         eq(copy.getLastTid(), self.cache.getLastTid())
         eq(len(copy), len(self.cache))
         eq(dict(copy.current), dict(self.cache.current))
-        eq(dict([(k, dict(v)) for (k, v) in copy.noncurrent.items()]),
-           dict([(k, dict(v)) for (k, v) in self.cache.noncurrent.items()]),
+        eq({k: dict(v) for (k, v) in copy.noncurrent.items()},
+           {k: dict(v) for (k, v) in self.cache.noncurrent.items()},
            )
         copy.close()
 
     def testCurrentObjectLargerThanCache(self):
         if self.cache.path:
             os.remove(self.cache.path)
         self.cache.close()
@@ -275,66 +275,66 @@
             cache.close()
             small = 50
             cache = ZEO.cache.ClientCache(
                 'cache', size=ZEO.cache.ZEC_HEADER_SIZE+small*recsize+extra)
             self.assertEqual(len(cache), small)
             self.assertEqual(os.path.getsize(
                 'cache'), ZEO.cache.ZEC_HEADER_SIZE+small*recsize+extra)
-            self.assertEqual(set(u64(oid) for (oid, tid) in cache.contents()),
+            self.assertEqual({u64(oid) for (oid, tid) in cache.contents()},
                              set(range(small)))
             for i in range(100, 110):
                 cache.store(p64(i), n1, None, data)
 
             # We use small-1 below because an extra object gets
             # evicted because of the optimization to assure that we
             # always get a free block after a new allocated block.
             expected_len = small - 1
             self.assertEqual(len(cache), expected_len)
             expected_oids = set(list(range(11, 50))+list(range(100, 110)))
             self.assertEqual(
-                set(u64(oid) for (oid, tid) in cache.contents()),
+                {u64(oid) for (oid, tid) in cache.contents()},
                 expected_oids)
 
             # Make sure we can reopen with same size
             cache.close()
             cache = ZEO.cache.ClientCache(
                 'cache', size=ZEO.cache.ZEC_HEADER_SIZE+small*recsize+extra)
             self.assertEqual(len(cache), expected_len)
-            self.assertEqual(set(u64(oid) for (oid, tid) in cache.contents()),
+            self.assertEqual({u64(oid) for (oid, tid) in cache.contents()},
                              expected_oids)
 
             # Now make it bigger
             cache.close()
             large = 150
             cache = ZEO.cache.ClientCache(
                 'cache', size=ZEO.cache.ZEC_HEADER_SIZE+large*recsize+extra)
             self.assertEqual(len(cache), expected_len)
             self.assertEqual(os.path.getsize(
                 'cache'), ZEO.cache.ZEC_HEADER_SIZE+large*recsize+extra)
-            self.assertEqual(set(u64(oid) for (oid, tid) in cache.contents()),
+            self.assertEqual({u64(oid) for (oid, tid) in cache.contents()},
                              expected_oids)
 
             for i in range(200, 305):
                 cache.store(p64(i), n1, None, data)
 
             # We use large-2 for the same reason we used small-1 above.
             expected_len = large-2
             self.assertEqual(len(cache), expected_len)
             expected_oids = set(list(range(11, 50)) +
                                 list(range(106, 110)) +
                                 list(range(200, 305)))
-            self.assertEqual(set(u64(oid) for (oid, tid) in cache.contents()),
+            self.assertEqual({u64(oid) for (oid, tid) in cache.contents()},
                              expected_oids)
 
             # Make sure we can reopen with same size
             cache.close()
             cache = ZEO.cache.ClientCache(
                 'cache', size=ZEO.cache.ZEC_HEADER_SIZE+large*recsize+extra)
             self.assertEqual(len(cache), expected_len)
-            self.assertEqual(set(u64(oid) for (oid, tid) in cache.contents()),
+            self.assertEqual({u64(oid) for (oid, tid) in cache.contents()},
                              expected_oids)
 
             # Cleanup
             cache.close()
             os.remove('cache')
 
     def testSetAnyLastTidOnEmptyCache(self):
@@ -1109,15 +1109,15 @@
     >>> logging.getLogger().removeHandler(handler)
     >>> logging.getLogger().setLevel(old_level)
     """
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(CacheTests))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(CacheTests))
     suite.addTest(
         doctest.DocTestSuite(
             setUp=zope.testing.setupstack.setUpDirectory,
             tearDown=zope.testing.setupstack.tearDown,
             checker=(ZODB.tests.util.checker +
                      zope.testing.renormalizing.RENormalizing([
                         (re.compile(r'31\.3%'), '31.2%')])),
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/test_client_credentials.py` & `ZEO-5.4.1/src/ZEO/tests/test_client_credentials.py`

 * *Files 19% similar despite different names*

```diff
@@ -51,10 +51,10 @@
         self.assertEqual(creds_log, [creds])
         client.close()
 
         stop()
 
 
 def test_suite():
-    suite = unittest.makeSuite(ClientAuthTests)
+    suite = unittest.defaultTestLoader.loadTestsFromTestCase(ClientAuthTests)
     suite.layer = threaded_server_tests
     return suite
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/test_client_side_conflict_resolution.py` & `ZEO-5.4.1/src/ZEO/tests/test_client_side_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/test_marshal.py` & `ZEO-5.4.1/src/ZEO/tests/test_marshal.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/test_sync.py` & `ZEO-5.4.1/src/ZEO/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/testssl.py` & `ZEO-5.4.1/src/ZEO/tests/testssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,16 +345,17 @@
 
 def pwfunc():
     return '1234'
 
 
 def test_suite():
     suite = unittest.TestSuite((
-        unittest.makeSuite(SSLConfigTest),
-        unittest.makeSuite(SSLConfigTestMockiavellian),
+        unittest.defaultTestLoader.loadTestsFromTestCase(SSLConfigTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(
+            SSLConfigTestMockiavellian),
         ))
     suite.layer = threaded_server_tests
     return suite
 
 
 # Helpers for other tests:
 server_config = """
```

### Comparing `ZEO-5.4.0/src/ZEO/tests/utils.py` & `ZEO-5.4.1/src/ZEO/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/zdoptions.test` & `ZEO-5.4.1/src/ZEO/tests/zdoptions.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/zeo-fan-out.test` & `ZEO-5.4.1/src/ZEO/tests/zeo-fan-out.test`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/tests/zeo_blob_cache.test` & `ZEO-5.4.1/src/ZEO/tests/zeo_blob_cache.test`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     ...             data = f.read()
     ...         if data != (chr(i)*100).encode('ascii'):
     ...             print('bad data', repr(chr(i)), repr(data))
     ...     db.close()
 
     >>> threads = [threading.Thread(target=run) for i in range(10)]
     >>> for thread in threads:
-    ...     thread.setDaemon(True)
+    ...     thread.daemon = True
     >>> for thread in threads:
     ...     thread.start()
     >>> for thread in threads:
     ...     thread.join(99)
     ...     if thread.is_alive():
     ...        print("Can't join thread.")
```

### Comparing `ZEO-5.4.0/src/ZEO/util.py` & `ZEO-5.4.1/src/ZEO/util.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/zconfig.py` & `ZEO-5.4.1/src/ZEO/zconfig.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/zeoctl.py` & `ZEO-5.4.1/src/ZEO/zeoctl.py`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO/zeoctl.xml` & `ZEO-5.4.1/src/ZEO/zeoctl.xml`

 * *Files identical despite different names*

### Comparing `ZEO-5.4.0/src/ZEO.egg-info/PKG-INFO` & `ZEO-5.4.1/src/ZEO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZEO
-Version: 5.4.0
+Version: 5.4.1
 Summary: ZEO - Single-server client-server database server for ZODB
 Home-page: https://github.com/zopefoundation/ZEO
 Author: Zope Foundation and Contributors
 Author-email: zodb@googlegroups.com
 License: ZPL 2.1
 Keywords: database,zodb
 Platform: any
@@ -56,14 +56,25 @@
   leverages the RDBMS servers to provide a client-server storage.
 
 The documentation is available on `readthedocs <http://zeo.readthedocs.io/en/latest/>`_.
 
 Changelog
 =========
 
+5.4.1 (2023-07-05)
+------------------
+
+- Fix `#226 <https://github.com/zopefoundation/ZEO/issues/226>`_
+  using an ``asyncio.Task`` (rather than a proprietary,
+  specially ZEO optimized task) for the connection process.
+  This is advisable because the connection process is not
+  implemented by ZEO but by foreign code which may
+  have problems with the limitations of ZEO tasks.
+
+
 5.4.0 (2023-01-18)
 ------------------
 
 - Reimplement and streamline the ``asyncio`` part of the ``ClientStorage``
   implementation:
 
    - switch from futures with explicit callbacks to `async/await`-like style
@@ -79,25 +90,25 @@
 - Remove support for interoperability with ZEO4 server. It turned out that ZEO5
   client, contrary to interoperability with ZEO5 server, implements support for
   interoperability with ZEO4 server incorrectly with concurrency bugs that lead
   to data corruption. The fix is not trivial and we believe that in 2022 noone
   actually uses ZEO5.client-ZEO4.server configuration. That's why support for
   ZEO4 server was dropped rather than fixed.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - If the ``zeopack`` script cannot connect to a server it sets exit status 1
   See `#214 <https://github.com/zopefoundation/ZEO/issues/214>`_.
 
 - Remove ``asyncio/mtacceptor`` module. It turned out that multi-threaded ZEO5
   server has concurrency issues that lead to data corruption. Multi-threaded
   server mode was already deprecated and scheduled for removal, so the fix is
   to finally remove it. From now on ZEO server is always single-threaded.
 
-  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>` for details.
+  See `issue 209 <https://github.com/zopefoundation/ZEO/issues/209>`_ for details.
 
 - Test ZEO only with the following storages
   ``FileStorage`` with server side blobs,
   ``FileStorage`` with shared blob directory,
   ``MappingStorage`` (without blobs).
 
   Those tests cover all storage features with impact on ZEO:
```

### Comparing `ZEO-5.4.0/src/ZEO.egg-info/SOURCES.txt` & `ZEO-5.4.1/src/ZEO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 src/ZEO/StorageServer.py
 src/ZEO/TransactionBuffer.py
 src/ZEO/__init__.py
 src/ZEO/_compat.py
 src/ZEO/_forker.py
 src/ZEO/cache.py
 src/ZEO/component.xml
-src/ZEO/hash.py
 src/ZEO/interfaces.py
 src/ZEO/monitor.py
 src/ZEO/nagios.py
 src/ZEO/nagios.rst
 src/ZEO/runzeo.py
 src/ZEO/schema.xml
 src/ZEO/server.xml
@@ -71,14 +70,16 @@
 src/ZEO/asyncio/README.rst
 src/ZEO/asyncio/__init__.py
 src/ZEO/asyncio/_futures.pyx
 src/ZEO/asyncio/_smp.pyx
 src/ZEO/asyncio/base.py
 src/ZEO/asyncio/client.py
 src/ZEO/asyncio/compat.py
+src/ZEO/asyncio/connectco_2.py
+src/ZEO/asyncio/connectco_3.py
 src/ZEO/asyncio/futures.py
 src/ZEO/asyncio/marshal.py
 src/ZEO/asyncio/server.py
 src/ZEO/asyncio/smp.py
 src/ZEO/asyncio/testing.py
 src/ZEO/asyncio/tests.py
 src/ZEO/scripts/README.txt
```

### Comparing `ZEO-5.4.0/tox.ini` & `ZEO-5.4.1/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 [testenv]
 usedevelop = true
 deps =
     !zodbmaster: ZODB >= 4.2.0b1
     zodbmaster: -e git+https://github.com/zopefoundation/ZODB.git@master\#egg=ZODB
     uvloop: uvloop
 setenv =
-    !py27-!pypy: PYTHONWARNINGS=ignore::ResourceWarning
     msgpack1: ZEO_MSGPACK=1
 commands =
     # Run unit tests first.
     zope-testrunner -u --test-path=src -a 1000 {posargs:-vc}
     # Only run functional tests if unit tests pass.
     zope-testrunner -f --test-path=src -a 1000 {posargs:-vc}
 extras =
```

