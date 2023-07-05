# Comparing `tmp/git-sim-0.3.2.tar.gz` & `tmp/git-sim-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-sim-0.3.2.tar", last modified: Mon Jun 12 02:56:59 2023, max compression
+gzip compressed data, was "git-sim-0.3.3.tar", last modified: Wed Jul  5 01:52:36 2023, max compression
```

## Comparing `git-sim-0.3.2.tar` & `git-sim-0.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.256162 git-sim-0.3.2/
--rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0    25490 2023-06-12 02:56:59.256162 git-sim-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    24683 2023-06-12 02:56:27.000000 git-sim-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.249657 git-sim-0.3.2/git_sim/
--rw-rw-rw-   0        0        0       23 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/__init__.py
--rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/__main__.py
--rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/add.py
--rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/animations.py
--rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/branch.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/checkout.py
--rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/cherrypick.py
--rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/clean.py
--rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/clone.py
--rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/commands.py
--rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/commit.py
--rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.2/git_sim/enums.py
--rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/fetch.py
--rw-rw-rw-   0        0        0    46330 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/git_sim_base_command.py
--rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.2/git_sim/log.py
--rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.2/git_sim/logo.png
--rw-rw-rw-   0        0        0     7258 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/merge.py
--rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/mv.py
--rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/pull.py
--rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.2/git_sim/push.py
--rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/rebase.py
--rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/reset.py
--rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/restore.py
--rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/revert.py
--rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/rm.py
--rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/settings.py
--rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/stash.py
--rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/status.py
--rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/switch.py
--rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/tag.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.254657 git-sim-0.3.2/git_sim.egg-info/
--rw-rw-rw-   0        0        0    25490 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 02:56:59.256162 git-sim-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.529848 git-sim-0.3.3/
+-rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    25490 2023-07-05 01:52:36.528497 git-sim-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    24683 2023-06-12 02:56:27.000000 git-sim-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.520305 git-sim-0.3.3/git_sim/
+-rw-rw-rw-   0        0        0       23 2023-07-05 01:51:56.000000 git-sim-0.3.3/git_sim/__init__.py
+-rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/__main__.py
+-rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/add.py
+-rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/animations.py
+-rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/branch.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/checkout.py
+-rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/cherrypick.py
+-rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/clean.py
+-rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/clone.py
+-rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/commands.py
+-rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/commit.py
+-rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.3/git_sim/enums.py
+-rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/fetch.py
+-rw-rw-rw-   0        0        0    46330 2023-06-12 02:56:27.000000 git-sim-0.3.3/git_sim/git_sim_base_command.py
+-rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.3/git_sim/log.py
+-rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.3/git_sim/logo.png
+-rw-rw-rw-   0        0        0     7258 2023-06-12 02:56:27.000000 git-sim-0.3.3/git_sim/merge.py
+-rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/mv.py
+-rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/pull.py
+-rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.3/git_sim/push.py
+-rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/rebase.py
+-rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/reset.py
+-rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/restore.py
+-rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/revert.py
+-rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.3/git_sim/rm.py
+-rw-rw-rw-   0        0        0     1566 2023-07-05 01:51:10.000000 git-sim-0.3.3/git_sim/settings.py
+-rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/stash.py
+-rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/status.py
+-rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/switch.py
+-rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.3/git_sim/tag.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:52:36.528497 git-sim-0.3.3/git_sim.egg-info/
+-rw-rw-rw-   0        0        0    25490 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 01:52:36.000000 git-sim-0.3.3/git_sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 01:52:36.529848 git-sim-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-07-05 01:48:30.000000 git-sim-0.3.3/setup.py
```

### Comparing `git-sim-0.3.2/LICENSE` & `git-sim-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/PKG-INFO` & `git-sim-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
```

### Comparing `git-sim-0.3.2/README.md` & `git-sim-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/__main__.py` & `git-sim-0.3.3/git_sim/__main__.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/add.py` & `git-sim-0.3.3/git_sim/add.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/animations.py` & `git-sim-0.3.3/git_sim/animations.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/branch.py` & `git-sim-0.3.3/git_sim/branch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/checkout.py` & `git-sim-0.3.3/git_sim/checkout.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/cherrypick.py` & `git-sim-0.3.3/git_sim/cherrypick.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/clean.py` & `git-sim-0.3.3/git_sim/clean.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/clone.py` & `git-sim-0.3.3/git_sim/clone.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/commands.py` & `git-sim-0.3.3/git_sim/commands.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/commit.py` & `git-sim-0.3.3/git_sim/commit.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/enums.py` & `git-sim-0.3.3/git_sim/enums.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/fetch.py` & `git-sim-0.3.3/git_sim/fetch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/git_sim_base_command.py` & `git-sim-0.3.3/git_sim/git_sim_base_command.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/log.py` & `git-sim-0.3.3/git_sim/log.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/logo.png` & `git-sim-0.3.3/git_sim/logo.png`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/merge.py` & `git-sim-0.3.3/git_sim/merge.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/mv.py` & `git-sim-0.3.3/git_sim/mv.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/pull.py` & `git-sim-0.3.3/git_sim/pull.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/push.py` & `git-sim-0.3.3/git_sim/push.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/rebase.py` & `git-sim-0.3.3/git_sim/rebase.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/reset.py` & `git-sim-0.3.3/git_sim/reset.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/restore.py` & `git-sim-0.3.3/git_sim/restore.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/revert.py` & `git-sim-0.3.3/git_sim/revert.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/rm.py` & `git-sim-0.3.3/git_sim/rm.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/settings.py` & `git-sim-0.3.3/git_sim/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import pathlib
 from typing import List, Union
 
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 
 from git_sim.enums import StyleOptions, ColorByOptions, ImgFormat, VideoFormat
 
 
 class Settings(BaseSettings):
-    allow_no_commits = False
-    animate = False
-    auto_open = True
-    n_default = 5
-    n = 5
+    allow_no_commits: bool = False
+    animate: bool = False
+    auto_open: bool = True
+    n_default: int = 5
+    n: int = 5
     files: Union[List[pathlib.Path], None] = None
-    hide_first_tag = False
+    hide_first_tag: bool = False
     img_format: ImgFormat = ImgFormat.JPG
-    INFO_STRING = "Simulating: git"
-    light_mode = False
-    transparent_bg = False
-    logo = pathlib.Path(__file__).parent.resolve() / "logo.png"
-    low_quality = False
-    max_branches_per_commit = 1
-    max_tags_per_commit = 1
-    media_dir = pathlib.Path().cwd()
-    outro_bottom_text = "Learn more at initialcommit.com"
-    outro_top_text = "Thanks for using Initial Commit!"
-    reverse = False
-    show_intro = False
-    show_outro = False
-    speed = 1.5
-    title = "Git-Sim, by initialcommit.com"
+    INFO_STRING: str = "Simulating: git"
+    light_mode: bool = False
+    transparent_bg: bool = False
+    logo: pathlib.Path = pathlib.Path(__file__).parent.resolve() / "logo.png"
+    low_quality: bool = False
+    max_branches_per_commit: int = 1
+    max_tags_per_commit: int = 1
+    media_dir: pathlib.Path = pathlib.Path().cwd()
+    outro_bottom_text: str = "Learn more at initialcommit.com"
+    outro_top_text: str = "Thanks for using Initial Commit!"
+    reverse: bool = False
+    show_intro: bool = False
+    show_outro: bool = False
+    speed: float = 1.5
+    title: str = "Git-Sim, by initialcommit.com"
     video_format: VideoFormat = VideoFormat.MP4
-    stdout = False
-    output_only_path = False
-    quiet = False
-    invert_branches = False
-    hide_merged_branches = False
-    all = False
+    stdout: bool = False
+    output_only_path: bool = False
+    quiet: bool = False
+    invert_branches: bool = False
+    hide_merged_branches: bool = False
+    all: bool = False
     color_by: Union[ColorByOptions, None] = None
-    highlight_commit_messages = False
+    highlight_commit_messages: bool = False
     style: Union[StyleOptions, None] = StyleOptions.CLEAN
 
     class Config:
         env_prefix = "git_sim_"
 
 
 settings = Settings()
```

### Comparing `git-sim-0.3.2/git_sim/stash.py` & `git-sim-0.3.3/git_sim/stash.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/status.py` & `git-sim-0.3.3/git_sim/status.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/switch.py` & `git-sim-0.3.3/git_sim/switch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim/tag.py` & `git-sim-0.3.3/git_sim/tag.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/git_sim.egg-info/PKG-INFO` & `git-sim-0.3.3/git_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
```

### Comparing `git-sim-0.3.2/git_sim.egg-info/SOURCES.txt` & `git-sim-0.3.3/git_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.2/setup.py` & `git-sim-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ],
     python_requires=">=3.7",
     install_requires=[
         "gitpython",
         "manim",
         "opencv-python-headless",
         "typer",
-        "pydantic",
+        "pydantic_settings",
         "git-dummy",
     ],
     keywords="git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run",
     project_urls={
         "Homepage": "https://initialcommit.com/tools/git-sim",
         "Source": "https://github.com/initialcommit-com/git-sim",
     },
```

