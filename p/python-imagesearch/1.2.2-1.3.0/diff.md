# Comparing `tmp/python-imagesearch-1.2.2.tar.gz` & `tmp/python-imagesearch-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-imagesearch-1.2.2.tar", last modified: Sat Feb 19 21:50:04 2022, max compression
+gzip compressed data, was "python-imagesearch-1.3.0.tar", last modified: Wed Jul  5 01:13:10 2023, max compression
```

## Comparing `python-imagesearch-1.2.2.tar` & `python-imagesearch-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2022-02-19 21:50:04.943812 python-imagesearch-1.2.2/
--rw-rw-r--   0 drov      (1000) drov      (1000)     1798 2022-02-19 21:50:04.943812 python-imagesearch-1.2.2/PKG-INFO
--rw-rw-r--   0 drov      (1000) drov      (1000)      994 2021-03-06 15:56:33.000000 python-imagesearch-1.2.2/README.md
-drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2022-02-19 21:50:04.943812 python-imagesearch-1.2.2/python_imagesearch/
--rw-r--r--   0 drov      (1000) drov      (1000)        0 2020-03-29 23:59:57.000000 python-imagesearch-1.2.2/python_imagesearch/__init__.py
--rw-rw-r--   0 drov      (1000) drov      (1000)     8877 2021-03-06 16:46:24.000000 python-imagesearch-1.2.2/python_imagesearch/imagesearch.py
-drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2022-02-19 21:50:04.943812 python-imagesearch-1.2.2/python_imagesearch.egg-info/
--rw-rw-r--   0 drov      (1000) drov      (1000)     1798 2022-02-19 21:50:04.000000 python-imagesearch-1.2.2/python_imagesearch.egg-info/PKG-INFO
--rw-rw-r--   0 drov      (1000) drov      (1000)      292 2022-02-19 21:50:04.000000 python-imagesearch-1.2.2/python_imagesearch.egg-info/SOURCES.txt
--rw-rw-r--   0 drov      (1000) drov      (1000)        1 2022-02-19 21:50:04.000000 python-imagesearch-1.2.2/python_imagesearch.egg-info/dependency_links.txt
--rw-rw-r--   0 drov      (1000) drov      (1000)       47 2022-02-19 21:50:04.000000 python-imagesearch-1.2.2/python_imagesearch.egg-info/requires.txt
--rw-rw-r--   0 drov      (1000) drov      (1000)       19 2022-02-19 21:50:04.000000 python-imagesearch-1.2.2/python_imagesearch.egg-info/top_level.txt
--rw-rw-r--   0 drov      (1000) drov      (1000)       38 2022-02-19 21:50:04.943812 python-imagesearch-1.2.2/setup.cfg
--rw-rw-r--   0 drov      (1000) drov      (1000)      767 2022-02-19 21:47:41.000000 python-imagesearch-1.2.2/setup.py
+drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2023-07-05 01:13:10.396861 python-imagesearch-1.3.0/
+-rw-rwxr--   0 drov      (1000) drov      (1000)     1062 2020-03-29 23:52:24.000000 python-imagesearch-1.3.0/LICENSE
+-rw-rw-r--   0 drov      (1000) drov      (1000)     1497 2023-07-05 01:13:10.396861 python-imagesearch-1.3.0/PKG-INFO
+-rw-rwxr--   0 drov      (1000) drov      (1000)      994 2021-03-06 15:56:33.000000 python-imagesearch-1.3.0/README.md
+drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2023-07-05 01:13:10.396861 python-imagesearch-1.3.0/python_imagesearch/
+-rw-rwxr--   0 drov      (1000) drov      (1000)        0 2020-03-29 23:59:57.000000 python-imagesearch-1.3.0/python_imagesearch/__init__.py
+-rw-rw-r--   0 drov      (1000) drov      (1000)    10794 2023-07-05 01:09:59.000000 python-imagesearch-1.3.0/python_imagesearch/imagesearch.py
+drwxrwxr-x   0 drov      (1000) drov      (1000)        0 2023-07-05 01:13:10.396861 python-imagesearch-1.3.0/python_imagesearch.egg-info/
+-rw-rwxr--   0 drov      (1000) drov      (1000)     1497 2023-07-05 01:13:10.000000 python-imagesearch-1.3.0/python_imagesearch.egg-info/PKG-INFO
+-rw-rwxr--   0 drov      (1000) drov      (1000)      300 2023-07-05 01:13:10.000000 python-imagesearch-1.3.0/python_imagesearch.egg-info/SOURCES.txt
+-rw-rwxr--   0 drov      (1000) drov      (1000)        1 2023-07-05 01:13:10.000000 python-imagesearch-1.3.0/python_imagesearch.egg-info/dependency_links.txt
+-rw-rwxr--   0 drov      (1000) drov      (1000)       47 2023-07-05 01:13:10.000000 python-imagesearch-1.3.0/python_imagesearch.egg-info/requires.txt
+-rw-rwxr--   0 drov      (1000) drov      (1000)       19 2023-07-05 01:13:10.000000 python-imagesearch-1.3.0/python_imagesearch.egg-info/top_level.txt
+-rw-rw-r--   0 drov      (1000) drov      (1000)       38 2023-07-05 01:13:10.396861 python-imagesearch-1.3.0/setup.cfg
+-rw-rwxr--   0 drov      (1000) drov      (1000)      767 2023-07-05 01:12:28.000000 python-imagesearch-1.3.0/setup.py
```

### Comparing `python-imagesearch-1.2.2/README.md` & `python-imagesearch-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-imagesearch-1.2.2/python_imagesearch/imagesearch.py` & `python-imagesearch-1.3.0/python_imagesearch/imagesearch.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import platform
 import subprocess
 import os
 import mss
 
 is_retina = False
 if platform.system() == "Darwin":
-    is_retina = subprocess.call("system_profiler SPDisplaysDataType | grep 'retina'", shell=True) == 0
+    is_retina = subprocess.call("system_profiler SPDisplaysDataType | grep -i 'retina'", shell=True) == 0
 
 '''
 
 grabs a region (topx, topy, bottomx, bottomy)
 to the tuple (topx, topy, width, height)
 
 input : a tuple containing the 4 coordinates of the region to capture
@@ -212,14 +212,45 @@
     while pos[0] == -1:
         time.sleep(timesample)
         pos = imagesearcharea(image, x1, y1, x2, y2, precision)
     return pos
 
 
 '''
+Searchs for an image on a region of the screen continuously until it's found or max number of samples reached.
+
+input :
+image : path to the image file (see opencv imread for supported types)
+time : Waiting time after failing to find the image
+maxSamples: maximum number of samples before function times out.
+x1 : top left x value
+y1 : top left y value
+x2 : bottom right x value
+y2 : bottom right y value
+precision : the higher, the lesser tolerant and fewer false positives are found default is 0.8
+
+returns :
+the top left corner coordinates of the element as an array [x,y]
+'''
+
+
+def imagesearch_region_numLoop(image, timesample, maxSamples, x1, y1, x2, y2, precision=0.8):
+    pos = imagesearcharea(image, x1, y1, x2, y2, precision)
+    count = 0
+    while pos[0] == -1:
+        time.sleep(timesample)
+        pos = imagesearcharea(image, x1, y1, x2, y2, precision)
+        count = count + 1
+        if count > maxSamples:
+            break
+    return pos
+
+
+
+'''
 Searches for an image on the screen and counts the number of occurrences.
 
 input :
 image : path to the target image file (see opencv imread for supported types)
 precision : the higher, the lesser tolerant and fewer false positives are found default is 0.9
 
 returns :
@@ -270,7 +301,29 @@
         pos = imagesearch(path+file, precision)
         imagesPos[path+file] = pos
     return imagesPos
 
 
 def r(num, rand):
     return num + rand * random.random()
+
+'''
+Wrapper around imagesearch and click_image
+
+# TODO: optimize so that we only read the file once.
+
+input :
+image : path to the image file (see opencv imread for supported types)
+action : button of the mouse to activate : "left" "right" "middle", see pyautogui.click documentation for more info
+delay : time taken for the mouse to move from where it was to the new position
+precision : the higher, the lesser tolerant and fewer false positives are found default is 0.8
+'''
+
+def imagesearch_click(image, action, delay, offset=5, precision=0.8):
+    pos = imagesearch(image, precision)
+    img = cv2.imread(image)
+    if img is None:
+        raise FileNotFoundError('Image file not found: {}'.format(image))
+    height, width, channels = img.shape
+    pyautogui.moveTo(pos[0] + r(width / 2, offset), pos[1] + r(height / 2, offset),
+                     delay)
+    pyautogui.click(button=action)
```

### Comparing `python-imagesearch-1.2.2/setup.py` & `python-imagesearch-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-imagesearch",
-    version="1.2.2",
+    version="1.3.0",
     install_requires=['opencv-python', 'numpy', 'python3_xlib', 'pyautogui', 'mss'],
     author="Martin Lees",
     author_email="drov.fr@protonmail.com",
     description="A wrapper around openCv to perform image searching",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drov0/python-imagesearch",
```

