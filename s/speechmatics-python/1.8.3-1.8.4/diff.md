# Comparing `tmp/speechmatics-python-1.8.3.tar.gz` & `tmp/speechmatics-python-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechmatics-python-1.8.3.tar", last modified: Fri May 26 12:06:28 2023, max compression
+gzip compressed data, was "speechmatics-python-1.8.4.tar", last modified: Wed Jul  5 09:06:20 2023, max compression
```

## Comparing `speechmatics-python-1.8.3.tar` & `speechmatics-python-1.8.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-05-26 12:06:28.611637 speechmatics-python-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 12:06:28.611637 speechmatics-python-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/speechmatics/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/batch_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27404 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/speechmatics_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/mock_rt_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_cli_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/speechmatics/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/batch_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28496 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/speechmatics/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/speechmatics_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 09:06:20.000000 speechmatics-python-1.8.4/speechmatics_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:20.938053 speechmatics-python-1.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/mock_rt_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25863 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_cli_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-05 09:06:09.000000 speechmatics-python-1.8.4/tests/utils.py
```

### Comparing `speechmatics-python-1.8.3/CHANGELOG.md` & `speechmatics-python-1.8.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.9.0] - 2023-06-07
+
+### Fixed
+
+- Fix error when language provided is whitespace
+
+### Added
+
+- Add support for transcript summarization
+- Example of using notifications
+
 ## [1.8.3]
 
 ### Added
 
 - Pass sdk information to batch and rt requests
 - Add support for providing just auth_token ConnectionSettings
 - Use default URLs + .toml config in python sdk
@@ -288,15 +299,20 @@
 
 ## [0.0.10] - 2020-10-01
 
 ### Added
 
 - Added authentication token support for RT-SaaS [@rakeshv247](https://github.com/rakeshv247).
 
-[unreleased]: https://github.com/speechmatics/speechmatics-python/compare/v1.7.0...HEAD
+[unreleased]: https://github.com/speechmatics/speechmatics-python/compare/v1.9.0...HEAD
+[1.9.0]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.9.0
+[1.8.3]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.8.3
+[1.8.2]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.8.2
+[1.8.1]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.8.1
+[1.8.0]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.8.0
 [1.7.0]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.7.0
 [1.6.4]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.6.4
 [1.6.3]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.6.3
 [1.6.2]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.6.2
 [1.6.1]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.6.1
 [1.6.0]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.6.0
 [1.5.0]: https://github.com/speechmatics/speechmatics-python/releases/tag/1.5.0
```

### Comparing `speechmatics-python-1.8.3/LICENSE.txt` & `speechmatics-python-1.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/PKG-INFO` & `speechmatics-python-1.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.8.3
+Version: 1.8.4
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
@@ -118,209 +118,215 @@
 
 ## Example command-line usage
 
 A complete list of commands and flags can be found in the SDK docs at https://speechmatics.github.io/speechmatics-python/.
 
   ### Configuring Auth Tokens
 - Setting an auth token for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --auth-token $AUTH_TOKEN
    ```
   Auth tokens are stored in toml config at HOME_DIR/.speechmatics/config.
   You may also set the auth_token for each CLI command using the --auth-token flag.
   The --auth-token flag overrides the value stored in the config file, e.g.
-   ```shell
+   ```bash
    speechmatics transcribe --auth-token $AUTH_TOKEN --generate-temp-token example_audio.wav
    ```
 
 - Removing an auth_token from the toml file:
-   ```shell
+   ```bash
    speechmatics config unset --auth-token
    ```
 
 - Setting --generate-temp-token flag globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --generate-temp-token
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config unset --generate-temp-token
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
 - Real-time transcription of online stream (needs ffmpeg installed):
-  ```shell
+  ```bash
   ffmpeg -v 0 -i https://cdn.bitmovin.com/content/assets/art-of-motion-dash-hls-progressive/mpds/f08e80da-bf1d-4e3d-8899-f0f6155f6efa.mpd \
   -f s16le -ar 44100 -ac 1 -acodec pcm_s16le - | \
   speechmatics transcribe --raw pcm_s16le --sample-rate 44100 --generate-temp-token -
 
 - Starting a real-time session for enterprise SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the a SaaS enterprise runtime
    URL=wss://neu.rt.speechmatics.com/v2/en
 
    speechmatics transcribe --url $URL example_audio.wav
    ```
 
 - Starting a real-time session for on-prem customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the local instance of the realtime appliance
    URL=ws://realtimeappliance.yourcompany:9000/v2
 
    speechmatics transcribe --url $URL --lang en --ssl-mode none example_audio.wav
    ```
 
 - Show the messages that are going over the websocket connection using verbose output:
 
-   ```shell
+   ```bash
    speechmatics -v transcribe --url $URL --ssl-mode none example_audio.wav
    ```
 
 - The CLI also accepts an audio stream on standard input.
   Transcribe the piped input audio:
 
-   ```shell
+   ```bash
    cat example_audio.wav | speechmatics transcribe --url $URL --ssl-mode none -
    ```
 
 - Pipe audio directly from the microphone (example uses MacOS with [ffmpeg](https://ffmpeg.org/ffmpeg-devices.html#avfoundation))
 
   List available input devices:
 
-  ```shell
+  ```bash
   ffmpeg -f avfoundation -list_devices true -i ""
   ```
 
   There needs to be at least one available microphone attached to your computer.
   The command below gets the microphone input and pipes it to the transcriber.
   You may need to change the sample rate to match the sample rate that your machine records at.
   You may also need to replace `:default` with something like `:0` or `:1` if you want to use a specific microphone.
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f avfoundation -i ":default" -f f32le -acodec pcm_f32le -ar 44100 - \
   >   | speechmatics transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 -
   ```
 
 - Transcribe in real-time with partials (example uses Ubuntu with ALSA).
   In this mode, the transcription engine produces words instantly, which may get updated as additional context becomes available.
 
   List available input devices:
 
-  ```shell
+  ```bash
   cat /proc/asound/cards
   ```
 
   Record microphone audio and pipe to transcriber:
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics transcribe --url $URL --ssl-mode none --enable-partials --raw pcm_f32le --sample-rate 44100 -
   ```
 
   Add the `--print-json` argument to see the raw JSON transcript messages being sent rather than just the plaintext transcript.
 
   ### Batch ASR
 - Submit a .wav file for batch ASR processing
 
-   ```shell
+   ```bash
    speechmatics batch transcribe --lang en example_audio.wav
    ```
 
 - Files may be submitted for asynchronous processing
 
-    ```shell
+    ```bash
    speechmatics batch submit example_audio.wav
     ```
 
 - Enterprise SaaS and on-prem customers can point to a custom runtime:
 
-   ```shell
+   ```bash
    # Point URL to a custom runtime (in this case, the trial runtime)
    URL=https://trial.asr.api.speechmatics.com/v2/
 
    speechmatics batch transcribe --url $URL example_audio.wav
    ```
 
 - Check processing status of a job
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch job-status --job-id $JOB_ID
     ```
 
 - Retrieve completed transcription
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch get-results --job-id $JOB_ID
     ```
   
 - Submit a job with automatic language identification
 
-    ```shell
+    ```bash
    speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
 - Submit a job with translation
 
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
+    ```bash
+  speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
     ```
   `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
   
   When combining language identification with translation, we can't know if the identified language can be translated
   to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
 
 - Start a real-time transcription with translation session using microphone audio and pipe to transcriber
 
-  ```shell
-  $ ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
+  ```bash
+  ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics rt transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 \
   --print-json --translation-langs fr -
   ```
 
+- Submit a job with summarization
+
+  ```bash
+  speechmatics batch transcribe --summarize --output-format json-v2 example_audio.wav
+    ```
+
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
-    ```shell
+    ```bash
   speechmatics transcribe --config-file transcription_config.json example_audio.wav
     ```
 - The format of this JSON file is described in detail in the 
   [Batch API documentation](https://docs.speechmatics.com/jobsapi#tag/TranscriptionConfig)
   and [RT API documentation](https://docs.speechmatics.com/rt-api-ref#transcription-config).
```

### Comparing `speechmatics-python-1.8.3/README.md` & `speechmatics-python-1.8.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -95,209 +95,215 @@
 
 ## Example command-line usage
 
 A complete list of commands and flags can be found in the SDK docs at https://speechmatics.github.io/speechmatics-python/.
 
   ### Configuring Auth Tokens
 - Setting an auth token for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --auth-token $AUTH_TOKEN
    ```
   Auth tokens are stored in toml config at HOME_DIR/.speechmatics/config.
   You may also set the auth_token for each CLI command using the --auth-token flag.
   The --auth-token flag overrides the value stored in the config file, e.g.
-   ```shell
+   ```bash
    speechmatics transcribe --auth-token $AUTH_TOKEN --generate-temp-token example_audio.wav
    ```
 
 - Removing an auth_token from the toml file:
-   ```shell
+   ```bash
    speechmatics config unset --auth-token
    ```
 
 - Setting --generate-temp-token flag globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --generate-temp-token
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config unset --generate-temp-token
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
 - Real-time transcription of online stream (needs ffmpeg installed):
-  ```shell
+  ```bash
   ffmpeg -v 0 -i https://cdn.bitmovin.com/content/assets/art-of-motion-dash-hls-progressive/mpds/f08e80da-bf1d-4e3d-8899-f0f6155f6efa.mpd \
   -f s16le -ar 44100 -ac 1 -acodec pcm_s16le - | \
   speechmatics transcribe --raw pcm_s16le --sample-rate 44100 --generate-temp-token -
 
 - Starting a real-time session for enterprise SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the a SaaS enterprise runtime
    URL=wss://neu.rt.speechmatics.com/v2/en
 
    speechmatics transcribe --url $URL example_audio.wav
    ```
 
 - Starting a real-time session for on-prem customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the local instance of the realtime appliance
    URL=ws://realtimeappliance.yourcompany:9000/v2
 
    speechmatics transcribe --url $URL --lang en --ssl-mode none example_audio.wav
    ```
 
 - Show the messages that are going over the websocket connection using verbose output:
 
-   ```shell
+   ```bash
    speechmatics -v transcribe --url $URL --ssl-mode none example_audio.wav
    ```
 
 - The CLI also accepts an audio stream on standard input.
   Transcribe the piped input audio:
 
-   ```shell
+   ```bash
    cat example_audio.wav | speechmatics transcribe --url $URL --ssl-mode none -
    ```
 
 - Pipe audio directly from the microphone (example uses MacOS with [ffmpeg](https://ffmpeg.org/ffmpeg-devices.html#avfoundation))
 
   List available input devices:
 
-  ```shell
+  ```bash
   ffmpeg -f avfoundation -list_devices true -i ""
   ```
 
   There needs to be at least one available microphone attached to your computer.
   The command below gets the microphone input and pipes it to the transcriber.
   You may need to change the sample rate to match the sample rate that your machine records at.
   You may also need to replace `:default` with something like `:0` or `:1` if you want to use a specific microphone.
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f avfoundation -i ":default" -f f32le -acodec pcm_f32le -ar 44100 - \
   >   | speechmatics transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 -
   ```
 
 - Transcribe in real-time with partials (example uses Ubuntu with ALSA).
   In this mode, the transcription engine produces words instantly, which may get updated as additional context becomes available.
 
   List available input devices:
 
-  ```shell
+  ```bash
   cat /proc/asound/cards
   ```
 
   Record microphone audio and pipe to transcriber:
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics transcribe --url $URL --ssl-mode none --enable-partials --raw pcm_f32le --sample-rate 44100 -
   ```
 
   Add the `--print-json` argument to see the raw JSON transcript messages being sent rather than just the plaintext transcript.
 
   ### Batch ASR
 - Submit a .wav file for batch ASR processing
 
-   ```shell
+   ```bash
    speechmatics batch transcribe --lang en example_audio.wav
    ```
 
 - Files may be submitted for asynchronous processing
 
-    ```shell
+    ```bash
    speechmatics batch submit example_audio.wav
     ```
 
 - Enterprise SaaS and on-prem customers can point to a custom runtime:
 
-   ```shell
+   ```bash
    # Point URL to a custom runtime (in this case, the trial runtime)
    URL=https://trial.asr.api.speechmatics.com/v2/
 
    speechmatics batch transcribe --url $URL example_audio.wav
    ```
 
 - Check processing status of a job
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch job-status --job-id $JOB_ID
     ```
 
 - Retrieve completed transcription
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch get-results --job-id $JOB_ID
     ```
   
 - Submit a job with automatic language identification
 
-    ```shell
+    ```bash
    speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
 - Submit a job with translation
 
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
+    ```bash
+  speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
     ```
   `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
   
   When combining language identification with translation, we can't know if the identified language can be translated
   to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
 
 - Start a real-time transcription with translation session using microphone audio and pipe to transcriber
 
-  ```shell
-  $ ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
+  ```bash
+  ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics rt transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 \
   --print-json --translation-langs fr -
   ```
 
+- Submit a job with summarization
+
+  ```bash
+  speechmatics batch transcribe --summarize --output-format json-v2 example_audio.wav
+    ```
+
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
-    ```shell
+    ```bash
   speechmatics transcribe --config-file transcription_config.json example_audio.wav
     ```
 - The format of this JSON file is described in detail in the 
   [Batch API documentation](https://docs.speechmatics.com/jobsapi#tag/TranscriptionConfig)
   and [RT API documentation](https://docs.speechmatics.com/rt-api-ref#transcription-config).
```

### Comparing `speechmatics-python-1.8.3/setup.py` & `speechmatics-python-1.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/adapters.py` & `speechmatics-python-1.8.4/speechmatics/adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/batch_client.py` & `speechmatics-python-1.8.4/speechmatics/batch_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/cli.py` & `speechmatics-python-1.8.4/speechmatics/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     BatchSpeakerDiarizationConfig,
     BatchTranscriptionConfig,
     ClientMessageType,
     ConnectionSettings,
     RTSpeakerDiarizationConfig,
     RTTranslationConfig,
     ServerMessageType,
+    SummarizationConfig,
     TranscriptionConfig,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 
 def print_symbol(symbol):
@@ -150,15 +151,15 @@
         if url is None and args.get("mode") == "rt" and "realtime_url" in stored_config:
             url = stored_config.get("realtime_url")
 
     if url is None:
         if args.get("mode") == "batch":
             url = BATCH_SELF_SERVICE_URL
         else:
-            url = f"{RT_SELF_SERVICE_URL}/{lang}"
+            url = f"{RT_SELF_SERVICE_URL}/{lang.strip()}"
 
     settings = ConnectionSettings(
         url=url,
         auth_token=auth_token,
         generate_temp_token=generate_temp_token,
     )
 
@@ -170,15 +171,17 @@
         settings.ssl_context.verify_mode = ssl.CERT_NONE
     elif args.get("ssl_mode") == "none":
         settings.ssl_context = None
 
     return settings
 
 
-def get_transcription_config(args):  # pylint: disable=too-many-branches
+def get_transcription_config(
+    args,
+):  # pylint: disable=too-many-branches, too-many-locals, too-many-statements
     """
     Helper function which returns a TranscriptionConfig object based on the
     command line options given to the program.
 
     :param args: Keyword arguments probably from the command line.
     :type args: dict
 
@@ -284,14 +287,37 @@
 
     if args.get("langid_expected_languages") is not None:
         langid_expected_languages = args.get("langid_expected_languages")
         config["language_identification_config"] = BatchLanguageIdentificationConfig(
             expected_languages=langid_expected_languages.split(",")
         )
 
+    # request summarization from config file
+    file_summarization_config = config.get("summarization_config", {})
+    # request summarization from cli
+    args_summarization = args.get("summarize")
+    if args_summarization or config.get("summarization_config") is not None:
+        summarization_config = SummarizationConfig()
+        content_type = args.get(
+            "content_type", file_summarization_config.get("content_type")
+        )
+        if content_type:
+            summarization_config.content_type = content_type
+        summary_length = args.get(
+            "summary_length", file_summarization_config.get("summary_length")
+        )
+        if summary_length:
+            summarization_config.summary_length = summary_length
+        summary_type = args.get(
+            "summary_type", file_summarization_config.get("summary_type")
+        )
+        if summary_type:
+            summarization_config.summary_type = summary_type
+        config["summarization_config"] = summarization_config
+
     if args["mode"] == "rt":
         # pylint: disable=unexpected-keyword-arg
         return TranscriptionConfig(**config)
     # pylint: disable=unexpected-keyword-arg
     return BatchTranscriptionConfig(**config)
```

### Comparing `speechmatics-python-1.8.3/speechmatics/cli_parser.py` & `speechmatics-python-1.8.4/speechmatics/cli_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,14 +230,48 @@
         "--langid-languages",
         dest="langid_expected_languages",
         type=str,
         default=None,
         help=("Comma-separated list of expected languages for language identification"),
     )
 
+    # Parent parser for batch summarize argument
+    batch_summarization_parser = argparse.ArgumentParser(add_help=False)
+    batch_summarization_parser.add_argument(
+        "--summarize",
+        dest="summarize",
+        action="store_true",
+        default=False,
+        help="Whether to generate transcript summarization",
+    )
+    batch_summarization_parser.add_argument(
+        "--summary-content-type",
+        dest="content_type",
+        default=None,
+        choices=["informative", "conversational", "auto"],
+        type=str,
+        required=False,
+    )
+    batch_summarization_parser.add_argument(
+        "--summary-length",
+        dest="summary_length",
+        default=None,
+        choices=["brief", "detailed"],
+        type=str,
+        required=False,
+    )
+    batch_summarization_parser.add_argument(
+        "--summary-type",
+        dest="summary_type",
+        default=None,
+        choices=["paragraphs", "bullets"],
+        type=str,
+        required=False,
+    )
+
     # Parent parser for output type
     output_format_parser = argparse.ArgumentParser(add_help=False)
     output_format_parser.add_argument(
         "--output-format",
         default="txt",
         choices=["txt", "json", "json-v2", "srt"],
         type=str,
@@ -411,26 +445,28 @@
         "transcribe",
         parents=[
             file_parser,
             connection_parser,
             config_parser,
             output_format_parser,
             batch_diarization_parser,
+            batch_summarization_parser,
         ],
         help="Transcribe one or more audio files using batch mode, while waiting for results.",
     )
 
     batch_subparsers.add_parser(
         "submit",
         parents=[
             file_parser,
             connection_parser,
             config_parser,
             output_format_parser,
             batch_diarization_parser,
+            batch_summarization_parser,
         ],
         help="Submit one or more files for transcription.",
     )
 
     batch_subparsers.add_parser(
         "list-jobs",
         parents=[connection_parser],
```

### Comparing `speechmatics-python-1.8.3/speechmatics/client.py` & `speechmatics-python-1.8.4/speechmatics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,19 +452,19 @@
             and self.connection_settings.auth_token is not None
         ):
             temp_token = await _get_temp_token(self.connection_settings.auth_token)
             token = f"Bearer {temp_token}"
             extra_headers["Authorization"] = token
 
         url = self.connection_settings.url
-        if not url.endswith(self.transcription_config.language):
+        if not url.endswith(self.transcription_config.language.strip()):
             if url.endswith("/"):
-                url += self.transcription_config.language
+                url += self.transcription_config.language.strip()
             else:
-                url += f"/{self.transcription_config.language}"
+                url += f"/{self.transcription_config.language.strip()}"
 
         # Extend connection url with sdk version information
         cli = "-cli" if from_cli is True else ""
         version = get_version()
         parsed_url = urlparse(url)
         query_params = dict(parse_qsl(parsed_url.query))
         query_params["sm-sdk"] = f"python{cli}-{version}"
```

### Comparing `speechmatics-python-1.8.3/speechmatics/config.py` & `speechmatics-python-1.8.4/speechmatics/config.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/exceptions.py` & `speechmatics-python-1.8.4/speechmatics/exceptions.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/helpers.py` & `speechmatics-python-1.8.4/speechmatics/helpers.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/speechmatics/models.py` & `speechmatics-python-1.8.4/speechmatics/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # (c) 2020, Cantab Research Ltd.
 """
 Data models and message types used by the library.
 """
 
 import json
 import ssl
+import sys
 from dataclasses import asdict, dataclass, field, fields
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from speechmatics.config import CONFIG_PATH, read_config_from_home
 from speechmatics.constants import BATCH_SELF_SERVICE_URL, RT_SELF_SERVICE_URL
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal  # pragma: no cover
+
+
+SummaryContentType = Literal["informative", "conversational", "auto"]
+SummaryLength = Literal["brief", "detailed"]
+SummaryType = Literal["paragraphs", "bullets"]
+
 
 @dataclass
 class FetchData:
     """Batch: Optional configuration for fetching file for transcription."""
 
     url: str
     """URL to fetch"""
@@ -165,14 +176,28 @@
 class BatchLanguageIdentificationConfig:
     """Batch mode: Language identification config."""
 
     expected_languages: List[str] = None
     """Expected languages for language identification"""
 
 
+@dataclass
+class SummarizationConfig:
+    """Defines summarization parameters."""
+
+    content_type: SummaryContentType = "auto"
+    """Optional summarization content_type parameter."""
+
+    summary_length: SummaryLength = "brief"
+    """Optional summarization summary_length parameter."""
+
+    summary_type: SummaryType = "bullets"
+    """Optional summarization summary_type parameter."""
+
+
 @dataclass(init=False)
 class TranscriptionConfig(_TranscriptionConfig):
     # pylint: disable=too-many-instance-attributes
     """
     Real-time: Defines transcription parameters.
     The `.as_config()` method removes translation_config and returns it wrapped into a Speechmatics json config.
     """
@@ -220,14 +245,15 @@
             dictionary["enable_partials"] = True
 
         return dictionary
 
 
 @dataclass(init=False)
 class BatchTranscriptionConfig(_TranscriptionConfig):
+    # pylint: disable=too-many-instance-attributes
     """Batch: Defines transcription parameters for batch requests.
     The `.as_config()` method will return it wrapped into a Speechmatics json config."""
 
     fetch_data: FetchData = None
     """Optional configuration for fetching file for transcription."""
 
     notification_config: NotificationConfig = None
@@ -244,24 +270,28 @@
 
     speaker_diarization_config: BatchSpeakerDiarizationConfig = None
     """The sensitivity of the speaker detection."""
 
     channel_diarization_labels: List[str] = None
     """Add your own speaker or channel labels to the transcript"""
 
+    summarization_config: SummarizationConfig = None
+    """Optional configuration for transcript summarization."""
+
     def as_config(self):
         dictionary = self.asdict()
 
         fetch_data = dictionary.pop("fetch_data", None)
         notification_config = dictionary.pop("notification_config", None)
         language_identification_config = dictionary.pop(
             "language_identification_config", None
         )
         translation_config = dictionary.pop("translation_config", None)
         srt_overrides = dictionary.pop("srt_overrides", None)
+        summarization_config = dictionary.pop("summarization_config", None)
 
         config = {"type": "transcription", "transcription_config": dictionary}
 
         if fetch_data:
             config["fetch_data"] = fetch_data
 
         if notification_config:
@@ -274,14 +304,17 @@
 
         if translation_config:
             config["translation_config"] = translation_config
 
         if srt_overrides:
             config["output_config"] = {"srt_overrides": srt_overrides}
 
+        if summarization_config:
+            config["summarization_config"] = summarization_config
+
         return json.dumps(config)
 
 
 @dataclass
 class AudioSettings:
     """Real-time: Defines audio parameters."""
```

### Comparing `speechmatics-python-1.8.3/speechmatics_python.egg-info/PKG-INFO` & `speechmatics-python-1.8.4/speechmatics_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.8.3
+Version: 1.8.4
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
@@ -118,209 +118,215 @@
 
 ## Example command-line usage
 
 A complete list of commands and flags can be found in the SDK docs at https://speechmatics.github.io/speechmatics-python/.
 
   ### Configuring Auth Tokens
 - Setting an auth token for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --auth-token $AUTH_TOKEN
    ```
   Auth tokens are stored in toml config at HOME_DIR/.speechmatics/config.
   You may also set the auth_token for each CLI command using the --auth-token flag.
   The --auth-token flag overrides the value stored in the config file, e.g.
-   ```shell
+   ```bash
    speechmatics transcribe --auth-token $AUTH_TOKEN --generate-temp-token example_audio.wav
    ```
 
 - Removing an auth_token from the toml file:
-   ```shell
+   ```bash
    speechmatics config unset --auth-token
    ```
 
 - Setting --generate-temp-token flag globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config set --generate-temp-token
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
-   ```shell
+   ```bash
    speechmatics config unset --generate-temp-token
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
 - Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
-   ```shell
+   ```bash
    speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
    ```
 
 - Unsetting transcriber URLs in the toml config:
-   ```shell
+   ```bash
    speechmatics config unset --rt-url --batch-url
    ```
 
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
 - Real-time transcription of online stream (needs ffmpeg installed):
-  ```shell
+  ```bash
   ffmpeg -v 0 -i https://cdn.bitmovin.com/content/assets/art-of-motion-dash-hls-progressive/mpds/f08e80da-bf1d-4e3d-8899-f0f6155f6efa.mpd \
   -f s16le -ar 44100 -ac 1 -acodec pcm_s16le - | \
   speechmatics transcribe --raw pcm_s16le --sample-rate 44100 --generate-temp-token -
 
 - Starting a real-time session for enterprise SaaS customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the a SaaS enterprise runtime
    URL=wss://neu.rt.speechmatics.com/v2/en
 
    speechmatics transcribe --url $URL example_audio.wav
    ```
 
 - Starting a real-time session for on-prem customers using a .wav file as the input audio:
 
-   ```shell
+   ```bash
    # Point URL to the local instance of the realtime appliance
    URL=ws://realtimeappliance.yourcompany:9000/v2
 
    speechmatics transcribe --url $URL --lang en --ssl-mode none example_audio.wav
    ```
 
 - Show the messages that are going over the websocket connection using verbose output:
 
-   ```shell
+   ```bash
    speechmatics -v transcribe --url $URL --ssl-mode none example_audio.wav
    ```
 
 - The CLI also accepts an audio stream on standard input.
   Transcribe the piped input audio:
 
-   ```shell
+   ```bash
    cat example_audio.wav | speechmatics transcribe --url $URL --ssl-mode none -
    ```
 
 - Pipe audio directly from the microphone (example uses MacOS with [ffmpeg](https://ffmpeg.org/ffmpeg-devices.html#avfoundation))
 
   List available input devices:
 
-  ```shell
+  ```bash
   ffmpeg -f avfoundation -list_devices true -i ""
   ```
 
   There needs to be at least one available microphone attached to your computer.
   The command below gets the microphone input and pipes it to the transcriber.
   You may need to change the sample rate to match the sample rate that your machine records at.
   You may also need to replace `:default` with something like `:0` or `:1` if you want to use a specific microphone.
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f avfoundation -i ":default" -f f32le -acodec pcm_f32le -ar 44100 - \
   >   | speechmatics transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 -
   ```
 
 - Transcribe in real-time with partials (example uses Ubuntu with ALSA).
   In this mode, the transcription engine produces words instantly, which may get updated as additional context becomes available.
 
   List available input devices:
 
-  ```shell
+  ```bash
   cat /proc/asound/cards
   ```
 
   Record microphone audio and pipe to transcriber:
 
-  ```shell
+  ```bash
   ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics transcribe --url $URL --ssl-mode none --enable-partials --raw pcm_f32le --sample-rate 44100 -
   ```
 
   Add the `--print-json` argument to see the raw JSON transcript messages being sent rather than just the plaintext transcript.
 
   ### Batch ASR
 - Submit a .wav file for batch ASR processing
 
-   ```shell
+   ```bash
    speechmatics batch transcribe --lang en example_audio.wav
    ```
 
 - Files may be submitted for asynchronous processing
 
-    ```shell
+    ```bash
    speechmatics batch submit example_audio.wav
     ```
 
 - Enterprise SaaS and on-prem customers can point to a custom runtime:
 
-   ```shell
+   ```bash
    # Point URL to a custom runtime (in this case, the trial runtime)
    URL=https://trial.asr.api.speechmatics.com/v2/
 
    speechmatics batch transcribe --url $URL example_audio.wav
    ```
 
 - Check processing status of a job
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch job-status --job-id $JOB_ID
     ```
 
 - Retrieve completed transcription
 
-    ```shell
+    ```bash
    # $JOB_ID is from the submit command output
    speechmatics batch get-results --job-id $JOB_ID
     ```
   
 - Submit a job with automatic language identification
 
-    ```shell
+    ```bash
    speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
 - Submit a job with translation
 
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
+    ```bash
+  speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
     ```
   `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
   
   When combining language identification with translation, we can't know if the identified language can be translated
   to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
 
 - Start a real-time transcription with translation session using microphone audio and pipe to transcriber
 
-  ```shell
-  $ ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
+  ```bash
+  ffmpeg -loglevel quiet -f alsa -i hw:0 -f f32le -acodec pcm_f32le -ar 44100 - \
       | speechmatics rt transcribe --url $URL --ssl-mode none --raw pcm_f32le --sample-rate 44100 \
   --print-json --translation-langs fr -
   ```
 
+- Submit a job with summarization
+
+  ```bash
+  speechmatics batch transcribe --summarize --output-format json-v2 example_audio.wav
+    ```
+
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
-    ```shell
+    ```bash
   speechmatics transcribe --config-file transcription_config.json example_audio.wav
     ```
 - The format of this JSON file is described in detail in the 
   [Batch API documentation](https://docs.speechmatics.com/jobsapi#tag/TranscriptionConfig)
   and [RT API documentation](https://docs.speechmatics.com/rt-api-ref#transcription-config).
```

### Comparing `speechmatics-python-1.8.3/speechmatics_python.egg-info/SOURCES.txt` & `speechmatics-python-1.8.4/speechmatics_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/conftest.py` & `speechmatics-python-1.8.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/mock_rt_server.py` & `speechmatics-python-1.8.4/tests/mock_rt_server.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/test_adapters.py` & `speechmatics-python-1.8.4/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/test_cli.py` & `speechmatics-python-1.8.4/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,14 +246,58 @@
                 "submit",
                 "--langid-langs=de,es,cs",
             ],
             {
                 "langid_expected_languages": "de,es,cs",
             },
         ),
+        (
+            ["batch", "transcribe", "--summarize"],
+            {
+                "summarize": True,
+            },
+        ),
+        (
+            [
+                "batch",
+                "transcribe",
+                "--summarize",
+                "--summary-content-type=informative",
+            ],
+            {
+                "summarize": True,
+                "content_type": "informative",
+            },
+        ),
+        (
+            [
+                "batch",
+                "transcribe",
+                "--summarize",
+                "--summary-content-type=informative",
+            ],
+            {
+                "summarize": True,
+                "content_type": "informative",
+            },
+        ),
+        (
+            ["batch", "transcribe", "--summarize", "--summary-length=detailed"],
+            {
+                "summarize": True,
+                "summary_length": "detailed",
+            },
+        ),
+        (
+            ["batch", "transcribe", "--summarize", "--summary-type=paragraphs"],
+            {
+                "summarize": True,
+                "summary_type": "paragraphs",
+            },
+        ),
     ],
 )
 def test_cli_arg_parse_with_file(args, values):
     common_transcribe_args = ["--auth-token=xyz", "--url=example", "fake_file.wav"]
     test_args = args + common_transcribe_args
     actual_values = vars(cli.parse_args(args=test_args))
```

### Comparing `speechmatics-python-1.8.3/tests/test_cli_handlers.py` & `speechmatics-python-1.8.4/tests/test_cli_handlers.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/test_client.py` & `speechmatics-python-1.8.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.3/tests/utils.py` & `speechmatics-python-1.8.4/tests/utils.py`

 * *Files identical despite different names*

