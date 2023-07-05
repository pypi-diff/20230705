# Comparing `tmp/convert_videos-2.8.8.tar.gz` & `tmp/convert_videos-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_videos-2.8.8.tar", max compression
+gzip compressed data, was "convert_videos-2.8.9.tar", max compression
```

## Comparing `convert_videos-2.8.8.tar` & `convert_videos-2.8.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-15 13:35:47.487404 convert_videos-2.8.8/LICENSE.md
--rw-r--r--   0        0        0     4316 2023-05-15 13:35:47.487404 convert_videos-2.8.8/README.md
--rwxr-xr-x   0        0        0      195 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/__init__.py
--rw-r--r--   0        0        0     4360 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/cli.py
--rw-r--r--   0        0        0      219 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/colour.py
--rw-r--r--   0        0        0     2399 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/ffmpeg_converter.py
--rw-r--r--   0        0        0     2196 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/processor.py
--rw-r--r--   0        0        0     4045 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/settings.py
--rw-r--r--   0        0        0     4514 2023-05-15 13:35:47.487404 convert_videos-2.8.8/convert_videos/video_processor.py
--rw-r--r--   0        0        0      837 2023-05-15 13:35:47.487404 convert_videos-2.8.8/pyproject.toml
--rw-r--r--   0        0        0     5269 1970-01-01 00:00:00.000000 convert_videos-2.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-05 10:23:21.936351 convert_videos-2.8.9/LICENSE.md
+-rw-r--r--   0        0        0     5281 2023-07-05 10:23:21.936351 convert_videos-2.8.9/README.md
+-rwxr-xr-x   0        0        0      195 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/__init__.py
+-rw-r--r--   0        0        0     4360 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/cli.py
+-rw-r--r--   0        0        0      219 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/colour.py
+-rw-r--r--   0        0        0     2399 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/ffmpeg_converter.py
+-rw-r--r--   0        0        0     2196 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/processor.py
+-rw-r--r--   0        0        0     4370 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/settings.py
+-rw-r--r--   0        0        0     4514 2023-07-05 10:23:21.936351 convert_videos-2.8.9/convert_videos/video_processor.py
+-rw-r--r--   0        0        0      837 2023-07-05 10:23:21.936351 convert_videos-2.8.9/pyproject.toml
+-rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 convert_videos-2.8.9/PKG-INFO
```

### Comparing `convert_videos-2.8.8/LICENSE.md` & `convert_videos-2.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.8/README.md` & `convert_videos-2.8.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,113 @@
 # Convert Videos
 
-![Test Status](https://github.com/justin8/convert_videos/workflows/Workflow/badge.svg?branch=master)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/convert_videos)](https://pypi.org/project/convert_videos/) [![PyPI version](https://badge.fury.io/py/convert_videos.svg)](https://badge.fury.io/py/convert_videos)
+
+[![Workflow](https://github.com/justin8/convert_videos/actions/workflows/workflow.yml/badge.svg)](https://github.com/convert_videos/video_utils/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/justin8/convert_videos/branch/master/graph/badge.svg)](https://codecov.io/gh/justin8/convert_videos)
+[![Downloads](https://pepy.tech/badge/convert_videos/month)](https://pepy.tech/project/convert_videos)
 
 This tool allows bulk conversion of videos using ffmpeg.
 
 By default it will append the codec name to the file, e.g. `Best Movie Ever.avi` -> `Best Movie Ever - x265.mkv`. This can be optionally overridden using the `--in-place` flag.
 
 Videos are only converted if they do not already match the desired codec, allowing you to process a folder of mixed format files and only convert the ones you desire. This can optionally be overridden.
 
-## File output
-
-### Container
-
-The default output container is `mkv` format. This can be changed with the `--container` flag to anything that is supported by FFMPEG and the chosen video and audio codecs
-
-## Video output
-
-Default settings is HEVC/x265 at quality of 23
-
-### Codecs
-
-Currently only HEVC (x265) and AVC (h264) are supported for video codecs.
-
-### Resizing
-
-Videos can be resized automatically by providing a width. Height is automatically calculated to ensure that the aspect ratio is maintained.
-
-### Hardware Acceleration
-
-Hardware acceleration is supported on nVidia and Intel devices.
-
-Caveats for nVidia:
-- Conversions use constqp mode for the quality setting instead of CRF, as nvenc does not support CRF
-- b-frames are not currently supported; nvenc itself supports them on 20xx+ series graphics cards.
-
-
-Caveats for Intel:
-- Conversions use global_quality mode as CRF isn't supported on Intel hardware. ICQ and LA-ICQ are apparently better, but only supported on Windows
-- Look-ahead is only supported on x264 (not HEVC)
-
-
-## Audio output
-
-Default settings is 160kbps 2 channel AAC.
-
-All audio streams will be included by default unless a language filter is specified with `--audio-language`.
-
-
-## Subtitles
-
-All subtitles will be copied from the source if they exist unless a language filter is specified with `--subtitle-language`.
-
 ## Usage
 
 ```
 Usage: convert-videos [OPTIONS] DIRECTORIES...
 
 Options:
   -i, --in-place                  Replace the original files instead of
                                   appending the new codec name
-
   -f, --force                     Force conversion even if the format of the
                                   file already matches the desired format
-
   --video-codec TEXT              A target video codec. Supported codecs:
                                   HEVC, AVC  [default: HEVC]
-
   -q, --quality INTEGER           The quantizer quality level to use.
                                   [default: 24]
-
   -p, --preset TEXT               FFmpeg preset to use.  [default: medium]
   -w, --width INTEGER             Specify a new width to enable resizing of
                                   the video
-
   --extra-input-args TEXT         Specify any extra arguments you would like
                                   to pass to FFMpeg input here
-
   --extra-output-args TEXT        Specify any extra arguments you would like
                                   to pass to FFMpeg output here
-
   --audio-codec TEXT              A target audio codec  [default: AAC]
   --audio-channels INTEGER        The number of channels to mux sound in to
                                   [default: 2]
-
   --audio-bitrate INTEGER         The bitrate to use for the audio codec
                                   [default: 160]
-
   --temp-dir TEXT                 Specify a temporary directory to use during
                                   conversions instead of the system default
-
   -v, --verbose                   Enable verbose log output
   --container TEXT                Specify a video container to convert the
                                   videos in to  [default: mkv]
-
   --dry-run                       Do not make actual changes
   --encoder [software|nvidia|intel]
                                   Optionally use a harwdare encoder to speed
                                   things up.  [default: software]
-
   --audio-language TEXT           Only include audio streams in this language
   --subtitle-language TEXT        Only include subtitle streams in this
                                   language
-
   -h, --help                      Show this message and exit.
 ```
+
+## Autocomplete
+
+To enable auto-completion:
+
+**zsh**
+Add the below to `~/.zshrc`
+`eval "$(_CONVERT_VIDEOS_COMPLETE=zsh_source convert-videos)"`
+
+**bash**
+Add the below to `~/.bashrc`
+`eval "$(_CONVERT_VIDEOS_COMPLETE=bash_source convert-videos)"`
+
+**fish**
+Add the following to `~/.config/fish/completions/convert-videos.fish`
+`eval (env _CONVERT_VIDEOS_COMPLETE=fish_source convert-videos)`
+
+## File output
+
+### Container
+
+The default output container is `mkv` format. This can be changed with the `--container` flag to anything that is supported by FFMPEG and the chosen video and audio codecs
+
+## Video output
+
+Default settings is HEVC/x265 at quality of 23
+
+### Codecs
+
+Currently only HEVC (x265) and AVC (h264) are supported for video codecs.
+
+### Resizing
+
+Videos can be resized automatically by providing a width. Height is automatically calculated to ensure that the aspect ratio is maintained.
+
+### Hardware Acceleration
+
+Hardware acceleration is supported on nVidia and Intel devices.
+
+Caveats for nVidia:
+
+- Conversions use constqp mode for the quality setting instead of CRF, as nvenc does not support CRF
+- b-frames are not currently supported; nvenc itself supports them on 20xx+ series graphics cards.
+
+Caveats for Intel:
+
+- Conversions use global_quality mode as CRF isn't supported on Intel hardware. ICQ and LA-ICQ are apparently better, but only supported on Windows
+- Look-ahead is only supported on x264 (not HEVC)
+- There is a bug (current as of 2023-05) where all videos converted with Intel's QSV with FFMPEG have a single I-frame at the start and no more; so currently this is unsuable
+
+## Audio output
+
+Default settings is 160kbps 2 channel AAC.
+
+All audio streams will be included by default unless a language filter is specified with `--audio-language`.
+
+## Subtitles
+
+All subtitles will be copied from the source if they exist unless a language filter is specified with `--subtitle-language`.
```

### Comparing `convert_videos-2.8.8/convert_videos/cli.py` & `convert_videos-2.8.9/convert_videos/cli.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.8/convert_videos/ffmpeg_converter.py` & `convert_videos-2.8.9/convert_videos/ffmpeg_converter.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.8/convert_videos/processor.py` & `convert_videos-2.8.9/convert_videos/processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.8/convert_videos/settings.py` & `convert_videos-2.8.9/convert_videos/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,19 @@
             # qsv doesn't support CRF either; they have their own methods at the link below
             # ICQ and LA-ICQ are apparently the gold standard; but only supported on windows (weird)
             # https://www.intel.com/content/www/us/en/developer/articles/technical/common-bitrate-control-methods-in-intel-media-sdk.html
             output = f" -global_quality {self.quality}"
             if self.codec.format_name == "AVC":
                 # Look-ahead is supported for x264 and is preferable for better quality
                 output += " -look_ahead 1"
+
+            # Fix for a bug in Intel QSV driver that causes it to only create a single I-frame at the start of a
+            # video. Forcing i-frame generation every 120 frames to counter this
+            # Source: https://github.com/intel/media-driver/issues/1576#issuecomment-1609128922
+            output += " -g:v 120"
         else:
             output = f" -crf {self.quality}"
         return output
 
     def _get_codec_settings(self):
         output = ""
         if self.codec == Codec("HEVC"):
```

### Comparing `convert_videos-2.8.8/convert_videos/video_processor.py` & `convert_videos-2.8.9/convert_videos/video_processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.8/pyproject.toml` & `convert_videos-2.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert_videos"
-version = "2.8.8"
+version = "2.8.9"
 description = "This tool allows bulk conversion of videos using ffmpeg"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `convert_videos-2.8.8/PKG-INFO` & `convert_videos-2.8.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-videos
-Version: 2.8.8
+Version: 2.8.9
 Summary: This tool allows bulk conversion of videos using ffmpeg
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,113 +21,119 @@
 Requires-Dist: prettytable (>=3.7.0,<4.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: video-utils (>=2.2.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Convert Videos
 
-![Test Status](https://github.com/justin8/convert_videos/workflows/Workflow/badge.svg?branch=master)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/convert_videos)](https://pypi.org/project/convert_videos/) [![PyPI version](https://badge.fury.io/py/convert_videos.svg)](https://badge.fury.io/py/convert_videos)
+
+[![Workflow](https://github.com/justin8/convert_videos/actions/workflows/workflow.yml/badge.svg)](https://github.com/convert_videos/video_utils/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/justin8/convert_videos/branch/master/graph/badge.svg)](https://codecov.io/gh/justin8/convert_videos)
+[![Downloads](https://pepy.tech/badge/convert_videos/month)](https://pepy.tech/project/convert_videos)
 
 This tool allows bulk conversion of videos using ffmpeg.
 
 By default it will append the codec name to the file, e.g. `Best Movie Ever.avi` -> `Best Movie Ever - x265.mkv`. This can be optionally overridden using the `--in-place` flag.
 
 Videos are only converted if they do not already match the desired codec, allowing you to process a folder of mixed format files and only convert the ones you desire. This can optionally be overridden.
 
-## File output
-
-### Container
-
-The default output container is `mkv` format. This can be changed with the `--container` flag to anything that is supported by FFMPEG and the chosen video and audio codecs
-
-## Video output
-
-Default settings is HEVC/x265 at quality of 23
-
-### Codecs
-
-Currently only HEVC (x265) and AVC (h264) are supported for video codecs.
-
-### Resizing
-
-Videos can be resized automatically by providing a width. Height is automatically calculated to ensure that the aspect ratio is maintained.
-
-### Hardware Acceleration
-
-Hardware acceleration is supported on nVidia and Intel devices.
-
-Caveats for nVidia:
-- Conversions use constqp mode for the quality setting instead of CRF, as nvenc does not support CRF
-- b-frames are not currently supported; nvenc itself supports them on 20xx+ series graphics cards.
-
-
-Caveats for Intel:
-- Conversions use global_quality mode as CRF isn't supported on Intel hardware. ICQ and LA-ICQ are apparently better, but only supported on Windows
-- Look-ahead is only supported on x264 (not HEVC)
-
-
-## Audio output
-
-Default settings is 160kbps 2 channel AAC.
-
-All audio streams will be included by default unless a language filter is specified with `--audio-language`.
-
-
-## Subtitles
-
-All subtitles will be copied from the source if they exist unless a language filter is specified with `--subtitle-language`.
-
 ## Usage
 
 ```
 Usage: convert-videos [OPTIONS] DIRECTORIES...
 
 Options:
   -i, --in-place                  Replace the original files instead of
                                   appending the new codec name
-
   -f, --force                     Force conversion even if the format of the
                                   file already matches the desired format
-
   --video-codec TEXT              A target video codec. Supported codecs:
                                   HEVC, AVC  [default: HEVC]
-
   -q, --quality INTEGER           The quantizer quality level to use.
                                   [default: 24]
-
   -p, --preset TEXT               FFmpeg preset to use.  [default: medium]
   -w, --width INTEGER             Specify a new width to enable resizing of
                                   the video
-
   --extra-input-args TEXT         Specify any extra arguments you would like
                                   to pass to FFMpeg input here
-
   --extra-output-args TEXT        Specify any extra arguments you would like
                                   to pass to FFMpeg output here
-
   --audio-codec TEXT              A target audio codec  [default: AAC]
   --audio-channels INTEGER        The number of channels to mux sound in to
                                   [default: 2]
-
   --audio-bitrate INTEGER         The bitrate to use for the audio codec
                                   [default: 160]
-
   --temp-dir TEXT                 Specify a temporary directory to use during
                                   conversions instead of the system default
-
   -v, --verbose                   Enable verbose log output
   --container TEXT                Specify a video container to convert the
                                   videos in to  [default: mkv]
-
   --dry-run                       Do not make actual changes
   --encoder [software|nvidia|intel]
                                   Optionally use a harwdare encoder to speed
                                   things up.  [default: software]
-
   --audio-language TEXT           Only include audio streams in this language
   --subtitle-language TEXT        Only include subtitle streams in this
                                   language
-
   -h, --help                      Show this message and exit.
 ```
 
+## Autocomplete
+
+To enable auto-completion:
+
+**zsh**
+Add the below to `~/.zshrc`
+`eval "$(_CONVERT_VIDEOS_COMPLETE=zsh_source convert-videos)"`
+
+**bash**
+Add the below to `~/.bashrc`
+`eval "$(_CONVERT_VIDEOS_COMPLETE=bash_source convert-videos)"`
+
+**fish**
+Add the following to `~/.config/fish/completions/convert-videos.fish`
+`eval (env _CONVERT_VIDEOS_COMPLETE=fish_source convert-videos)`
+
+## File output
+
+### Container
+
+The default output container is `mkv` format. This can be changed with the `--container` flag to anything that is supported by FFMPEG and the chosen video and audio codecs
+
+## Video output
+
+Default settings is HEVC/x265 at quality of 23
+
+### Codecs
+
+Currently only HEVC (x265) and AVC (h264) are supported for video codecs.
+
+### Resizing
+
+Videos can be resized automatically by providing a width. Height is automatically calculated to ensure that the aspect ratio is maintained.
+
+### Hardware Acceleration
+
+Hardware acceleration is supported on nVidia and Intel devices.
+
+Caveats for nVidia:
+
+- Conversions use constqp mode for the quality setting instead of CRF, as nvenc does not support CRF
+- b-frames are not currently supported; nvenc itself supports them on 20xx+ series graphics cards.
+
+Caveats for Intel:
+
+- Conversions use global_quality mode as CRF isn't supported on Intel hardware. ICQ and LA-ICQ are apparently better, but only supported on Windows
+- Look-ahead is only supported on x264 (not HEVC)
+- There is a bug (current as of 2023-05) where all videos converted with Intel's QSV with FFMPEG have a single I-frame at the start and no more; so currently this is unsuable
+
+## Audio output
+
+Default settings is 160kbps 2 channel AAC.
+
+All audio streams will be included by default unless a language filter is specified with `--audio-language`.
+
+## Subtitles
+
+All subtitles will be copied from the source if they exist unless a language filter is specified with `--subtitle-language`.
+
```

