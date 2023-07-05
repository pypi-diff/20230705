# Comparing `tmp/quickverifyimg-1.0.6.tar.gz` & `tmp/quickverifyimg-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickverifyimg-1.0.6.tar", last modified: Thu Jun 29 04:06:48 2023, max compression
+gzip compressed data, was "quickverifyimg-1.0.7.tar", last modified: Wed Jul  5 08:10:05 2023, max compression
```

## Comparing `quickverifyimg-1.0.6.tar` & `quickverifyimg-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.350533 quickverifyimg-1.0.6/
--rw-r--r--   0 yy         (501) staff       (20)     1060 2019-08-27 18:29:08.000000 quickverifyimg-1.0.6/LICENSE
--rw-r--r--   0 yy         (501) staff       (20)      212 2023-06-29 04:06:48.350227 quickverifyimg-1.0.6/PKG-INFO
--rw-r--r--   0 yy         (501) staff       (20)      175 2022-12-21 02:30:15.000000 quickverifyimg-1.0.6/README.md
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.328807 quickverifyimg-1.0.6/quickverifyimg/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-13 06:52:51.000000 quickverifyimg-1.0.6/quickverifyimg/__init__.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.335534 quickverifyimg-1.0.6/quickverifyimg/log/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-14 09:46:01.000000 quickverifyimg-1.0.6/quickverifyimg/log/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)      728 2022-11-16 08:12:52.000000 quickverifyimg-1.0.6/quickverifyimg/log/logger.py
--rw-r--r--   0 yy         (501) staff       (20)    11658 2023-06-29 02:41:15.000000 quickverifyimg-1.0.6/quickverifyimg/quick_verify.py
--rw-r--r--   0 yy         (501) staff       (20)    12076 2023-06-29 04:05:49.000000 quickverifyimg-1.0.6/quickverifyimg/quick_verify_simple.py
--rw-r--r--   0 yy         (501) staff       (20)    11953 2023-03-08 06:33:42.000000 quickverifyimg-1.0.6/quickverifyimg/quick_verify_video.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.344304 quickverifyimg-1.0.6/quickverifyimg/utils/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-12-15 06:27:15.000000 quickverifyimg-1.0.6/quickverifyimg/utils/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)     1167 2022-12-21 08:22:00.000000 quickverifyimg-1.0.6/quickverifyimg/utils/aircv_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     3598 2022-12-21 08:33:09.000000 quickverifyimg-1.0.6/quickverifyimg/utils/cv2_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     3130 2022-11-14 01:28:16.000000 quickverifyimg-1.0.6/quickverifyimg/utils/hash_utils.py
--rw-r--r--   0 yy         (501) staff       (20)     1952 2022-12-15 07:13:33.000000 quickverifyimg-1.0.6/quickverifyimg/utils/image_utils.py
--rw-r--r--   0 yy         (501) staff       (20)      856 2022-11-16 08:29:15.000000 quickverifyimg-1.0.6/quickverifyimg/utils/psnr.py
--rw-r--r--   0 yy         (501) staff       (20)      879 2022-12-16 06:14:51.000000 quickverifyimg-1.0.6/quickverifyimg/utils/thread_utils.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.333349 quickverifyimg-1.0.6/quickverifyimg.egg-info/
--rw-r--r--   0 yy         (501) staff       (20)      212 2023-06-29 04:06:48.000000 quickverifyimg-1.0.6/quickverifyimg.egg-info/PKG-INFO
--rw-r--r--   0 yy         (501) staff       (20)      738 2023-06-29 04:06:48.000000 quickverifyimg-1.0.6/quickverifyimg.egg-info/SOURCES.txt
--rw-r--r--   0 yy         (501) staff       (20)        1 2023-06-29 04:06:48.000000 quickverifyimg-1.0.6/quickverifyimg.egg-info/dependency_links.txt
--rw-r--r--   0 yy         (501) staff       (20)       51 2023-06-29 04:06:48.000000 quickverifyimg-1.0.6/quickverifyimg.egg-info/requires.txt
--rw-r--r--   0 yy         (501) staff       (20)       21 2023-06-29 04:06:48.000000 quickverifyimg-1.0.6/quickverifyimg.egg-info/top_level.txt
--rw-r--r--   0 yy         (501) staff       (20)       38 2023-06-29 04:06:48.350648 quickverifyimg-1.0.6/setup.cfg
--rw-r--r--   0 yy         (501) staff       (20)      826 2023-06-29 04:06:45.000000 quickverifyimg-1.0.6/setup.py
-drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-06-29 04:06:48.349375 quickverifyimg-1.0.6/tests/
--rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-16 07:13:08.000000 quickverifyimg-1.0.6/tests/__init__.py
--rw-r--r--   0 yy         (501) staff       (20)     4350 2022-12-23 10:36:53.000000 quickverifyimg-1.0.6/tests/analyze_memory.py
--rw-r--r--   0 yy         (501) staff       (20)     1969 2023-06-29 03:56:46.000000 quickverifyimg-1.0.6/tests/verify_test.py
--rw-r--r--   0 yy         (501) staff       (20)     1604 2022-12-22 07:03:15.000000 quickverifyimg-1.0.6/tests/verify_video_test.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.813320 quickverifyimg-1.0.7/
+-rw-r--r--   0 yy         (501) staff       (20)     1060 2019-08-27 18:29:08.000000 quickverifyimg-1.0.7/LICENSE
+-rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:10:05.812920 quickverifyimg-1.0.7/PKG-INFO
+-rw-r--r--   0 yy         (501) staff       (20)      175 2022-12-21 02:30:15.000000 quickverifyimg-1.0.7/README.md
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.779073 quickverifyimg-1.0.7/quickverifyimg/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-13 06:52:51.000000 quickverifyimg-1.0.7/quickverifyimg/__init__.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.787270 quickverifyimg-1.0.7/quickverifyimg/log/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-14 09:46:01.000000 quickverifyimg-1.0.7/quickverifyimg/log/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)      728 2022-11-16 08:12:52.000000 quickverifyimg-1.0.7/quickverifyimg/log/logger.py
+-rw-r--r--   0 yy         (501) staff       (20)    11658 2023-06-29 02:41:15.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify.py
+-rw-r--r--   0 yy         (501) staff       (20)    12076 2023-06-29 04:05:49.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify_simple.py
+-rw-r--r--   0 yy         (501) staff       (20)    11953 2023-03-08 06:33:42.000000 quickverifyimg-1.0.7/quickverifyimg/quick_verify_video.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.803498 quickverifyimg-1.0.7/quickverifyimg/utils/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-12-15 06:27:15.000000 quickverifyimg-1.0.7/quickverifyimg/utils/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)     1167 2022-12-21 08:22:00.000000 quickverifyimg-1.0.7/quickverifyimg/utils/aircv_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     3598 2022-12-21 08:33:09.000000 quickverifyimg-1.0.7/quickverifyimg/utils/cv2_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     3130 2022-11-14 01:28:16.000000 quickverifyimg-1.0.7/quickverifyimg/utils/hash_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)     2017 2023-07-05 08:00:18.000000 quickverifyimg-1.0.7/quickverifyimg/utils/image_utils.py
+-rw-r--r--   0 yy         (501) staff       (20)      856 2022-11-16 08:29:15.000000 quickverifyimg-1.0.7/quickverifyimg/utils/psnr.py
+-rw-r--r--   0 yy         (501) staff       (20)      879 2022-12-16 06:14:51.000000 quickverifyimg-1.0.7/quickverifyimg/utils/thread_utils.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.783565 quickverifyimg-1.0.7/quickverifyimg.egg-info/
+-rw-r--r--   0 yy         (501) staff       (20)      212 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/PKG-INFO
+-rw-r--r--   0 yy         (501) staff       (20)      738 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/SOURCES.txt
+-rw-r--r--   0 yy         (501) staff       (20)        1 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/dependency_links.txt
+-rw-r--r--   0 yy         (501) staff       (20)       51 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/requires.txt
+-rw-r--r--   0 yy         (501) staff       (20)       21 2023-07-05 08:10:05.000000 quickverifyimg-1.0.7/quickverifyimg.egg-info/top_level.txt
+-rw-r--r--   0 yy         (501) staff       (20)       38 2023-07-05 08:10:05.813475 quickverifyimg-1.0.7/setup.cfg
+-rw-r--r--   0 yy         (501) staff       (20)      826 2023-07-05 08:10:01.000000 quickverifyimg-1.0.7/setup.py
+drwxr-xr-x   0 yy         (501) staff       (20)        0 2023-07-05 08:10:05.812055 quickverifyimg-1.0.7/tests/
+-rw-r--r--   0 yy         (501) staff       (20)        0 2022-11-16 07:13:08.000000 quickverifyimg-1.0.7/tests/__init__.py
+-rw-r--r--   0 yy         (501) staff       (20)     4350 2022-12-23 10:36:53.000000 quickverifyimg-1.0.7/tests/analyze_memory.py
+-rw-r--r--   0 yy         (501) staff       (20)     1969 2023-06-29 03:56:46.000000 quickverifyimg-1.0.7/tests/verify_test.py
+-rw-r--r--   0 yy         (501) staff       (20)     1615 2023-07-05 08:08:23.000000 quickverifyimg-1.0.7/tests/verify_video_test.py
```

### Comparing `quickverifyimg-1.0.6/LICENSE` & `quickverifyimg-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/log/logger.py` & `quickverifyimg-1.0.7/quickverifyimg/log/logger.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/quick_verify.py` & `quickverifyimg-1.0.7/quickverifyimg/quick_verify.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/quick_verify_simple.py` & `quickverifyimg-1.0.7/quickverifyimg/quick_verify_simple.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/quick_verify_video.py` & `quickverifyimg-1.0.7/quickverifyimg/quick_verify_video.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/aircv_utils.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/aircv_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/cv2_utils.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/cv2_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/hash_utils.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/image_utils.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/image_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,10 +45,11 @@
         count = 1
         success, frame = cap.read()
         while success:
             frame_name = f"{count}.png"
             target_path = os.path.join(save_path, frame_name)
             if crop_region:
                 frame = crop_frame(frame, **crop_region)
-            cv2.imwrite(target_path, frame)
+            # cv2.imwrite(target_path, frame)
+            cv2.imencode(".png", frame)[1].tofile(target_path)
             success, frame = cap.read()
             count += 1
```

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/psnr.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/psnr.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg/utils/thread_utils.py` & `quickverifyimg-1.0.7/quickverifyimg/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/quickverifyimg.egg-info/SOURCES.txt` & `quickverifyimg-1.0.7/quickverifyimg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/setup.py` & `quickverifyimg-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Package meta-data.
 NAME = 'quickverifyimg'
 DESCRIPTION = 'quick verify img'
 URL = ''
 EMAIL = 'fengzhiyuan@yy.com'
 AUTHOR = 'Zhiyuan Feng'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 
 # Setting.
 def parse_requirements(filename):
     """ load requirements from a pip requirements file. (replacing from pip.req import parse_requirements)"""
     lineiter = (line.strip() for line in open(filename))
     reqs = [line for line in lineiter if line and not line.startswith("#")]
```

### Comparing `quickverifyimg-1.0.6/tests/analyze_memory.py` & `quickverifyimg-1.0.7/tests/analyze_memory.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/tests/verify_test.py` & `quickverifyimg-1.0.7/tests/verify_test.py`

 * *Files identical despite different names*

### Comparing `quickverifyimg-1.0.6/tests/verify_video_test.py` & `quickverifyimg-1.0.7/tests/verify_video_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 logger = get_logger(__name__)
 
 if __name__ == '__main__':
     """
     crop_place：{ size: 需要识别的区域的大小， 百分比, offset: 需要识别的区域的左上角坐标点位置， 百分比}
     quick_verify: 是否快速校验，即不对已校验过的对照集图片继续校验
     """
-    origin_video = "./images/video/origin_video.mp4"
-    target_video = "./images/video/target_video.mp4"
+    origin_video = "./images/video/20230705142724.mp4"
+    target_video = "./images/video/1001390-多巴胺女孩.mp4"
     crop_place = {"size": (0.48, 0.95), "offset": (0.13, 0)}
     # 选择使用的图片匹配算法和阈值
     # ac_tpl：模版匹配：大图找小图，速度快推荐
     # hist: 直方图匹配：速度一般，效果
     # ssim: ssim匹配算法：精准，速度不快，适合作为第二个算法补充
     # psnr: 峰值信噪比算法：目前只判断40以上为匹配，即认为相似度0.999
     # hash_p: 感知哈希算法：速度快，效果一般
     # hash_a: 均值哈希算法：速度快，效果一般
     # hash_d: 查值哈希算法：速度快，效果一般
     verify_engine_list = [
         ('ac_tpl', 0.99),
         ('hist', 0.995)
     ]
-    quick_v = QuickVerifyVideo(verify_engine_list, 0.8, crop_place=crop_place, background_similar=0.999)
+    quick_v = QuickVerifyVideo(verify_engine_list, 0.8, crop_place=crop_place, background_similar=1.1)
     ret = quick_v.verify_video_effect(origin_video, target_video)
     print(f"匹配结果：{ret['result']}")
     print(f"匹配失败图片：{ret['verify_fail_screenshots']}")
     print(f"整体成功率：{ret['final_match_rate']}")
```

