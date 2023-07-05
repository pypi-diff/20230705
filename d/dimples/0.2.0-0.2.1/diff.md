# Comparing `tmp/dimples-0.2.0.tar.gz` & `tmp/dimples-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.2.0.tar", last modified: Sun Jun 18 14:42:05 2023, max compression
+gzip compressed data, was "dist/dimples-0.2.1.tar", last modified: Wed Jul  5 17:47:29 2023, max compression
```

## Comparing `dimples-0.2.0.tar` & `dimples-0.2.1.tar`

### file list

```diff
@@ -1,138 +1,135 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-18 14:42:05.000000 dimples-0.2.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.0/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7204 2023-06-18 14:35:59.000000 dimples-0.2.0/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.2.0/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.2.0/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.2.0/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.2.0/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.2.0/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.2.0/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.2.0/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.0/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.0/dimples/client/cpu/text.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.0/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     9951 2023-06-12 14:16:50.000000 dimples-0.2.0/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.0/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.0/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.0/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.0/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.2.0/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.0/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2235 2023-06-18 14:35:34.000000 dimples-0.2.0/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5559 2023-06-18 11:38:34.000000 dimples-0.2.0/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.0/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.0/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.0/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.0/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.0/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.0/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.0/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-06-18 14:35:34.000000 dimples-0.2.0/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.0/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.0/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.0/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.2.0/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.0/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.0/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.0/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.0/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.0/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.0/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.0/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.0/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.0/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.0/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.0/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.0/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.2.0/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.0/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.0/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.0/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.0/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.0/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.0/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.0/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.0/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.0/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.0/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.0/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.0/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.0/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.0/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.0/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.0/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.0/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.0/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.0/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.2.0/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.0/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.0/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.0/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2681 2023-06-18 09:57:24.000000 dimples-0.2.0/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.0/dimples/server/broadcast.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.2.0/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2668 2023-06-17 15:58:30.000000 dimples-0.2.0/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.2.0/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3464 2023-06-12 12:55:43.000000 dimples-0.2.0/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.2.0/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13588 2023-06-17 07:30:46.000000 dimples-0.2.0/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.0/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.0/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.2.0/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.0/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     7978 2023-06-16 11:57:03.000000 dimples-0.2.0/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)     9704 2023-06-18 10:50:13.000000 dimples-0.2.0/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.0/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.0/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     6089 2023-06-18 11:39:31.000000 dimples-0.2.0/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.0/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.0/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.0/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.0/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.0/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3265 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-18 14:42:05.000000 dimples-0.2.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-16 08:07:02.000000 dimples-0.2.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-05 17:47:29.000000 dimples-0.2.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.1/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7179 2023-07-05 16:12:35.000000 dimples-0.2.1/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1966 2023-07-05 17:00:59.000000 dimples-0.2.1/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2117 2023-07-05 16:57:49.000000 dimples-0.2.1/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.2.1/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.2.1/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.2.1/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.2.1/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.2.1/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.1/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.1/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.1/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     9952 2023-07-05 17:01:39.000000 dimples-0.2.1/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.1/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.1/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.1/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.1/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7022 2023-07-05 17:01:13.000000 dimples-0.2.1/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.1/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2213 2023-07-05 16:06:45.000000 dimples-0.2.1/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5644 2023-06-19 15:11:53.000000 dimples-0.2.1/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.1/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.1/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.1/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.1/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.1/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.1/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.1/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2023-07-05 16:06:45.000000 dimples-0.2.1/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.1/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.1/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.1/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.1/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.1/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.1/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.1/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.1/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.1/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.1/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.1/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.1/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.1/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.1/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.1/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7085 2023-06-19 07:42:03.000000 dimples-0.2.1/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.1/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.1/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.1/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.1/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.1/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.1/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.1/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.1/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.1/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.1/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.1/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.1/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.1/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.1/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.1/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.1/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.1/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.1/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.1/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5929 2023-06-19 07:20:16.000000 dimples-0.2.1/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.1/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.1/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.1/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2654 2023-07-05 16:58:00.000000 dimples-0.2.1/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.1/dimples/server/broadcast.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.2.1/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2023-07-05 17:27:48.000000 dimples-0.2.1/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-19 07:56:29.000000 dimples-0.2.1/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3610 2023-07-05 17:26:22.000000 dimples-0.2.1/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4009 2023-07-05 17:20:53.000000 dimples-0.2.1/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3517 2023-07-05 17:23:20.000000 dimples-0.2.1/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13524 2023-07-05 17:00:59.000000 dimples-0.2.1/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.1/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.1/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5615 2023-07-05 17:00:01.000000 dimples-0.2.1/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.1/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     7978 2023-06-16 11:57:03.000000 dimples-0.2.1/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)     9722 2023-06-26 11:02:55.000000 dimples-0.2.1/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.1/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.1/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     6424 2023-06-19 07:20:09.000000 dimples-0.2.1/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.1/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.1/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.1/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.1/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.1/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3170 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-05 17:47:29.000000 dimples-0.2.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-07-05 17:12:33.000000 dimples-0.2.1/setup.py
```

### Comparing `dimples-0.2.0/PKG-INFO` & `dimples-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.0
+Version: 0.2.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.0/README.md` & `dimples-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/__init__.py` & `dimples-0.2.1/dimples/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 # SOFTWARE.
 # ==============================================================================
 
 from mkm.protocol import *
 from dimp.mkm import *
 from dimp.dkd import *
 from dimsdk import *
-from dimsdk.cpu import *
 from dimplugins import *
 from dimplugins.network import NetworkType
 from dimplugins.entity import EntityID, EntityIDFactory
 
 from .common import *
 from .config import Config
```

### Comparing `dimples-0.2.0/dimples/client/__init__.py` & `dimples-0.2.1/dimples/client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = [
 
     #
     #   CPU
     #
     'HandshakeCommandProcessor',
     'LoginCommandProcessor',
-    'ReceiptCommandProcessor',
 
     #
     #   Client
     #
     'ClientSession', 'SessionState',
 
     'GroupManager',
```

### Comparing `dimples-0.2.0/dimples/client/cpu/__init__.py` & `dimples-0.2.1/dimples/client/cpu/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,28 +30,28 @@
     Processors for contents
 """
 
 from .text import TextContentProcessor
 
 from .handshake import HandshakeCommandProcessor
 from .login import LoginCommandProcessor
-from .receipt import ReceiptCommandProcessor
 
 from .history import HistoryCommandProcessor, GroupCommandProcessor
 from .grp_invite import InviteCommandProcessor
 from .grp_expel import ExpelCommandProcessor
 from .grp_quit import QuitCommandProcessor
 from .grp_reset import ResetCommandProcessor
 from .grp_query import QueryCommandProcessor
 
 __all__ = [
+
     'TextContentProcessor',
 
     'HandshakeCommandProcessor',
     'LoginCommandProcessor',
-    'ReceiptCommandProcessor',
 
     'HistoryCommandProcessor',
     'GroupCommandProcessor',
     'InviteCommandProcessor', 'ExpelCommandProcessor', 'QuitCommandProcessor',
     'ResetCommandProcessor', 'QueryCommandProcessor',
+
 ]
```

### Comparing `dimples-0.2.0/dimples/client/cpu/grp_expel.py` & `dimples-0.2.1/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/grp_invite.py` & `dimples-0.2.1/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/grp_query.py` & `dimples-0.2.1/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/grp_quit.py` & `dimples-0.2.1/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/grp_reset.py` & `dimples-0.2.1/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/handshake.py` & `dimples-0.2.1/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/history.py` & `dimples-0.2.1/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/login.py` & `dimples-0.2.1/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/cpu/receipt.py` & `dimples-0.2.1/dimples/client/cpu/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2019 Albert Moky
+# Copyright (c) 2023 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,29 +20,29 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Receipt Command Processor
-    ~~~~~~~~~~~~~~~~~~~~~~~~~
+    Text Command Processor
+    ~~~~~~~~~~~~~~~~~~~~~~
 
 """
 
 from typing import List
 
 from dimp import ReliableMessage
-from dimp import Content
+from dimp import Content, TextContent
 
-from dimsdk.cpu import BaseCommandProcessor
+from dimsdk.cpu import BaseContentProcessor
 
-from ...common import ReceiptCommand
+from ...utils import Log
 
 
-class ReceiptCommandProcessor(BaseCommandProcessor):
+class TextContentProcessor(BaseContentProcessor):
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, ReceiptCommand), 'receipt command error: %s' % content
-        # nickname = self.facebook.name(identifier=sender)
+        assert isinstance(content, TextContent), 'text content error: %s' % content
+        Log.warning(msg='received text content: %s, %s => %s' % (content.get_str(key='text'), msg.sender, msg.receiver))
         return []
```

### Comparing `dimples-0.2.0/dimples/client/cpu/text.py` & `dimples-0.2.1/dimples/server/cpu/ans.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,29 +20,54 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Text Command Processor
-    ~~~~~~~~~~~~~~~~~~~~~~
+    Command Processor for 'ans'
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+    ANS protocol
 """
 
-from typing import List
+from typing import Optional, List
 
+from dimp import ID
 from dimp import ReliableMessage
-from dimp import Content, TextContent
+from dimp import Content
 
-from dimsdk.cpu import BaseContentProcessor
+from dimsdk.cpu import BaseCommandProcessor
 
 from ...utils import Log
+from ...common import AnsCommand
 
 
-class TextContentProcessor(BaseContentProcessor):
+class AnsCommandProcessor(BaseCommandProcessor):
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, TextContent), 'text content error: %s' % content
-        Log.warning(msg='received text content: %s, %s => %s' % (content.get_str(key='text'), msg.sender, msg.receiver))
-        return []
+        assert isinstance(content, AnsCommand), 'report command error: %s' % content
+        names = content.names
+        if len(names) == 0:
+            text = 'ANS command error.'
+            return self._respond_text(text=text)
+        records = {}
+        missed = []
+        for item in names:
+            # get record from ANS factory
+            identifier = self.ans_id(name=item)
+            if identifier is None:
+                missed.append(item)
+            else:
+                records[item] = str(identifier)
+        res = AnsCommand.response(names=names, records=records)
+        if len(missed) > 0:
+            res['missed'] = missed
+        return [res]
+
+    @classmethod
+    def ans_id(cls, name: str) -> Optional[ID]:
+        try:
+            return ID.parse(identifier=name)
+        except ValueError as e:
+            Log.warning(msg='ANS record not exists: %s, %s' % (name, e))
```

### Comparing `dimples-0.2.0/dimples/client/group.py` & `dimples-0.2.1/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/messenger.py` & `dimples-0.2.1/dimples/client/messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
     # Override
     def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # call super
         responses = super().process_reliable_message(msg=msg)
         if len(responses) == 0 and self._needs_receipt(msg=msg):
             current_user = self.facebook.current_user
-            res = ReceiptCommand.create(text='Message received', msg=msg)
+            res = ReceiptCommand.create(text='Message received.', msg=msg)
             env = Envelope.create(sender=current_user.identifier, receiver=msg.sender)
             i_msg = InstantMessage.create(head=env, body=res)
             s_msg = self.encrypt_message(msg=i_msg)
             assert s_msg is not None, 'failed to encrypt message: %s -> %s' % (current_user, msg.sender)
             r_msg = self.sign_message(msg=s_msg)
             assert r_msg is not None, 'failed to sign message: %s -> %s' % (current_user, msg.sender)
             responses = [r_msg]
```

### Comparing `dimples-0.2.0/dimples/client/network/__init__.py` & `dimples-0.2.1/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/network/session.py` & `dimples-0.2.1/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/network/state.py` & `dimples-0.2.1/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/network/transition.py` & `dimples-0.2.1/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/packer.py` & `dimples-0.2.1/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/client/processor.py` & `dimples-0.2.1/dimples/client/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,32 +27,30 @@
     Client extensions for MessageProcessor
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 
 import time
 from typing import List, Optional, Union
 
-from dimp import EntityType
-from dimp import SecureMessage, ReliableMessage
-from dimp import ContentType, Content, TextContent
-from dimp import GroupCommand
-
+from dimsdk import EntityType
+from dimsdk import SecureMessage, ReliableMessage
+from dimsdk import ContentType, Content, TextContent
+from dimsdk import GroupCommand
+from dimsdk import ReceiptCommand
 from dimsdk import ContentProcessor, ContentProcessorCreator
 from dimsdk import MessageProcessor
-
-from dimsdk.cpu import BaseContentProcessor, BaseContentProcessorCreator
+from dimsdk import BaseContentProcessor, BaseContentProcessorCreator
 
 from ..utils import Logging
-from ..common import HandshakeCommand, ReceiptCommand, LoginCommand
+from ..common import HandshakeCommand, LoginCommand
 from ..common import CommonMessenger
 
 from .cpu import TextContentProcessor
 from .cpu import HandshakeCommandProcessor
 from .cpu import LoginCommandProcessor
-from .cpu import ReceiptCommandProcessor
 from .cpu import HistoryCommandProcessor, GroupCommandProcessor
 from .cpu import InviteCommandProcessor, ExpelCommandProcessor, QuitCommandProcessor
 from .cpu import ResetCommandProcessor, QueryCommandProcessor
 
 
 class ClientMessageProcessor(MessageProcessor, Logging):
 
@@ -117,15 +115,15 @@
 
 
 class ClientContentProcessorCreator(BaseContentProcessorCreator):
 
     # Override
     def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
         # text
-        if msg_type == ContentType.TEXT:
+        if msg_type == ContentType.TEXT.value:
             return TextContentProcessor(facebook=self.facebook, messenger=self.messenger)
         # history
         if msg_type == ContentType.HISTORY.value:
             return HistoryCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # default
         if msg_type == 0:
             return BaseContentProcessor(facebook=self.facebook, messenger=self.messenger)
@@ -136,17 +134,14 @@
     def create_command_processor(self, msg_type: Union[int, ContentType], cmd: str) -> Optional[ContentProcessor]:
         # handshake
         if cmd == HandshakeCommand.HANDSHAKE:
             return HandshakeCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # login
         if cmd == LoginCommand.LOGIN:
             return LoginCommandProcessor(facebook=self.facebook, messenger=self.messenger)
-        # receipt
-        if cmd == ReceiptCommand.RECEIPT:
-            return ReceiptCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # group commands
         if cmd == 'group':
             return GroupCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         elif cmd == GroupCommand.INVITE:
             return InviteCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         elif cmd == GroupCommand.EXPEL:
             return ExpelCommandProcessor(facebook=self.facebook, messenger=self.messenger)
```

### Comparing `dimples-0.2.0/dimples/client/terminal.py` & `dimples-0.2.1/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/__init__.py` & `dimples-0.2.1/dimples/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 
 __all__ = [
     #
     #   protocol
     #
     'HandshakeCommand', 'HandshakeState',
-    'ReceiptCommand',
     'LoginCommand',
     'ReportCommand',
     'AnsCommand',
 
     #
     #   Database Interface
     #
```

### Comparing `dimples-0.2.0/dimples/common/ans.py` & `dimples-0.2.1/dimples/common/ans.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,28 +107,30 @@
             return True
 
     def fix(self, records: Dict[str, str]) -> int:
         """ remove the keywords temporary before save new records """
         count = 0
         self.__reserved['apns'] = False
         self.__reserved['master'] = False
+        self.__reserved['monitor'] = False
         self.__reserved['archivist'] = False
         self.__reserved['assistant'] = False
         # self.__reserved['station'] = False
         for alias in records:
             value = records[alias]
             if value is None or len(value) == 0:
                 continue
             identifier = ID.parse(identifier=value)
             assert identifier is not None, 'record error: %s => %s' % (alias, value)
             if self.save(name=alias, identifier=identifier):
                 count += 1
         # self.__reserved['station'] = True
         self.__reserved['assistant'] = True
         self.__reserved['archivist'] = True
+        self.__reserved['monitor'] = True
         self.__reserved['master'] = True
         self.__reserved['apns'] = True
         return count
 
 
 class ANSFactory(IDFactory):
```

### Comparing `dimples-0.2.0/dimples/common/dbi/__init__.py` & `dimples-0.2.1/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/dbi/account.py` & `dimples-0.2.1/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/dbi/message.py` & `dimples-0.2.1/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/dbi/session.py` & `dimples-0.2.1/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/facebook.py` & `dimples-0.2.1/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/messenger.py` & `dimples-0.2.1/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/packer.py` & `dimples-0.2.1/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/protocol/__init__.py` & `dimples-0.2.1/dimples/common/protocol/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,28 +25,25 @@
 
 from dimsdk import Command
 from dimsdk import CommandFactoryBuilder
 from dimsdk import register_all_factories as register_core_factories
 from dimplugins import register_plugins
 
 from .handshake import HandshakeCommand, HandshakeState
-from .receipt import ReceiptCommand
 from .login import LoginCommand
 from .report import ReportCommand
 from .ans import AnsCommand
 
 
 def register_all_factories():
     # Register core factories
     register_core_factories()
 
     # Handshake
     Command.register(cmd=HandshakeCommand.HANDSHAKE, factory=CommandFactoryBuilder(command_class=HandshakeCommand))
-    # Receipt
-    Command.register(cmd=ReceiptCommand.RECEIPT, factory=CommandFactoryBuilder(command_class=ReceiptCommand))
     # Login
     Command.register(cmd=LoginCommand.LOGIN, factory=CommandFactoryBuilder(command_class=LoginCommand))
     # Report
     Command.register(cmd=ReportCommand.REPORT, factory=CommandFactoryBuilder(command_class=ReportCommand))
     # ANS
     Command.register(cmd=AnsCommand.ANS, factory=CommandFactoryBuilder(command_class=AnsCommand))
 
@@ -54,12 +51,11 @@
 register_all_factories()
 register_plugins()
 
 
 __all__ = [
 
     'HandshakeCommand', 'HandshakeState',
-    'ReceiptCommand',
     'LoginCommand',
     'ReportCommand',
     'AnsCommand',
 ]
```

### Comparing `dimples-0.2.0/dimples/common/protocol/ans.py` & `dimples-0.2.1/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/protocol/handshake.py` & `dimples-0.2.1/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/protocol/login.py` & `dimples-0.2.1/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/protocol/report.py` & `dimples-0.2.1/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/common/session.py` & `dimples-0.2.1/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/config.py` & `dimples-0.2.1/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/__init__.py` & `dimples-0.2.1/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/gate.py` & `dimples-0.2.1/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/gatekeeper.py` & `dimples-0.2.1/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/mars.py` & `dimples-0.2.1/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/mtp.py` & `dimples-0.2.1/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/protocol/__init__.py` & `dimples-0.2.1/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/protocol/mars.py` & `dimples-0.2.1/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/protocol/ws.py` & `dimples-0.2.1/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/queue.py` & `dimples-0.2.1/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/seeker.py` & `dimples-0.2.1/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/session.py` & `dimples-0.2.1/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/conn/ws.py` & `dimples-0.2.1/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/__init__.py` & `dimples-0.2.1/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/account.py` & `dimples-0.2.1/dimples/database/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,22 @@
 
     #
     #   Document DBI
     #
 
     # Override
     def save_document(self, document: Document) -> bool:
-        # check with exists
+        # check meta first
         meta = self.__meta_table.meta(identifier=document.identifier)
         if meta is None:
             raise LookupError('meta not exists: %s' % document.identifier)
+        # check document valid before saving it
         if not (document.valid or document.verify(public_key=meta.key)):
             raise ValueError('document error: %s' % document.identifier)
+        # document ok, try to save it
         return self.__doc_table.save_document(document=document)
 
     # Override
     def document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
         return self.__doc_table.document(identifier=identifier, doc_type=doc_type)
 
     #
```

### Comparing `dimples-0.2.0/dimples/database/dos/__init__.py` & `dimples-0.2.1/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/base.py` & `dimples-0.2.1/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/document.py` & `dimples-0.2.1/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/group.py` & `dimples-0.2.1/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/login.py` & `dimples-0.2.1/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/meta.py` & `dimples-0.2.1/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/private.py` & `dimples-0.2.1/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/station.py` & `dimples-0.2.1/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/dos/user.py` & `dimples-0.2.1/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/message.py` & `dimples-0.2.1/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/session.py` & `dimples-0.2.1/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_cipherkey.py` & `dimples-0.2.1/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_document.py` & `dimples-0.2.1/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_group.py` & `dimples-0.2.1/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_login.py` & `dimples-0.2.1/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_message.py` & `dimples-0.2.1/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_meta.py` & `dimples-0.2.1/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_private.py` & `dimples-0.2.1/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_station.py` & `dimples-0.2.1/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/database/t_user.py` & `dimples-0.2.1/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/edge/__init__.py` & `dimples-0.2.1/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/edge/octopus.py` & `dimples-0.2.1/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/edge/shared.py` & `dimples-0.2.1/dimples/edge/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import getopt
 import sys
+import time
 from typing import Optional, Tuple
 
 from dimsdk import ID, Station
 
 from ..utils import Singleton
 from ..common import CommonFacebook
 from ..common import AccountDBI, MessageDBI, SessionDBI
@@ -127,15 +128,24 @@
     facebook = CommonFacebook(database=database)
     # make sure private keys exists
     sign_key = facebook.private_key_for_visa_signature(identifier=current_user)
     msg_keys = facebook.private_keys_for_decryption(identifier=current_user)
     assert sign_key is not None, 'failed to get sign key for current user: %s' % current_user
     assert msg_keys is not None and len(msg_keys) > 0, 'failed to get msg keys: %s' % current_user
     print('set current user: %s' % current_user)
-    facebook.current_user = facebook.user(identifier=current_user)
+    user = facebook.user(identifier=current_user)
+    assert user is not None, 'failed to get current user: %s' % current_user
+    visa = user.visa
+    if visa is not None:
+        # refresh visa
+        now = time.time()
+        visa.set_property(key='time', value=now)
+        visa.sign(private_key=sign_key)
+        facebook.save_document(document=visa)
+    facebook.current_user = user
     return facebook
 
 
 def create_session(facebook: CommonFacebook, database: SessionDBI, host: str, port: int) -> ClientSession:
     # 1. create station with remote host & port
     station = Station(host=host, port=port)
     station.data_source = facebook
```

### Comparing `dimples-0.2.0/dimples/edge/start.py` & `dimples-0.2.1/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/register/__init__.py` & `dimples-0.2.1/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/register/generate.py` & `dimples-0.2.1/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/register/modify.py` & `dimples-0.2.1/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/register/run.py` & `dimples-0.2.1/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/register/shared.py` & `dimples-0.2.1/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/__init__.py` & `dimples-0.2.1/dimples/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 __all__ = [
 
     #
     #   CPU
     #
     'HandshakeCommandProcessor', 'LoginCommandProcessor', 'ReportCommandProcessor',
-    'AnsCommandProcessor', 'DocumentCommandProcessor', 'ReceiptCommandProcessor',
+    'AnsCommandProcessor', 'DocumentCommandProcessor',
 
     # Session
     'ServerSession', 'SessionCenter',  # 'SessionPool',
 
     'BroadcastRecipientManager',
 
     # Push Notification
```

### Comparing `dimples-0.2.0/dimples/server/broadcast.py` & `dimples-0.2.1/dimples/server/broadcast.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/cpu/__init__.py` & `dimples-0.2.1/dimples/server/cpu/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,20 +33,18 @@
 from .handshake import HandshakeCommandProcessor
 from .login import LoginCommandProcessor
 from .report import ReportCommandProcessor
 from .ans import AnsCommandProcessor
 
 from .document import DocumentCommandProcessor
 
-from .receipt import ReceiptCommandProcessor
-
 
 __all__ = [
+
     'HandshakeCommandProcessor',
     'LoginCommandProcessor',
     'ReportCommandProcessor',
     'AnsCommandProcessor',
 
     'DocumentCommandProcessor',
 
-    'ReceiptCommandProcessor',
 ]
```

### Comparing `dimples-0.2.0/dimples/server/cpu/ans.py` & `dimples-0.2.1/dimples/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2023 Albert Moky
+# Copyright (c) 2019 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,54 +20,49 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Command Processor for 'ans'
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    Utils
+    ~~~~~
 
-    ANS protocol
+    I'm too lazy to write codes for demo project, so I borrow some utils here
+    from the <dimsdk> packages, but I don't suggest you to do it also, because
+    I won't promise these private utils will not be changed. Hia hia~ :P
+                                             -- Albert Moky @ Jan. 23, 2019
 """
 
-from typing import Optional, List
-
-from dimp import ID
-from dimp import ReliableMessage
-from dimp import Content
-
-from dimsdk.cpu import BaseCommandProcessor
-
-from ...utils import Log
-from ...common import AnsCommand
-
-
-class AnsCommandProcessor(BaseCommandProcessor):
-
-    # Override
-    def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, AnsCommand), 'report command error: %s' % content
-        names = content.names
-        if names is None or len(names) == 0:
-            text = 'ANS command error'
-            return self._respond_text(text=text)
-        records = {}
-        missed = []
-        for item in names:
-            # get record from ANS factory
-            identifier = self.ans_id(name=item)
-            if identifier is None:
-                missed.append(item)
-            else:
-                records[item] = str(identifier)
-        res = AnsCommand.response(names=names, records=records)
-        if len(missed) > 0:
-            res['missed'] = missed
-        return [res]
-
-    @classmethod
-    def ans_id(cls, name: str) -> Optional[ID]:
-        try:
-            return ID.parse(identifier=name)
-        except ValueError as e:
-            Log.warning(msg='ANS record not exists: %s, %s' % (name, e))
+from dimsdk import md5, sha1, sha256
+from dimsdk import base64_encode, base64_decode
+from dimsdk import utf8_encode, utf8_decode
+from dimsdk import hex_encode, hex_decode
+from dimsdk import json_encode, json_decode
+from dimplugins.aes import random_bytes
+
+from startrek.fsm import Runnable, Runner
+
+from .singleton import Singleton
+from .log import Log, Logging
+from .dos import Path, File, TextFile, JSONFile
+from .cache import CachePool, CacheHolder, CacheManager
+from .checker import FrequencyChecker, QueryFrequencyChecker
+
+
+__all__ = [
+
+    'md5', 'sha1', 'sha256',
+    'base64_encode', 'base64_decode',
+    'utf8_encode', 'utf8_decode',
+    'hex_encode', 'hex_decode',
+    'json_encode', 'json_decode',
+    'random_bytes',
+
+    'Runnable', 'Runner',
+
+    'Singleton',
+    'Log', 'Logging',
+    'Path', 'File', 'TextFile', 'JSONFile',
+    'CachePool', 'CacheHolder', 'CacheManager',
+    'FrequencyChecker', 'QueryFrequencyChecker',
+]
```

### Comparing `dimples-0.2.0/dimples/server/cpu/document.py` & `dimples-0.2.1/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/cpu/handshake.py` & `dimples-0.2.1/dimples/server/cpu/handshake.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,20 @@
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, HandshakeCommand), 'handshake command error: %s' % content
         title = content.title
         if title in ['DIM?', 'DIM!']:
             # S -> C
-            text = 'Handshake command error: %s' % title
-            return self._respond_text(text=text)
+            return self._respond_text(text='Command not support.', extra={
+                'template': 'Handshake command error: title="${title}".',
+                'replacements': {
+                    'title': title,
+                }
+            })
         # C -> S: Hello world!
         assert 'Hello world!' == title, 'Handshake command error: %s' % content
         # set/update session in session server with new session key
         messenger = self.messenger
         session = messenger.session
         if session.key == content.session:
             # session key match
```

### Comparing `dimples-0.2.0/dimples/server/cpu/login.py` & `dimples-0.2.1/dimples/server/cpu/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,20 @@
             # forwarded login command
             self.info(msg='user login: %s -> %s, forwarded by %s' % (sender, roaming, session.identifier))
             return []
         # 3. update session flag
         session.set_active(active=True)
         # only respond the user login to this station
         self.info(msg='user login: %s -> %s' % (sender, roaming))
-        return self._respond_text(text='Login received.')
+        return self._respond_text(text='Login received.', extra={
+            'template': 'Login command received: ${ID}.',
+            'replacements': {
+                'ID': str(sender),
+            }
+        })
 
 
 def add_roaming(user: ID, station: ID):
     """ add roaming user to dispatcher """
     from ..dispatcher import Dispatcher
     dispatcher = Dispatcher()
     dispatcher.add_roaming(user=user, station=station)
```

### Comparing `dimples-0.2.0/dimples/server/cpu/receipt.py` & `dimples-0.2.1/dimples/station/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # -*- coding: utf-8 -*-
+#
+#   DIMS : DIM Station
+#
+#                                Written in 2022 by Moky <albert.moky@gmail.com>
+#
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2019 Albert Moky
+# Copyright (c) 2022 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,30 +24,22 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-"""
-    Receipt Command Processor
-    ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 """
+    DIM Station
+    ~~~~~~~~~~~
 
-from typing import List
-
-from dimp import ReliableMessage
-from dimp import Content
-
-from dimsdk.cpu import BaseCommandProcessor
+    DIM network server node
+"""
 
-from ...common import ReceiptCommand
+from .handler import RequestHandler
 
 
-class ReceiptCommandProcessor(BaseCommandProcessor):
+__all__ = [
 
-    # Override
-    def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, ReceiptCommand), 'receipt command error: %s' % content
-        # nickname = self.facebook.name(identifier=sender)
-        return []
+    'RequestHandler',
+]
```

### Comparing `dimples-0.2.0/dimples/server/dispatcher.py` & `dimples-0.2.1/dimples/server/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 """
 
 import threading
 from abc import ABC, abstractmethod
 from typing import Optional, List
 
 from dimsdk import EntityType, ID
-from dimsdk import Content
+from dimsdk import Content, ReceiptCommand
 from dimsdk import ReliableMessage
 
 from ..utils import Singleton, Logging, Runner
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
-from ..common import LoginCommand, ReceiptCommand
+from ..common import LoginCommand
 
 from .session_center import SessionCenter
 from .push import PushCenter
 
 
 class MessageDeliver(ABC):
     """ Delegate for deliver message """
@@ -164,20 +164,20 @@
                 # failed to push message, user not online and not roamed to other station,
                 # push notification for the receiver
                 center = PushCenter()
                 center.push_notification(msg=msg)
         # OK
         if responses is None:
             # user not online, and not roaming to other station
-            text = 'Message cached'
+            text = 'Message cached.'
             res = ReceiptCommand.create(text=text, msg=msg)
             return [res]
         elif len(responses) == 0:
             # user roamed to other station, but bridge not found
-            text = 'Message received'
+            text = 'Message received.'
             res = ReceiptCommand.create(text=text, msg=msg)
             return [res]
         else:
             # message delivered
             return responses
 
     def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
@@ -292,15 +292,15 @@
         :param receiver: actual receiver
         :return: responses
         """
         assert receiver.is_user, 'receiver ID error: %s' % receiver
         assert receiver.type != EntityType.STATION, 'should not push message for station: %s' % receiver
         # 1. try to push message directly
         if session_push(msg=msg, receiver=receiver) > 0:
-            text = 'Message delivered for recipient'
+            text = 'Message delivered.'
             cmd = ReceiptCommand.create(text=text, msg=msg)
             cmd['recipient'] = str(receiver)
             return [cmd]
         # 2. get roaming station
         roaming = get_roaming_station(receiver=receiver, database=self.database)
         if roaming is None:
             # login command not found
@@ -326,15 +326,15 @@
         if neighbor == current:
             self.debug(msg='same destination: %s, msg %s => %s' % (neighbor, msg.sender, msg.receiver))
             # the user is roaming to current station, but it's not online now
             # return None to tell the push center to push notification for it.
             return None
         # 1. try to push message to neighbor station directly
         if session_push(msg=msg, receiver=neighbor) > 0:
-            text = 'Message redirected to neighbor station'
+            text = 'Message redirected.'
             cmd = ReceiptCommand.create(text=text, msg=msg)
             cmd['neighbor'] = str(neighbor)
             return [cmd]
         # 2. push message to bridge
         return bridge_message(msg=msg, neighbor=neighbor, bridge=current)
 
 
@@ -350,15 +350,15 @@
     # NOTE: the messenger will serialize this message immediately, so
     #       we don't need to clone this dictionary to avoid 'neighbor'
     #       be changed to another value before pushing to the bridge.
     # clone = msg.copy_dictionary()
     # msg = ReliableMessage.parse(msg=clone)
     msg['neighbor'] = str(neighbor)
     if session_push(msg=msg, receiver=bridge) > 0:
-        text = 'Message redirected to neighbor station via the bridge'
+        text = 'Message redirected.'
         cmd = ReceiptCommand.create(text=text, msg=msg)
         cmd['neighbor'] = str(neighbor)
         return [cmd]
     else:
         # station bridge not found
         # return an empty array to avoid calling push center
         return []
```

### Comparing `dimples-0.2.0/dimples/server/messenger.py` & `dimples-0.2.1/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/packer.py` & `dimples-0.2.1/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/processor.py` & `dimples-0.2.1/dimples/server/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,32 @@
 """
 
 import time
 from typing import List, Optional, Union
 
 from dimsdk import EntityType
 from dimsdk import ReliableMessage
-from dimsdk import Content, ContentType, TextContent, Command
+from dimsdk import Content, ContentType, Command
+from dimsdk import TextContent, ReceiptCommand
 from dimsdk import ContentProcessor, ContentProcessorCreator
 from dimsdk import MessageProcessor
 
 from dimsdk.cpu import BaseContentProcessor, BaseContentProcessorCreator
 
 from ..utils import Logging
 from ..common import HandshakeCommand, LoginCommand
-from ..common import ReceiptCommand, ReportCommand, AnsCommand
+from ..common import ReportCommand, AnsCommand
 from ..common import CommonMessenger
 
 from .cpu import HandshakeCommandProcessor
 from .cpu import LoginCommandProcessor
 from .cpu import ReportCommandProcessor
 from .cpu import AnsCommandProcessor
 
 from .cpu import DocumentCommandProcessor
-from .cpu import ReceiptCommandProcessor
 
 
 class ServerMessageProcessor(MessageProcessor, Logging):
 
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
@@ -118,17 +118,14 @@
             return DocumentCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # handshake
         if cmd == HandshakeCommand.HANDSHAKE:
             return HandshakeCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # login
         if cmd == LoginCommand.LOGIN:
             return LoginCommandProcessor(facebook=self.facebook, messenger=self.messenger)
-        # receipt
-        if cmd == ReceiptCommand.RECEIPT:
-            return ReceiptCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # report
         if cmd == ReportCommand.REPORT:
             return ReportCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # ans
         if cmd == AnsCommand.ANS:
             return AnsCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # others
```

### Comparing `dimples-0.2.0/dimples/server/push.py` & `dimples-0.2.1/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/session.py` & `dimples-0.2.1/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/session_center.py` & `dimples-0.2.1/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/server/trace.py` & `dimples-0.2.1/dimples/server/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,17 +271,18 @@
         self.__pool = LockedPool()
 
     def is_traced(self, msg: ReliableMessage, node: ID) -> bool:
         """ merge traces from msg into cached pool,
             after that, check whether this node exists
         """
         pool = self.__pool
-        pool.purge(now=msg.time)  # call when verifying new message
         cached = pool.set_traces(msg=msg)
-        return cached.search(node=node) >= 0
+        pos = cached.search(node=node)
+        pool.purge(now=msg.time)  # call when verifying new message
+        return pos >= 0
 
     def get_traces(self, msg: ReliableMessage) -> TraceList:
         """ merge traces from msg into cached pool """
         pool = self.__pool
         return pool.set_traces(msg=msg)
 
     def set_nodes(self, msg: ReliableMessage, nodes: Set[ID]):
```

### Comparing `dimples-0.2.0/dimples/station/handler.py` & `dimples-0.2.1/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/station/shared.py` & `dimples-0.2.1/dimples/station/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import getopt
 import sys
+import time
 from typing import Optional, Tuple
 
 from dimsdk import ID
 
 from ..utils import Singleton
 from ..common import AddressNameServer, ANSFactory, CommonFacebook
 from ..common import AccountDBI, MessageDBI, SessionDBI
@@ -127,15 +128,24 @@
     facebook = CommonFacebook(database=database)
     # make sure private keys exists
     sign_key = facebook.private_key_for_visa_signature(identifier=current_user)
     msg_keys = facebook.private_keys_for_decryption(identifier=current_user)
     assert sign_key is not None, 'failed to get sign key for current user: %s' % current_user
     assert msg_keys is not None and len(msg_keys) > 0, 'failed to get msg keys: %s' % current_user
     print('set current user: %s' % current_user)
-    facebook.current_user = facebook.user(identifier=current_user)
+    user = facebook.user(identifier=current_user)
+    assert user is not None, 'failed to get current user: %s' % current_user
+    visa = user.visa
+    if visa is not None:
+        # refresh visa
+        now = time.time()
+        visa.set_property(key='time', value=now)
+        visa.sign(private_key=sign_key)
+        facebook.save_document(document=visa)
+    facebook.current_user = user
     return facebook
 
 
 def create_dispatcher(shared: GlobalVariable) -> Dispatcher:
     """ Step 4: create dispatcher """
     dispatcher = Dispatcher()
     dispatcher.mdb = shared.mdb
```

### Comparing `dimples-0.2.0/dimples/station/start.py` & `dimples-0.2.1/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/utils/cache.py` & `dimples-0.2.1/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/utils/checker.py` & `dimples-0.2.1/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/utils/dos.py` & `dimples-0.2.1/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/utils/log.py` & `dimples-0.2.1/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples/utils/singleton.py` & `dimples-0.2.1/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.0/dimples.egg-info/PKG-INFO` & `dimples-0.2.1/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.0
+Version: 0.2.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.0/dimples.egg-info/SOURCES.txt` & `dimples-0.2.1/dimples.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 dimples/client/cpu/grp_invite.py
 dimples/client/cpu/grp_query.py
 dimples/client/cpu/grp_quit.py
 dimples/client/cpu/grp_reset.py
 dimples/client/cpu/handshake.py
 dimples/client/cpu/history.py
 dimples/client/cpu/login.py
-dimples/client/cpu/receipt.py
 dimples/client/cpu/text.py
 dimples/client/network/__init__.py
 dimples/client/network/session.py
 dimples/client/network/state.py
 dimples/client/network/transition.py
 dimples/common/__init__.py
 dimples/common/ans.py
@@ -39,15 +38,14 @@
 dimples/common/dbi/account.py
 dimples/common/dbi/message.py
 dimples/common/dbi/session.py
 dimples/common/protocol/__init__.py
 dimples/common/protocol/ans.py
 dimples/common/protocol/handshake.py
 dimples/common/protocol/login.py
-dimples/common/protocol/receipt.py
 dimples/common/protocol/report.py
 dimples/conn/__init__.py
 dimples/conn/gate.py
 dimples/conn/gatekeeper.py
 dimples/conn/mars.py
 dimples/conn/mtp.py
 dimples/conn/queue.py
@@ -99,15 +97,14 @@
 dimples/server/session_center.py
 dimples/server/trace.py
 dimples/server/cpu/__init__.py
 dimples/server/cpu/ans.py
 dimples/server/cpu/document.py
 dimples/server/cpu/handshake.py
 dimples/server/cpu/login.py
-dimples/server/cpu/receipt.py
 dimples/server/cpu/report.py
 dimples/station/__init__.py
 dimples/station/handler.py
 dimples/station/shared.py
 dimples/station/start.py
 dimples/utils/__init__.py
 dimples/utils/cache.py
```

### Comparing `dimples-0.2.0/setup.py` & `dimples-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -49,16 +49,16 @@
     },
     install_requires=[
         # 'pycryptodome',  # 3.14.1
         # 'base58',  # 1.0.3
         # 'ecdsa',   # 0.16.1
         'dimplugins>=0.1.4',
 
-        'dimsdk>=0.8.5',
-        'dimp>=0.12.8',
+        'dimsdk>=0.8.6',
+        'dimp>=0.12.9',
         'dkd>=0.12.7',
         'mkm>=0.12.7',
 
         'startrek>=0.4.1',
         'tcp>=0.4.1',
         'udp>=0.5.10',
     ]
```

