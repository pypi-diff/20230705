# Comparing `tmp/google-cloud-vision-3.4.3.tar.gz` & `tmp/google-cloud-vision-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vision-3.4.3.tar", last modified: Tue Jun 20 15:29:37 2023, max compression
+gzip compressed data, was "google-cloud-vision-3.4.4.tar", last modified: Wed Jul  5 15:30:19 2023, max compression
```

## Comparing `google-cloud-vision-3.4.3.tar` & `google-cloud-vision-3.4.4.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5795 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4882 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.762554 google-cloud-vision-3.4.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.762554 google-cloud-vision-3.4.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision/
--rw-rw-r--   0 root         (0)     1003    10158 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_helpers/
--rw-rw-r--   0 root         (0)     1003     3638 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_helpers/__init__.py
--rw-rw-r--   0 root         (0)     1003     4181 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_helpers/decorators.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/
--rw-rw-r--   0 root         (0)     1003     8417 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10150 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.766553 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    30191 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39070 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9543 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17763 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18097 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    33053 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110841 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   118546 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    21786 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.770551 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22251 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41006 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41751 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106831 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/
--rw-rw-r--   0 root         (0)     1003     5104 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3163 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    57369 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8095 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34296 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14108 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6798 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     3530 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1073 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    13774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    22022 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6594 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12086 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12291 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12849 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.774550 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2054 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2372 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    36850 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    13946 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003     4513 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1505 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19293 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    27363 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7741 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14438 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14719 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/
--rw-rw-r--   0 root         (0)     1003     2684 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    47056 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003     7754 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8961 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.778549 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19480 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    28835 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7602 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14454 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14735 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   104793 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   113091 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.782548 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21005 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39061 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    39775 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   100971 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/
--rw-rw-r--   0 root         (0)     1003     4658 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    49756 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    31431 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003     8625 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10164 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    29872 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39259 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.786547 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9001 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17798 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18132 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30869 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110849 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   119297 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21446 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41195 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41940 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106302 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.790545 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/
--rw-rw-r--   0 root         (0)     1003     5270 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2803 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/face.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    56382 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34408 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6861 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/
--rw-r--r--   0 root         (0)     1003     5795 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     8892 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-20 15:29:37.000000 google-cloud-vision-3.4.3/google_cloud_vision.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-20 15:29:37.802542 google-cloud-vision-3.4.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2917 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/data/
--rw-rw-r--   0 root         (0)     1003   283497 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/faces.jpg
--rw-rw-r--   0 root         (0)     1003    21568 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/logo.png
--rw-rw-r--   0 root         (0)     1003    15615 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/data/pdf_test.pdf
--rw-rw-r--   0 root         (0)     1003    38159 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.794544 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   127996 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   460770 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    70208 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    90057 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    91693 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   443181 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 15:29:37.798543 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   128156 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   461030 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
--rw-rw-r--   0 root         (0)     1003     4068 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/test_decorators.py
--rw-rw-r--   0 root         (0)     1003     5105 2023-06-20 15:27:08.000000 google-cloud-vision-3.4.3/tests/unit/test_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.406167 google-cloud-vision-3.4.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5795 2023-07-05 15:30:19.406167 google-cloud-vision-3.4.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4882 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.362164 google-cloud-vision-3.4.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.366164 google-cloud-vision-3.4.4/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.370164 google-cloud-vision-3.4.4/google/cloud/vision/
+-rw-rw-r--   0 root         (0)     1003    10158 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.370164 google-cloud-vision-3.4.4/google/cloud/vision_helpers/
+-rw-rw-r--   0 root         (0)     1003     3638 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_helpers/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4181 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_helpers/decorators.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.370164 google-cloud-vision-3.4.4/google/cloud/vision_v1/
+-rw-rw-r--   0 root         (0)     1003     8417 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10150 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.370164 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.370164 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30222 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39070 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.374165 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9543 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17763 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18097 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    33053 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.374165 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110871 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   118546 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    21786 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.378165 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22251 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41006 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41751 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106831 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.378165 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5104 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3163 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    57369 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8095 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34296 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14108 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6798 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.378165 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     3530 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1073 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.378165 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.378165 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13805 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22022 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6594 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12086 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12291 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12849 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2054 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2372 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    36850 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    13946 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003     4513 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1505 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19324 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27363 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.382165 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7741 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14438 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14719 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.386166 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2684 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    47056 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.386166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003     7754 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8961 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.386166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.386166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19511 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28835 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.386166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7602 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14454 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14735 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.390166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104823 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   113091 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.390166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21005 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39061 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    39775 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   100971 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.390166 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/
+-rw-rw-r--   0 root         (0)     1003     4658 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    49756 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    31431 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.390166 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003     8625 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10164 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.394166 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.394166 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29903 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39259 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.394166 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9001 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17798 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18132 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30869 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.394166 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110879 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   119297 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.398167 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21446 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41195 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41940 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106302 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.398167 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/
+-rw-rw-r--   0 root         (0)     1003     5270 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2803 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/face.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    56382 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34408 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6861 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.398167 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/
+-rw-r--r--   0 root         (0)     1003     5795 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     8892 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:30:19.000000 google-cloud-vision-3.4.4/google_cloud_vision.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:30:19.406167 google-cloud-vision-3.4.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2917 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.398167 google-cloud-vision-3.4.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/data/
+-rw-rw-r--   0 root         (0)     1003   283497 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/data/faces.jpg
+-rw-rw-r--   0 root         (0)     1003    21568 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/data/logo.png
+-rw-rw-r--   0 root         (0)     1003    15615 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/data/pdf_test.pdf
+-rw-rw-r--   0 root         (0)     1003    38159 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   127996 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   461566 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    70208 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.402167 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    90057 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.406167 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91693 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   443977 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:30:19.406167 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   128156 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   461826 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
+-rw-rw-r--   0 root         (0)     1003     4068 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/test_decorators.py
+-rw-rw-r--   0 root         (0)     1003     5105 2023-07-05 15:27:10.000000 google-cloud-vision-3.4.4/tests/unit/test_helpers.py
```

### Comparing `google-cloud-vision-3.4.3/LICENSE` & `google-cloud-vision-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/MANIFEST.in` & `google-cloud-vision-3.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/PKG-INFO` & `google-cloud-vision-3.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.3
+Version: 3.4.4
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vision-3.4.3/README.rst` & `google-cloud-vision-3.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_helpers/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_helpers/decorators.py` & `google-cloud-vision-3.4.4/google/cloud/vision_helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_metadata.json` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,15 +716,15 @@
             image_annotator.AsyncBatchAnnotateFilesResponse,
             metadata_type=image_annotator.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ImageAnnotatorAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2739,15 +2739,15 @@
             empty_pb2.Empty,
             metadata_type=product_search_service.BatchOperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ProductSearchAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/pagers.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/geometry.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/image_annotator.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/product_search_service.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/text_annotation.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1/types/web_detection.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_metadata.json` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ImageAnnotatorAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/geometry.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/image_annotator.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/text_annotation.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p1beta1/types/web_detection.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p1beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_metadata.json` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,15 +453,15 @@
             image_annotator.AsyncBatchAnnotateFilesResponse,
             metadata_type=image_annotator.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ImageAnnotatorAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/geometry.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/image_annotator.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/text_annotation.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p2beta1/types/web_detection.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p2beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_metadata.json` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,15 +454,15 @@
             image_annotator.AsyncBatchAnnotateFilesResponse,
             metadata_type=image_annotator.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ImageAnnotatorAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2588,15 +2588,15 @@
             product_search_service.ImportProductSetsResponse,
             metadata_type=product_search_service.BatchOperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ProductSearchAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/geometry.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/image_annotator.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/product_search_service.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/text_annotation.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p3beta1/types/web_detection.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p3beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_metadata.json` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/gapic_version.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.3"  # {x-release-please-version}
+__version__ = "3.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
             image_annotator.AsyncBatchAnnotateFilesResponse,
             metadata_type=image_annotator.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ImageAnnotatorAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2724,15 +2724,15 @@
             empty_pb2.Empty,
             metadata_type=product_search_service.BatchOperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ProductSearchAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/client.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/__init__.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/face.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/face.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/geometry.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/image_annotator.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/product_search_service.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/text_annotation.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google/cloud/vision_v1p4beta1/types/web_detection.py` & `google-cloud-vision-3.4.4/google/cloud/vision_v1p4beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/google_cloud_vision.egg-info/PKG-INFO` & `google-cloud-vision-3.4.4/google_cloud_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.3
+Version: 3.4.4
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vision-3.4.3/google_cloud_vision.egg-info/SOURCES.txt` & `google-cloud-vision-3.4.4/google_cloud_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/setup.py` & `google-cloud-vision-3.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/__init__.py` & `google-cloud-vision-3.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/data/faces.jpg` & `google-cloud-vision-3.4.4/tests/data/faces.jpg`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/data/logo.png` & `google-cloud-vision-3.4.4/tests/data/logo.png`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/data/pdf_test.pdf` & `google-cloud-vision-3.4.4/tests/data/pdf_test.pdf`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/system.py` & `google-cloud-vision-3.4.4/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_image_annotator.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1/test_product_search.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1/test_product_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1420,17 +1420,19 @@
                     product_search_service.ProductSet(),
                     product_search_service.ProductSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_product_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2839,17 +2841,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4517,17 +4521,19 @@
                     product_search_service.ReferenceImage(),
                     product_search_service.ReferenceImage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_reference_images(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5701,17 +5707,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products_in_product_set(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p3beta1/test_product_search.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p3beta1/test_product_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1421,17 +1421,19 @@
                     product_search_service.ProductSet(),
                     product_search_service.ProductSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_product_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2840,17 +2842,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4518,17 +4522,19 @@
                     product_search_service.ReferenceImage(),
                     product_search_service.ReferenceImage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_reference_images(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5702,17 +5708,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products_in_product_set(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/gapic/vision_v1p4beta1/test_product_search.py` & `google-cloud-vision-3.4.4/tests/unit/gapic/vision_v1p4beta1/test_product_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,17 +1422,19 @@
                     product_search_service.ProductSet(),
                     product_search_service.ProductSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_product_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2841,17 +2843,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4519,17 +4523,19 @@
                     product_search_service.ReferenceImage(),
                     product_search_service.ReferenceImage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_reference_images(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5703,17 +5709,19 @@
                     product_search_service.Product(),
                     product_search_service.Product(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_products_in_product_set(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-vision-3.4.3/tests/unit/test_decorators.py` & `google-cloud-vision-3.4.4/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.3/tests/unit/test_helpers.py` & `google-cloud-vision-3.4.4/tests/unit/test_helpers.py`

 * *Files identical despite different names*

