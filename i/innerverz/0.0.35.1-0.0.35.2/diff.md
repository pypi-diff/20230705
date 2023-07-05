# Comparing `tmp/innerverz-0.0.35.1.tar.gz` & `tmp/innerverz-0.0.35.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.35.1.tar", last modified: Wed Jul  5 10:43:09 2023, max compression
+gzip compressed data, was "innerverz-0.0.35.2.tar", last modified: Wed Jul  5 10:49:05 2023, max compression
```

## Comparing `innerverz-0.0.35.1.tar` & `innerverz-0.0.35.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.669426 innerverz-0.0.35.1/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.35.1/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      196 2023-07-05 10:43:09.669525 innerverz-0.0.35.1/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.35.1/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.642627 innerverz-0.0.35.1/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1741 2023-07-05 10:37:06.000000 innerverz-0.0.35.1/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.643932 innerverz-0.0.35.1/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.0.35.1/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.644573 innerverz-0.0.35.1/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.0.35.1/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.645130 innerverz-0.0.35.1/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.0.35.1/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.646433 innerverz-0.0.35.1/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.35.1/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.647565 innerverz-0.0.35.1/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.648262 innerverz-0.0.35.1/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.0.35.1/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.648977 innerverz-0.0.35.1/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.0.35.1/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.649882 innerverz-0.0.35.1/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.0.35.1/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.650310 innerverz-0.0.35.1/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.650889 innerverz-0.0.35.1/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.651611 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.652208 innerverz-0.0.35.1/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.0.35.1/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.652657 innerverz-0.0.35.1/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.0.35.1/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8101 2023-07-04 12:20:23.000000 innerverz-0.0.35.1/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.653259 innerverz-0.0.35.1/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.653616 innerverz-0.0.35.1/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8178 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.654017 innerverz-0.0.35.1/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24825 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4325 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.654328 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.655148 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.0.35.1/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.0.35.1/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.655784 innerverz-0.0.35.1/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2908 2023-07-04 11:15:48.000000 innerverz-0.0.35.1/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.656858 innerverz-0.0.35.1/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5523 2023-07-05 10:29:48.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.659761 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.660504 innerverz-0.0.35.1/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.0.35.1/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.662432 innerverz-0.0.35.1/innerverz/landmark_warping/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-04 12:10:40.000000 innerverz-0.0.35.1/innerverz/landmark_warping/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3311 2023-07-05 10:15:15.000000 innerverz-0.0.35.1/innerverz/landmark_warping/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.663904 innerverz-0.0.35.1/innerverz/landmark_warping/nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.0.35.1/innerverz/landmark_warping/nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.0.35.1/innerverz/landmark_warping/nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2847 2023-07-04 10:48:50.000000 innerverz-0.0.35.1/innerverz/landmark_warping/nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.0.35.1/innerverz/landmark_warping/nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4240 2023-07-05 10:42:13.000000 innerverz-0.0.35.1/innerverz/landmark_warping/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.0.35.1/innerverz/landmark_warping/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.0.35.1/innerverz/landmark_warping/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.664630 innerverz-0.0.35.1/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.35.1/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.0.35.1/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.35.1/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.35.1/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.665208 innerverz-0.0.35.1/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.0.35.1/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.667017 innerverz-0.0.35.1/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.0.35.1/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.667787 innerverz-0.0.35.1/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.668387 innerverz-0.0.35.1/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.668527 innerverz-0.0.35.1/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.0.35.1/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.669274 innerverz-0.0.35.1/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.35.1/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:43:09.643585 innerverz-0.0.35.1/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      196 2023-07-05 10:43:09.000000 innerverz-0.0.35.1/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4760 2023-07-05 10:43:09.000000 innerverz-0.0.35.1/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-05 10:43:09.000000 innerverz-0.0.35.1/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-05 10:43:09.000000 innerverz-0.0.35.1/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-05 10:43:09.000000 innerverz-0.0.35.1/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.35.1/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-05 10:43:09.670629 innerverz-0.0.35.1/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      811 2023-07-05 10:43:01.000000 innerverz-0.0.35.1/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.207667 innerverz-0.0.35.2/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.35.2/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      196 2023-07-05 10:49:05.207754 innerverz-0.0.35.2/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.35.2/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.179598 innerverz-0.0.35.2/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1741 2023-07-05 10:37:06.000000 innerverz-0.0.35.2/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.180740 innerverz-0.0.35.2/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.0.35.2/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.181663 innerverz-0.0.35.2/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.0.35.2/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.182327 innerverz-0.0.35.2/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.0.35.2/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.183739 innerverz-0.0.35.2/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.35.2/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.186051 innerverz-0.0.35.2/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.186540 innerverz-0.0.35.2/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.0.35.2/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.187443 innerverz-0.0.35.2/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.0.35.2/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.189419 innerverz-0.0.35.2/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.0.35.2/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.189947 innerverz-0.0.35.2/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.190559 innerverz-0.0.35.2/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.192932 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.193811 innerverz-0.0.35.2/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.0.35.2/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.194376 innerverz-0.0.35.2/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.0.35.2/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8101 2023-07-04 12:20:23.000000 innerverz-0.0.35.2/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.196108 innerverz-0.0.35.2/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.196955 innerverz-0.0.35.2/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8178 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.197382 innerverz-0.0.35.2/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24825 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4325 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.197735 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.198636 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.0.35.2/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.0.35.2/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.199320 innerverz-0.0.35.2/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2908 2023-07-04 11:15:48.000000 innerverz-0.0.35.2/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.199985 innerverz-0.0.35.2/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5523 2023-07-05 10:29:48.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.200711 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.201322 innerverz-0.0.35.2/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.0.35.2/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.202114 innerverz-0.0.35.2/innerverz/landmark_warping/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-04 12:10:40.000000 innerverz-0.0.35.2/innerverz/landmark_warping/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3311 2023-07-05 10:15:15.000000 innerverz-0.0.35.2/innerverz/landmark_warping/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4240 2023-07-05 10:42:13.000000 innerverz-0.0.35.2/innerverz/landmark_warping/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.202727 innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2847 2023-07-04 10:48:50.000000 innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.0.35.2/innerverz/landmark_warping/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.0.35.2/innerverz/landmark_warping/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.203553 innerverz-0.0.35.2/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.35.2/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.0.35.2/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.35.2/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.35.2/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.204146 innerverz-0.0.35.2/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.0.35.2/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.204813 innerverz-0.0.35.2/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.0.35.2/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.205772 innerverz-0.0.35.2/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.206599 innerverz-0.0.35.2/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.206753 innerverz-0.0.35.2/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.0.35.2/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.207515 innerverz-0.0.35.2/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.35.2/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 10:49:05.180429 innerverz-0.0.35.2/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      196 2023-07-05 10:49:05.000000 innerverz-0.0.35.2/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4776 2023-07-05 10:49:05.000000 innerverz-0.0.35.2/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-05 10:49:05.000000 innerverz-0.0.35.2/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-05 10:49:05.000000 innerverz-0.0.35.2/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-05 10:49:05.000000 innerverz-0.0.35.2/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.35.2/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-05 10:49:05.208731 innerverz-0.0.35.2/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      811 2023-07-05 10:49:02.000000 innerverz-0.0.35.2/setup.py
```

### Comparing `innerverz-0.0.35.1/LICENSE.txt` & `innerverz-0.0.35.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/__init__.py` & `innerverz-0.0.35.2/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/data_process/main.py` & `innerverz-0.0.35.2/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deblurrer/main.py` & `innerverz-0.0.35.2/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deblurrer/nets.py` & `innerverz-0.0.35.2/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deblurrer/test.py` & `innerverz-0.0.35.2/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/main.py` & `innerverz-0.0.35.2/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/FLAME.py` & `innerverz-0.0.35.2/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/decoders.py` & `innerverz-0.0.35.2/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/detectors.py` & `innerverz-0.0.35.2/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/encoders.py` & `innerverz-0.0.35.2/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.35.2/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/lbs.py` & `innerverz-0.0.35.2/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/models/resnet.py` & `innerverz-0.0.35.2/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/test.py` & `innerverz-0.0.35.2/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/cfg.py` & `innerverz-0.0.35.2/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.35.2/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/renderer.py` & `innerverz-0.0.35.2/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.35.2/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.35.2/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deca/utils/util.py` & `innerverz-0.0.35.2/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deep3dmm/main.py` & `innerverz-0.0.35.2/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deep3dmm/nets.py` & `innerverz-0.0.35.2/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/deep3dmm/test.py` & `innerverz-0.0.35.2/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.35.2/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/landmark.py` & `innerverz-0.0.35.2/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/main.py` & `innerverz-0.0.35.2/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.35.2/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/test.py` & `innerverz-0.0.35.2/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.35.2/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.35.2/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/main.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_color_transfer/test.py` & `innerverz-0.0.35.2/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_enhancer/main.py` & `innerverz-0.0.35.2/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_enhancer/nets.py` & `innerverz-0.0.35.2/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_enhancer/test.py` & `innerverz-0.0.35.2/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/main.py` & `innerverz-0.0.35.2/innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/generators.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/ops.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/nets/utils.py` & `innerverz-0.0.35.2/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_matting/test.py` & `innerverz-0.0.35.2/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_parser/main.py` & `innerverz-0.0.35.2/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_parser/nets.py` & `innerverz-0.0.35.2/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/face_parser/test.py` & `innerverz-0.0.35.2/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/main.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/head_color_transfer/test.py` & `innerverz-0.0.35.2/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/id_extractor/main.py` & `innerverz-0.0.35.2/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/id_extractor/nets.py` & `innerverz-0.0.35.2/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/id_extractor/test.py` & `innerverz-0.0.35.2/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/main.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/nets/LadderEncoder.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/nets/dense_motion.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/nets/util.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/nets.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/test.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/landmark_warping/util.py` & `innerverz-0.0.35.2/innerverz/landmark_warping/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/reage/main.py` & `innerverz-0.0.35.2/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/reage/net.py` & `innerverz-0.0.35.2/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/reage/net_utils.py` & `innerverz-0.0.35.2/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/reage/test.py` & `innerverz-0.0.35.2/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/relighter/main.py` & `innerverz-0.0.35.2/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/relighter/nets.py` & `innerverz-0.0.35.2/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/relighter/test.py` & `innerverz-0.0.35.2/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/upsampler/main.py` & `innerverz-0.0.35.2/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/upsampler/nets.py` & `innerverz-0.0.35.2/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/upsampler/test.py` & `innerverz-0.0.35.2/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/utils/download.py` & `innerverz-0.0.35.2/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/utils/input.py` & `innerverz-0.0.35.2/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/utils/utils.py` & `innerverz-0.0.35.2/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/main.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/nets.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.35.2/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.35.1/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.35.2/innerverz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,18 +96,18 @@
 innerverz/id_extractor/nets.py
 innerverz/id_extractor/test.py
 innerverz/landmark_warping/__init__.py
 innerverz/landmark_warping/main.py
 innerverz/landmark_warping/nets.py
 innerverz/landmark_warping/test.py
 innerverz/landmark_warping/util.py
-innerverz/landmark_warping/nets/LadderEncoder.py
-innerverz/landmark_warping/nets/__init__.py
-innerverz/landmark_warping/nets/dense_motion.py
-innerverz/landmark_warping/nets/util.py
+innerverz/landmark_warping/sub_nets/LadderEncoder.py
+innerverz/landmark_warping/sub_nets/__init__.py
+innerverz/landmark_warping/sub_nets/dense_motion.py
+innerverz/landmark_warping/sub_nets/util.py
 innerverz/reage/__init__.py
 innerverz/reage/main.py
 innerverz/reage/net.py
 innerverz/reage/net_utils.py
 innerverz/reage/test.py
 innerverz/relighter/__init__.py
 innerverz/relighter/main.py
```

### Comparing `innerverz-0.0.35.1/setup.py` & `innerverz-0.0.35.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.35.1",
+    version="0.0.35.2",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

