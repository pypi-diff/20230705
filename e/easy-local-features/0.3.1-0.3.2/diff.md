# Comparing `tmp/easy_local_features-0.3.1.tar.gz` & `tmp/easy_local_features-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.3.1.tar", last modified: Tue Jul  4 22:59:08 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.2.tar", last modified: Wed Jul  5 12:51:57 2023, max compression
```

## Comparing `easy_local_features-0.3.1.tar` & `easy_local_features-0.3.2.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.584116 easy_local_features-0.3.1/
--rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.1/LICENSE_DISK.txt
--rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.1/LICENSE_R2D2.txt
--rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.1/LICENSE_SUPERGLUE.txt
--rw-r--r--   0 cadar      (501) staff       (20)     1947 2023-07-04 22:59:08.583968 easy_local_features-0.3.1/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     1695 2023-07-04 22:58:44.000000 easy_local_features-0.3.1/README.md
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.574657 easy_local_features-0.3.1/easy_local_features/
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.1/easy_local_features/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.575700 easy_local_features-0.3.1/easy_local_features/datasets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/datasets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/datasets/download.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.576606 easy_local_features-0.3.1/easy_local_features/features/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:09:54.000000 easy_local_features-0.3.1/easy_local_features/features/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)    34250 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-01 09:14:35.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-01 15:51:12.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-01 17:02:37.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-01 16:59:28.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_superpoint.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577113 easy_local_features-0.3.1/easy_local_features/matching/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.1/easy_local_features/matching/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2103 2023-07-04 22:47:59.000000 easy_local_features-0.3.1/easy_local_features/matching/baseline_loftr.py
--rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.1/easy_local_features/matching/baseline_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.1/easy_local_features/matching/core.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577219 easy_local_features-0.3.1/easy_local_features/submodules/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.1/easy_local_features/submodules/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577378 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577503 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/
--rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577780 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2675 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/structs.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.578327 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/
--rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      271 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
--rw-r--r--   0 cadar      (501) staff       (20)     2253 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/epi.py
--rw-r--r--   0 cadar      (501) staff       (20)     3377 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/pose.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.579177 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/
--rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2744 2023-07-01 15:52:24.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     2544 2023-07-01 15:34:26.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     5573 2023-07-01 15:33:05.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/detector.py
--rw-r--r--   0 cadar      (501) staff       (20)     2265 2023-07-01 15:52:15.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      881 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/nms.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.579986 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract.py
--rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract_kapture.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.581075 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/losses.py
--rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/patchnet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/sampler.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582006 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/common.py
--rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/dataloader.py
--rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/trainer.py
--rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms.py
--rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
--rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/viz.py
--rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/train.py
--rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582197 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582815 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/matching.py
--rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superpoint.py
--rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.575347 easy_local_features-0.3.1/easy_local_features.egg-info/
--rw-r--r--   0 cadar      (501) staff       (20)     1947 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     3314 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/SOURCES.txt
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/dependency_links.txt
--rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/top_level.txt
--rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-04 22:59:08.584161 easy_local_features-0.3.1/setup.cfg
--rw-r--r--   0 cadar      (501) staff       (20)      760 2023-07-04 22:57:43.000000 easy_local_features-0.3.1/setup.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.583752 easy_local_features-0.3.1/tests/
--rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:20.000000 easy_local_features-0.3.1/tests/test_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:19.000000 easy_local_features-0.3.1/tests/test_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:19.000000 easy_local_features-0.3.1/tests/test_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:18.000000 easy_local_features-0.3.1/tests/test_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)      170 2023-07-04 22:12:18.000000 easy_local_features-0.3.1/tests/test_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)      173 2023-07-04 22:12:16.000000 easy_local_features-0.3.1/tests/test_superpoint.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    32722 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_DISK.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    21121 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_R2D2.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7009 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/LICENSE_SUPERGLUE.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1942 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1690 2023-07-05 12:20:10.000000 easy_local_features-0.3.2/README.md
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/__init__.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features/datasets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/datasets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/datasets/download.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/feature/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2624 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_deal.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6746 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_disk.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6012 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_r2d2.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2857 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/feature/baseline_superpoint.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/matching/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2103 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/baseline_loftr.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5116 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/baseline_superglue.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/matching/core.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/__init__.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/__init__.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       24 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2652 2023-07-05 12:00:59.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.802528 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       79 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      291 2023-07-05 12:01:08.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2096 2023-07-05 12:01:56.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3406 2023-07-05 12:02:13.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      113 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2732 2023-07-05 12:02:43.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2566 2023-07-05 12:03:01.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5454 2023-07-05 12:04:18.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2177 2023-07-05 12:05:58.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      865 2023-07-05 12:04:30.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      249 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4159 2023-07-05 11:59:54.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/blocks.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2070 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/ops.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3289 2023-07-05 12:00:26.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/unet.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1291 2023-07-05 10:39:12.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/unets/utils.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6223 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     9927 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.806527 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2360 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1720 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7158 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1760 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2006 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    15031 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1080 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    14318 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2208 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    18298 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     7160 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5647 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     5018 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/train.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4203 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/__init__.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3417 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    11537 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     8092 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    20039 2023-07-05 10:01:47.000000 easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/utils.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/easy_local_features/utils/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 10:28:06.000000 easy_local_features-0.3.2/easy_local_features/utils/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      293 2023-07-05 10:29:53.000000 easy_local_features-0.3.2/easy_local_features/utils/generic_match.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-07-05 12:51:57.798528 easy_local_features-0.3.2/easy_local_features.egg-info/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     1942 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3607 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       68 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/requires.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-07-05 12:51:57.000000 easy_local_features-0.3.2/easy_local_features.egg-info/top_level.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-07-05 12:51:57.810528 easy_local_features-0.3.2/setup.cfg
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      910 2023-07-05 12:51:15.000000 easy_local_features-0.3.2/setup.py
```

### Comparing `easy_local_features-0.3.1/LICENSE_DISK.txt` & `easy_local_features-0.3.2/LICENSE_DISK.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/LICENSE_R2D2.txt` & `easy_local_features-0.3.2/LICENSE_R2D2.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/LICENSE_SUPERGLUE.txt` & `easy_local_features-0.3.2/LICENSE_SUPERGLUE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/PKG-INFO` & `easy_local_features-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_local_features
-Version: 0.3.1
+Version: 0.3.2
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
@@ -28,19 +28,19 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features.features.baseline_deal import DEAL_baseline
-# from easy_local_features.features.baseline_dalf import DALF_baseline
-# from easy_local_features.features.baseline_disk import DISK_baseline
-# from easy_local_features.features.baseline_r2d2 import R2D2_baseline
-# from easy_local_features.features.baseline_superpoint import SuperPoint_baseline
+from easy_local_features.feature.baseline_deal import DEAL_baseline
+# from easy_local_features.feature.baseline_dalf import DALF_baseline
+# from easy_local_features.feature.baseline_disk import DISK_baseline
+# from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
 extractor = DEAL_baseline()
```

### Comparing `easy_local_features-0.3.1/README.md` & `easy_local_features-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features.features.baseline_deal import DEAL_baseline
-# from easy_local_features.features.baseline_dalf import DALF_baseline
-# from easy_local_features.features.baseline_disk import DISK_baseline
-# from easy_local_features.features.baseline_r2d2 import R2D2_baseline
-# from easy_local_features.features.baseline_superpoint import SuperPoint_baseline
+from easy_local_features.feature.baseline_deal import DEAL_baseline
+# from easy_local_features.feature.baseline_dalf import DALF_baseline
+# from easy_local_features.feature.baseline_disk import DISK_baseline
+# from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
 extractor = DEAL_baseline()
```

### Comparing `easy_local_features-0.3.1/easy_local_features/datasets/download.py` & `easy_local_features-0.3.2/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/features/baseline_dalf.py` & `easy_local_features-0.3.2/easy_local_features/feature/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/features/baseline_deal.py` & `easy_local_features-0.3.2/easy_local_features/feature/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/features/baseline_disk.py` & `easy_local_features-0.3.2/easy_local_features/feature/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/features/baseline_r2d2.py` & `easy_local_features-0.3.2/easy_local_features/feature/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/features/baseline_superpoint.py` & `easy_local_features-0.3.2/easy_local_features/feature/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/matching/baseline_loftr.py` & `easy_local_features-0.3.2/easy_local_features/matching/baseline_loftr.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/matching/baseline_superglue.py` & `easy_local_features-0.3.2/easy_local_features/matching/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/structs.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/common/structs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch, abc, sys
 
-from torch_dimcheck import dimchecked
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
 # the class/object below is there for making type annotations like
 # def my_function(args) -> NpArray[OutputType]
 if sys.version_info >= (3, 7):
     class NpArray:
         def __class_getitem__(self, arg):
             pass
@@ -13,16 +14,16 @@
     class _NpArray:
         def __getitem__(self, _idx):
             pass
     
     NpArray = _NpArray()
 
 class Features:
-    @dimchecked
-    def __init__(self, kp: ['N', 2], desc: ['N', 'F'], kp_logp: ['N']):
+    # @dimchecked
+    def __init__(self, kp, desc, kp_logp):
         assert kp.device == desc.device
         assert kp.device == kp_logp.device
 
         self.kp      = kp
         self.desc    = desc
         self.kp_logp = kp_logp
 
@@ -53,19 +54,19 @@
             self.kp.to(*args, **kwargs),
             self.desc.to(*args, **kwargs),
             self.kp_logp.to(*args, **kwargs) if self.kp_logp is not None else None,
         )
 
 class MatchDistribution(abc.ABC):
     @abc.abstractmethod
-    def sample(self) -> [2, 'K']:
+    def sample(self):
         pass
 
     @abc.abstractmethod
-    def mle(self) -> [2, 'K']:
+    def mle(self):
         pass
 
     @abc.abstractmethod
     def dense_logp(self):
         pass
 
     @abc.abstractmethod
@@ -91,16 +92,16 @@
             self.features_1().kp,
             self.features_2().kp,
             matches,    
         )
 
 
 class MatchedPairs:
-    @dimchecked
-    def __init__(self, kps1: ['N', 2], kps2: ['M', 2], matches: [2, 'K']):
+    # @dimchecked
+    def __init__(self, kps1, kps2, matches):
         self.kps1    = kps1
         self.kps2    = kps2
         self.matches = matches
 
     def to(self, *args, **kwargs):
         return MatchedPairs(
             self.kps1.to(*args, **kwargs),
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/epi.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/epi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import torch
 
-from torch_dimcheck import dimchecked
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
-@dimchecked
-def cross_product_matrix(v: [3]) -> [3, 3]:
+# @dimchecked
+def cross_product_matrix(v):
     ''' following
         en.wikipedia.org/wiki/Cross_product#Conversion_to_matrix_multiplication
     '''
 
     return torch.tensor([
         [    0, -v[2],  v[1]],
         [ v[2],     0, -v[0]],
         [-v[1],  v[0],     0]
     ], dtype=v.dtype, device=v.device)
 
-@dimchecked
-def xy_to_xyw(xy: [2, 'N']) -> [3, 'N']:
+# @dimchecked
+def xy_to_xyw(xy):
     ones = torch.ones(1, xy.shape[1], device=xy.device, dtype=xy.dtype)
     return torch.cat([xy, ones], dim=0)
 
-@dimchecked
-def ims2E(im1, im2) -> [3, 3]:
+# @dimchecked
+def ims2E(im1, im2):
     R = im2.R @ im1.R.T
     T = im2.T - R @ im1.T
     return cross_product_matrix(T) @ R
 
-@dimchecked
-def ims2F(im1, im2) -> [3, 3]:
+# @dimchecked
+def ims2F(im1, im2):
     E = ims2E(im1, im2)
     return im2.K_inv.T @ E @ im1.K_inv
  
-@dimchecked
-def symdimm(x1: [2, 'N'], x2: [2, 'M'], im1, im2) -> ['N', 'M']:
+# @dimchecked
+def symdimm(x1, x2, im1, im2):
     x1n = im1.K_inv @ xy_to_xyw(x1)
     x2n = im2.K_inv @ xy_to_xyw(x2)
 
     E = ims2E(im1, im2)
 
     E_x1  = E @ x1n
     Et_x2 = E.T @ x2n
@@ -45,47 +46,47 @@
 
     n1 = 1 / n(E_x1[:2])[None, :]
     n2 = 1 / n(Et_x2[:2])[:, None]
     norm = n1 + n2
     dist = x2_E_x1.pow(2) * norm
     return dist.T
 
-@dimchecked
-def asymmdist(x1: [2, 'N'], x2: [2, 'M'], F: [3, 3]) -> ['N', 'M']:
+# @dimchecked
+def asymmdist(x1, x2, F):
     '''
     following http://www.cs.toronto.edu/~jepson/csc420/notes/epiPolarGeom.pdf
     (page 12)
     '''
 
     x1_h = xy_to_xyw(x1)
     x2_h = xy_to_xyw(x2)
 
     Ft_x2 = F.T @ x2_h
     norm  = torch.norm(Ft_x2[:2], p=2, dim=0)
     dist  = (Ft_x2 / norm).T @ x1_h
     return dist.T
 
-@dimchecked
-def asymmdist_from_imgs(x1: [2, 'N'], x2: [2, 'M'], im1, im2) -> ['N', 'M']:
+# @dimchecked
+def asymmdist_from_imgs(x1, x2, im1, im2):
     F = ims2F(im1, im2)
     return asymmdist(x1, x2, F)
 
-@dimchecked
-def p_asymmdist(x1: [2, 'N'], x2: [2, 'N'], F: [3, 3]) -> ['N']:
+# @dimchecked
+def p_asymmdist(x1, x2, F) :
     '''
     following http://www.cs.toronto.edu/~jepson/csc420/notes/epiPolarGeom.pdf
     (page 12)
     '''
 
     x1_h = xy_to_xyw(x1)
     x2_h = xy_to_xyw(x2)
 
     Ft_x2 = F.T @ x2_h
     norm  = torch.norm(Ft_x2[:2], p=2, dim=0)
     Ft_x2_n = Ft_x2 / norm
 
     return torch.einsum('ca,ca->a', (Ft_x2_n, x1_h))
 
-@dimchecked
-def p_asymmdist_from_imgs(x1: [2, 'N'], x2: [2, 'N'], im1, im2) -> ['N']:
+# @dimchecked
+def p_asymmdist_from_imgs(x1, x2, im1, im2) :
     F = ims2F(im1, im2)
     return p_asymmdist(x1, x2, F)
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/pose.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/geom/pose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing, torch, math
 import numpy as np
 import torch.nn.functional as F
 
-from torch_dimcheck import dimchecked
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
 RAD_TO_DEG = 57.29
 
 class PoseError(typing.NamedTuple):
     Δ_θ    : float
     Δ_T    : float
 
@@ -79,31 +80,31 @@
             p1.T.unsqueeze(0),
             p2.T.unsqueeze(0)
         ).squeeze(0)
         Δ_T = RAD_TO_DEG * math.acos(torch.clamp(cos_sim, -1., 1.).item())
             
         return PoseError(θ_deg, Δ_T)
         
-def _normalized_cosine_error(v1: ['N'], v2: ['N']):
+def _normalized_cosine_error(v1, v2):
     EPS = 1e-15
 
     def normalize(v):
         v = v.to(torch.float64)
         return v / (torch.norm(v) + EPS)
 
     v1 = normalize(v1)
     v2 = normalize(v2)
 
     cos = max(EPS, 1. - torch.dot(v1, v2).pow(2).item())
     err = math.acos(math.sqrt(1. - cos))
 
     return err
 
-@dimchecked
-def matrix_to_quaternion(M: [3, 3]) -> [4]:
+# @dimchecked
+def matrix_to_quaternion(M):
     '''
     adapted from
     https://github.com/vcg-uvic/sfm_benchmark/blob/2b28c76635f754cbc32f30571adf80f3eba13f4c/utils/eval_helper.py#L170
     '''
 
     #TODO: this appears unused
     m00 = M[0, 0].item()
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 from torch import nn
 from torch.distributions import Categorical
-from torch_dimcheck import dimchecked
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
 from ..common.structs import Features, NpArray, MatchDistribution
 from ..geom import distance_matrix
 
 class ConsistentMatchDistribution(MatchDistribution):
     def __init__(
         self,
@@ -25,49 +26,49 @@
 
         self._cat_I = Categorical(logits=affinity)
         self._cat_T = Categorical(logits=affinity.T)
 
         self._dense_logp = None
         self._dense_p    = None
 
-    @dimchecked
-    def dense_p(self) -> ['N', 'M']:
+    # @dimchecked
+    def dense_p(self):
         if self._dense_p is None:
             self._dense_p = self._cat_I.probs * self._cat_T.probs.T
 
         return self._dense_p
 
-    @dimchecked
-    def dense_logp(self) -> ['N', 'M']:
+    # @dimchecked
+    def dense_logp(self):
         if self._dense_logp is None:
             self._dense_logp = self._cat_I.logits + self._cat_T.logits.T
 
         return self._dense_logp
 
-    @dimchecked
-    def _select_cycle_consistent(self, left: ['N'], right: ['M']) -> [2, 'K']:
+    # @dimchecked
+    def _select_cycle_consistent(self, left, right):
         indexes = torch.arange(left.shape[0], device=left.device)
         cycle_consistent = right[left] == indexes
 
         paired_left = left[cycle_consistent]
 
         return torch.stack([
             right[paired_left],
             paired_left,
         ], dim=0)
 
-    @dimchecked
-    def sample(self) -> [2, 'K']:
+    # @dimchecked
+    def sample(self):
         samples_I = self._cat_I.sample()
         samples_T = self._cat_T.sample()
 
         return self._select_cycle_consistent(samples_I, samples_T)
 
-    @dimchecked
-    def mle(self) -> [2, 'K']:
+    # @dimchecked
+    def mle(self):
         maxes_I = self._cat_I.logits.argmax(dim=1)
         maxes_T = self._cat_T.logits.argmax(dim=1)
 
         # FIXME UPSTREAM: this detachment is necessary until the bug is fixed
         maxes_I = maxes_I.detach()
         maxes_T = maxes_T.detach()
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import torch, typing
 import numpy as np
-from torch_dimcheck import dimchecked
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
 from ..common.structs import NpArray, Features, MatchedPairs
 from ..geom import distance_matrix
 
 class CycleMatcher:
-    @dimchecked
-    def match_features(self, feat_1: ['N', 'F'], feat_2: ['M', 'F']) -> [2, 'K']:
+    # @dimchecked
+    def match_features(self, feat_1, feat_2):
         dist_m = distance_matrix(feat_1, feat_2)
 
         if dist_m.shape[0] == 0 or dist_m.shape[1] == 0:
             msg = '''
             Feature matching failed because one image has 0 detected features.
             This likely means that the algorithm has converged to a local
             optimum of detecting no features at all (0 reward). This can arise
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/detector.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import torch
 import numpy as np
 import torch.nn.functional as F
 
 from torch.distributions import Categorical, Bernoulli
-from torch_dimcheck import dimchecked
+
+# from torch_dimcheck import dimchecked
+# from ...submodules.torch_dimcheck import dimchecked
 
 from ..common.structs import NpArray, Features
 from ..model.nms import nms
 
-@dimchecked
-def select_on_last(values: [..., 'T'], indices: [...]) -> [...]:
+# @dimchecked
+def select_on_last(values, indices):
     '''
     WARNING: this may be reinventing the wheel, but I don't know how to do
     it otherwise with PyTorch.
 
     This function uses an array of linear indices `indices` between [0, T] to
     index into `values` which has equal shape as `indices` and then one extra
     dimension of size T.
     '''
     return torch.gather(
         values,
         -1,
         indices[..., None]
     ).squeeze(-1)
 
-@dimchecked
+# @dimchecked
 def point_distribution(
-    logits: [..., 'T']
-) -> ([...], [...], [...]):
+    logits
+):
     '''
     Implements the categorical proposal -> Bernoulli acceptance sampling
     scheme. Given a tensor of logits, performs samples on the last dimension,
     returning
         a) the proposals
         b) a binary mask indicating which ones were accepted
         c) the logp-probability of (proposal and acceptance decision)
@@ -55,21 +57,21 @@
 class Keypoints:
     '''
     A simple, temporary struct used to store keypoint detections and their
     log-probabilities. After construction, merge_with_descriptors is used to
     select corresponding descriptors from unet output.
     '''
 
-    @dimchecked
-    def __init__(self, xys: ['N', 2], logp: ['N']):
+    # @dimchecked
+    def __init__(self, xys, logp):
         self.xys  = xys
         self.logp = logp
 
-    @dimchecked
-    def merge_with_descriptors(self, descriptors: ['C', 'H', 'W']) -> Features:
+    # @dimchecked
+    def merge_with_descriptors(self, descriptors) -> Features:
         '''
         Select descriptors from a dense `descriptors` tensor, at locations
         given by `self.xys`
         '''
         x, y = self.xys.T
 
         desc = descriptors[:, y, x].T
@@ -77,16 +79,16 @@
 
         return Features(self.xys.to(torch.float32), desc, self.logp)
 
 class Detector:
     def __init__(self, window=8):
         self.window = window
 
-    @dimchecked
-    def _tile(self, heatmap: ['B', 'C', 'H', 'W']) -> ['B', 'C', 'h', 'w', 'T']:
+    # @dimchecked
+    def _tile(self, heatmap):
         '''
         Divides the heatmap `heatmap` into tiles of size (v, v) where
         v==self.window. The tiles are flattened, resulting in the last
         dimension of the output T == v * v.
         '''
         v = self.window
         b, c, h, w = heatmap.shape
@@ -94,16 +96,16 @@
         assert heatmap.shape[2] % v == 0
         assert heatmap.shape[3] % v == 0
 
         return heatmap.unfold(2, v, v) \
                       .unfold(3, v, v) \
                       .reshape(b, c, h // v, w // v, v*v)
 
-    @dimchecked
-    def sample(self, heatmap: ['B', 1, 'H', 'W']) -> NpArray[Keypoints]:
+    # @dimchecked
+    def sample(self, heatmap) -> NpArray[Keypoints]:
         '''
             Implements the training-time grid-based sampling protocol
         '''
         v = self.window
         dev = heatmap.device
         B, _, H, W = heatmap.shape
 
@@ -137,18 +139,18 @@
             keypoints.append(Keypoints(
                 xys[i][mask],
                 logp[i][mask],
             ))
 
         return np.array(keypoints, dtype=object)
 
-    @dimchecked
+    # @dimchecked
     def nms(
         self,
-        heatmap: ['B', 1, 'H', 'W'],
+        heatmap,
         n=None,
         **kwargs
     ) -> NpArray[Keypoints]:
         '''
             Inference-time nms-based detection protocol
         '''
         heatmap = heatmap.squeeze(1)
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/disk.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/disk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import numpy as np
 
-from torch_dimcheck import dimchecked
-from unets import Unet, thin_setup
+# from ...submodules.torch_dimcheck import dimchecked
+from ..unets import Unet, thin_setup
 
 from .detector import Detector
 from ..common.structs import NpArray, Features
 
 DEFAULT_SETUP = {**thin_setup, 'bias': True, 'padding': True}
 
 class DISK(torch.nn.Module):
@@ -24,31 +24,30 @@
             in_features=3, size=kernel_size,
             down=[16, 32, 64, 64, 64],
             up=[64, 64, 64, desc_dim+1],
             setup=setup,
         )
         self.detector = Detector(window=window)
 
-    @dimchecked
-    def _split(self, unet_output: ['B', 'C', 'H', 'W']) \
-                -> (['B', 'C-1', 'H', 'W'], ['B', 1, 'H', 'W']):
+    # @dimchecked
+    def _split(self, unet_output):
         '''
         Splits the raw Unet output into descriptors and detection heatmap.
         '''
         assert unet_output.shape[1] == self.desc_dim + 1
 
         descriptors = unet_output[:, :self.desc_dim]
         heatmap     = unet_output[:, self.desc_dim:]
 
         return descriptors, heatmap
 
-    @dimchecked
+    # @dimchecked
     def features(
         self,
-        images: ['B', 'C', 'H', 'W'],
+        images,
         kind='rng',
         **kwargs
     ) -> NpArray[Features]:
         ''' allowed values for `kind`:
             * rng
             * nms
         '''
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/nms.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_disk/disk/model/nms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import torch.nn.functional as F
-from torch_dimcheck import dimchecked
 
-@dimchecked
-def nms(signal: ['B', 'H', 'W'], window_size=5, cutoff=0.) -> ['B', 'H', 'W']:
+# from ...submodules.torch_dimcheck import dimchecked
+
+# @dimchecked
+def nms(signal, window_size=5, cutoff=0.) :
     if window_size % 2 != 1:
         raise ValueError(f'window_size has to be odd, got {window_size}')
 
     _, ixs = F.max_pool2d(
         signal,
         kernel_size=window_size,
         stride=1,
```

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract_kapture.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/extract_kapture.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/ap_loss.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/ap_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/losses.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/losses.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/patchnet.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/patchnet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/sampler.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/nets/sampler.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/common.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/common.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/dataloader.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/dataloader.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/trainer.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/viz.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/tools/viz.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/train.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/train.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/viz_heatmaps.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_r2d2/viz_heatmaps.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/matching.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/matching.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superglue.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superpoint.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/utils.py` & `easy_local_features-0.3.2/easy_local_features/submodules/git_superglue/models/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.1/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.3.2/easy_local_features.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-local-features
-Version: 0.3.1
+Version: 0.3.2
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
@@ -28,19 +28,19 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features.features.baseline_deal import DEAL_baseline
-# from easy_local_features.features.baseline_dalf import DALF_baseline
-# from easy_local_features.features.baseline_disk import DISK_baseline
-# from easy_local_features.features.baseline_r2d2 import R2D2_baseline
-# from easy_local_features.features.baseline_superpoint import SuperPoint_baseline
+from easy_local_features.feature.baseline_deal import DEAL_baseline
+# from easy_local_features.feature.baseline_dalf import DALF_baseline
+# from easy_local_features.feature.baseline_disk import DISK_baseline
+# from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
 extractor = DEAL_baseline()
```

### Comparing `easy_local_features-0.3.1/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.3.2/easy_local_features.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 LICENSE_SUPERGLUE.txt
 README.md
 setup.py
 easy_local_features/__init__.py
 easy_local_features.egg-info/PKG-INFO
 easy_local_features.egg-info/SOURCES.txt
 easy_local_features.egg-info/dependency_links.txt
+easy_local_features.egg-info/requires.txt
 easy_local_features.egg-info/top_level.txt
 easy_local_features/datasets/__init__.py
 easy_local_features/datasets/download.py
-easy_local_features/features/__init__.py
-easy_local_features/features/baseline_dalf.py
-easy_local_features/features/baseline_deal.py
-easy_local_features/features/baseline_disk.py
-easy_local_features/features/baseline_r2d2.py
-easy_local_features/features/baseline_superpoint.py
+easy_local_features/feature/__init__.py
+easy_local_features/feature/baseline_dalf.py
+easy_local_features/feature/baseline_deal.py
+easy_local_features/feature/baseline_disk.py
+easy_local_features/feature/baseline_r2d2.py
+easy_local_features/feature/baseline_superpoint.py
 easy_local_features/matching/__init__.py
 easy_local_features/matching/baseline_loftr.py
 easy_local_features/matching/baseline_superglue.py
 easy_local_features/matching/core.py
 easy_local_features/submodules/__init__.py
 easy_local_features/submodules/git_disk/__init__.py
 easy_local_features/submodules/git_disk/disk/__init__.py
@@ -31,14 +32,19 @@
 easy_local_features/submodules/git_disk/disk/geom/pose.py
 easy_local_features/submodules/git_disk/disk/model/__init__.py
 easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
 easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
 easy_local_features/submodules/git_disk/disk/model/detector.py
 easy_local_features/submodules/git_disk/disk/model/disk.py
 easy_local_features/submodules/git_disk/disk/model/nms.py
+easy_local_features/submodules/git_disk/disk/unets/__init__.py
+easy_local_features/submodules/git_disk/disk/unets/blocks.py
+easy_local_features/submodules/git_disk/disk/unets/ops.py
+easy_local_features/submodules/git_disk/disk/unets/unet.py
+easy_local_features/submodules/git_disk/disk/unets/utils.py
 easy_local_features/submodules/git_r2d2/__init__.py
 easy_local_features/submodules/git_r2d2/extract.py
 easy_local_features/submodules/git_r2d2/extract_kapture.py
 easy_local_features/submodules/git_r2d2/train.py
 easy_local_features/submodules/git_r2d2/viz_heatmaps.py
 easy_local_features/submodules/git_r2d2/nets/__init__.py
 easy_local_features/submodules/git_r2d2/nets/ap_loss.py
@@ -56,13 +62,9 @@
 easy_local_features/submodules/git_r2d2/tools/viz.py
 easy_local_features/submodules/git_superglue/__init__.py
 easy_local_features/submodules/git_superglue/models/__init__.py
 easy_local_features/submodules/git_superglue/models/matching.py
 easy_local_features/submodules/git_superglue/models/superglue.py
 easy_local_features/submodules/git_superglue/models/superpoint.py
 easy_local_features/submodules/git_superglue/models/utils.py
-tests/test_dalf.py
-tests/test_deal.py
-tests/test_disk.py
-tests/test_r2d2.py
-tests/test_superglue.py
-tests/test_superpoint.py
+easy_local_features/utils/__init__.py
+easy_local_features/utils/generic_match.py
```

### Comparing `easy_local_features-0.3.1/setup.py` & `easy_local_features-0.3.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,16 +12,24 @@
         long_description = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.3.1',
+    version='0.3.2',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
-    install_requires=[],
+    install_requires=[
+        'numpy',
+        'scipy',
+        'torch>=1.9.1',
+        'torchvision>=0.9.1',
+        'opencv-python',
+        'wget',
+        'tqdm',
+    ],
     long_description_content_type='text/markdown',
     long_description=long_description,
 )
```

