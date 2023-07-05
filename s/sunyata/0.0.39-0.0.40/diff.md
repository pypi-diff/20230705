# Comparing `tmp/sunyata-0.0.39.tar.gz` & `tmp/sunyata-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.39.tar", last modified: Thu Apr 27 07:15:19 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.40.tar", last modified: Wed Jul  5 07:27:54 2023, max compression
```

## Comparing `sunyata-0.0.39.tar` & `sunyata-0.0.40.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-27 07:15:19.000000 sunyata-0.0.39/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1399 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       69 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.39/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.39/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.39/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.39/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.39/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.39/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.39/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.39/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/etcd.py
--rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     3251 2023-04-20 08:32:35.000000 sunyata-0.0.39/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.39/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.39/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.39/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.39/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.39/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.39/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-20 03:05:05.000000 sunyata-0.0.39/sunyata/http/rawserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.39/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.39/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.39/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11863 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2474 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.39/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)    11659 2023-04-26 09:22:35.000000 sunyata-0.0.39/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-25 09:18:13.000000 sunyata-0.0.39/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-27 07:15:19.000000 sunyata-0.0.39/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/
+-rw-r--r--   0 admin      (501) staff       (20)      486 2023-07-05 07:27:54.000000 sunyata-0.0.40/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      486 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1421 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       52 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)       69 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata/
+-rw-r--r--   0 admin      (501) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/db.py
+-rw-r--r--   0 admin      (501) staff       (20)      306 2023-07-05 07:23:02.000000 sunyata-0.0.40/sunyata/concurrent.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/log.py
+-rw-r--r--   0 admin      (501) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.40/sunyata/util.py
+-rw-r--r--   0 admin      (501) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/orm.py
+-rwxr-xr-x   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/eventloop.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata/cli/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/cli/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/cli/cli.py
+-rw-r--r--   0 admin      (501) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/cli/entry.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata/algorithm/
+-rw-r--r--   0 admin      (501) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.40/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.40/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.40/sunyata/algorithm/avltree.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/algorithm/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.40/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 admin      (501) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.40/sunyata/algorithm/btree.py
+-rw-r--r--   0 admin      (501) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.40/sunyata/algorithm/bintree.py
+-rw-r--r--   0 admin      (501) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/algorithm/lru.py
+-rw-r--r--   0 admin      (501) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/algorithm/trie.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.40/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/redislock.py
+-rw-r--r--   0 admin      (501) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.40/sunyata/etcd.py
+-rw-r--r--   0 admin      (501) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.40/sunyata/consul.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata/http/
+-rw-r--r--   0 admin      (501) staff       (20)     3277 2023-05-06 02:45:23.000000 sunyata-0.0.40/sunyata/http/server.py
+-rw-r--r--   0 admin      (501) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.40/sunyata/http/request_stream.py
+-rw-r--r--   0 admin      (501) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.40/sunyata/http/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.40/sunyata/http/request.py
+-rw-r--r--   0 admin      (501) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.40/sunyata/http/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.40/sunyata/http/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.40/sunyata/http/factory.py
+-rw-r--r--   0 admin      (501) staff       (20)     3703 2023-05-06 03:00:50.000000 sunyata-0.0.40/sunyata/http/rawserver.py
+-rw-r--r--   0 admin      (501) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.40/sunyata/http/router.py
+-rw-r--r--   0 admin      (501) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.40/sunyata/http/status.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/cache_wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/compress.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 07:27:54.000000 sunyata-0.0.40/sunyata/rpc/
+-rw-r--r--   0 admin      (501) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/rpc/encrypt.py
+-rw-r--r--   0 admin      (501) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.40/sunyata/rpc/serialize.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/rpc/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)    12758 2023-05-06 09:25:56.000000 sunyata-0.0.40/sunyata/rpc/server.py
+-rw-r--r--   0 admin      (501) staff       (20)     2474 2023-05-06 03:27:50.000000 sunyata-0.0.40/sunyata/rpc/discovery.py
+-rw-r--r--   0 admin      (501) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.40/sunyata/rpc/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.40/sunyata/rpc/client.py
+-rw-r--r--   0 admin      (501) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/rpc/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/rpc/compress.py
+-rw-r--r--   0 admin      (501) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.40/sunyata/rpc/method.py
+-rw-r--r--   0 admin      (501) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.40/sunyata/rpc/protocal.py
+-rw-r--r--   0 admin      (501) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/rpc/const.py
+-rw-r--r--   0 admin      (501) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.40/sunyata/table_writer.py
+-rw-r--r--   0 admin      (501) staff       (20)     3907 2023-05-06 11:08:14.000000 sunyata-0.0.40/sunyata/wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)    11659 2023-04-26 09:22:35.000000 sunyata-0.0.40/README.md
+-rwxr-xr-x   0 admin      (501) staff       (20)     1026 2023-07-05 07:22:05.000000 sunyata-0.0.40/setup.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 07:27:54.000000 sunyata-0.0.40/setup.cfg
```

### Comparing `sunyata-0.0.39/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.40/sunyata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 sunyata/__init__.py
 sunyata/cache_wrap.py
 sunyata/compress.py
+sunyata/concurrent.py
 sunyata/consul.py
 sunyata/db.py
 sunyata/etcd.py
 sunyata/eventloop.py
 sunyata/log.py
 sunyata/orm.py
 sunyata/redislock.py
```

### Comparing `sunyata-0.0.39/sunyata/db.py` & `sunyata-0.0.40/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/log.py` & `sunyata-0.0.40/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/orm.py` & `sunyata-0.0.40/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/cli/cli.py` & `sunyata-0.0.40/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.40/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/algorithm/lru.py` & `sunyata-0.0.40/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/algorithm/trie.py` & `sunyata-0.0.40/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/algorithm/hashtable.py` & `sunyata-0.0.40/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/redislock.py` & `sunyata-0.0.40/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/etcd.py` & `sunyata-0.0.40/sunyata/etcd.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/consul.py` & `sunyata-0.0.40/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/http/server.py` & `sunyata-0.0.40/sunyata/http/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def __init__(self, bind = '0.0.0.0', port=9989, log_level='error'):
         RawHttpServer.__init__(self, bind=bind, port=port)
         self.config = uvicorn.Config("sunyata.http.server:HttpServer", host=self.bind, port=self.port, log_level=log_level)
 
     def serve(self):
         server = uvicorn.Server(self.config)
         print('http running on http://%s:%s' % (self.bind, self.port) )
+        self.dumpRoutes()
         server.run()
 
     async def asyncServe(self):
         server = uvicorn.Server(self.config)
         server.config.setup_event_loop()
         await server.serve()
```

### Comparing `sunyata-0.0.39/sunyata/http/transport.py` & `sunyata-0.0.40/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/http/request.py` & `sunyata-0.0.40/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/http/response.py` & `sunyata-0.0.40/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/http/factory.py` & `sunyata-0.0.40/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/http/rawserver.py` & `sunyata-0.0.40/sunyata/http/rawserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sunyata.http.factory import HttpFactory
 from sunyata.http.status import *
 from sunyata.http.request_stream import RequestStream
 from sunyata.http.response import HttpResponse
+from sunyata.table_writer import TableWriter
 from traceback import format_exc
 from types import MethodType,FunctionType
 import asyncio
 import uvloop
 import inspect
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
@@ -80,9 +81,18 @@
 
     @classmethod
     def route(cls, path, methods = None):
         def wrapper(func):
             cls.addRoute(path, func, methods)
             return func
         return wrapper
+    
+    def dumpRoutes(self):
+        twHeaders = ['Path', 'Methods']
+        twRows = []
+        for path, httpRouter in self.routerMap.items():
+            twRows.append([path, httpRouter.methods])
+        tw = TableWriter(twHeaders, twRows)
+        tw.dump()
+
 
 route = RawHttpServer.route
```

### Comparing `sunyata-0.0.39/sunyata/http/status.py` & `sunyata-0.0.40/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/cache_wrap.py` & `sunyata-0.0.40/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/serialize.py` & `sunyata-0.0.40/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/server.py` & `sunyata-0.0.40/sunyata/rpc/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from sunyata.rpc.compress import RpcCompress
 from types import FunctionType
 from sunyata.rpc.method import RpcMethod
 import asyncio
 import uvloop
 import inspect
 from sunyata.http.server import HttpServer
+from sunyata.table_writer import TableWriter
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
 class RpcServer(object):
 
     funcMap = {}
     funcList = []
@@ -78,14 +79,20 @@
         cls.regist(func)
         return func
     
     def printLogo(self):
         logo = """"""
         print(logo)
 
+    def dumpRpcFuncs(self):
+        twHeaders = ['RPC Methods']
+        twRows = [ [elem] for elem in self.funcList ]
+        tw = TableWriter(twHeaders, list(twRows))
+        tw.dump()
+
 
 class SimpleTcpRpcServer(RpcServer):
     
     def __init__(self, host, port):
         RpcServer.__init__(self)
         self.host = host
         self.port = port
@@ -119,14 +126,15 @@
             except Exception as ex:
                 conn.close()
                 return
 
     def serve(self):
         self.protocal.transport.bind()
         self.printLogo()
+        self.dumpRpcFuncs()
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         while 1:
             conn, _ = self.protocal.transport.accept()
             t = threading.Thread(target=self.handle, args=(conn,) )
             t.setDaemon(True)
             t.start()
@@ -164,14 +172,15 @@
         if self.discovery and self.discoveryConfig:
             registTask = asyncio.create_task(self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True))
             tasks.append(registTask)
         await asyncio.wait(tasks)
 
     def serve(self):
         print('http rpc running on http://%s:%s' % (self.host, self.port) )
+        self.dumpRpcFuncs()
         asyncio.run(self.asyncServe())
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
@@ -251,17 +260,17 @@
         tasks = []
         tRegist = None
         if self.discovery and self.discoveryConfig:
             tRegist = self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
             tasks.append(tRegist)
         coro = asyncio.start_server(self.handle, self.host, self.port, loop=loop)
         tasks.append(coro)
-        rs = loop.run_until_complete(asyncio.gather(*tasks))
-        self.printLogo()
         print('tcp rpc running on tcp://%s:%s' % (self.host, self.port) )
+        self.dumpRpcFuncs()
+        rs = loop.run_until_complete(asyncio.gather(*tasks))
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         server = rs[-1]
         # Close the server
         server.close()
@@ -294,24 +303,43 @@
                 msg = body.get('msg')
                 request = self.protocal.unserialize(msg)
                 func, args, kwargs = self.protocal.parseRequest(request)
                 resp = self.run(func, args, kwargs)
                 self.protocal.transport.sendPeer(self.protocal.serialize(resp), addr = addr)
             except Exception as ex:
                 print('UDP handler exception:', ex)
-    
-    def serve(self):
-        self.startWorkers()
-        self.protocal.transport.bind()
-        self.printLogo()
-        print('udp rpc running on udp://%s:%s' % (self.host, self.port))
-        if self.discovery and self.discoveryConfig:
-            self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
+
+    async def handlePackage(self):
         while 1:
             try:
                 msg, cliAddr = self.protocal.transport.recv()
                 self.queue.put({'msg' : msg, 'addr' : cliAddr})
             except socket.timeout:
                 pass
 
+    async def asyncServe(self):
+        self.startWorkers()
+        self.protocal.transport.bind()
+        self.printLogo()
+        print('udp rpc running on udp://%s:%s' % (self.host, self.port))
+        self.dumpRpcFuncs()
+        tasks = []
+        if self.discovery and self.discoveryConfig:
+            tasks.append(asyncio.create_task(self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)))
+        tasks.append(asyncio.create_task(self.handlePackage()))
+        loop = asyncio.get_event_loop()
+        rs = loop.run_until_complete(asyncio.gather(*tasks))
+        try:
+            loop.run_forever()
+        except KeyboardInterrupt:
+            pass
+        server = rs[-1]
+        # Close the server
+        server.close()
+        loop.run_until_complete(server.wait_closed())
+        loop.close()
+    
+    def serve(self):
+        asyncio.run(self.asyncServe())
+
 
 rpc = RpcServer.rpc
```

### Comparing `sunyata-0.0.39/sunyata/rpc/discovery.py` & `sunyata-0.0.40/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/transport.py` & `sunyata-0.0.40/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/client.py` & `sunyata-0.0.40/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/method.py` & `sunyata-0.0.40/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/rpc/protocal.py` & `sunyata-0.0.40/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/sunyata/table_writer.py` & `sunyata-0.0.40/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/README.md` & `sunyata-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.39/setup.py` & `sunyata-0.0.40/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.39'
+DEFINE_VERSION = '0.0.40'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'ujson==1.35',
     'uvloop==0.19.0',
     'uvicorn==0.18.0',
```

