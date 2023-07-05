# Comparing `tmp/MeUtils-2023.7.3.8.8.54.tar.gz` & `tmp/MeUtils-2023.7.5.18.44.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.7.3.8.8.54.tar", last modified: Mon Jul  3 00:08:54 2023, max compression
+gzip compressed data, was "MeUtils-2023.7.5.18.44.14.tar", last modified: Wed Jul  5 10:44:15 2023, max compression
```

## Comparing `MeUtils-2023.7.3.8.8.54.tar` & `MeUtils-2023.7.5.18.44.14.tar`

### file list

```diff
@@ -1,539 +1,548 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.706780 MeUtils-2023.7.3.8.8.54/
--rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.7.3.8.8.54/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.632087 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    18220 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1039 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-03 00:08:54.706604 MeUtils-2023.7.3.8.8.54/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.7.3.8.8.54/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      105 2023-06-12 01:19:08.000000 MeUtils-2023.7.3.8.8.54/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.7.3.8.8.54/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.634622 MeUtils-2023.7.3.8.8.54/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.7.3.8.8.54/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.634878 MeUtils-2023.7.3.8.8.54/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_audio/asr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.635116 MeUtils-2023.7.3.8.8.54/meutils/ai_cv/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_cv/ocr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.636079 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.636445 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-06-05 05:29:27.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.638013 MeUtils-2023.7.3.8.8.54/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.638255 MeUtils-2023.7.3.8.8.54/meutils/ann/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.638378 MeUtils-2023.7.3.8.8.54/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6025 2023-07-01 05:18:51.000000 MeUtils-2023.7.3.8.8.54/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.639466 MeUtils-2023.7.3.8.8.54/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.640069 MeUtils-2023.7.3.8.8.54/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.640311 MeUtils-2023.7.3.8.8.54/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    10268 2023-07-03 00:08:33.000000 MeUtils-2023.7.3.8.8.54/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.640551 MeUtils-2023.7.3.8.8.54/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.648746 MeUtils-2023.7.3.8.8.54/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.7.3.8.8.54/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-07-03 00:08:54.000000 MeUtils-2023.7.3.8.8.54/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.649261 MeUtils-2023.7.3.8.8.54/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.7.3.8.8.54/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.650712 MeUtils-2023.7.3.8.8.54/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     7041 2023-06-28 06:27:16.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.7.3.8.8.54/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.7.3.8.8.54/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.651376 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.651621 MeUtils-2023.7.3.8.8.54/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.7.3.8.8.54/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.652210 MeUtils-2023.7.3.8.8.54/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.7.3.8.8.54/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.7.3.8.8.54/meutils/fileparser/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.7.3.8.8.54/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.7.3.8.8.54/meutils/fileparser/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.7.3.8.8.54/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.7.3.8.8.54/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.652560 MeUtils-2023.7.3.8.8.54/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.7.3.8.8.54/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1303 2023-06-04 08:38:47.000000 MeUtils-2023.7.3.8.8.54/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-05-05 10:52:25.000000 MeUtils-2023.7.3.8.8.54/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.653169 MeUtils-2023.7.3.8.8.54/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.7.3.8.8.54/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.7.3.8.8.54/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.7.3.8.8.54/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.7.3.8.8.54/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.654132 MeUtils-2023.7.3.8.8.54/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.7.3.8.8.54/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.654885 MeUtils-2023.7.3.8.8.54/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.655380 MeUtils-2023.7.3.8.8.54/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.656101 MeUtils-2023.7.3.8.8.54/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/other/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.7.3.8.8.54/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.656644 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.658900 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.664043 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.664561 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.665847 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.666556 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.666962 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.668066 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.668694 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.669359 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.669996 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.670743 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.671675 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.672595 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.673289 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.673910 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.674633 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.675275 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.675953 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.680849 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.681407 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.682261 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.682531 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.682845 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.683135 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.683424 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.683617 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.683772 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.684935 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.685459 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.685671 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.7.3.8.8.54/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.686054 MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.7.3.8.8.54/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8434 2023-06-05 05:29:27.000000 MeUtils-2023.7.3.8.8.54/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.687074 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/plot_utils/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.687847 MeUtils-2023.7.3.8.8.54/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.688229 MeUtils-2023.7.3.8.8.54/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.688479 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.688730 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2110 2023-05-31 05:48:53.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.689085 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/errors/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/errors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/errors/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/errors/validation_error.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.689581 MeUtils-2023.7.3.8.8.54/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.689705 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.690444 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/flow.svg
--rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.690695 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/executors/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.690957 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.691858 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.692426 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.692684 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.693083 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_1_分词.py
--rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_3_文本匹配.py
--rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.7.3.8.8.54/meutils/serving/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.693212 MeUtils-2023.7.3.8.8.54/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.693753 MeUtils-2023.7.3.8.8.54/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.694283 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.7.3.8.8.54/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.696615 MeUtils-2023.7.3.8.8.54/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.697716 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.697871 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.700433 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.700593 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.703285 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.703441 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.703916 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.704423 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.704872 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.7.3.8.8.54/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.705755 MeUtils-2023.7.3.8.8.54/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/typings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.7.3.8.8.54/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      351 2023-06-28 06:59:00.000000 MeUtils-2023.7.3.8.8.54/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.7.3.8.8.54/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.7.3.8.8.54/requirements_fileparser.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-03 00:08:54.706357 MeUtils-2023.7.3.8.8.54/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-07-03 00:08:54.706831 MeUtils-2023.7.3.8.8.54/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.7.3.8.8.54/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.493704 MeUtils-2023.7.5.18.44.14/
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.7.5.18.44.14/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.395385 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    18529 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1039 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-07-05 10:44:15.000000 MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-07-05 10:44:15.493536 MeUtils-2023.7.5.18.44.14/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.7.5.18.44.14/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      105 2023-06-12 01:19:08.000000 MeUtils-2023.7.5.18.44.14/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.7.5.18.44.14/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.399106 MeUtils-2023.7.5.18.44.14/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.7.5.18.44.14/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.399477 MeUtils-2023.7.5.18.44.14/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_audio/asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.399949 MeUtils-2023.7.5.18.44.14/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_cv/ocr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.402353 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.403017 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-06-05 05:29:27.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/sentence_transformers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.405738 MeUtils-2023.7.5.18.44.14/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.406136 MeUtils-2023.7.5.18.44.14/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.406301 MeUtils-2023.7.5.18.44.14/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6114 2023-07-05 10:33:35.000000 MeUtils-2023.7.5.18.44.14/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.407616 MeUtils-2023.7.5.18.44.14/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.408352 MeUtils-2023.7.5.18.44.14/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.408637 MeUtils-2023.7.5.18.44.14/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10300 2023-07-05 08:01:27.000000 MeUtils-2023.7.5.18.44.14/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.408923 MeUtils-2023.7.5.18.44.14/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.416290 MeUtils-2023.7.5.18.44.14/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.7.5.18.44.14/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-07-05 10:44:14.000000 MeUtils-2023.7.5.18.44.14/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.421556 MeUtils-2023.7.5.18.44.14/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.7.5.18.44.14/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.423470 MeUtils-2023.7.5.18.44.14/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7099 2023-07-03 09:51:08.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.7.5.18.44.14/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.7.5.18.44.14/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.425206 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.425566 MeUtils-2023.7.5.18.44.14/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.7.5.18.44.14/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.426629 MeUtils-2023.7.5.18.44.14/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.7.5.18.44.14/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.7.5.18.44.14/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.7.5.18.44.14/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.7.5.18.44.14/meutils/fileparser/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.7.5.18.44.14/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.7.5.18.44.14/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.427140 MeUtils-2023.7.5.18.44.14/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.7.5.18.44.14/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1303 2023-06-04 08:38:47.000000 MeUtils-2023.7.5.18.44.14/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-05-05 10:52:25.000000 MeUtils-2023.7.5.18.44.14/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.428184 MeUtils-2023.7.5.18.44.14/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.7.5.18.44.14/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.7.5.18.44.14/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.7.5.18.44.14/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.7.5.18.44.14/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.429516 MeUtils-2023.7.5.18.44.14/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.7.5.18.44.14/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.430621 MeUtils-2023.7.5.18.44.14/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.431546 MeUtils-2023.7.5.18.44.14/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.432768 MeUtils-2023.7.5.18.44.14/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.7.5.18.44.14/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.436028 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.7.5.18.44.14/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.7.5.18.44.14/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.436518 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.439338 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.443456 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.443723 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.444988 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.445409 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.445656 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.446605 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.447452 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.448328 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.449169 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.449851 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.450719 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.451869 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.452691 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.453391 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.454242 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.455249 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.456393 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.459803 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.460432 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.461164 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.461399 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.461676 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.461931 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.462196 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.462347 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.462499 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.463189 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.463646 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.463797 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.7.5.18.44.14/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.464309 MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.7.5.18.44.14/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8435 2023-07-04 01:07:58.000000 MeUtils-2023.7.5.18.44.14/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.465963 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/plot_utils/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.467076 MeUtils-2023.7.5.18.44.14/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.467671 MeUtils-2023.7.5.18.44.14/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.468172 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.468706 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-07-03 09:53:08.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.469298 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/errors/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/errors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/errors/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/errors/validation_error.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.470316 MeUtils-2023.7.5.18.44.14/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.470579 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.471748 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.472272 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/executors/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.472841 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.473933 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.474904 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.475365 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.475924 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.7.5.18.44.14/meutils/serving/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.476163 MeUtils-2023.7.5.18.44.14/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.476952 MeUtils-2023.7.5.18.44.14/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.477644 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.7.5.18.44.14/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.480413 MeUtils-2023.7.5.18.44.14/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.481783 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.481976 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.486074 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.486274 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.488611 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.488863 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.489213 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.489596 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.490482 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.7.5.18.44.14/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.492483 MeUtils-2023.7.5.18.44.14/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/typings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.7.5.18.44.14/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2023-06-28 06:59:00.000000 MeUtils-2023.7.5.18.44.14/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.7.5.18.44.14/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.7.5.18.44.14/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-05 10:44:15.493251 MeUtils-2023.7.5.18.44.14/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-07-05 10:44:15.493755 MeUtils-2023.7.5.18.44.14/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.7.5.18.44.14/setup.py
```

### Comparing `MeUtils-2023.7.3.8.8.54/.gitignore` & `MeUtils-2023.7.5.18.44.14/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/LICENSE` & `MeUtils-2023.7.5.18.44.14/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.3.8.8.54
+Version: 2023.7.5.18.44.14
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 meutils/ai_cv/ocr.py
 meutils/ai_nlp/SplitSentence.py
 meutils/ai_nlp/Untitled-1(1).py
 meutils/ai_nlp/__init__.py
 meutils/ai_nlp/_lda.py
 meutils/ai_nlp/lda.py
 meutils/ai_nlp/ner.py
+meutils/ai_nlp/sentence_transformers.py
 meutils/ai_nlp/textsplitter.py
 meutils/ai_nlp/word_segmentation.py
 meutils/ai_nlp/_textsplitter/__init__.py
 meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
 meutils/ai_nlp/_textsplitter/text_split.py
 meutils/ann/README.md
 meutils/ann/README_gensim.md
@@ -144,17 +145,24 @@
 meutils/office_automation/__init__.py
 meutils/office_automation/doc.py
 meutils/office_automation/pdf.py
 meutils/office_automation/pdm.py
 meutils/office_automation/pdm_run.py
 meutils/office_automation/投资管理系统O3.2_交易组.pdm
 meutils/office_automation/report/__init__.py
+meutils/other/__demo.py
 meutils/other/__init__.py
 meutils/other/besttable.py
 meutils/other/crontab.py
+meutils/other/aiomultiprocess/__init__.py
+meutils/other/aiomultiprocess/__version__.py
+meutils/other/aiomultiprocess/core.py
+meutils/other/aiomultiprocess/pool.py
+meutils/other/aiomultiprocess/scheduler.py
+meutils/other/aiomultiprocess/types.py
 meutils/other/docarray/__init__.py
 meutils/other/docarray/base.py
 meutils/other/docarray/helper.py
 meutils/other/docarray/array/__init__.py
 meutils/other/docarray/array/annlite.py
 meutils/other/docarray/array/base.py
 meutils/other/docarray/array/chunk.py
```

### Comparing `MeUtils-2023.7.3.8.8.54/MeUtils.egg-info/requires.txt` & `MeUtils-2023.7.5.18.44.14/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -23,47 +23,47 @@
 schedule
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-schedule
-pandas-profiling[notebook]
-seaborn
-pymongo
-jmespath
+jieba
 pymupd
-filetype
-geopy
-faiss-cpu
+pretty_errors
 pyarrow
-reportlab
-thriftpy2
-pandas_summary
-jinja2
-asyncmy
-polars
-iteration_utilities
-pymysql
+sqlalchemy
 fastapi[all]
-pretty_errors
-redis-py-cluster
-missingno
+iteration_utilities
+thefuck
+pymongo
+polars
 cachetools
 pymilvus
-faiss-gpu
+geopy
 simplejson
-thefuck
+jmespath
+jinja2
 gensim
+thriftpy2
+seaborn
+reportlab
+faiss-gpu
+missingno
+schedule
+pandas-profiling[notebook]
+pandas_summary
+faiss-cpu
+filetype
+streamlit
+redis-py-cluster
 dataframe_image
-jieba
+pymysql
+asyncmy
 uvicorn
-sqlalchemy
-streamlit
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2023.7.3.8.8.54/PKG-INFO` & `MeUtils-2023.7.5.18.44.14/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.3.8.8.54
+Version: 2023.7.5.18.44.14
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.3.8.8.54/README.md` & `MeUtils-2023.7.5.18.44.14/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/clear_git_history.sh` & `MeUtils-2023.7.5.18.44.14/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_audio/asr.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_lda.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/lda.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/ner.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/textsplitter.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2023.7.5.18.44.14/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/README.md` & `MeUtils-2023.7.5.18.44.14/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/README_gensim.md` & `MeUtils-2023.7.5.18.44.14/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann_faiss.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann_gensim.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann_inmemory.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann_service.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/ann_v1.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/cli.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/examples/client.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/ann/shake_demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/cache_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/cache_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,26 @@
 import joblib
 
 from typing import Iterable
 from functools import lru_cache
 from pathlib import Path
 from joblib import Memory
 from loguru import logger
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 from tqdm.auto import tqdm
 from cachetools import cached, cachedmethod, LRUCache, RRCache, TTLCache as _TTLCache, keys
 
 # ME
-from meutils.decorators import decorator, singleton
+from meutils.decorators import decorator, singleton, background_task
 from meutils.hash_utils import md5
 
 TTLCache = lru_cache()(_TTLCache)
 
 
-def _pickle(obj, file):
-    with open(file) as f:
-        pickle.dump(obj, f)
-
-
 def map_cache():
     return cached({})
 
 
 def ttl_cache(ttl=60, maxsize=1024, key=keys.hashkey):
     """https://cachetools.readthedocs.io/en/stable/
 
@@ -102,32 +98,37 @@
 
         df = func(*args, **kwargs)
         df.to_sql(k, conn, if_exists='replace', index=False)
         return df
 
 
 @decorator
-def disk_cache(func, location='cachedir', maxsize=128, ttl=np.inf, *args, **kwargs):
+def disk_cache(func, location='cachedir', maxsize=128, ttl=np.inf, verbose=True, *args, **kwargs):
     ttl_cache = _TTLCache(maxsize, ttl)  # 单例
 
     k = md5(f"cache_{func.__name__}_{args}_{kwargs}")  # uuid
     output = Path(location) / Path(k) / '__output.pkl'
 
     if (ttl == np.inf or k in ttl_cache) and output.is_file():  # ttl=np.inf 不作key判断, 相当于maxsize无穷大
         # return joblib.load(output)
         return pickle.load(open(output, 'rb'))
 
     else:
         ttl_cache[k] = 0  # 更新cache
 
-        logger.info(f"CacheKey: {k}")
-        output.parent.mkdir(parents=True, exist_ok=True)
         _ = func(*args, **kwargs)
-        # joblib.dump(_, output)
-        pickle.dump(_, open(output, 'wb'))
+
+        @background_task
+        def dump():
+            if verbose:
+                logger.info(f"CacheKey: {k}")
+            output.parent.mkdir(parents=True, exist_ok=True)
+            pickle.dump(_, open(output, 'wb'))
+
+        dump()
         return _
 
 
 def mecache(location='mecache', maxsize=128, ttl=np.inf):
     ttl_cache = TTLCache(maxsize, ttl)
 
     @wrapt.decorator
@@ -193,16 +194,14 @@
                 batch = tqdm(batch, desc='miss')
             return list(map(wrap, batch))  # 递归
         return func(batch)  # 需支持单条输入
 
     return wrap(args[0])
 
 
-
-
 if __name__ == '__main__':
     from meutils.pipe import *
 
 
     @timer()
     @pickle_cache(location='demo')
     def func(x):
```

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/cli.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/conf.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/cron.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/monitor.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/clis/nesc.py` & `MeUtils-2023.7.5.18.44.14/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/cmds/README.md` & `MeUtils-2023.7.5.18.44.14/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.7.5.18.44.14/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/coding/find132.py` & `MeUtils-2023.7.5.18.44.14/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/common.py` & `MeUtils-2023.7.5.18.44.14/meutils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     typing.Literal = Literal
 
 from typing import *
 from pathlib import Path
 from pprint import pprint
 from abc import abstractmethod
 from dataclasses import dataclass
-from functools import reduce, lru_cache, partial
+from functools import reduce, lru_cache, cached_property, partial
 from collections import Counter, OrderedDict
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 import matplotlib.pyplot as plt
 from matplotlib.font_manager import FontProperties
 
 plt.rcParams['axes.unicode_minus'] = False
@@ -72,15 +72,15 @@
 # logger.remove()
 # logger.add(sys.stderr,
 #            format='<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <4}</level> - <level>{message}</level>')
 
 from dotenv import load_dotenv
 
 load_dotenv(
-    os.getenv('EVN', "/Users/betterme/PycharmProjects/AI/.env"),  # # EVN=传入绝对路径 todo: 自定义 .env.secret
+    os.getenv('EVN', "/Users/betterme/PycharmProjects/AI/.env"),  # EVN=传入绝对路径 todo: 自定义 .env.secret
     verbose=True
 )
 
 from tqdm.auto import tqdm
 
 tqdm.pandas()
 
@@ -97,15 +97,15 @@
 from meutils.other.crontab import CronTab
 from meutils.other.besttable import Besttable
 
 # ME
 from meutils._utils import *
 from meutils.init.evn import *
 from meutils.init.oo import O000OO0O0000OO00O
-from meutils.decorators import decorator, args, singleton, timer, background
+from meutils.decorators import decorator, args, singleton, timer, background, background_task
 from meutils.hash_utils import murmurhash
 from meutils.path_utils import get_module_path, get_resolve_path, sys_path_append, path2list, get_config
 from meutils.cache_utils import ttl_cache, disk_cache
 
 O000OO0O0000OO00O()
 
 try:
```

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.7.5.18.44.14/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/data/SimHei.ttf` & `MeUtils-2023.7.5.18.44.14/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/data/coordinate.py` & `MeUtils-2023.7.5.18.44.14/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/date_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/db/README.md` & `MeUtils-2023.7.5.18.44.14/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/db/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/db/mongo.py` & `MeUtils-2023.7.5.18.44.14/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/db/neo4j.py` & `MeUtils-2023.7.5.18.44.14/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/__ai.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/catch.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/common.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from contextlib import contextmanager
 
 # ME
 from meutils.decorators.decorator import decorator
 
 
 @decorator
-def clear_cuda_cache(func, device='cuda', bins=1, *args, **kwargs):
+def clear_cuda_cache(func, device='cuda', bins=1, *args, **kwargs):  # todo: 后端运行
     """
 
     :param device:
     :param bins: 每次都清，bins=2表示每隔一秒（每两秒）一清
     :param args:
     :param kwargs:
     :return:
@@ -150,15 +150,15 @@
 @decorator
 def timeout(func, seconds=1, *args, **kwargs):
     future = ThreadPoolExecutor(1).submit(func, *args, **kwargs)
     return future.result(timeout=seconds)
 
 
 @decorator
-def background(func, max_workers=3, *args, **kwargs):
+def background_task(func, max_workers=3, *args, **kwargs):
     """通过全局变量回收结果
         @backend
         def func(x):
             import time
             print(time.time())
             time.sleep(3)
             print(time.time())
@@ -194,14 +194,17 @@
     # pool.shutdown(wait=False)  # 不等待
     # pool.shutdown(wait=True)  # 等待
     pool = ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='🐶')
     future = pool.submit(func, *args, **kwargs)  # pool.map(fun4, ips)
     return future.running()  # future.done()
 
 
+background = background_task
+
+
 # @backend
 @decorator
 def scheduler(func, scheduler_=schedule.every(2).seconds, stop_func=lambda: False, *args, **kwargs):
     """设置调度的参数，这里是每2秒执行一次
 
         t = time.time() + 10
         def f():
```

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/decorator.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/decorator_demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/feishu.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/retry.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/decorators/scheduler.py` & `MeUtils-2023.7.5.18.44.14/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/dist_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.7.5.18.44.14/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/easy_search/es.py` & `MeUtils-2023.7.5.18.44.14/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/fileparser/PDF抽取.py` & `MeUtils-2023.7.5.18.44.14/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/hash_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/import_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/init/evn.py` & `MeUtils-2023.7.5.18.44.14/meutils/init/evn.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/init/oo.py` & `MeUtils-2023.7.5.18.44.14/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/io/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/io/image.py` & `MeUtils-2023.7.5.18.44.14/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/io/tf_io.py` & `MeUtils-2023.7.5.18.44.14/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/jinja_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/log_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/emails.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/feishu.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/file_post.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/wechat.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/wechat_.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/wecom.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/notice/weekmeet.py` & `MeUtils-2023.7.5.18.44.14/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/np_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdf.py` & `MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdm.py` & `MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/office_automation/pdm_run.py` & `MeUtils-2023.7.5.18.44.14/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.7.5.18.44.14/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/besttable.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/crontab.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/annlite.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/base.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/chunk.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/document.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/elastic.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/match.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/memory.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/milvus.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/content.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/dataloader/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/dataloader/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/delitem.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/embed.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/empty.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/evaluation.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/getattr.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/getitem.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/group.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/binary.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/common.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/csv.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/dataframe.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/from_gen.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/json.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/pbar.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/io/pushpull.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/match.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/parallel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/plot.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/post.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/pydantic.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/reduce.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/sample.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/setitem.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/strawberry.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/text.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/mixins/traverse.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/opensearch.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/qdrant.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/lookup.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/queryset/parser.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/redis.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/sqlite.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/annlite/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/base/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/elastic/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/memory/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/milvus/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/opensearch/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/qdrant/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/redis/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/sqlite/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/backend.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/find.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/storage/weaviate/seqlike.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/array/weaviate.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/base.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/enums.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/getter.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/setter.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/dataclasses/types.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/data.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/generators.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/_property.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/attribute.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/audio.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/blob.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/content.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/convert.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/dump.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/featurehash.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/image.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/mesh.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/multimodal.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/plot.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/porting.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/property.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/protobuf.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/pydantic.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/rich_embedding.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/strawberry.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/sugar.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/text.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/mixins/video.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/pydantic_model.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/document/strawberry_type.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/numpy.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/paddle.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/tensorflow.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/distance/torch.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/evaluation.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/helper.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/math/ndarray.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/io/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/io/ndarray.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb/docarray_pb2.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/proto/pb2/docarray_pb2.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/ci-vendors.json` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/resources/embedding-projector/index.html.gz` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/data.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/score/mixins/property.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/other/docarray/typing/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/opt.py` & `MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/path_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/pd_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/pipe.py` & `MeUtils-2023.7.5.18.44.14/meutils/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
 
     """
     loop = asyncio.get_event_loop()
     _ = asyncio.gather(*tasks, return_exceptions=return_exceptions)  # asyncio.wait(tasks)
     return loop.run_until_complete(_)
 
 
+
 if __name__ == '__main__':
     @Pipe
     def xfunc1(x):
         _ = x.split()
         print(_)
         return _
```

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/echarts.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/embedding_plot.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/mecharts.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/metrics.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/plot_utils/plot_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/plot_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/request_utils/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/request_utils/crawler.py` & `MeUtils-2023.7.5.18.44.14/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/request_utils/download.py` & `MeUtils-2023.7.5.18.44.14/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/request_utils/results.py` & `MeUtils-2023.7.5.18.44.14/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/request_utils/公网ip.py` & `MeUtils-2023.7.5.18.44.14/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/_fastapi.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/common.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 
     @router.get('/', name='xxxx')
     def f():
         return {'1': '2'}
 
 
     app.include_router(router)
-    app.run()
+    app.run(port=8899)
```

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/fastapi/errors/validation_error.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/fastapi/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/gui/bar.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/gui/demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/client.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/flow.svg` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/flow.svg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/__demo/server.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/__demo/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/executors/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/_test.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/st_utils/common.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/st_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/webui/.streamlit/_config.toml` & `MeUtils-2023.7.5.18.44.14/meutils/serving/webui/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_1_分词.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_1_分词.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_2_词性标注与实体识别.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/serving/webui/pages/_3_文本匹配.py` & `MeUtils-2023.7.5.18.44.14/meutils/serving/webui/pages/_3_文本匹配.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/sftp.py` & `MeUtils-2023.7.5.18.44.14/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/sk_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/smooth_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/spark/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/Translator.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/__init__.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/json_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/str_utils/regular_expression.py` & `MeUtils-2023.7.5.18.44.14/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/demo.j2` & `MeUtils-2023.7.5.18.44.14/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/demo.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/demox.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/df_html.j2` & `MeUtils-2023.7.5.18.44.14/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/hegui.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/markmap.html` & `MeUtils-2023.7.5.18.44.14/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.7.5.18.44.14/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/tpl.docx` & `MeUtils-2023.7.5.18.44.14/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/x.html` & `MeUtils-2023.7.5.18.44.14/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/templates/合规日报模板.docx` & `MeUtils-2023.7.5.18.44.14/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/todo.py` & `MeUtils-2023.7.5.18.44.14/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/tools/cprint.py` & `MeUtils-2023.7.5.18.44.14/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/tools/machine_monitor.py` & `MeUtils-2023.7.5.18.44.14/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/tools/monitor.yml` & `MeUtils-2023.7.5.18.44.14/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/tools/seize.py` & `MeUtils-2023.7.5.18.44.14/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/tools/service_monitor.py` & `MeUtils-2023.7.5.18.44.14/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/meutils/zk_utils.py` & `MeUtils-2023.7.5.18.44.14/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/pypi.sh` & `MeUtils-2023.7.5.18.44.14/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.3.8.8.54/setup.py` & `MeUtils-2023.7.5.18.44.14/setup.py`

 * *Files identical despite different names*

