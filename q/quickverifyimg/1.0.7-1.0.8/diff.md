# Comparing `tmp/quickverifyimg-1.0.7.tar.gz` & `tmp/quickverifyimg-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickverifyimg-1.0.7.tar", last modified: Wed Jul  5 08:10:05 2023, max compression
+gzip compressed data, was "quickverifyimg-1.0.8.tar", last modified: Wed Jul  5 08:31:14 2023, max compression
```

## Comparing `quickverifyimg-1.0.7.tar` & `quickverifyimg-1.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.813320 quickverifyimg-1.0.7/
--rw-r--r--   0 yy         (501) staff       (20)     1060 2019-08-27 18:29:08.000000 quickverifyimg-1.0.7/LICENSE
--rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:10:05.812920 quickverifyimg-1.0.7/PKG-INFO
--rw-r--r--   0 yy         (501) staff       (20)      175 2022-12-21 02:30:15.000000 quickverifyimg-1.0.7/README.md
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.779073 quickverifyimg-1.0.7/quickverifyimg/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-13 06:52:51.000000 quickverifyimg-1.0.7/quickverifyimg/__init__.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.787270 quickverifyimg-1.0.7/quickverifyimg/log/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-14 09:46:01.000000 quickverifyimg-1.0.7/quickverifyimg/log/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)      728 2022-11-16 08:12:52.000000 quickverifyimg-1.0.7/quickverifyimg/log/logger.py
--rw-r--r--   0 yy         (501) staff       (20)    11658 2023-06-29 02:41:15.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify.py
--rw-r--r--   0 yy         (501) staff       (20)    12076 2023-06-29 04:05:49.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify_simple.py
--rw-r--r--   0 yy         (501) staff       (20)    11953 2023-03-08 06:33:42.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify_video.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.803498 quickverifyimg-1.0.7/quickverifyimg/utils/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-12-15 06:27:15.000000 quickverifyimg-1.0.7/quickverifyimg/utils/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)     1167 2022-12-21 08:22:00.000000 quickverifyimg-1.0.7/quickverifyimg/utils/aircv_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     3598 2022-12-21 08:33:09.000000 quickverifyimg-1.0.7/quickverifyimg/utils/cv2_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     3130 2022-11-14 01:28:16.000000 quickverifyimg-1.0.7/quickverifyimg/utils/hash_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     2017 2023-07-05 08:00:18.000000 quickverifyimg-1.0.7/quickverifyimg/utils/image_utils.py
--rw-r--r--   0 yy         (501) staff       (20)      856 2022-11-16 08:29:15.000000 quickverifyimg-1.0.7/quickverifyimg/utils/psnr.py
--rw-r--r--   0 yy         (501) staff       (20)      879 2022-12-16 06:14:51.000000 quickverifyimg-1.0.7/quickverifyimg/utils/thread_utils.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.783565 quickverifyimg-1.0.7/quickverifyimg.egg-info/
--rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/PKG-INFO
--rw-r--r--   0 yy         (501) staff       (20)      738 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/SOURCES.txt
--rw-r--r--   0 yy         (501) staff       (20)        1 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/dependency_links.txt
--rw-r--r--   0 yy         (501) staff       (20)       51 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/requires.txt
--rw-r--r--   0 yy         (501) staff       (20)       21 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/top_level.txt
--rw-r--r--   0 yy         (501) staff       (20)       38 2023-07-05 08:10:05.813475 quickverifyimg-1.0.7/setup.cfg
--rw-r--r--   0 yy         (501) staff       (20)      826 2023-07-05 08:10:01.000000 quickverifyimg-1.0.7/setup.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.812055 quickverifyimg-1.0.7/tests/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-16 07:13:08.000000 quickverifyimg-1.0.7/tests/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)     4350 2022-12-23 10:36:53.000000 quickverifyimg-1.0.7/tests/analyze_memory.py
--rw-r--r--   0 yy         (501) staff       (20)     1969 2023-06-29 03:56:46.000000 quickverifyimg-1.0.7/tests/verify_test.py
--rw-r--r--   0 yy         (501) staff       (20)     1615 2023-07-05 08:08:23.000000 quickverifyimg-1.0.7/tests/verify_video_test.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:14.016357 quickverifyimg-1.0.8/
+-rw-r--r--   0 yy         (501) staff       (20)     1060 2019-08-27 18:29:08.000000 quickverifyimg-1.0.8/LICENSE
+-rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:31:14.015724 quickverifyimg-1.0.8/PKG-INFO
+-rw-r--r--   0 yy         (501) staff       (20)      175 2022-12-21 02:30:15.000000 quickverifyimg-1.0.8/README.md
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:13.973899 quickverifyimg-1.0.8/quickverifyimg/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-13 06:52:51.000000 quickverifyimg-1.0.8/quickverifyimg/__init__.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:13.984190 quickverifyimg-1.0.8/quickverifyimg/log/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-14 09:46:01.000000 quickverifyimg-1.0.8/quickverifyimg/log/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)      728 2022-11-16 08:12:52.000000 quickverifyimg-1.0.8/quickverifyimg/log/logger.py
+-rw-r--r--   0 yy         (501) staff       (20)    11658 2023-06-29 02:41:15.000000 quickverifyimg-1.0.8/quickverifyimg/quick_verify.py
+-rw-r--r--   0 yy         (501) staff       (20)    12076 2023-06-29 04:05:49.000000 quickverifyimg-1.0.8/quickverifyimg/quick_verify_simple.py
+-rw-r--r--   0 yy         (501) staff       (20)    11959 2023-07-05 08:26:53.000000 quickverifyimg-1.0.8/quickverifyimg/quick_verify_video.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:14.003735 quickverifyimg-1.0.8/quickverifyimg/utils/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-12-15 06:27:15.000000 quickverifyimg-1.0.8/quickverifyimg/utils/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)     1167 2022-12-21 08:22:00.000000 quickverifyimg-1.0.8/quickverifyimg/utils/aircv_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     3598 2022-12-21 08:33:09.000000 quickverifyimg-1.0.8/quickverifyimg/utils/cv2_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     3130 2022-11-14 01:28:16.000000 quickverifyimg-1.0.8/quickverifyimg/utils/hash_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     2471 2023-07-05 08:26:53.000000 quickverifyimg-1.0.8/quickverifyimg/utils/image_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)      856 2022-11-16 08:29:15.000000 quickverifyimg-1.0.8/quickverifyimg/utils/psnr.py
+-rw-r--r--   0 yy         (501) staff       (20)      879 2022-12-16 06:14:51.000000 quickverifyimg-1.0.8/quickverifyimg/utils/thread_utils.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:13.979248 quickverifyimg-1.0.8/quickverifyimg.egg-info/
+-rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:31:13.000000 quickverifyimg-1.0.8/quickverifyimg.egg-info/PKG-INFO
+-rw-r--r--   0 yy         (501) staff       (20)      738 2023-07-05 08:31:13.000000 quickverifyimg-1.0.8/quickverifyimg.egg-info/SOURCES.txt
+-rw-r--r--   0 yy         (501) staff       (20)        1 2023-07-05 08:31:13.000000 quickverifyimg-1.0.8/quickverifyimg.egg-info/dependency_links.txt
+-rw-r--r--   0 yy         (501) staff       (20)       51 2023-07-05 08:31:13.000000 quickverifyimg-1.0.8/quickverifyimg.egg-info/requires.txt
+-rw-r--r--   0 yy         (501) staff       (20)       21 2023-07-05 08:31:13.000000 quickverifyimg-1.0.8/quickverifyimg.egg-info/top_level.txt
+-rw-r--r--   0 yy         (501) staff       (20)       38 2023-07-05 08:31:14.016645 quickverifyimg-1.0.8/setup.cfg
+-rw-r--r--   0 yy         (501) staff       (20)      826 2023-07-05 08:31:10.000000 quickverifyimg-1.0.8/setup.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:31:14.014212 quickverifyimg-1.0.8/tests/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-16 07:13:08.000000 quickverifyimg-1.0.8/tests/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)     4350 2022-12-23 10:36:53.000000 quickverifyimg-1.0.8/tests/analyze_memory.py
+-rw-r--r--   0 yy         (501) staff       (20)     1969 2023-06-29 03:56:46.000000 quickverifyimg-1.0.8/tests/verify_test.py
+-rw-r--r--   0 yy         (501) staff       (20)     1615 2023-07-05 08:08:23.000000 quickverifyimg-1.0.8/tests/verify_video_test.py
```

### Comparing `quickverifyimg-1.0.7/LICENSE` & `quickverifyimg-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/log/logger.py` & `quickverifyimg-1.0.8/quickverifyimg/log/logger.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/quick_verify.py` & `quickverifyimg-1.0.8/quickverifyimg/quick_verify.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/quick_verify_simple.py` & `quickverifyimg-1.0.8/quickverifyimg/quick_verify_simple.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/quick_verify_video.py` & `quickverifyimg-1.0.8/quickverifyimg/quick_verify_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import copy
 
 from quickverifyimg.log.logger import get_logger
 from quickverifyimg.utils.aircv_utils import match_image
 from quickverifyimg.utils.cv2_utils import compare_hist, ssim
 from quickverifyimg.utils.hash_utils import getHash_similarity_p, getHash_similarity_d, getHash_similarity_a
-from quickverifyimg.utils.image_utils import crop_frame, extract_video_frame
+from quickverifyimg.utils.image_utils import crop_frame, extract_video_frame, cv_imread
 from quickverifyimg.utils.psnr import get_psnr_similar
 from quickverifyimg.utils.thread_utils import MyThread
 logger = get_logger(__name__)
 
 switcher = {
     'ac_tpl': match_image,
     'hist': compare_hist,
@@ -45,15 +45,15 @@
         self.match_rate_threshold = match_rate_threshold
         self.offset_size = offset_size
         self.background_similar = background_similar
         # 默认背景帧
         self.background_path = background_path
         self.background_img = None
         if self.background_path:
-            self.background_img = cv2.imread(self.background_path)
+            self.background_img = cv_imread(self.background_path)
             self.background_img = crop_frame(self.background_img, **crop_place)
         # 排除掉背景图的帧列表
         self.origin_frame_img = []
         self.target_frame_img = []
 
 
     def verify_video_effect(self, origin_video_path, target_video_path, img_threshold = 10):
@@ -141,21 +141,21 @@
         return ret
 
 
     def _analyse_origin_frame(self, video_frame_path=""):
         all_effect_frame_save_dir_list = os.listdir(video_frame_path)
         all_effect_frame_save_dir_list.sort(key=lambda x: int(x[:-4]) if x[:-4].isdigit() else x[:-4])  # 去掉后缀名来排序
         # 默认设置第一帧为背景图
-        background_img = cv2.imread(os.path.join(video_frame_path, all_effect_frame_save_dir_list[0]))
+        background_img = cv_imread(os.path.join(video_frame_path, all_effect_frame_save_dir_list[0]))
 
         def analyse_frame(all_list_temp, background_img, verify_engine_list):
             img_list = []
             for image_name in all_list_temp:
                 img_path = os.path.join(video_frame_path, image_name)
-                img = cv2.imread(img_path)
+                img = cv_imread(img_path)
                 is_background, best_similar, best_engine = self._is_image_similar(img, background_img, verify_engine_list, is_background=True)
                 if not is_background:
                     img_list.append(img_path)
             return img_list
 
         img_threshold = 50
         thread_list = []
@@ -201,25 +201,25 @@
         :param verify_img_index: 对照图片集开始顺序
         :return:
         """
         cut_match_index = -1
         match_times = 0  # 跟verify_images_dir对比，相似度超过阈值的图片数量
         verify_fail_screenshots = []
         for img_path in img_list:
-            img = cv2.imread(img_path)
+            img = cv_imread(img_path)
             best_matching_name = ''
             best_matching_similar = 0
             best_matching_engine = ''
             verify_images = self.origin_frame_img[verify_img_index:len(self.origin_frame_img)]
             tmp_verify_images = copy.deepcopy(verify_images)
             for index, verify_img_path in enumerate(verify_images):
                 # 因为截图和校验图都是连续的，所以如果有校验通过了的校验图，下次校验时可以跳过此次之前的图片
                 if self.quick_verify and index <= cut_match_index:
                     continue
-                verify_img = cv2.imread(verify_img_path)
+                verify_img = cv_imread(verify_img_path)
                 is_similar, similar, engine = self._is_image_similar(img, verify_img, verify_engine_list)
                 if is_similar:
                     logger.debug(f"目标帧: {os.path.basename(img_path)} match 源视频帧：{os.path.basename(verify_img_path)}, similiar: {similar} , engine_type :{engine}")
                     if not self.quick_verify:
                         tmp_verify_images.pop(index)
                     cut_match_index = index
                     match_times += 1
```

### Comparing `quickverifyimg-1.0.7/quickverifyimg/utils/aircv_utils.py` & `quickverifyimg-1.0.8/quickverifyimg/utils/aircv_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/utils/cv2_utils.py` & `quickverifyimg-1.0.8/quickverifyimg/utils/cv2_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/utils/hash_utils.py` & `quickverifyimg-1.0.8/quickverifyimg/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/utils/psnr.py` & `quickverifyimg-1.0.8/quickverifyimg/utils/psnr.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg/utils/thread_utils.py` & `quickverifyimg-1.0.8/quickverifyimg/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/quickverifyimg.egg-info/SOURCES.txt` & `quickverifyimg-1.0.8/quickverifyimg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/setup.py` & `quickverifyimg-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Package meta-data.
 NAME = 'quickverifyimg'
 DESCRIPTION = 'quick verify img'
 URL = ''
 EMAIL = 'fengzhiyuan@yy.com'
 AUTHOR = 'Zhiyuan Feng'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 
 
 # Setting.
 def parse_requirements(filename):
     """ load requirements from a pip requirements file. (replacing from pip.req import parse_requirements)"""
     lineiter = (line.strip() for line in open(filename))
     reqs = [line for line in lineiter if line and not line.startswith("#")]
```

### Comparing `quickverifyimg-1.0.7/tests/analyze_memory.py` & `quickverifyimg-1.0.8/tests/analyze_memory.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/tests/verify_test.py` & `quickverifyimg-1.0.8/tests/verify_test.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.7/tests/verify_video_test.py` & `quickverifyimg-1.0.8/tests/verify_video_test.py`

 * *Files identical despite different names*

