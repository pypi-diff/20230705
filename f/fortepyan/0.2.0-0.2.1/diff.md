# Comparing `tmp/fortepyan-0.2.0.tar.gz` & `tmp/fortepyan-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.2.0.tar", last modified: Sun Jun 11 11:47:03 2023, max compression
+gzip compressed data, was "fortepyan-0.2.1.tar", last modified: Wed Jul  5 16:50:11 2023, max compression
```

## Comparing `fortepyan-0.2.0.tar` & `fortepyan-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-06-11 11:47:03.037683 fortepyan-0.2.0/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.0/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-06-11 11:46:44.000000 fortepyan-0.2.0/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/analytics/
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/analytics/clustering/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7846 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/process.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/views.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.0/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.0/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.0/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.0/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.0/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.0/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      208 2023-06-11 08:17:56.000000 fortepyan-0.2.0/fortepyan/view/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.0/fortepyan/view/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.0/fortepyan/view/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      761 2023-06-11 08:41:24.000000 fortepyan-0.2.0/fortepyan/view/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5002 2023-06-11 08:41:45.000000 fortepyan-0.2.0/fortepyan/view/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/pianoroll/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       65 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5426 2023-06-11 08:19:09.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2925 2023-06-11 08:18:40.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      808 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      157 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1452 2023-06-11 11:46:44.000000 fortepyan-0.2.0/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-06-11 11:47:03.037683 fortepyan-0.2.0/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.319666 fortepyan-0.2.1/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-05 16:50:11.315666 fortepyan-0.2.1/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.1/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-05 16:49:56.000000 fortepyan-0.2.1/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/analytics/
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/analytics/clustering/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7846 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/process.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/views.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.1/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.1/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.1/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.1/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.1/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.1/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      208 2023-06-11 08:17:56.000000 fortepyan-0.2.1/fortepyan/view/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.1/fortepyan/view/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.1/fortepyan/view/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      761 2023-06-11 08:41:24.000000 fortepyan-0.2.1/fortepyan/view/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.1/fortepyan/view/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/pianoroll/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       65 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5568 2023-07-05 16:45:29.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3321 2023-07-05 16:48:53.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      808 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      157 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1452 2023-07-05 16:49:56.000000 fortepyan-0.2.1/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-05 16:50:11.319666 fortepyan-0.2.1/setup.cfg
```

### Comparing `fortepyan-0.2.0/PKG-INFO` & `fortepyan-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.0/README.md` & `fortepyan-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/analytics/clustering/process.py` & `fortepyan-0.2.1/fortepyan/analytics/clustering/process.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/analytics/clustering/structures.py` & `fortepyan-0.2.1/fortepyan/analytics/clustering/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/analytics/clustering/views.py` & `fortepyan-0.2.1/fortepyan/analytics/clustering/views.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/audio/render.py` & `fortepyan-0.2.1/fortepyan/audio/render.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/audio/soundfont.py` & `fortepyan-0.2.1/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/main.py` & `fortepyan-0.2.1/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/midi/structures.py` & `fortepyan-0.2.1/fortepyan/midi/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/midi/tools.py` & `fortepyan-0.2.1/fortepyan/midi/tools.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/view/animation/evolution.py` & `fortepyan-0.2.1/fortepyan/view/animation/evolution.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/view/animation/main.py` & `fortepyan-0.2.1/fortepyan/view/animation/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/fortepyan/view/animation/pianoroll.py` & `fortepyan-0.2.1/fortepyan/view/animation/pianoroll.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 from fortepyan.midi.structures import MidiPiece
 from fortepyan.view.pianoroll import main as roll
-from fortepyan.view.pianoroll.structures import PianoRoll
+from fortepyan.view.pianoroll.structures import PianoRoll, FigureResolution
 
 
 class PianoRollScene:
     def __init__(self, piece: MidiPiece, title: str, cmap: str = "GnBu"):
         self.axes = []
         self.content_dir = Path(tempfile.mkdtemp())
 
         self.frame_paths = []
 
         self.piece = piece
         self.title = title
         self.cmap = cmap
 
+        figres = FigureResolution()
         f, axes = plt.subplots(
             nrows=2,
             ncols=1,
-            figsize=[16, 9],
+            figsize=figres.figsize,
+            dpi=figres.dpi,
             gridspec_kw={
                 "height_ratios": [4, 1],
                 "hspace": 0,
             },
         )
 
         self.figure = f
```

### Comparing `fortepyan-0.2.0/fortepyan/view/pianoroll/main.py` & `fortepyan-0.2.1/fortepyan/view/pianoroll/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import matplotlib
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 from fortepyan.midi.structures import MidiPiece
-from fortepyan.view.pianoroll.structures import PianoRoll
+from fortepyan.view.pianoroll.structures import PianoRoll, FigureResolution
 
 
 def draw_pianoroll_with_velocities(
     midi_piece: MidiPiece,
     time_end: float = None,
     title: str = None,
     cmap: str = "GnBu",
+    figres: FigureResolution = None,
 ):
+    if not figres:
+        figres = FigureResolution()
+
     fig, axes = plt.subplots(
         nrows=2,
         ncols=1,
-        figsize=[16, 9],
+        figsize=figres.figsize,
+        dpi=figres.dpi,
         gridspec_kw={
             "height_ratios": [4, 1],
             "hspace": 0,
         },
     )
     piece = sanitize_midi_piece(midi_piece)
     piano_roll = PianoRoll(piece, time_end=time_end)
```

### Comparing `fortepyan-0.2.0/fortepyan/view/pianoroll/structures.py` & `fortepyan-0.2.1/fortepyan/view/pianoroll/structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,7 +84,26 @@
 
         # Prepare x ticks and labels
         n_ticks = min(30, self.duration)
         step = np.ceil(self.duration / n_ticks)
         x_ticks = np.arange(0, step * n_ticks, step)
         self.x_ticks = np.round(x_ticks)
         self.x_labels = [round(xt) for xt in self.x_ticks]
+
+
+@dataclass
+class FigureResolution:
+    w_pixels: int = 1920 // 2
+    h_pixels: int = 1080 // 2
+    dpi: int = 72
+
+    @property
+    def w_inches(self) -> float:
+        return self.w_pixels / self.dpi
+
+    @property
+    def h_inches(self) -> float:
+        return self.h_pixels / self.dpi
+
+    @property
+    def figsize(self) -> tuple[float, float]:
+        return self.w_inches, self.h_inches
```

### Comparing `fortepyan-0.2.0/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.2.1/fortepyan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.0/fortepyan.egg-info/SOURCES.txt` & `fortepyan-0.2.1/fortepyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.0/pyproject.toml` & `fortepyan-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.2.0"
+version = "0.2.1"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -42,15 +42,15 @@
     "fortepyan.audio",
     "fortepyan.view.animation",
     "fortepyan.view.pianoroll",
     "fortepyan.analytics.clustering",
 ]
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

