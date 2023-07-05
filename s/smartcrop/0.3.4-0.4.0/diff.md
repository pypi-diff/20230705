# Comparing `tmp/smartcrop-0.3.4.tar.gz` & `tmp/smartcrop-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcrop-0.3.4.tar", last modified: Tue Jul  4 16:03:43 2023, max compression
+gzip compressed data, was "smartcrop-0.4.0.tar", last modified: Wed Jul  5 11:30:42 2023, max compression
```

## Comparing `smartcrop-0.3.4.tar` & `smartcrop-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,36 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.982387 smartcrop-0.3.4/
--rw-r--r--   0 david     (1000) david     (1000)      139 2019-01-25 20:19:19.000000 smartcrop-0.3.4/AUTHORS
--rw-r--r--   0 david     (1000) david     (1000)     1079 2019-01-25 20:19:19.000000 smartcrop-0.3.4/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)     2488 2023-07-04 16:03:43.982387 smartcrop-0.3.4/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1870 2023-07-04 15:38:23.000000 smartcrop-0.3.4/README.rst
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-04 16:03:43.982387 smartcrop-0.3.4/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1072 2023-07-04 16:03:16.000000 smartcrop-0.3.4/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.978387 smartcrop-0.3.4/smartcrop.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     2488 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      304 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       47 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2019-01-25 20:31:01.000000 smartcrop-0.3.4/smartcrop.egg-info/not-zip-safe
--rw-r--r--   0 david     (1000) david     (1000)       20 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       10 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/top_level.txt
--rwxrwxr-x   0 david     (1000) david     (1000)    14330 2023-07-04 15:39:37.000000 smartcrop-0.3.4/smartcrop.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.982387 smartcrop-0.3.4/tests/
--rw-rw-r--   0 david     (1000) david     (1000)      941 2023-07-04 15:39:37.000000 smartcrop-0.3.4/tests/test_smartcrop.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.643406 smartcrop-0.4.0/
+-rw-rw-r--   0 david     (1000) david     (1000)      150 2023-07-05 11:24:48.000000 smartcrop-0.4.0/.flake8
+-rw-rw-r--   0 david     (1000) david     (1000)      207 2023-07-05 11:24:48.000000 smartcrop-0.4.0/.gitignore
+-rw-rw-r--   0 david     (1000) david     (1000)    16176 2023-07-05 11:24:48.000000 smartcrop-0.4.0/.pylintrc
+-rw-rw-r--   0 david     (1000) david     (1000)      652 2023-07-05 11:24:48.000000 smartcrop-0.4.0/.travis.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      173 2023-07-05 08:12:33.000000 smartcrop-0.4.0/AUTHORS
+-rw-rw-r--   0 david     (1000) david     (1000)     1884 2023-07-05 11:28:05.000000 smartcrop-0.4.0/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1079 2023-07-05 08:12:33.000000 smartcrop-0.4.0/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)     3333 2023-07-05 11:30:42.643406 smartcrop-0.4.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2480 2023-07-05 11:24:48.000000 smartcrop-0.4.0/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.635406 smartcrop-0.4.0/examples/
+-rwxrwxr-x   0 david     (1000) david     (1000)     2319 2023-07-05 11:24:48.000000 smartcrop-0.4.0/examples/test_bed.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2272 2023-07-05 11:28:22.000000 smartcrop-0.4.0/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      270 2023-07-05 11:24:48.000000 smartcrop-0.4.0/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)      197 2023-07-05 11:24:48.000000 smartcrop-0.4.0/requirements.install.apt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-05 11:30:42.643406 smartcrop-0.4.0/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-05 11:30:37.000000 smartcrop-0.4.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.635406 smartcrop-0.4.0/smartcrop/
+-rw-rw-r--   0 david     (1000) david     (1000)      100 2023-07-05 11:24:48.000000 smartcrop-0.4.0/smartcrop/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1886 2023-07-05 11:24:48.000000 smartcrop-0.4.0/smartcrop/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13734 2023-07-05 11:24:48.000000 smartcrop-0.4.0/smartcrop/library.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.635406 smartcrop-0.4.0/smartcrop.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     3333 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      589 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2023-07-05 11:30:42.000000 smartcrop-0.4.0/smartcrop.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.635406 smartcrop-0.4.0/tests/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-05 11:30:42.643406 smartcrop-0.4.0/tests/images/
+-rw-r--r--   0 david     (1000) david     (1000)   488535 2023-07-05 08:12:33.000000 smartcrop-0.4.0/tests/images/business-work-1.jpg
+-rw-r--r--   0 david     (1000) david     (1000)   972335 2023-07-05 08:12:33.000000 smartcrop-0.4.0/tests/images/nature-1.jpg
+-rw-rw-r--   0 david     (1000) david     (1000)  4314660 2023-07-05 11:24:48.000000 smartcrop-0.4.0/tests/images/orientation.jpg
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-07-05 08:12:33.000000 smartcrop-0.4.0/tests/images/photo_credits.txt
+-rw-r--r--   0 david     (1000) david     (1000)   859392 2023-07-05 08:12:33.000000 smartcrop-0.4.0/tests/images/travel-1.jpg
+-rw-rw-r--   0 david     (1000) david     (1000)     1006 2023-07-05 11:24:48.000000 smartcrop-0.4.0/tests/test_smartcrop.py
```

### Comparing `smartcrop-0.3.4/LICENSE` & `smartcrop-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcrop-0.3.4/PKG-INFO` & `smartcrop-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,89 @@
-Metadata-Version: 2.1
-Name: smartcrop
-Version: 0.3.4
-Summary: smartcrop implementation in Python
-Home-page: https://github.com/smartcrop/smartcrop.py
-Author: Hideo Hattori
-Author-email: hhatto.jp@gmail.com
-License: MIT
-Keywords: image,crop,PIL,Pillow
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities
-License-File: LICENSE
-License-File: AUTHORS
+[![image](https://travis-ci.com/smartcrop/smartcrop.py.svg?branch=master)](https://travis-ci.com/smartcrop/smartcrop.py)
 
-.. image:: https://travis-ci.com/smartcrop/smartcrop.py.svg?branch=master
-    :target: https://travis-ci.com/smartcrop/smartcrop.py
-
-smartcrop.py
-============
+# smartcrop.py
 
 smartcrop implementation in Python.
 
-smartcrop finds good crops for arbitrary images and crop sizes, based on Jonas Wagner's `smartcrop.js`_.
-
-.. _`smartcrop.js`: https://github.com/jwagner/smartcrop.js
+smartcrop finds good crops for arbitrary images and crop sizes, based on
+Jonas Wagner\'s [smartcrop.js](https://github.com/jwagner/smartcrop.js).
 
-.. image:: https://i.gyazo.com/c602d20e025e58f5b15180cd9a262814.jpg
-    :width: 50%
+![image](https://i.gyazo.com/c602d20e025e58f5b15180cd9a262814.jpg){width="50.0%"}
 
-.. image:: https://i.gyazo.com/5fbc9026202f54b13938de621562ed3d.jpg
-    :width: 25%
+![image](https://i.gyazo.com/5fbc9026202f54b13938de621562ed3d.jpg){width="25.0%"}
 
-.. image:: https://i.gyazo.com/88ee22ca9e1dd7e9eba7ea96db084e5e.jpg
-    :width: 50%
+![image](https://i.gyazo.com/88ee22ca9e1dd7e9eba7ea96db084e5e.jpg){width="50.0%"}
 
-Requirements
-------------
+## Requirements
 
-* numpy
-* PIL or Pillow
+Python requirements are defined in [pyproject.toml](pyproject.toml).
 
-Installation
-------------
+Moreover the packages such as `PyGObject` and `GExiv2` requires additional system packages that has to be installed using your OS package manager. Please check [requirements.install.apt](requirements.install.apt) for that purpose (tuned on Ubuntu 22.04).
 
-.. code-block:: sh
+## Installation
 
-    pip3 install smartcrop
+``` sh
+sudo apt-get install <...> # list from requirements.install.apt
+pip3 install -U pip setuptools wheel # optional but recommended
+pip3 install smartcrop
+```
 
 or directly from GitHub:
 
-.. code-block:: sh
-
-    pip install -e git+git://github.com/hhatto/smartcrop.py.git@master#egg=smartcrop
+``` sh
+sudo apt-get install <...> # list from requirements.install.apt
+pip3 install -U pip setuptools wheel # optional but recommended
+pip install -e git+git://github.com/hhatto/smartcrop.py.git@master#egg=smartcrop
+```
 
-Usage
------
+## Usage
 
 Use the basic command-line tool:
 
-.. code-block:: sh
-
-    $ smartcroppy --help
-    usage: smartcroppy [-h] [--debug] [--width WIDTH] [--height HEIGHT]
-                       INPUT_FILE OUTPUT_FILE
-
-    positional arguments:
-      INPUT_FILE       input image file
-      OUTPUT_FILE      output image file
-
-    optional arguments:
-      -h, --help       show this help message and exit
-      --debug          debug mode
-      --width WIDTH    crop width
-      --height HEIGHT  crop height
+``` sh
+$ smartcroppy --help
+usage: smartcroppy [-h] [--debug-file DEBUG_FILE] [--width WIDTH] [--height HEIGHT] INPUT_FILE OUTPUT_FILE
+
+positional arguments:
+  INPUT_FILE            Input image file
+  OUTPUT_FILE           Output image file
+
+options:
+  -h, --help            show this help message and exit
+  --debug-file DEBUG_FILE
+                        Debugging image file
+  --width WIDTH         Crop width
+  --height HEIGHT       Crop height
+```
 
 Processing an image:
 
-.. code-block:: sh
-
-  smartcroppy --width 300 --height 300 tests/images/business-work-1.jpg output.jpg --debug-file debug.jpg
-
-Or use the module it in your code (this is a really basic example):
-
-.. code-block:: python
-
-    import json
-    import sys
-
-    import smartcrop
-    from PIL import Image
-
-    image = Image.open(sys.argv[1])
-
-    sc = smartcrop.SmartCrop()
-    result = sc.crop(image, 100, 100)
-    print(json.dumps(result, indent=2))
+``` sh
+smartcroppy --width 300 --height 300 tests/images/business-work-1.jpg output.jpg --debug-file debug.jpg
+```
+
+Or use the module it in your code (this is a really basic example, see [examples/](examples/) and [smartcrop/cli.py](smartcrop/cli.py) for inspiration):
+
+``` python
+import json
+import sys
+
+import smartcrop
+from PIL import Image
+
+image = Image.open(sys.argv[1])
+cropper = smartcrop.SmartCrop()
+result = cropper.crop(image, 100, 100)
+print(json.dumps(result, indent=2))
+```
+
+## Testing
+
+Install dependencies for testing, then call `pytest`:
+``` sh
+pip3 install smartcrop[test]
+pytest
+```
 
-License
--------
+## License
 
 MIT
```

### Comparing `smartcrop-0.3.4/smartcrop.py` & `smartcrop-0.4.0/smartcrop/library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-#!/usr/bin/env python
+from __future__ import annotations
 
-import argparse
-import json
 import math
 import sys
 
 import numpy as np
 from PIL import Image, ImageDraw
 from PIL.ImageFilter import Kernel
 
 
-def saturation(image):
+def saturation(image) -> np.ndarray:
     r, g, b = image.split()
     r, g, b = np.array(r), np.array(g), np.array(b)
     r, g, b = r.astype(float), g.astype(float), b.astype(float)
     maximum = np.maximum(np.maximum(r, g), b)  # [0; 255]
     minimum = np.minimum(np.minimum(r, g), b)  # [0; 255]
-    s = (maximum + minimum) / 255  # [0.0; 1.0]
-    d = (maximum - minimum) / 255  # [0.0; 1.0]
+    s = (maximum + minimum) / 255  # [0.0; 1.0] pylint:disable=invalid-name
+    d = (maximum - minimum) / 255  # [0.0; 1.0] pylint:disable=invalid-name
     d[maximum == minimum] = 0  # if maximum == minimum:
     s[maximum == minimum] = 1  # -> saturation = 0 / 1 = 0
     mask = s > 1
     s[mask] = 2 - d[mask]
     return d / s  # [0.0; 1.0]
 
 
 def thirds(x):
     """gets value in the range of [0, 1] where 0 is the center of the pictures
     returns weight of rule of thirds [0, 1]"""
     x = ((x + 2 / 3) % 2 * 0.5 - 0.5) * 16
     return max(1 - x * x, 0)
 
 
-class SmartCrop(object):
+class SmartCrop(object):  # pylint:disable=too-many-instance-attributes
 
-    DEFAULT_SKIN_COLOR = [0.78, 0.57, 0.44]
+    DEFAULT_SKIN_COLOR: tuple[float, float, float] = (0.78, 0.57, 0.44)
 
-    def __init__(
+    def __init__(  # pylint:disable=too-many-arguments,too-many-locals
         self,
-        detail_weight=0.2,
-        edge_radius=0.4,
-        edge_weight=-20,
-        outside_importance=-0.5,
-        rule_of_thirds=True,
-        saturation_bias=0.2,
-        saturation_brightness_max=0.9,
-        saturation_brightness_min=0.05,
-        saturation_threshold=0.4,
-        saturation_weight=0.3,
-        score_down_sample=8,
-        skin_bias=0.01,
-        skin_brightness_max=1,
-        skin_brightness_min=0.2,
-        skin_color=None,
-        skin_threshold=0.8,
-        skin_weight=1.8
+        detail_weight: float = 0.2,
+        edge_radius: float = 0.4,
+        edge_weight: float = -20,
+        outside_importance: float = -0.5,
+        rule_of_thirds: bool = True,
+        saturation_bias: float = 0.2,
+        saturation_brightness_max: float = 0.9,
+        saturation_brightness_min: float = 0.05,
+        saturation_threshold: float = 0.4,
+        saturation_weight: float = 0.3,
+        score_down_sample: int = 8,
+        skin_bias: float = 0.01,
+        skin_brightness_max: float = 1,
+        skin_brightness_min: float = 0.2,
+        skin_color: tuple[float, float, float] | None = None,
+        skin_threshold: float = 0.8,
+        skin_weight: float = 1.8
     ):
         self.detail_weight = detail_weight
         self.edge_radius = edge_radius
         self.edge_weight = edge_weight
         self.outside_importance = outside_importance
         self.rule_of_thirds = rule_of_thirds
         self.saturation_bias = saturation_bias
@@ -70,24 +68,24 @@
         self.skin_bias = skin_bias
         self.skin_brightness_max = skin_brightness_max
         self.skin_brightness_min = skin_brightness_min
         self.skin_color = skin_color or self.DEFAULT_SKIN_COLOR
         self.skin_threshold = skin_threshold
         self.skin_weight = skin_weight
 
-    def analyse(
+    def analyse(  # pylint:disable=too-many-arguments,too-many-locals
         self,
         image,
-        crop_width,
-        crop_height,
-        max_scale=1,
-        min_scale=0.9,
-        scale_step=0.1,
-        step=8
-    ):
+        crop_width: int,
+        crop_height: int,
+        max_scale: float = 1,
+        min_scale: float = 0.9,
+        scale_step: float = 0.1,
+        step: int = 8
+    ) -> dict:
         """
         Analyze image and return some suggestions of crops (coordinates).
         This implementation / algorithm is really slow for large images.
         Use `crop()` which is pre-scaling the image before analyzing it.
         """
         cie_image = image.convert('L', (0.2126, 0.7152, 0.0722, 0))
         cie_array = np.array(cie_image)  # [0; 255]
@@ -126,25 +124,25 @@
             crop['score'] = self.score(score_image, crop)
             if crop['score']['total'] > top_score:
                 top_crop = crop
                 top_score = crop['score']['total']
 
         return {'analyse_image': analyse_image, 'crops': crops, 'top_crop': top_crop}
 
-    def crop(
+    def crop(  # pylint:disable=too-many-arguments,too-many-locals
         self,
         image,
-        width,
-        height,
-        prescale=True,
-        max_scale=1,
-        min_scale=0.9,
-        scale_step=0.1,
-        step=8
-    ):
+        width: int,
+        height: int,
+        prescale: bool = True,
+        max_scale: float = 1,
+        min_scale: float = 0.9,
+        scale_step: float = 0.1,
+        step: int = 8
+    ) -> dict:
         """Not yet fully cleaned from https://github.com/hhatto/smartcrop.py."""
         scale = min(image.size[0] / width, image.size[1] / height)
         crop_width = int(math.floor(width * scale))
         crop_height = int(math.floor(height * scale))
         # img = 100x100, width = 95x95, scale = 100/95, 1/scale > min
         # don't set minscale smaller than 1/scale
         # -> don't pick crops that need upscaling
@@ -177,109 +175,112 @@
             crop['x'] = int(math.floor(crop['x'] / prescale_size))
             crop['y'] = int(math.floor(crop['y'] / prescale_size))
             crop['width'] = int(math.floor(crop['width'] / prescale_size))
             crop['height'] = int(math.floor(crop['height'] / prescale_size))
             result['crops'][i] = crop
         return result
 
-    def crops(
+    def crops(  # pylint:disable=too-many-arguments
         self,
         image,
-        crop_width,
-        crop_height,
-        max_scale=1,
-        min_scale=0.9,
-        scale_step=0.1,
-        step=8
-    ):
+        crop_width: int,
+        crop_height: int,
+        max_scale: float = 1,
+        min_scale: float = 0.9,
+        scale_step: float = 0.1,
+        step: int = 8
+    ) -> list[dict]:
         image_width, image_height = image.size
         crops = []
         for scale in (
             i / 100 for i in range(
                 int(max_scale * 100),
                 int((min_scale - scale_step) * 100),
                 -int(scale_step * 100))
         ):
             for y in range(0, image_height, step):
-                if not (y + crop_height * scale <= image_height):
+                if y + crop_height * scale > image_height:
                     break
                 for x in range(0, image_width, step):
-                    if not (x + crop_width * scale <= image_width):
+                    if x + crop_width * scale > image_width:
                         break
                     crops.append({
                         'x': x,
                         'y': y,
                         'width': crop_width * scale,
                         'height': crop_height * scale,
                     })
         if not crops:
             raise ValueError(locals())
         return crops
 
-    def debug_crop(self, analyse_image, crop):
+    def debug_crop(self, analyse_image, crop: dict):
         debug_image = analyse_image.copy()
         debug_pixels = debug_image.getdata()
         debug_crop_image = Image.new(
             'RGBA',
             (
                 int(math.floor(crop['width'])),
                 int(math.floor(crop['height']))
             ),
             (255, 0, 0, 25)
         )
         ImageDraw.Draw(debug_crop_image).rectangle(
-            ((0, 0), (crop['width'], crop['height'])),
+            (
+                (0, 0),
+                (crop['width'], crop['height'])
+            ),
             outline=(255, 0, 0))
 
         for y in range(analyse_image.size[1]):        # height
             for x in range(analyse_image.size[0]):    # width
-                p = y * analyse_image.size[0] + x
+                index = y * analyse_image.size[0] + x
                 importance = self.importance(crop, x, y)
                 if importance > 0:
                     debug_pixels.putpixel(
                         (x, y),
                         (
-                            debug_pixels[p][0],
-                            int(debug_pixels[p][1] + importance * 32),
-                            debug_pixels[p][2]
+                            debug_pixels[index][0],
+                            int(debug_pixels[index][1] + importance * 32),
+                            debug_pixels[index][2]
                         ))
                 elif importance < 0:
                     debug_pixels.putpixel(
                         (x, y),
                         (
-                            int(debug_pixels[p][0] + importance * -64),
-                            debug_pixels[p][1],
-                            debug_pixels[p][2]
+                            int(debug_pixels[index][0] + importance * -64),
+                            debug_pixels[index][1],
+                            debug_pixels[index][2]
                         ))
         debug_image.paste(debug_crop_image, (crop['x'], crop['y']), debug_crop_image.split()[3])
         return debug_image
 
     def detect_edge(self, cie_image):
         return cie_image.filter(Kernel((3, 3), (0, -1, 0, -1, 4, -1, 0, -1, 0), 1, 1))
 
-    def detect_saturation(self, cie_array, source_image):
+    def detect_saturation(self, cie_array: np.ndarray, source_image):
         threshold = self.saturation_threshold
         saturation_data = saturation(source_image)
         mask = (
             (saturation_data > threshold) &
             (cie_array >= self.saturation_brightness_min * 255) &
             (cie_array <= self.saturation_brightness_max * 255))
 
         saturation_data[~mask] = 0
         saturation_data[mask] = (saturation_data[mask] - threshold) * (255 / (1 - threshold))
 
         return Image.fromarray(saturation_data.astype('uint8'))
 
-    def detect_skin(self, cie_array, source_image):
+    def detect_skin(self, cie_array: np.ndarray, source_image):
         r, g, b = source_image.split()
         r, g, b = np.array(r), np.array(g), np.array(b)
         r, g, b = r.astype(float), g.astype(float), b.astype(float)
-        rd = np.ones_like(r) * -self.skin_color[0]
-        gd = np.ones_like(g) * -self.skin_color[1]
-        bd = np.ones_like(b) * -self.skin_color[2]
+        rd = np.ones_like(r) * -self.skin_color[0]  # pylint:disable=invalid-name
+        gd = np.ones_like(g) * -self.skin_color[1]  # pylint:disable=invalid-name
+        bd = np.ones_like(b) * -self.skin_color[2]  # pylint:disable=invalid-name
 
         mag = np.sqrt(r * r + g * g + b * b)
         mask = ~(abs(mag) < 1e-6)
         rd[mask] = r[mask] / mag[mask] - self.skin_color[0]
         gd[mask] = g[mask] / mag[mask] - self.skin_color[1]
         bd[mask] = b[mask] / mag[mask] - self.skin_color[2]
 
@@ -290,37 +291,38 @@
             (cie_array <= self.skin_brightness_max * 255))
 
         skin_data = (skin - self.skin_threshold) * (255 / (1 - self.skin_threshold))
         skin_data[~mask] = 0
 
         return Image.fromarray(skin_data.astype('uint8'))
 
-    def importance(self, crop, x, y):
+    def importance(self, crop: dict, x: int, y: int) -> float:
         if (
             crop['x'] > x or x >= crop['x'] + crop['width'] or
             crop['y'] > y or y >= crop['y'] + crop['height']
         ):
             return self.outside_importance
 
         x = (x - crop['x']) / crop['width']
         y = (y - crop['y']) / crop['height']
-        px, py = abs(0.5 - x) * 2, abs(0.5 - y) * 2
+        px, py = abs(0.5 - x) * 2, abs(0.5 - y) * 2  # pylint:disable=invalid-name
 
         # distance from edge
-        dx = max(px - 1 + self.edge_radius, 0)
-        dy = max(py - 1 + self.edge_radius, 0)
-        d = (dx * dx + dy * dy) * self.edge_weight
-        s = 1.41 - math.sqrt(px * px + py * py)
+        dx = max(px - 1 + self.edge_radius, 0)      # pylint:disable=invalid-name
+        dy = max(py - 1 + self.edge_radius, 0)      # pylint:disable=invalid-name
+        d = (dx * dx + dy * dy) * self.edge_weight  # pylint:disable=invalid-name
+        s = 1.41 - math.sqrt(px * px + py * py)     # pylint:disable=invalid-name
 
         if self.rule_of_thirds:
+            # pylint:disable=invalid-name
             s += (max(0, s + d + 0.5) * 1.2) * (thirds(px) + thirds(py))
 
         return s + d
 
-    def score(self, target_image, crop):
+    def score(self, target_image, crop: dict) -> dict:  # pylint:disable=too-many-locals
         score = {
             'detail': 0,
             'saturation': 0,
             'skin': 0,
             'total': 0,
         }
         target_data = target_image.getdata()
@@ -329,75 +331,27 @@
         down_sample = self.score_down_sample
         inv_down_sample = 1 / down_sample
         target_width_down_sample = target_width * down_sample
         target_height_down_sample = target_height * down_sample
 
         for y in range(0, target_height_down_sample, down_sample):
             for x in range(0, target_width_down_sample, down_sample):
-                p = int(
+                index = int(
                     math.floor(y * inv_down_sample) * target_width +
                     math.floor(x * inv_down_sample)
                 )
                 importance = self.importance(crop, x, y)
-                detail = target_data[p][1] / 255
+                detail = target_data[index][1] / 255
                 score['skin'] += (
-                    target_data[p][0] / 255 *
-                    (detail + self.skin_bias) *
-                    importance
+                    target_data[index][0] / 255 * (detail + self.skin_bias) * importance
                 )
                 score['detail'] += detail * importance
                 score['saturation'] += (
-                    target_data[p][2] / 255 *
-                    (detail + self.saturation_bias) *
-                    importance
+                    target_data[index][2] / 255 * (detail + self.saturation_bias) * importance
                 )
         score['total'] = (
             score['detail'] * self.detail_weight +
             score['skin'] * self.skin_weight +
             score['saturation'] * self.saturation_weight
         ) / (crop['width'] * crop['height'])
-        return score
-
-
-def parse_argument():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('inputfile', metavar='INPUT_FILE', help='Input image file')
-    parser.add_argument('outputfile', metavar='OUTPUT_FILE', help='Output image file')
-    parser.add_argument('--debug-file', metavar='DEBUG_FILE', help='Debugging image file')
-    parser.add_argument('--width', dest='width', type=int, default=100, help='Crop width')
-    parser.add_argument('--height', dest='height', type=int, default=100, help='Crop height')
-    return parser.parse_args()
-
-
-def main():
-    options = parse_argument()
-
-    image = Image.open(options.inputfile)
-    if image.mode != 'RGB' and image.mode != 'RGBA':
-        sys.stderr.write("{1} convert from mode='{0}' to mode='RGB'\n".format(
-            image.mode, options.inputfile))
-        new_image = Image.new('RGB', image.size)
-        new_image.paste(image)
-        image = new_image
-
-    cropper = SmartCrop()
-    result = cropper.crop(image, width=100, height=int(options.height / options.width * 100))
-
-    box = (
-        result['top_crop']['x'],
-        result['top_crop']['y'],
-        result['top_crop']['width'] + result['top_crop']['x'],
-        result['top_crop']['height'] + result['top_crop']['y']
-    )
-
-    if options.debug_file:
-        analyse_image = result.pop('analyse_image')
-        cropper.debug_crop(analyse_image, result['top_crop']).save(options.debug_file)
-        print(json.dumps(result))
-
-    cropped_image = image.crop(box)
-    cropped_image.thumbnail((options.width, options.height), Image.Resampling.LANCZOS)
-    cropped_image.save(options.outputfile, 'JPEG', quality=90)
 
-
-if __name__ == '__main__':
-    main()
+        return score
```

### Comparing `smartcrop-0.3.4/tests/test_smartcrop.py` & `smartcrop-0.4.0/tests/test_smartcrop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import os
+
 import pytest
 from PIL import Image
 from smartcrop import SmartCrop
 
+
 def load_image(name):
     here = os.path.abspath(os.path.dirname(__file__))
     img = Image.open(os.path.join(here, 'images', name))
     return img
 
+
 @pytest.mark.parametrize('image, crop', [
     ('business-work-1.jpg', (41, 0, 1193, 1152)),
     ('nature-1.jpg', (705, 235, 3639, 3169)),
     ('travel-1.jpg', (52, 52, 1370, 1370)),
+    ('orientation.jpg', (972, 216, 3669, 2913))
 ])
 def test_square_thumbs(image, crop):
-    sc = SmartCrop()
+    cropper = SmartCrop()
 
     img = load_image(image)
-    ret = sc.crop(img.copy(), 200, 200)
+    ret = cropper.crop(img.copy(), 200, 200)
 
     box = (ret['top_crop']['x'],
            ret['top_crop']['y'],
            ret['top_crop']['width'] + ret['top_crop']['x'],
            ret['top_crop']['height'] + ret['top_crop']['y'])
 
     print(box)
```

