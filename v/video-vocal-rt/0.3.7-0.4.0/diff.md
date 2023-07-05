# Comparing `tmp/video_vocal_rt-0.3.7.tar.gz` & `tmp/video_vocal_rt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_vocal_rt-0.3.7.tar", max compression
+gzip compressed data, was "video_vocal_rt-0.4.0.tar", max compression
```

## Comparing `video_vocal_rt-0.3.7.tar` & `video_vocal_rt-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-03-12 02:11:47.157280 video_vocal_rt-0.3.7/LICENSE.md
--rw-r--r--   0        0        0     1131 2023-03-30 22:37:30.878131 video_vocal_rt-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1875 2023-03-12 03:21:00.098677 video_vocal_rt-0.3.7/README.md
--rw-r--r--   0        0        0        0 2023-03-11 20:15:53.793665 video_vocal_rt-0.3.7/video_vocal_rt/__init__.py
--rw-r--r--   0        0        0    10249 2023-03-30 22:37:20.694876 video_vocal_rt-0.3.7/video_vocal_rt/experiment.py
--rw-r--r--   0        0        0     3061 1970-01-01 00:00:00.000000 video_vocal_rt-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-03-12 02:11:47.157280 video_vocal_rt-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1198 2023-07-05 18:26:27.365860 video_vocal_rt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1875 2023-03-12 03:21:00.098677 video_vocal_rt-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-11 20:15:53.793665 video_vocal_rt-0.4.0/video_vocal_rt/__init__.py
+-rw-r--r--   0        0        0    10488 2023-07-05 18:30:23.918279 video_vocal_rt-0.4.0/video_vocal_rt/experiment.py
+-rw-r--r--   0        0        0     3136 1970-01-01 00:00:00.000000 video_vocal_rt-0.4.0/PKG-INFO
```

### Comparing `video_vocal_rt-0.3.7/LICENSE.md` & `video_vocal_rt-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_vocal_rt-0.3.7/pyproject.toml` & `video_vocal_rt-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video-vocal-rt"
-version = "0.3.7"
+version = "0.4.0"
 description = "Video-Vocal-RT: a minimal package for vocal response to video"
 authors = ["Loonan Chauvette <loonan.chauvette@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/LoonanChauvette/video-vocal-RT"
 repository = "https://github.com/LoonanChauvette/video-vocal-RT"
 keywords = ["video", "audio", "psychology", "reaction time"]
@@ -24,16 +24,19 @@
 moviepy = "^1.0.3"
 sounddevice = "^0.4.6"
 scipy = "^1.10.1"
 opencv-python = "^4.7.0.72"
 numpy = "^1.24.2"
 openpyxl = "^3.1.2"
 pysimplegui = "^4.60.4"
+pillow = "<10.0.0"
+ffpyplayer = "^4.5.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
+pyinstaller = "^5.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `video_vocal_rt-0.3.7/README.md` & `video_vocal_rt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `video_vocal_rt-0.3.7/video_vocal_rt/experiment.py` & `video_vocal_rt-0.4.0/video_vocal_rt/experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import cv2
 import PySimpleGUI as sg
 import sounddevice as sd 
 import numpy as np
 import tkinter as tk
 from scipy.io.wavfile import write
 from openpyxl import Workbook
+from PIL import Image, ImageDraw, ImageFont
+
 
 def is_dir(dir_path: str) -> str:
     """
     Determines if a given string represents a valid directory path.
 
     Args:
         dir_path (str): The directory path to be checked.
@@ -166,44 +168,51 @@
 def get_parameters_from_user():
     parameters = Parameters()
     parameters.get_from_gui()
     return parameters
 
 def create_white_screen():
     root = tk.Tk()
-    height = root.winfo_screenheight()
-    width = root.winfo_screenwidth()
+    h = root.winfo_screenheight()
+    w = root.winfo_screenwidth()
     root.destroy()
-    return np.ones((height, width, 3), dtype=np.uint8) * 255
+    return Image.new('RGB', (w, h), color = (255, 255, 255))
 
 def get_center_coordinates(image):
-    height, width, _ = image.shape
-    return (width // 2, height // 2)    # return (x, y)
+    width, height = image.size
+    return (width // 2, height // 2)
 
 def create_instruction_screen(text):
+    font_size = 24
     instructions = create_white_screen()
+    draw = ImageDraw.Draw(instructions)
     x_mid, y_mid = get_center_coordinates(instructions)
-    x0, y0 = x_mid //2, y_mid //2
-    dy = 18
-    for i, line in enumerate(text.split('\n')):
-        y = y0 + i * dy
-        x = x0
-        cv2.putText(img=instructions, text=line, org = (x,y),
-                    fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=1,
-                    color=(0,0,0), thickness=2, lineType=cv2.LINE_AA)
-    return instructions
+
+    font = ImageFont.truetype("NotoSans-Regular.ttf", font_size)
+    lines = text.split('\n')
+    text_height = len(lines) * font_size * 1.2
+    y = y_mid - text_height // 2 + font_size // 2
+    
+    for line in lines:
+        bbox = font.getbbox(line)
+        f_width, f_height = bbox[2] - bbox[0], bbox[3] - bbox[1]
+        x = x_mid - f_width // 2
+        draw.text((x, y), line, font=font, fill=(0, 0, 0))
+        y += f_height * 1.4
+    return np.array(instructions)
 
 def create_fixation_screen():
     fixation = create_white_screen()
+    draw = ImageDraw.Draw(fixation)
     x, y = get_center_coordinates(fixation)
 
     size = 20
-    cv2.line(fixation, (x - size, y), (x + size, y), (0, 0, 0), thickness=2)
-    cv2.line(fixation, (x, y - size), (x, y + size), (0, 0, 0), thickness=2)
-    return fixation
+    draw.line([(x - size, y), (x + size, y)], fill=(0, 0, 0), width=3)
+    draw.line([(x, y - size), (x, y + size)], fill=(0, 0, 0), width=3)
+    return np.array(fixation)
 
 def run():
     # Create the GUI to enter experiment parameters, returns a parameters object
     params = get_parameters_from_user()
 
     # List of all the files in the video directory and shuffle them
     video_files = [f for f in os.listdir(params.video_dir) if f.endswith('.avi')]
@@ -215,18 +224,18 @@
 
     # Set up excel file
     wb = Workbook()
     ws = wb.active
     ws.append(['ID', 'Order', 'Video', 'Audio_path'])
 
     # Display blank screen and wait for key press
-    blank = create_white_screen()
+    blank = np.array(create_white_screen())
     fixation = create_fixation_screen()
     try:
-        with open (params.inst_path, 'r') as f:
+        with open (params.inst_path, 'r', encoding='utf-8') as f:
             instructions = create_instruction_screen(f.read())
     except FileNotFoundError:
         instructions = create_instruction_screen("Press any key to continue...")
 
     cv2.namedWindow('main_window', cv2.WINDOW_NORMAL)
     cv2.imshow('main_window', instructions)
     cv2.waitKey(0)
@@ -251,15 +260,15 @@
                 exit()
             
         # white screen display
         cv2.imshow('main_window', blank)
         cv2.waitKey(params.white_dur)
 
         sd.wait() # wait for recording to finish
-        audio_file = f"{video_file[:-4]}_{params.participant_id}_{params.unique_key}.wav"
+        audio_file = f"{video_file[:-4]}_{params.participant_id}.wav"
         audio_path = os.path.join(participant_dir, audio_file)
         write(audio_path, params.sample_rate, recording)
 
         ws.append([params.participant_id, i+1, video_file, audio_path])
 
         video.release()
```

### Comparing `video_vocal_rt-0.3.7/PKG-INFO` & `video_vocal_rt-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-vocal-rt
-Version: 0.3.7
+Version: 0.4.0
 Summary: Video-Vocal-RT: a minimal package for vocal response to video
 Home-page: https://github.com/LoonanChauvette/video-vocal-RT
 License: MIT
 Keywords: video,audio,psychology,reaction time
 Author: Loonan Chauvette
 Author-email: loonan.chauvette@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -14,18 +14,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
+Requires-Dist: ffpyplayer (>=4.5.0,<5.0.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pillow (<10.0.0)
 Requires-Dist: pysimplegui (>=4.60.4,<5.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sounddevice (>=0.4.6,<0.5.0)
 Project-URL: Repository, https://github.com/LoonanChauvette/video-vocal-RT
 Description-Content-Type: text/markdown
 
 # video-vocal-RT
```

