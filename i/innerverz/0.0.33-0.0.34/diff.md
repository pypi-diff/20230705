# Comparing `tmp/innerverz-0.0.33.tar.gz` & `tmp/innerverz-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.33.tar", last modified: Wed Jul  5 01:39:18 2023, max compression
+gzip compressed data, was "innerverz-0.0.34.tar", last modified: Wed Jul  5 10:29:06 2023, max compression
```

## Comparing `innerverz-0.0.33.tar` & `innerverz-0.0.34.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.835412 innerverz-0.0.33/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.33/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      230 2023-07-05 01:39:18.835527 innerverz-0.0.33/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.33/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.792700 innerverz-0.0.33/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1713 2023-07-04 12:11:52.000000 innerverz-0.0.33/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.793974 innerverz-0.0.33/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.0.33/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.794577 innerverz-0.0.33/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-04 10:37:03.000000 innerverz-0.0.33/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.795037 innerverz-0.0.33/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.0.33/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.796196 innerverz-0.0.33/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.33/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.797039 innerverz-0.0.33/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.797314 innerverz-0.0.33/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.0.33/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.797878 innerverz-0.0.33/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.0.33/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.798952 innerverz-0.0.33/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)    10106 2023-07-04 11:49:44.000000 innerverz-0.0.33/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.800402 innerverz-0.0.33/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.800922 innerverz-0.0.33/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5345 2023-07-04 11:18:33.000000 innerverz-0.0.33/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.802799 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.803363 innerverz-0.0.33/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.0.33/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.804048 innerverz-0.0.33/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.0.33/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8101 2023-07-04 12:20:23.000000 innerverz-0.0.33/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.808425 innerverz-0.0.33/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.808708 innerverz-0.0.33/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8178 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.809005 innerverz-0.0.33/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24825 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4325 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.809247 innerverz-0.0.33/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.815533 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.0.33/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.0.33/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.816035 innerverz-0.0.33/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2908 2023-07-04 11:15:48.000000 innerverz-0.0.33/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.824083 innerverz-0.0.33/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5537 2023-07-04 11:16:19.000000 innerverz-0.0.33/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.825289 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.826905 innerverz-0.0.33/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.0.33/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.829565 innerverz-0.0.33/innerverz/landmark_warping/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-04 12:10:40.000000 innerverz-0.0.33/innerverz/landmark_warping/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3296 2023-07-04 12:03:56.000000 innerverz-0.0.33/innerverz/landmark_warping/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4246 2023-07-04 10:39:19.000000 innerverz-0.0.33/innerverz/landmark_warping/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.0.33/innerverz/landmark_warping/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.0.33/innerverz/landmark_warping/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.830217 innerverz-0.0.33/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.33/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.0.33/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.33/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.33/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.830726 innerverz-0.0.33/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.0.33/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.831269 innerverz-0.0.33/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2404 2023-07-04 11:17:23.000000 innerverz-0.0.33/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.831777 innerverz-0.0.33/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.834333 innerverz-0.0.33/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.834602 innerverz-0.0.33/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.0.33/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.835271 innerverz-0.0.33/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.33/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 01:39:18.793670 innerverz-0.0.33/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      230 2023-07-05 01:39:18.000000 innerverz-0.0.33/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4579 2023-07-05 01:39:18.000000 innerverz-0.0.33/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-05 01:39:18.000000 innerverz-0.0.33/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-05 01:39:18.000000 innerverz-0.0.33/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-05 01:39:18.000000 innerverz-0.0.33/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.33/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-05 01:39:18.835867 innerverz-0.0.33/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      809 2023-07-05 01:39:14.000000 innerverz-0.0.33/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.414151 innerverz-0.0.34/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.34/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-07-05 10:29:06.414271 innerverz-0.0.34/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.34/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.392879 innerverz-0.0.34/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1713 2023-07-04 12:11:52.000000 innerverz-0.0.34/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.394030 innerverz-0.0.34/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.0.34/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.394637 innerverz-0.0.34/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.0.34/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.395300 innerverz-0.0.34/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.0.34/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.396776 innerverz-0.0.34/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.34/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.397835 innerverz-0.0.34/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.398144 innerverz-0.0.34/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.0.34/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.399048 innerverz-0.0.34/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.0.34/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.400431 innerverz-0.0.34/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.0.34/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.401076 innerverz-0.0.34/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.401859 innerverz-0.0.34/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.0.34/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.402737 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.403375 innerverz-0.0.34/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.0.34/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.403855 innerverz-0.0.34/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.0.34/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8101 2023-07-04 12:20:23.000000 innerverz-0.0.34/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.404475 innerverz-0.0.34/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.404790 innerverz-0.0.34/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8178 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.405138 innerverz-0.0.34/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24825 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4325 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.405405 innerverz-0.0.34/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.406377 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.0.34/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.0.34/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.407127 innerverz-0.0.34/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2908 2023-07-04 11:15:48.000000 innerverz-0.0.34/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.407719 innerverz-0.0.34/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5537 2023-07-04 11:16:19.000000 innerverz-0.0.34/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.408403 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.408933 innerverz-0.0.34/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.0.34/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.409623 innerverz-0.0.34/innerverz/landmark_warping/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-04 12:10:40.000000 innerverz-0.0.34/innerverz/landmark_warping/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3311 2023-07-05 10:15:15.000000 innerverz-0.0.34/innerverz/landmark_warping/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4246 2023-07-04 10:39:19.000000 innerverz-0.0.34/innerverz/landmark_warping/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.0.34/innerverz/landmark_warping/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.0.34/innerverz/landmark_warping/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.410386 innerverz-0.0.34/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.34/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.0.34/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.34/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.34/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.411313 innerverz-0.0.34/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.0.34/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.411987 innerverz-0.0.34/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.0.34/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.412569 innerverz-0.0.34/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.413145 innerverz-0.0.34/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.413293 innerverz-0.0.34/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.0.34/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.413998 innerverz-0.0.34/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.34/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:29:06.393647 innerverz-0.0.34/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-07-05 10:29:06.000000 innerverz-0.0.34/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4579 2023-07-05 10:29:06.000000 innerverz-0.0.34/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-05 10:29:06.000000 innerverz-0.0.34/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-05 10:29:06.000000 innerverz-0.0.34/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-05 10:29:06.000000 innerverz-0.0.34/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.34/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-05 10:29:06.415563 innerverz-0.0.34/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-07-05 10:28:58.000000 innerverz-0.0.34/setup.py
```

### Comparing `innerverz-0.0.33/LICENSE.txt` & `innerverz-0.0.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/__init__.py` & `innerverz-0.0.34/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/data_process/main.py` & `innerverz-0.0.34/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deblurrer/main.py` & `innerverz-0.0.34/innerverz/deblurrer/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,32 +5,14 @@
 import torch.nn.functional as F
 from torchvision import transforms
 from ..utils import check_ckpt_exist, convert_image_type, get_url_id
 from .nets import MyGenerator
 
 class DeBlurrer(nn.Module):
     def __init__(self, size=1024, folder_name='deblurrer', ckpt_name='G_1024_65000.pt', force=False, device='cuda'):
-        super(DeBlurrer, self).__init__()
-        self.device = device
-        self.size = size
-        url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
-        root = os.path.join('~/.invz_pack/', folder_name)
-        ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
-        ckpt = torch.load(ckpt_path, map_location=self.device)
-        
-        self.deblurrer = MyGenerator().to(self.device)
-        self.deblurrer.load_state_dict(ckpt['model'])
-        for param in self.deblurrer.parameters():
-            param.requires_grad = False
-        self.deblurrer.eval()
-        del ckpt
-        
-        self.dicts = {}
-
-    def forward(self, tensor_image, output_size=None):
         """
         Input
         ---------
             - dtype : tensor
             - shape : (1, 3, 1024, 1024)
             - min max : (-1, 1)
             
@@ -46,14 +28,32 @@
                 - shape : (1, 3, 1024, 1024)
                 - min max : (-1, 1)
             edge
                 - dtype : tensor
                 - shape : (1, 3, 1024, 1024)
                 - min max : (-1, 1)
         """
+        super(DeBlurrer, self).__init__()
+        self.device = device
+        self.size = size
+        url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
+        root = os.path.join('~/.invz_pack/', folder_name)
+        ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
+        ckpt = torch.load(ckpt_path, map_location=self.device)
+        
+        self.deblurrer = MyGenerator().to(self.device)
+        self.deblurrer.load_state_dict(ckpt['model'])
+        for param in self.deblurrer.parameters():
+            param.requires_grad = False
+        self.deblurrer.eval()
+        del ckpt
+        
+        self.dicts = {}
+
+    def forward(self, tensor_image, output_size=None):
         _, _, origin_h, origin_w = tensor_image.shape
         tensor_image = F.interpolate(tensor_image, (self.size, self.size), mode='bilinear')
         fake, fake_res, edge = self.deblurrer(tensor_image)
         if output_size == None:
             _fake = F.interpolate(fake, (origin_h, origin_w), mode='bilinear')
             _fake_res = F.interpolate(fake_res, (origin_h, origin_w), mode='bilinear')
             _edge = F.interpolate(edge, (origin_h, origin_w), mode='bilinear')
```

### Comparing `innerverz-0.0.33/innerverz/deblurrer/nets.py` & `innerverz-0.0.34/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deblurrer/test.py` & `innerverz-0.0.34/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/main.py` & `innerverz-0.0.34/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/FLAME.py` & `innerverz-0.0.34/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/decoders.py` & `innerverz-0.0.34/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/detectors.py` & `innerverz-0.0.34/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/encoders.py` & `innerverz-0.0.34/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.34/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/lbs.py` & `innerverz-0.0.34/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/models/resnet.py` & `innerverz-0.0.34/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/test.py` & `innerverz-0.0.34/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/cfg.py` & `innerverz-0.0.34/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.34/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/renderer.py` & `innerverz-0.0.34/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.34/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.34/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deca/utils/util.py` & `innerverz-0.0.34/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deep3dmm/main.py` & `innerverz-0.0.34/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deep3dmm/nets.py` & `innerverz-0.0.34/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/deep3dmm/test.py` & `innerverz-0.0.34/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.34/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/landmark.py` & `innerverz-0.0.34/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/main.py` & `innerverz-0.0.34/innerverz/face_alignment/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         - align_face_from_5
         - align_face_from_106
         - affine_transform
         
         Return
         --------
         dicts
-        '
         '''
         
         self.backbone = RetinaFace()
         self.lmk_detector = Landmark()
         self.size = size
         self.align_style = align_style
         if self.align_style == 'ffhq':
```

### Comparing `innerverz-0.0.33/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.34/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/test.py` & `innerverz-0.0.34/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.34/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.34/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/main.py` & `innerverz-0.0.34/innerverz/face_color_transfer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                     - shape : (b, 1, 512, 512)
                     - min max : (-1, 1)
                 - target_face_mask
                     - dtype : tensor
                     - shape : (b, 1, 512, 512)
                     - min max : (0 or 1)
                 
-            - Output
+            - Output : dict
                 - result
                     - shape : (1, 3, 512, 512)
                     - min max : (-1, 1)
                 - color reference map
                     - shape : (1, 3, 512, 512))
                     - min max : (-1, 1)
```

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.34/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.34/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_color_transfer/test.py` & `innerverz-0.0.34/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_enhancer/main.py` & `innerverz-0.0.34/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_enhancer/nets.py` & `innerverz-0.0.34/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_enhancer/test.py` & `innerverz-0.0.34/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/main.py` & `innerverz-0.0.34/innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.0.34/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.0.34/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/generators.py` & `innerverz-0.0.34/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/ops.py` & `innerverz-0.0.34/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.0.34/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.0.34/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/nets/utils.py` & `innerverz-0.0.34/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_matting/test.py` & `innerverz-0.0.34/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_parser/main.py` & `innerverz-0.0.34/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_parser/nets.py` & `innerverz-0.0.34/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/face_parser/test.py` & `innerverz-0.0.34/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/main.py` & `innerverz-0.0.34/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.34/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.34/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/head_color_transfer/test.py` & `innerverz-0.0.34/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/id_extractor/main.py` & `innerverz-0.0.34/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/id_extractor/nets.py` & `innerverz-0.0.34/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/id_extractor/test.py` & `innerverz-0.0.34/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/landmark_warping/main.py` & `innerverz-0.0.34/innerverz/landmark_warping/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch.nn as nn
 
 from .nets import MyGenerator
 from .util import set_random_colors, plot_kpts
 from ..utils import check_ckpt_exist, get_url_id
 
 class Landmark_Warping(nn.Module):
-    def __init__(self, img_size : int = 512, folder_name='landmark_warping', ckpt_name = 'G_13000.pt', force=False, device = 'cuda'):
+    def __init__(self, img_size : int = 512, folder_name='landmark_warping', ckpt_name = 'G_38k_unalign_multiaug.pt', force=False, device = 'cuda'):
         """
             Related Links
             --------
             https://meta-portrait.github.io/
             
             Options
             --------
```

### Comparing `innerverz-0.0.33/innerverz/landmark_warping/nets.py` & `innerverz-0.0.34/innerverz/landmark_warping/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/landmark_warping/test.py` & `innerverz-0.0.34/innerverz/landmark_warping/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/landmark_warping/util.py` & `innerverz-0.0.34/innerverz/landmark_warping/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/reage/main.py` & `innerverz-0.0.34/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/reage/net.py` & `innerverz-0.0.34/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/reage/net_utils.py` & `innerverz-0.0.34/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/reage/test.py` & `innerverz-0.0.34/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/relighter/main.py` & `innerverz-0.0.34/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/relighter/nets.py` & `innerverz-0.0.34/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/relighter/test.py` & `innerverz-0.0.34/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/upsampler/main.py` & `innerverz-0.0.34/innerverz/upsampler/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
         ---------
         - forward
             - input
                 - dtype : tensor
                 - shape : (b, 3, h, w)
                     - model is operated on 256*256 size, it will automactically resize
                 - min max : (0 1)
-            - output
-                dict
+            - output : dict
                 'result'
                     - dtype : tensor
                     - shape : (b 3 1024 1024)
                     - min max : (0 1)
         """
         
         super(Upsampler, self).__init__()
```

### Comparing `innerverz-0.0.33/innerverz/upsampler/nets.py` & `innerverz-0.0.34/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/upsampler/test.py` & `innerverz-0.0.34/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/utils/download.py` & `innerverz-0.0.34/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/utils/input.py` & `innerverz-0.0.34/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/utils/utils.py` & `innerverz-0.0.34/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/main.py` & `innerverz-0.0.34/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/nets.py` & `innerverz-0.0.34/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.34/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.34/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.34/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.34/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.34/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.33/setup.py` & `innerverz-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.33",
+    version="0.0.34",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

