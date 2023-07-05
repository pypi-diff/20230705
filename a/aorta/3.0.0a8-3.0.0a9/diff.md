# Comparing `tmp/aorta-3.0.0a8.tar.gz` & `tmp/aorta-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta-3.0.0a8.tar", last modified: Sun Mar  5 16:59:29 2023, max compression
+gzip compressed data, was "aorta-3.0.0a9.tar", last modified: Sun Mar  5 18:51:52 2023, max compression
```

## Comparing `aorta-3.0.0a8.tar` & `aorta-3.0.0a9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.919656 aorta-3.0.0a8/
--rw-r--r--   0 cochise    (501) staff       (20)      291 2022-02-08 18:24:28.000000 aorta-3.0.0a8/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)     1665 2023-03-05 16:59:29.919433 aorta-3.0.0a8/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-05 16:59:17.000000 aorta-3.0.0a8/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.909337 aorta-3.0.0a8/aorta/
--rw-r--r--   0 cochise    (501) staff       (20)     1572 2023-03-05 13:51:54.000000 aorta-3.0.0a8/aorta/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     5093 2023-03-05 14:05:20.000000 aorta-3.0.0a8/aorta/baserunner.py
--rw-r--r--   0 cochise    (501) staff       (20)      876 2023-02-28 09:44:55.000000 aorta-3.0.0a8/aorta/commandhandler.py
--rw-r--r--   0 cochise    (501) staff       (20)      897 2023-02-28 09:45:01.000000 aorta-3.0.0a8/aorta/eventlistener.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.906044 aorta-3.0.0a8/aorta/ext/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.910376 aorta-3.0.0a8/aorta/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)      493 2023-02-28 14:32:02.000000 aorta-3.0.0a8/aorta/ext/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3153 2023-02-28 14:57:43.000000 aorta-3.0.0a8/aorta/ext/google/pubsubtransport.py
--rw-r--r--   0 cochise    (501) staff       (20)      704 2023-03-04 10:21:17.000000 aorta-3.0.0a8/aorta/localrunner.py
--rw-r--r--   0 cochise    (501) staff       (20)     2449 2023-03-05 14:39:25.000000 aorta-3.0.0a8/aorta/messagehandler.py
--rw-r--r--   0 cochise    (501) staff       (20)     1256 2023-02-28 13:52:55.000000 aorta-3.0.0a8/aorta/messagepublisher.py
--rw-r--r--   0 cochise    (501) staff       (20)      838 2023-02-28 13:53:31.000000 aorta-3.0.0a8/aorta/nulltransport.py
--rw-r--r--   0 cochise    (501) staff       (20)     1715 2023-02-28 14:48:57.000000 aorta-3.0.0a8/aorta/package.json
--rw-r--r--   0 cochise    (501) staff       (20)      624 2023-03-02 03:07:06.000000 aorta-3.0.0a8/aorta/ping.py
--rw-r--r--   0 cochise    (501) staff       (20)     1623 2023-03-05 14:05:04.000000 aorta-3.0.0a8/aorta/provider.py
--rw-r--r--   0 cochise    (501) staff       (20)     1137 2023-03-05 16:58:50.000000 aorta-3.0.0a8/aorta/sewer.py
--rw-r--r--   0 cochise    (501) staff       (20)     1618 2023-03-05 14:35:51.000000 aorta-3.0.0a8/aorta/transaction.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.914902 aorta-3.0.0a8/aorta/types/
--rw-r--r--   0 cochise    (501) staff       (20)     1358 2023-02-28 12:29:39.000000 aorta-3.0.0a8/aorta/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1184 2023-03-05 14:34:57.000000 aorta-3.0.0a8/aorta/types/command.py
--rw-r--r--   0 cochise    (501) staff       (20)      624 2023-02-28 09:29:59.000000 aorta-3.0.0a8/aorta/types/commandenvelope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1301 2023-02-28 09:38:44.000000 aorta-3.0.0a8/aorta/types/commandtype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1576 2023-02-28 13:25:23.000000 aorta-3.0.0a8/aorta/types/envelope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1238 2023-03-05 14:34:07.000000 aorta-3.0.0a8/aorta/types/event.py
--rw-r--r--   0 cochise    (501) staff       (20)      622 2023-02-28 01:49:21.000000 aorta-3.0.0a8/aorta/types/eventenvelope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1281 2023-02-28 09:38:53.000000 aorta-3.0.0a8/aorta/types/eventtype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1031 2023-03-05 14:33:00.000000 aorta-3.0.0a8/aorta/types/imessagehandler.py
--rw-r--r--   0 cochise    (501) staff       (20)      745 2023-02-28 13:41:31.000000 aorta-3.0.0a8/aorta/types/ipublisher.py
--rw-r--r--   0 cochise    (501) staff       (20)      568 2023-03-04 10:21:17.000000 aorta-3.0.0a8/aorta/types/irunner.py
--rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-03-05 14:32:33.000000 aorta-3.0.0a8/aorta/types/itransaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      664 2023-02-28 13:53:06.000000 aorta-3.0.0a8/aorta/types/itransport.py
--rw-r--r--   0 cochise    (501) staff       (20)      576 2023-02-28 08:33:36.000000 aorta-3.0.0a8/aorta/types/message.py
--rw-r--r--   0 cochise    (501) staff       (20)     2635 2023-02-28 09:41:58.000000 aorta-3.0.0a8/aorta/types/messagehandlertype.py
--rw-r--r--   0 cochise    (501) staff       (20)     2509 2023-03-05 14:26:46.000000 aorta-3.0.0a8/aorta/types/messageheader.py
--rw-r--r--   0 cochise    (501) staff       (20)     2043 2023-03-05 14:37:41.000000 aorta-3.0.0a8/aorta/types/messagemetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     1711 2023-02-28 09:38:32.000000 aorta-3.0.0a8/aorta/types/messagetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      721 2023-03-05 14:31:52.000000 aorta-3.0.0a8/aorta/types/publishable.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.915959 aorta-3.0.0a8/aorta/types/test/
--rw-r--r--   0 cochise    (501) staff       (20)     3854 2023-03-05 14:03:16.000000 aorta-3.0.0a8/aorta/types/test/messagehandler.py
--rw-r--r--   0 cochise    (501) staff       (20)     4707 2023-03-05 14:37:29.000000 aorta-3.0.0a8/aorta/types/test/messagetype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1615 2023-02-28 09:40:35.000000 aorta-3.0.0a8/aorta/types/test/transaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      882 2023-02-28 14:57:04.000000 aorta-3.0.0a8/aorta/types/test/transport.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.909900 aorta-3.0.0a8/aorta.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)     1665 2023-03-05 16:59:29.000000 aorta-3.0.0a8/aorta.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)     1403 2023-03-05 16:59:29.000000 aorta-3.0.0a8/aorta.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-05 16:59:29.000000 aorta-3.0.0a8/aorta.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)       89 2023-03-05 16:59:29.000000 aorta-3.0.0a8/aorta.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       28 2023-03-05 16:59:29.000000 aorta-3.0.0a8/aorta.egg-info/top_level.txt
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.906280 aorta-3.0.0a8/docs/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.916250 aorta-3.0.0a8/docs/source/
--rw-r--r--   0 cochise    (501) staff       (20)      937 2023-02-28 00:54:45.000000 aorta-3.0.0a8/docs/source/conf.py
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-05 16:59:29.919716 aorta-3.0.0a8/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1425 2022-02-08 18:24:28.000000 aorta-3.0.0a8/setup.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.916625 aorta-3.0.0a8/tests/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 00:54:45.000000 aorta-3.0.0a8/tests/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1860 2023-02-28 12:54:33.000000 aorta-3.0.0a8/tests/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.916911 aorta-3.0.0a8/tests/ext/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 14:32:27.000000 aorta-3.0.0a8/tests/ext/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.917598 aorta-3.0.0a8/tests/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 14:32:38.000000 aorta-3.0.0a8/tests/ext/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      667 2023-02-28 14:45:44.000000 aorta-3.0.0a8/tests/ext/google/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)      588 2023-02-28 14:35:59.000000 aorta-3.0.0a8/tests/ext/google/test_system_event.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 16:59:29.918269 aorta-3.0.0a8/tests/types/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 00:54:45.000000 aorta-3.0.0a8/tests/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1187 2023-02-28 09:40:48.000000 aorta-3.0.0a8/tests/types/test_unit_command.py
--rw-r--r--   0 cochise    (501) staff       (20)     1177 2023-02-28 09:40:52.000000 aorta-3.0.0a8/tests/types/test_unit_event.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.130412 aorta-3.0.0a9/
+-rw-r--r--   0 cochise    (501) staff       (20)      291 2022-02-08 18:24:28.000000 aorta-3.0.0a9/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)     1665 2023-03-05 18:51:52.130256 aorta-3.0.0a9/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-05 18:51:43.000000 aorta-3.0.0a9/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.121469 aorta-3.0.0a9/aorta/
+-rw-r--r--   0 cochise    (501) staff       (20)     1572 2023-03-05 13:51:54.000000 aorta-3.0.0a9/aorta/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4870 2023-03-05 18:51:08.000000 aorta-3.0.0a9/aorta/baserunner.py
+-rw-r--r--   0 cochise    (501) staff       (20)      876 2023-02-28 09:44:55.000000 aorta-3.0.0a9/aorta/commandhandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)      897 2023-02-28 09:45:01.000000 aorta-3.0.0a9/aorta/eventlistener.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.117477 aorta-3.0.0a9/aorta/ext/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.123006 aorta-3.0.0a9/aorta/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)      493 2023-02-28 14:32:02.000000 aorta-3.0.0a9/aorta/ext/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3153 2023-02-28 14:57:43.000000 aorta-3.0.0a9/aorta/ext/google/pubsubtransport.py
+-rw-r--r--   0 cochise    (501) staff       (20)      704 2023-03-04 10:21:17.000000 aorta-3.0.0a9/aorta/localrunner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2449 2023-03-05 14:39:25.000000 aorta-3.0.0a9/aorta/messagehandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1256 2023-02-28 13:52:55.000000 aorta-3.0.0a9/aorta/messagepublisher.py
+-rw-r--r--   0 cochise    (501) staff       (20)      838 2023-02-28 13:53:31.000000 aorta-3.0.0a9/aorta/nulltransport.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1715 2023-02-28 14:48:57.000000 aorta-3.0.0a9/aorta/package.json
+-rw-r--r--   0 cochise    (501) staff       (20)      624 2023-03-02 03:07:06.000000 aorta-3.0.0a9/aorta/ping.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1623 2023-03-05 14:05:04.000000 aorta-3.0.0a9/aorta/provider.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1137 2023-03-05 16:58:50.000000 aorta-3.0.0a9/aorta/sewer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1618 2023-03-05 14:35:51.000000 aorta-3.0.0a9/aorta/transaction.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.127573 aorta-3.0.0a9/aorta/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1358 2023-02-28 12:29:39.000000 aorta-3.0.0a9/aorta/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1184 2023-03-05 14:34:57.000000 aorta-3.0.0a9/aorta/types/command.py
+-rw-r--r--   0 cochise    (501) staff       (20)      624 2023-02-28 09:29:59.000000 aorta-3.0.0a9/aorta/types/commandenvelope.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1507 2023-03-05 18:50:01.000000 aorta-3.0.0a9/aorta/types/commandtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1576 2023-02-28 13:25:23.000000 aorta-3.0.0a9/aorta/types/envelope.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1238 2023-03-05 14:34:07.000000 aorta-3.0.0a9/aorta/types/event.py
+-rw-r--r--   0 cochise    (501) staff       (20)      622 2023-02-28 01:49:21.000000 aorta-3.0.0a9/aorta/types/eventenvelope.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1481 2023-03-05 18:48:25.000000 aorta-3.0.0a9/aorta/types/eventtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1031 2023-03-05 14:33:00.000000 aorta-3.0.0a9/aorta/types/imessagehandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)      745 2023-02-28 13:41:31.000000 aorta-3.0.0a9/aorta/types/ipublisher.py
+-rw-r--r--   0 cochise    (501) staff       (20)      568 2023-03-04 10:21:17.000000 aorta-3.0.0a9/aorta/types/irunner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-03-05 14:32:33.000000 aorta-3.0.0a9/aorta/types/itransaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      664 2023-02-28 13:53:06.000000 aorta-3.0.0a9/aorta/types/itransport.py
+-rw-r--r--   0 cochise    (501) staff       (20)      576 2023-02-28 08:33:36.000000 aorta-3.0.0a9/aorta/types/message.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2635 2023-02-28 09:41:58.000000 aorta-3.0.0a9/aorta/types/messagehandlertype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2509 2023-03-05 14:26:46.000000 aorta-3.0.0a9/aorta/types/messageheader.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2043 2023-03-05 14:37:41.000000 aorta-3.0.0a9/aorta/types/messagemetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1821 2023-03-05 18:39:40.000000 aorta-3.0.0a9/aorta/types/messagetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      721 2023-03-05 14:31:52.000000 aorta-3.0.0a9/aorta/types/publishable.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.128283 aorta-3.0.0a9/aorta/types/test/
+-rw-r--r--   0 cochise    (501) staff       (20)     3694 2023-03-05 18:22:45.000000 aorta-3.0.0a9/aorta/types/test/messagehandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4801 2023-03-05 18:47:47.000000 aorta-3.0.0a9/aorta/types/test/messagetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1615 2023-02-28 09:40:35.000000 aorta-3.0.0a9/aorta/types/test/transaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      882 2023-02-28 14:57:04.000000 aorta-3.0.0a9/aorta/types/test/transport.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.122633 aorta-3.0.0a9/aorta.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)     1665 2023-03-05 18:51:52.000000 aorta-3.0.0a9/aorta.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)     1403 2023-03-05 18:51:52.000000 aorta-3.0.0a9/aorta.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-05 18:51:52.000000 aorta-3.0.0a9/aorta.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       89 2023-03-05 18:51:52.000000 aorta-3.0.0a9/aorta.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       28 2023-03-05 18:51:52.000000 aorta-3.0.0a9/aorta.egg-info/top_level.txt
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.117719 aorta-3.0.0a9/docs/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.128529 aorta-3.0.0a9/docs/source/
+-rw-r--r--   0 cochise    (501) staff       (20)      937 2023-02-28 00:54:45.000000 aorta-3.0.0a9/docs/source/conf.py
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-05 18:51:52.130447 aorta-3.0.0a9/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1425 2022-02-08 18:24:28.000000 aorta-3.0.0a9/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.128865 aorta-3.0.0a9/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 00:54:45.000000 aorta-3.0.0a9/tests/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2042 2023-03-05 18:23:25.000000 aorta-3.0.0a9/tests/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.128984 aorta-3.0.0a9/tests/ext/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 14:32:27.000000 aorta-3.0.0a9/tests/ext/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.129374 aorta-3.0.0a9/tests/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 14:32:38.000000 aorta-3.0.0a9/tests/ext/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      667 2023-02-28 14:45:44.000000 aorta-3.0.0a9/tests/ext/google/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      588 2023-02-28 14:35:59.000000 aorta-3.0.0a9/tests/ext/google/test_system_event.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-05 18:51:52.129991 aorta-3.0.0a9/tests/types/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-28 00:54:45.000000 aorta-3.0.0a9/tests/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1187 2023-02-28 09:40:48.000000 aorta-3.0.0a9/tests/types/test_unit_command.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1177 2023-02-28 09:40:52.000000 aorta-3.0.0a9/tests/types/test_unit_event.py
```

### Comparing `aorta-3.0.0a8/PKG-INFO` & `aorta-3.0.0a9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aorta
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: Enter a description for this Unimatrix package
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `aorta-3.0.0a8/aorta/__init__.py` & `aorta-3.0.0a9/aorta/__init__.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/baserunner.py` & `aorta-3.0.0a9/aorta/baserunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,15 @@
 class BaseRunner:
     __module__: str = 'aorta'
     logger: logging.Logger = logging.getLogger('aorta')
     provider: type[Provider] | Provider
     publisher: IPublisher
 
     async def run(self, envelope: Envelope[Any]) -> bool:
-        if not envelope.is_known():
-            self.logger.critical(
-                "Got unexpected Aorta message: %s/%s (id: %s)",
-                envelope.api_version, envelope.kind, envelope.metadata.uid
-            )
-            return True
-        if envelope.is_bound():
+        if envelope.is_bound() and envelope.is_known():
             handlers = self.get_handlers(envelope, False)
             assert len(handlers) == 1, len(handlers)
             handler_class = handlers.pop()
             self.logger.debug(
                 "Running handler %s for bound envelope (id: %s, kind; %s, version: %s)",
                 handler_class.__name__, envelope.metadata.uid, envelope.kind,
                 envelope.api_version
```

### Comparing `aorta-3.0.0a8/aorta/commandhandler.py` & `aorta-3.0.0a9/aorta/commandhandler.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/eventlistener.py` & `aorta-3.0.0a9/aorta/eventlistener.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/ext/google/pubsubtransport.py` & `aorta-3.0.0a9/aorta/ext/google/pubsubtransport.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/localrunner.py` & `aorta-3.0.0a9/aorta/localrunner.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/messagehandler.py` & `aorta-3.0.0a9/aorta/messagehandler.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/messagepublisher.py` & `aorta-3.0.0a9/aorta/messagepublisher.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/nulltransport.py` & `aorta-3.0.0a9/aorta/nulltransport.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/package.json` & `aorta-3.0.0a9/aorta/package.json`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/ping.py` & `aorta-3.0.0a9/aorta/ping.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/provider.py` & `aorta-3.0.0a9/aorta/provider.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/sewer.py` & `aorta-3.0.0a9/aorta/sewer.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/transaction.py` & `aorta-3.0.0a9/aorta/transaction.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/__init__.py` & `aorta-3.0.0a9/aorta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/command.py` & `aorta-3.0.0a9/aorta/types/command.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/commandenvelope.py` & `aorta-3.0.0a9/aorta/types/commandenvelope.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/commandtype.py` & `aorta-3.0.0a9/aorta/types/commandtype.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,23 +12,32 @@
 import pydantic.main
 
 from .commandenvelope import CommandEnvelope
 from .messageheader import MessageHeader
 from .messagetype import MessageType
 
 
+class UnknownCommandEnvelope(CommandEnvelope[Any]):
+    spec: dict[str, Any]
+
+    def is_known(self) -> bool:
+        return False
+
+
 class CommandType(MessageType):
     __module__: str = 'aorta.types'
     __registry__: dict[tuple[str, str], type[CommandEnvelope[Any]]] = {}
     envelope_attr: str = 'spec'
     envelope_class: type[CommandEnvelope[Any]] = CommandEnvelope
     typename: str = 'unimatrixone.io/command'
 
     @staticmethod
     def parse(data: Any) -> CommandEnvelope[Any] | MessageHeader | None:
         header = None
         try:
             header = MessageHeader.parse_obj(data)
             if header.type == CommandType.typename:
                 return CommandType.__registry__[(header.api_version, header.kind)].parse_obj(data)
-        except (pydantic.ValidationError, KeyError, TypeError, ValueError):
+        except KeyError:
+            return UnknownCommandEnvelope.parse_obj(data)
+        except (pydantic.ValidationError, TypeError, ValueError):
             return header
```

### Comparing `aorta-3.0.0a8/aorta/types/envelope.py` & `aorta-3.0.0a9/aorta/types/envelope.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/event.py` & `aorta-3.0.0a9/aorta/types/event.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/eventenvelope.py` & `aorta-3.0.0a9/aorta/types/eventenvelope.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/eventtype.py` & `aorta-3.0.0a9/aorta/types/eventtype.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,32 @@
 import pydantic.main
 
 from .eventenvelope import EventEnvelope
 from .messageheader import MessageHeader
 from .messagetype import MessageType
 
 
+class UnknownEventEnvelope(EventEnvelope[Any]):
+    data: dict[str, Any]
+
+    def is_known(self) -> bool:
+        return False
+
+
 class EventType(MessageType):
     __module__: str = 'aorta.types'
     __registry__: dict[tuple[str, str], type[EventEnvelope[Any]]] = {}
     envelope_attr: str = 'data'
     envelope_class: type[EventEnvelope[Any]] = EventEnvelope
     typename: str = 'unimatrixone.io/event'
 
     @staticmethod
     def parse(data: Any) -> EventEnvelope[Any] | MessageHeader | None:
         header = None
         try:
             header = MessageHeader.parse_obj(data)
             if header.type == EventType.typename:
                 return EventType.__registry__[(header.api_version, header.kind)].parse_obj(data)
-        except (pydantic.ValidationError, KeyError, TypeError, ValueError):
+        except KeyError:
+            return UnknownEventEnvelope.parse_obj(data)
+        except (pydantic.ValidationError, TypeError, ValueError):
             return header
```

### Comparing `aorta-3.0.0a8/aorta/types/imessagehandler.py` & `aorta-3.0.0a9/aorta/types/imessagehandler.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/ipublisher.py` & `aorta-3.0.0a9/aorta/types/ipublisher.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/irunner.py` & `aorta-3.0.0a9/aorta/types/irunner.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/itransaction.py` & `aorta-3.0.0a9/aorta/types/itransaction.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/itransport.py` & `aorta-3.0.0a9/aorta/types/itransport.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/message.py` & `aorta-3.0.0a9/aorta/types/message.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/messagehandlertype.py` & `aorta-3.0.0a9/aorta/types/messagehandlertype.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/messageheader.py` & `aorta-3.0.0a9/aorta/types/messageheader.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/messagemetadata.py` & `aorta-3.0.0a9/aorta/types/messagemetadata.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/messagetype.py` & `aorta-3.0.0a9/aorta/types/messagetype.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         cls,
         name: str,
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **params: Any
     ) -> 'MessageType':
         is_abstract = namespace.pop('__abstract__', False)
+        skip_register: bool = namespace.pop('__aorta_disable__', False)
         new_class =  super().__new__(cls, name, bases, namespace, **params) # type: ignore
         namespace.setdefault('__version__', 'v1')
         if not is_abstract:
             k: tuple[str, str] = (namespace['__version__'], name)
             if k in cls.__registry__:
                 raise TypeError('Message {0}/{1} is already registered.'.format(*k))
             new_class.__envelope__ = type(
@@ -40,10 +41,11 @@
                 (cls.envelope_class,), # type: ignore
                 {
                     '__annotations__': {
                         cls.envelope_attr: new_class
                     }
                 }
             )
-            cls.__registry__[k] = new_class.__envelope__ # type: ignore
+            if not skip_register:
+                cls.__registry__[k] = new_class.__envelope__ # type: ignore
         
         return new_class # type: ignore
```

### Comparing `aorta-3.0.0a8/aorta/types/publishable.py` & `aorta-3.0.0a9/aorta/types/publishable.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/test/messagehandler.py` & `aorta-3.0.0a9/aorta/types/test/messagehandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
 from unittest.mock import AsyncMock
 
 import pytest
 
 import aorta
 
 
@@ -21,22 +20,14 @@
     'test_run_exception_on_bound_envelope',
     'test_run_exception_on_unbound_envelope',
     'test_publish_event',
     'test_get_handlers',
 ]
 
 
-class Sewer(aorta.Sewer):
-
-    async def handle(self, message: aorta.types.Envelope[Any]) -> None:
-        pass
-
-aorta.register(Sewer)
-
-
 @pytest.mark.asyncio
 async def test_handle_success(
     transaction: aorta.types.ITransaction,
     message: aorta.types.Publishable,
     MessageHandler: type[aorta.types.IMessageHandler]
 ):
     envelope = message.envelope()
```

### Comparing `aorta-3.0.0a8/aorta/types/test/messagetype.py` & `aorta-3.0.0a9/aorta/types/test/messagetype.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,17 +129,22 @@
 
 
 def test_parse_valid_unknown(
     message: aorta.types.Publishable,
     parse: Callable[[Any], aorta.types.Envelope[Any] | None]
 ):
     cls = type(type(message))
-    e2 = parse({'apiVersion': 'v1', 'kind': 'Unknown', 'type': cls.typename})
+    e2 = parse({
+        **message.envelope().dict(),
+        'apiVersion': 'v1',
+        'kind': 'Unknown',
+        'type': cls.typename
+    })
     assert e2 is not None
-    assert type(e2) == aorta.types.MessageHeader
+    assert not e2.is_known()
     assert e2.kind == 'Unknown', e2.kind
     assert e2.api_version == 'v1', e2.api_version
 
 
 def test_global_parse_unknown():
     assert aorta.parse({'apiVersion': 'v1', 'kind': 'Unknown'}) is None
     assert aorta.parse([]) is None
@@ -155,12 +160,17 @@
     assert e1.metadata.uid == e2.metadata.uid
 
 
 def test_global_parse_valid_unknown(
     message: aorta.types.Publishable,
 ):
     cls = type(type(message))
-    e2 = aorta.parse({'apiVersion': 'v1', 'kind': 'Unknown', 'type': cls.typename})
+    e2 = aorta.parse({
+        **message.envelope().dict(),
+        'apiVersion': 'v1',
+        'kind': 'Unknown',
+        'type': cls.typename
+    })
     assert e2 is not None
-    assert type(e2) == aorta.types.MessageHeader
+    assert not e2.is_known()
     assert e2.kind == 'Unknown', e2.kind
     assert e2.api_version == 'v1', e2.api_version
```

### Comparing `aorta-3.0.0a8/aorta/types/test/transaction.py` & `aorta-3.0.0a9/aorta/types/test/transaction.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta/types/test/transport.py` & `aorta-3.0.0a9/aorta/types/test/transport.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/aorta.egg-info/PKG-INFO` & `aorta-3.0.0a9/aorta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aorta
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: Enter a description for this Unimatrix package
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `aorta-3.0.0a8/aorta.egg-info/SOURCES.txt` & `aorta-3.0.0a9/aorta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/docs/source/conf.py` & `aorta-3.0.0a9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/setup.py` & `aorta-3.0.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/tests/conftest.py` & `aorta-3.0.0a9/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 
 
 @pytest.fixture # type: ignore
 def EventListener() -> type[aorta.MessageHandler]:
     return FooListener
 
 
+@pytest.fixture # type: ignore
+def Sewer() -> type[aorta.MessageHandler]:
+    return FallbackHandler
+
+
 @pytest.fixture
 def command() -> aorta.Command:
     return FooCommand(foo=1)
 
 
 @pytest.fixture
 def event() -> aorta.Event:
@@ -68,19 +73,24 @@
 
 class FooHandler(aorta.CommandHandler):
 
     async def handle(self, command: FooCommand):
         return 'foo'
 
 
+class FallbackHandler(aorta.Sewer):
+    pass
+
+
 class FooEvent(aorta.Event):
     foo: int
 
 
 class FooListener(aorta.EventListener):
 
     async def handle(self, event: FooEvent):
         return 'foo'
 
 
 aorta.register(FooHandler)
-aorta.register(FooListener)
+aorta.register(FooListener)
+aorta.register(FallbackHandler)
```

### Comparing `aorta-3.0.0a8/tests/ext/google/conftest.py` & `aorta-3.0.0a9/tests/ext/google/conftest.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/tests/ext/google/test_system_event.py` & `aorta-3.0.0a9/tests/ext/google/test_system_event.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/tests/types/test_unit_command.py` & `aorta-3.0.0a9/tests/types/test_unit_command.py`

 * *Files identical despite different names*

### Comparing `aorta-3.0.0a8/tests/types/test_unit_event.py` & `aorta-3.0.0a9/tests/types/test_unit_event.py`

 * *Files identical despite different names*

