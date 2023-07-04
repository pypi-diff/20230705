# Comparing `tmp/easy_local_features-0.3.0.tar.gz` & `tmp/easy_local_features-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.3.0.tar", last modified: Sat Jul  1 17:24:56 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.1.tar", last modified: Tue Jul  4 22:59:08 2023, max compression
```

## Comparing `easy_local_features-0.3.0.tar` & `easy_local_features-0.3.1.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.709808 easy_local_features-0.3.0/
--rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.0/LICENSE_DISK.txt
--rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.0/LICENSE_R2D2.txt
--rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.0/LICENSE_SUPERGLUE.txt
--rw-r--r--   0 cadar      (501) staff       (20)     1597 2023-07-01 17:24:56.709543 easy_local_features-0.3.0/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     1345 2023-07-01 17:24:12.000000 easy_local_features-0.3.0/README.md
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.696457 easy_local_features-0.3.0/easy_local_features/
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.0/easy_local_features/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)    34250 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/baseline_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-01 09:14:35.000000 easy_local_features-0.3.0/easy_local_features/baseline_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-01 15:51:12.000000 easy_local_features-0.3.0/easy_local_features/baseline_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-01 17:02:37.000000 easy_local_features-0.3.0/easy_local_features/baseline_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.0/easy_local_features/baseline_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-01 16:59:28.000000 easy_local_features-0.3.0/easy_local_features/baseline_superpoint.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697523 easy_local_features-0.3.0/easy_local_features/datasets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/datasets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/datasets/download.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697694 easy_local_features-0.3.0/easy_local_features/submodules/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.0/easy_local_features/submodules/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697860 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.698012 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/
--rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.698432 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2675 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/structs.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.699742 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/
--rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      271 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
--rw-r--r--   0 cadar      (501) staff       (20)     2253 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/epi.py
--rw-r--r--   0 cadar      (501) staff       (20)     3377 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/pose.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.701372 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/
--rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2744 2023-07-01 15:52:24.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     2544 2023-07-01 15:34:26.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     5573 2023-07-01 15:33:05.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/detector.py
--rw-r--r--   0 cadar      (501) staff       (20)     2265 2023-07-01 15:52:15.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      881 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/nms.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.702965 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract.py
--rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract_kapture.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.704634 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/losses.py
--rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/patchnet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/sampler.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.706082 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/common.py
--rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/dataloader.py
--rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/trainer.py
--rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms.py
--rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
--rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/viz.py
--rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/train.py
--rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.706318 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.707414 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/matching.py
--rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superpoint.py
--rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697180 easy_local_features-0.3.0/easy_local_features.egg-info/
--rw-r--r--   0 cadar      (501) staff       (20)     1597 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     3094 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/SOURCES.txt
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/dependency_links.txt
--rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/top_level.txt
--rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-01 17:24:56.709863 easy_local_features-0.3.0/setup.cfg
--rw-r--r--   0 cadar      (501) staff       (20)      760 2023-07-01 17:18:43.000000 easy_local_features-0.3.0/setup.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.709127 easy_local_features-0.3.0/tests/
--rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:21:05.000000 easy_local_features-0.3.0/tests/test_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:20:49.000000 easy_local_features-0.3.0/tests/test_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:20:35.000000 easy_local_features-0.3.0/tests/test_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:21:41.000000 easy_local_features-0.3.0/tests/test_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)      161 2023-07-01 17:21:58.000000 easy_local_features-0.3.0/tests/test_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)      164 2023-07-01 17:22:12.000000 easy_local_features-0.3.0/tests/test_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.584116 easy_local_features-0.3.1/
+-rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.1/LICENSE_DISK.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.1/LICENSE_R2D2.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.1/LICENSE_SUPERGLUE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     1947 2023-07-04 22:59:08.583968 easy_local_features-0.3.1/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     1695 2023-07-04 22:58:44.000000 easy_local_features-0.3.1/README.md
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.574657 easy_local_features-0.3.1/easy_local_features/
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.1/easy_local_features/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.575700 easy_local_features-0.3.1/easy_local_features/datasets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/datasets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/datasets/download.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.576606 easy_local_features-0.3.1/easy_local_features/features/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:09:54.000000 easy_local_features-0.3.1/easy_local_features/features/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    34250 2023-06-12 19:58:13.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-01 09:14:35.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-01 15:51:12.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-01 17:02:37.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-01 16:59:28.000000 easy_local_features-0.3.1/easy_local_features/features/baseline_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577113 easy_local_features-0.3.1/easy_local_features/matching/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.1/easy_local_features/matching/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2103 2023-07-04 22:47:59.000000 easy_local_features-0.3.1/easy_local_features/matching/baseline_loftr.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.1/easy_local_features/matching/baseline_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.1/easy_local_features/matching/core.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577219 easy_local_features-0.3.1/easy_local_features/submodules/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.1/easy_local_features/submodules/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577378 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577503 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/
+-rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.577780 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2675 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.578327 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/
+-rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      271 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2253 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3377 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.579177 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/
+-rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2744 2023-07-01 15:52:24.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2544 2023-07-01 15:34:26.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5573 2023-07-01 15:33:05.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2265 2023-07-01 15:52:15.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      881 2023-07-01 08:54:41.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.579986 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.581075 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582006 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/train.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582197 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.582815 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.575347 easy_local_features-0.3.1/easy_local_features.egg-info/
+-rw-r--r--   0 cadar      (501) staff       (20)     1947 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     3314 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/SOURCES.txt
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/dependency_links.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-04 22:59:08.000000 easy_local_features-0.3.1/easy_local_features.egg-info/top_level.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-04 22:59:08.584161 easy_local_features-0.3.1/setup.cfg
+-rw-r--r--   0 cadar      (501) staff       (20)      760 2023-07-04 22:57:43.000000 easy_local_features-0.3.1/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-04 22:59:08.583752 easy_local_features-0.3.1/tests/
+-rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:20.000000 easy_local_features-0.3.1/tests/test_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:19.000000 easy_local_features-0.3.1/tests/test_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:19.000000 easy_local_features-0.3.1/tests/test_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      155 2023-07-04 22:12:18.000000 easy_local_features-0.3.1/tests/test_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)      170 2023-07-04 22:12:18.000000 easy_local_features-0.3.1/tests/test_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)      173 2023-07-04 22:12:16.000000 easy_local_features-0.3.1/tests/test_superpoint.py
```

### Comparing `easy_local_features-0.3.0/LICENSE_DISK.txt` & `easy_local_features-0.3.1/LICENSE_DISK.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/LICENSE_R2D2.txt` & `easy_local_features-0.3.1/LICENSE_R2D2.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/LICENSE_SUPERGLUE.txt` & `easy_local_features-0.3.1/LICENSE_SUPERGLUE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/PKG-INFO` & `easy_local_features-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_local_features
-Version: 0.3.0
+Version: 0.3.1
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
@@ -28,34 +28,42 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features.baseline_deal import DEAL_baseline
-# from easy_local_features.baseline_dalf import DALF_baseline
-# from easy_local_features.baseline_disk import DISK_baseline
-# from easy_local_features.baseline_r2d2 import R2D2_baseline
-# from easy_local_features.baseline_superglue import SuperGlue_baseline
-# from easy_local_features.baseline_superpoint import SuperPoint_baseline
+from easy_local_features.features.baseline_deal import DEAL_baseline
+# from easy_local_features.features.baseline_dalf import DALF_baseline
+# from easy_local_features.features.baseline_disk import DISK_baseline
+# from easy_local_features.features.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.features.baseline_superpoint import SuperPoint_baseline
+# from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
 extractor = DEAL_baseline()
 
 # Return keypoints and descriptors just like OpenCV
 keypoints, descriptors = extractor.detectAndCompute(img)
 
 ```
 # TODO
 
 - [x] Add a setup.py to make it a pip package
+- [ ] Make a general maching class
+  - The idea is to have a class that can match images using any local feature extractor and any matching method.
+- [ ] Fix requirements to install automatically with the package (maybe)
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
-  - [ ] ASLFeat
+  - [x] DEAL
+  - [x] R2D2
+  - [x] DISK
+  - [x] SuperPoin
+  - [x] SuperGlue
   - [x] DELF
-  - [ ] LoFTR
+  - [ ] ASLFeat
+  - [x] LoFTR
   - [ ] DKM
```

### Comparing `easy_local_features-0.3.0/README.md` & `easy_local_features-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -18,34 +18,42 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features.baseline_deal import DEAL_baseline
-# from easy_local_features.baseline_dalf import DALF_baseline
-# from easy_local_features.baseline_disk import DISK_baseline
-# from easy_local_features.baseline_r2d2 import R2D2_baseline
-# from easy_local_features.baseline_superglue import SuperGlue_baseline
-# from easy_local_features.baseline_superpoint import SuperPoint_baseline
+from easy_local_features.features.baseline_deal import DEAL_baseline
+# from easy_local_features.features.baseline_dalf import DALF_baseline
+# from easy_local_features.features.baseline_disk import DISK_baseline
+# from easy_local_features.features.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.features.baseline_superpoint import SuperPoint_baseline
+# from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
 extractor = DEAL_baseline()
 
 # Return keypoints and descriptors just like OpenCV
 keypoints, descriptors = extractor.detectAndCompute(img)
 
 ```
 # TODO
 
 - [x] Add a setup.py to make it a pip package
+- [ ] Make a general maching class
+  - The idea is to have a class that can match images using any local feature extractor and any matching method.
+- [ ] Fix requirements to install automatically with the package (maybe)
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
-  - [ ] ASLFeat
+  - [x] DEAL
+  - [x] R2D2
+  - [x] DISK
+  - [x] SuperPoin
+  - [x] SuperGlue
   - [x] DELF
-  - [ ] LoFTR
+  - [ ] ASLFeat
+  - [x] LoFTR
   - [ ] DKM
```

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_dalf.py` & `easy_local_features-0.3.1/easy_local_features/features/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_deal.py` & `easy_local_features-0.3.1/easy_local_features/features/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_disk.py` & `easy_local_features-0.3.1/easy_local_features/features/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_r2d2.py` & `easy_local_features-0.3.1/easy_local_features/features/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_superglue.py` & `easy_local_features-0.3.1/easy_local_features/matching/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/baseline_superpoint.py` & `easy_local_features-0.3.1/easy_local_features/features/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/datasets/download.py` & `easy_local_features-0.3.1/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/structs.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/common/structs.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/epi.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/epi.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/pose.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/geom/pose.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/detector.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/detector.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/disk.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/nms.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_disk/disk/model/nms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract_kapture.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/extract_kapture.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/ap_loss.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/ap_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/losses.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/losses.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/patchnet.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/patchnet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/sampler.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/nets/sampler.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/common.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/common.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/dataloader.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/dataloader.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/trainer.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/viz.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/tools/viz.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/train.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/train.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/viz_heatmaps.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_r2d2/viz_heatmaps.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/matching.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/matching.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superglue.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superpoint.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/utils.py` & `easy_local_features-0.3.1/easy_local_features/submodules/git_superglue/models/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.0/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.3.1/easy_local_features.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE_DISK.txt
 LICENSE_R2D2.txt
 LICENSE_SUPERGLUE.txt
 README.md
 setup.py
 easy_local_features/__init__.py
-easy_local_features/baseline_dalf.py
-easy_local_features/baseline_deal.py
-easy_local_features/baseline_disk.py
-easy_local_features/baseline_r2d2.py
-easy_local_features/baseline_superglue.py
-easy_local_features/baseline_superpoint.py
 easy_local_features.egg-info/PKG-INFO
 easy_local_features.egg-info/SOURCES.txt
 easy_local_features.egg-info/dependency_links.txt
 easy_local_features.egg-info/top_level.txt
 easy_local_features/datasets/__init__.py
 easy_local_features/datasets/download.py
+easy_local_features/features/__init__.py
+easy_local_features/features/baseline_dalf.py
+easy_local_features/features/baseline_deal.py
+easy_local_features/features/baseline_disk.py
+easy_local_features/features/baseline_r2d2.py
+easy_local_features/features/baseline_superpoint.py
+easy_local_features/matching/__init__.py
+easy_local_features/matching/baseline_loftr.py
+easy_local_features/matching/baseline_superglue.py
+easy_local_features/matching/core.py
 easy_local_features/submodules/__init__.py
 easy_local_features/submodules/git_disk/__init__.py
 easy_local_features/submodules/git_disk/disk/__init__.py
 easy_local_features/submodules/git_disk/disk/common/__init__.py
 easy_local_features/submodules/git_disk/disk/common/structs.py
 easy_local_features/submodules/git_disk/disk/geom/__init__.py
 easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
```

### Comparing `easy_local_features-0.3.0/setup.py` & `easy_local_features-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         long_description = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.3.0',
+    version='0.3.1',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
     install_requires=[],
     long_description_content_type='text/markdown',
     long_description=long_description,
```

