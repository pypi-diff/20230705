# Comparing `tmp/asciinema-2.2.0.tar.gz` & `tmp/asciinema-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciinema-2.2.0.tar", last modified: Sat May  7 19:10:09 2022, max compression
+gzip compressed data, was "asciinema-2.3.0.tar", last modified: Wed Jul  5 14:10:09 2023, max compression
```

## Comparing `asciinema-2.2.0.tar` & `asciinema-2.3.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/
--rw-r--r--   0 marcin    (1000) marcin    (1000)     8351 2022-05-07 18:33:47.000000 asciinema-2.2.0/CHANGELOG.md
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     3229 2022-02-13 21:57:25.000000 asciinema-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 marcin    (1000) marcin    (1000)     4048 2022-05-07 18:30:58.000000 asciinema-2.2.0/CONTRIBUTING.md
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    35147 2022-02-13 21:57:25.000000 asciinema-2.2.0/LICENSE
--rw-r--r--   0 marcin    (1000) marcin    (1000)    16523 2022-05-07 19:10:09.732002 asciinema-2.2.0/PKG-INFO
--rw-r--r--   0 marcin    (1000) marcin    (1000)    15451 2022-05-07 18:33:47.000000 asciinema-2.2.0/README.md
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.731002 asciinema-2.2.0/asciinema/
--rw-r--r--   0 marcin    (1000) marcin    (1000)      801 2022-05-07 18:33:20.000000 asciinema-2.2.0/asciinema/__init__.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     6629 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/__main__.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     3125 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/api.py
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/asciinema/asciicast/
--rw-r--r--   0 marcin    (1000) marcin    (1000)     4404 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/asciicast/__init__.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1061 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/asciicast/events.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1322 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/asciicast/raw.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1779 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/asciicast/v1.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     4896 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/asciicast/v2.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1450 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/async_worker.py
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/asciinema/commands/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        0 2022-02-13 21:57:25.000000 asciinema-2.2.0/asciinema/commands/__init__.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)      741 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/auth.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)      862 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/cat.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)      980 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/command.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1141 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/play.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     5507 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/record.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)      891 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/commands/upload.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     6737 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/config.py
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/asciinema/data/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    25280 2022-02-20 16:03:23.000000 asciinema-2.2.0/asciinema/data/icon-256x256.png
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1206 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/file_writer.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       47 2022-02-13 21:57:25.000000 asciinema-2.2.0/asciinema/http_adapter.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     3299 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/notifier.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     3222 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/player.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     5331 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/pty_.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     5750 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/recorder.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1022 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/tty_.py
--rw-r--r--   0 marcin    (1000) marcin    (1000)     4225 2022-05-07 18:27:47.000000 asciinema-2.2.0/asciinema/urllib_http_adapter.py
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.731002 asciinema-2.2.0/asciinema.egg-info/
--rw-r--r--   0 marcin    (1000) marcin    (1000)    16523 2022-05-07 19:10:09.000000 asciinema-2.2.0/asciinema.egg-info/PKG-INFO
--rw-r--r--   0 marcin    (1000) marcin    (1000)      977 2022-05-07 19:10:09.000000 asciinema-2.2.0/asciinema.egg-info/SOURCES.txt
--rw-r--r--   0 marcin    (1000) marcin    (1000)        1 2022-05-07 19:10:09.000000 asciinema-2.2.0/asciinema.egg-info/dependency_links.txt
--rw-r--r--   0 marcin    (1000) marcin    (1000)       54 2022-05-07 19:10:09.000000 asciinema-2.2.0/asciinema.egg-info/entry_points.txt
--rw-r--r--   0 marcin    (1000) marcin    (1000)       10 2022-05-07 19:10:09.000000 asciinema-2.2.0/asciinema.egg-info/top_level.txt
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/doc/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     2104 2022-02-13 21:57:25.000000 asciinema-2.2.0/doc/asciicast-v1.md
--rw-r--r--   0 marcin    (1000) marcin    (1000)     5747 2022-05-07 18:27:47.000000 asciinema-2.2.0/doc/asciicast-v2.md
-drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2022-05-07 19:10:09.732002 asciinema-2.2.0/man/
--rw-r--r--   0 marcin    (1000) marcin    (1000)    11170 2022-05-07 18:27:47.000000 asciinema-2.2.0/man/asciinema.1
--rw-r--r--   0 marcin    (1000) marcin    (1000)      834 2022-05-07 18:27:47.000000 asciinema-2.2.0/pyproject.toml
--rw-r--r--   0 marcin    (1000) marcin    (1000)     1486 2022-05-07 19:10:09.733002 asciinema-2.2.0/setup.cfg
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     9309 2023-07-05 13:50:05.000000 asciinema-2.3.0/CHANGELOG.md
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     3229 2022-02-13 21:57:25.000000 asciinema-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     4048 2023-04-24 19:43:02.000000 asciinema-2.3.0/CONTRIBUTING.md
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    35147 2022-02-13 21:57:25.000000 asciinema-2.3.0/LICENSE
+-rw-r--r--   0 marcin    (1000) marcin    (1000)    18700 2023-07-05 14:10:09.661268 asciinema-2.3.0/PKG-INFO
+-rw-r--r--   0 marcin    (1000) marcin    (1000)    17647 2023-07-05 13:50:05.000000 asciinema-2.3.0/README.md
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.657934 asciinema-2.3.0/asciinema/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      801 2023-07-05 13:51:13.000000 asciinema-2.3.0/asciinema/__init__.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     7547 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/__main__.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     3263 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/api.py
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/asciinema/asciicast/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     4412 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/asciicast/__init__.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      978 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/asciicast/events.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1715 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/asciicast/raw.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1842 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/asciicast/v1.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     5040 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/asciicast/v2.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1567 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/async_worker.py
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/asciinema/commands/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)        0 2022-02-13 21:57:25.000000 asciinema-2.3.0/asciinema/commands/__init__.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      741 2023-04-24 19:43:02.000000 asciinema-2.3.0/asciinema/commands/auth.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1014 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/commands/cat.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      982 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/commands/command.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1752 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/commands/play.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     6407 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/commands/record.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      933 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/commands/upload.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     6966 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/config.py
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/asciinema/data/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)    25280 2022-05-17 15:10:51.000000 asciinema-2.3.0/asciinema/data/icon-256x256.png
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      871 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/file_writer.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       47 2022-02-13 21:57:25.000000 asciinema-2.3.0/asciinema/http_adapter.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     3299 2023-04-24 19:43:02.000000 asciinema-2.3.0/asciinema/notifier.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     6057 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/player.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     6192 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/pty_.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     5833 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/recorder.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1022 2023-04-24 19:43:02.000000 asciinema-2.3.0/asciinema/tty_.py
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     4221 2023-07-05 13:50:05.000000 asciinema-2.3.0/asciinema/urllib_http_adapter.py
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/asciinema.egg-info/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)    18700 2023-07-05 14:10:09.000000 asciinema-2.3.0/asciinema.egg-info/PKG-INFO
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      998 2023-07-05 14:10:09.000000 asciinema-2.3.0/asciinema.egg-info/SOURCES.txt
+-rw-r--r--   0 marcin    (1000) marcin    (1000)        1 2023-07-05 14:10:09.000000 asciinema-2.3.0/asciinema.egg-info/dependency_links.txt
+-rw-r--r--   0 marcin    (1000) marcin    (1000)       54 2023-07-05 14:10:09.000000 asciinema-2.3.0/asciinema.egg-info/entry_points.txt
+-rw-r--r--   0 marcin    (1000) marcin    (1000)       10 2023-07-05 14:10:09.000000 asciinema-2.3.0/asciinema.egg-info/top_level.txt
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/doc/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     2104 2022-02-13 21:57:25.000000 asciinema-2.3.0/doc/asciicast-v1.md
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     6287 2023-07-05 13:50:05.000000 asciinema-2.3.0/doc/asciicast-v2.md
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/man/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)    11170 2023-04-24 19:43:02.000000 asciinema-2.3.0/man/asciinema.1
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      834 2023-04-24 19:43:02.000000 asciinema-2.3.0/pyproject.toml
+-rw-r--r--   0 marcin    (1000) marcin    (1000)     1487 2023-07-05 14:10:09.661268 asciinema-2.3.0/setup.cfg
+drwxr-xr-x   0 marcin    (1000) marcin    (1000)        0 2023-07-05 14:10:09.661268 asciinema-2.3.0/tests/
+-rw-r--r--   0 marcin    (1000) marcin    (1000)      415 2023-04-24 19:43:02.000000 asciinema-2.3.0/tests/test_helper.py
```

### Comparing `asciinema-2.2.0/CHANGELOG.md` & `asciinema-2.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # asciinema changelog
 
+## 2.3.0 (2023-07-05)
+
+* Added official support for Python 3.11
+* Dropped official support for Python 3.6
+* Implemented markers in `rec` and `play -m` commands
+* Added `--loop` option for looped playback in `play` command
+* Added `--stream` and `--out-fmt` option for customizing output of `play` command
+* Improved terminal charset detection (thanks @djds)
+* Extended `cat` command to support multiple files (thanks @Low-power)
+* Improved upload error messages
+* Fixed direct playback from URL
+* Made raw output start with terminal size sequence (`\e[8;H;Wt`)
+* Prevented recording to stdout when it's a TTY
+* Added target file permission checks to avoid ugly errors
+* Removed named pipe re-opening, which was causing hangs in certain scenarios
+* Improved PTY/TTY data reading - it goes in bigger chunks now (256 kb)
+* Fixed deadlock in PTY writes (thanks @Low-power)
+* Improved input forwarding from stdin
+* Ignored OSC responses in recorded stdin stream
+
 ## 2.2.0 (2022-05-07)
 
 * Added official support for Python 3.8, 3.9, 3.10
 * Dropped official support for Python 3.5
 * Added `--cols` / `--rows` options for overriding size of pseudo-terminal reported to recorded program
 * Improved behaviour of `--append` when output file doesn't exist
 * Keyboard input is now explicitly read from a TTY device in addition to stdin (when stdin != TTY)
```

### Comparing `asciinema-2.2.0/CODE_OF_CONDUCT.md` & `asciinema-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/CONTRIBUTING.md` & `asciinema-2.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/LICENSE` & `asciinema-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/PKG-INFO` & `asciinema-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: asciinema
-Version: 2.2.0
-Summary: Terminal session recorder
-Home-page: https://asciinema.org
-Download-URL: 
-https://github.com/asciinema/asciinema/archive/v2.2.0.tar.gz
-Author: Marcin Kulik
-Author-email: m@ku1ik.com
-License: GNU GPLv3
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Shells
-Classifier: Topic :: Terminals
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
 # asciinema
 
 [![Build Status](https://github.com/asciinema/asciinema/actions/workflows/asciinema.yml/badge.svg)](https://github.com/asciinema/asciinema/actions/workflows/asciinema.yml)
 [![PyPI](https://img.shields.io/pypi/v/asciinema.svg)](https://pypi.org/project/asciinema/)
 [![license](http://img.shields.io/badge/license-GNU-blue.svg)](https://raw.githubusercontent.com/asciinema/asciinema/master/LICENSE)
 
 Terminal session recorder and the best companion of
@@ -158,39 +129,41 @@
 ```sh
 python3 -m asciinema --version
 ```
 
 ### Docker image
 
 asciinema Docker image is based on [Ubuntu
-20.04](https://releases.ubuntu.com/20.04/) and has the latest version of
+22.04](https://releases.ubuntu.com/22.04/) and has the latest version of
 asciinema recorder pre-installed.
 
 ```sh
-docker pull docker.io/asciinema/asciinema
+docker pull ghcr.io/asciinema/asciinema
 ```
 
 When running it don't forget to allocate a pseudo-TTY (`-t`), keep STDIN open
 (`-i`) and mount config directory volume (`-v`):
 
 ```sh
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" ghcr.io/asciinema/asciinema rec
 ```
 
 Container's entrypoint is set to `/usr/local/bin/asciinema` so you can run the
 container with any arguments you would normally pass to `asciinema` binary (see
 Usage section for commands and options).
 
 There's not much software installed in this image though. In most cases you may
 want to install extra programs before recording. One option is to derive new
-image from this one (start your custom Dockerfile with `FROM asciinema/asciinema`). Another option is to start the container with `/bin/bash`
-as the entrypoint, install extra packages and manually start `asciinema rec`:
+image from this one (start your custom Dockerfile with `FROM
+ghcr.io/asciinema/asciinema`). Another option is to start the container with
+`/bin/bash` as the entrypoint, install extra packages and manually start
+`asciinema rec`:
 
 ```console
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash ghcr.io/asciinema/asciinema rec
 root@6689517d99a1:~# apt-get install foobar
 root@6689517d99a1:~# asciinema rec
 ```
 
 It is also possible to run the docker container as a non-root user, which has
 security benefits. You can specify a user and group id at runtime to give the
 application permission similar to the calling user on your host.
@@ -198,15 +171,15 @@
 ```sh
 docker run --rm -it \
     --env=ASCIINEMA_CONFIG_HOME="/run/user/$(id -u)/.config/asciinema" \
     --user="$(id -u):$(id -g)" \
     --volume="${HOME}/.config/asciinema:/run/user/$(id -u)/.config/asciinema:rw" \
     --volume="${PWD}:/data:rw" \
     --workdir='/data' \
-    docker.io/asciinema/asciinema rec
+    ghcr.io/asciinema/asciinema rec
 ```
 
 ## Usage
 
 asciinema is composed of multiple commands, similar to `git`, `apt-get` or
 `brew`.
 
@@ -261,15 +234,15 @@
 - `--rows=<n>` - Override terminal rows for recorded process
 - `-y, --yes` - Answer "yes" to all prompts (e.g. upload confirmation)
 - `-q, --quiet` - Be quiet, suppress all notices/warnings (implies -y)
 
 Stdin recording allows for capturing of all characters typed in by the user in
 the currently recorded shell. This may be used by a player (e.g.
 [asciinema-player](https://github.com/asciinema/asciinema-player)) to display
-pressed keys. Because it's basically a key-logging (scoped to a single shell
+pressed keys. Because it's basically key-logging (scoped to a single shell
 instance), it's disabled by default, and has to be explicitly enabled via
 `--stdin` option.
 
 ### `play <filename>`
 
 **Replay recorded asciicast in a terminal.**
 
@@ -318,14 +291,29 @@
 asciinema play dweb:/ipfs/QmNe7FsYaHc9SaDEAEXbaagAzNw9cH7YbzN4xV7jV1MCzK/ascii.cast
 ```
 
 Available options:
 
 - `-i, --idle-time-limit=<sec>` - Limit replayed terminal inactivity to max `<sec>` seconds
 - `-s, --speed=<factor>` - Playback speed (can be fractional)
+- `-l, --loop` - Play in a loop
+- `-m, --pause-on-markers` - Automatically pause on [markers](#markers)
+- `--stream=<stream>` - Select stream to play (see below)
+- `--out-fmt=<format>` - Select output format (see below)
+
+By default the output stream (`o`) is played. This is what you want in most
+cases.  If you recorded the input stream (`i`) with `asciinema rec --stdin` then
+you can replay it with `asciinema play --stream=i <filename>`.
+
+By default the selected stream is written to stdout in original, raw data form.
+This is also what you want in majority of cases. However you can change the
+output format to asciicast (newline delimited JSON) with `asciinema play
+--out-fmt=asciicast <filename>`. This allows delegating actual rendering to
+another place (e.g. outside of your terminal) by piping output of `asciinema
+play` to a tool of your choice.
 
 > For the best playback experience it is recommended to run `asciinema play` in
 > a terminal of dimensions not smaller than the one used for recording, as
 > there's no "transcoding" of control sequences for new terminal size.
 
 ### `cat <filename>`
 
@@ -370,14 +358,37 @@
 > A new install ID is generated on each machine and system user account you use
 > asciinema on, so in order to keep all recordings under a single asciinema.org
 > account you need to run `asciinema auth` on all of those machines.
 
 > asciinema versions prior to 2.0 confusingly referred to install ID as "API
 > token".
 
+## Markers
+
+Markers allow marking specific time locations in a recording, which can be used
+for navigation, as well as for automatic pausing of the playback.
+
+Markers can be added to a recording in several ways:
+
+- while you are recording, by pressing a configured hotkey, see [add_marker_key
+  config option](#configuration-file)
+- for existing recording, by inserting marker events (`"m"`) in the asciicast
+  file, see [marker event](doc/asciicast-v2.md#m---marker)
+
+When replaying a recording with `asciinema play` you can enable
+auto-pause-on-marker behaviour with `-m`/`--pause-on-markers` option (it's off
+by default). When a marker is encountered, the playback automatically pauses and
+can be resumed by pressing space bar key. The playback continues until next
+marker is encountered. You can also fast-forward to the next marker by pressing
+`]` key (when paused).
+
+Markers can be useful in e.g. live demos: you can create a recording with
+markers, then play it back during presentation, and have it stop wherever you
+want to explain terminal contents in more detail.
+
 ## Hosting the recordings on the web
 
 As mentioned in the `Usage > rec` section above, if the `filename` argument to
 `asciinema rec` is omitted then the recorded asciicast is uploaded to
 [asciinema.org](https://asciinema.org). You can watch it there and share it via
 secret URL.
 
@@ -428,14 +439,17 @@
 ; Be quiet, suppress all notices/warnings, default: no
 quiet = true
 
 ; Define hotkey for pausing recording (suspending capture of output),
 ; default: C-\ (control + backslash)
 pause_key = C-p
 
+; Define hotkey for adding a marker, default: none
+add_marker_key = C-x
+
 ; Define hotkey prefix key - when defined other recording hotkeys must
 ; be preceeded by it, default: no prefix
 prefix_key = C-a
 
 [play]
 
 ; Playback speed (can be fractional), default: 1
@@ -445,16 +459,20 @@
 idle_time_limit = 1
 
 ; Define hotkey for pausing/resuming playback,
 ; default: space
 pause_key = p
 
 ; Define hotkey for stepping through playback, a frame at a time,
-; default: .
-step_key = ]
+; default: . (dot)
+step_key = s
+
+; Define hotkey for jumping to the next marker,
+; default: ]
+next_marker_key = m
 
 [notifications]
 ; Desktop notifications are displayed on certain occasions, e.g. when
 ; pausing/resuming the capture of terminal with C-\ keyboard shortcut.
 
 ; Should desktop notifications be enabled, default: yes
 enabled = no
@@ -480,25 +498,27 @@
 
 If `$XDG_CONFIG_HOME` is set on Linux then asciinema uses
 `$XDG_CONFIG_HOME/asciinema` instead of `$HOME/.config/asciinema`.
 
 > asciinema versions prior to 1.1 used `$HOME/.asciinema`. If you have it
 > there you should `mv $HOME/.asciinema $HOME/.config/asciinema`.
 
+## Consulting
+
+I offer consulting services for asciinema project. See https://asciinema.org/consulting for more information.
+
 ## Contributing
 
 If you want to contribute to this project check out
 [Contributing](https://asciinema.org/contributing) page.
 
 ## Authors
 
 Developed with passion by [Marcin Kulik](http://ku1ik.com) and great open
 source [contributors](https://github.com/asciinema/asciinema/contributors).
 
 ## License
 
-Copyright &copy; 2011–2021 Marcin Kulik.
+© 2011 Marcin Kulik.
 
 All code is licensed under the GPL, v3 or later. See [LICENSE](./LICENSE) file
 for details.
-
-
```

### Comparing `asciinema-2.2.0/README.md` & `asciinema-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: asciinema
+Version: 2.3.0
+Summary: Terminal session recorder
+Home-page: https://asciinema.org
+Download-URL: 
+https://github.com/asciinema/asciinema/archive/v2.3.0.tar.gz
+Author: Marcin Kulik
+Author-email: m@ku1ik.com
+License: GNU GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
 # asciinema
 
 [![Build Status](https://github.com/asciinema/asciinema/actions/workflows/asciinema.yml/badge.svg)](https://github.com/asciinema/asciinema/actions/workflows/asciinema.yml)
 [![PyPI](https://img.shields.io/pypi/v/asciinema.svg)](https://pypi.org/project/asciinema/)
 [![license](http://img.shields.io/badge/license-GNU-blue.svg)](https://raw.githubusercontent.com/asciinema/asciinema/master/LICENSE)
 
 Terminal session recorder and the best companion of
@@ -129,39 +157,41 @@
 ```sh
 python3 -m asciinema --version
 ```
 
 ### Docker image
 
 asciinema Docker image is based on [Ubuntu
-20.04](https://releases.ubuntu.com/20.04/) and has the latest version of
+22.04](https://releases.ubuntu.com/22.04/) and has the latest version of
 asciinema recorder pre-installed.
 
 ```sh
-docker pull docker.io/asciinema/asciinema
+docker pull ghcr.io/asciinema/asciinema
 ```
 
 When running it don't forget to allocate a pseudo-TTY (`-t`), keep STDIN open
 (`-i`) and mount config directory volume (`-v`):
 
 ```sh
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" ghcr.io/asciinema/asciinema rec
 ```
 
 Container's entrypoint is set to `/usr/local/bin/asciinema` so you can run the
 container with any arguments you would normally pass to `asciinema` binary (see
 Usage section for commands and options).
 
 There's not much software installed in this image though. In most cases you may
 want to install extra programs before recording. One option is to derive new
-image from this one (start your custom Dockerfile with `FROM asciinema/asciinema`). Another option is to start the container with `/bin/bash`
-as the entrypoint, install extra packages and manually start `asciinema rec`:
+image from this one (start your custom Dockerfile with `FROM
+ghcr.io/asciinema/asciinema`). Another option is to start the container with
+`/bin/bash` as the entrypoint, install extra packages and manually start
+`asciinema rec`:
 
 ```console
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash ghcr.io/asciinema/asciinema rec
 root@6689517d99a1:~# apt-get install foobar
 root@6689517d99a1:~# asciinema rec
 ```
 
 It is also possible to run the docker container as a non-root user, which has
 security benefits. You can specify a user and group id at runtime to give the
 application permission similar to the calling user on your host.
@@ -169,15 +199,15 @@
 ```sh
 docker run --rm -it \
     --env=ASCIINEMA_CONFIG_HOME="/run/user/$(id -u)/.config/asciinema" \
     --user="$(id -u):$(id -g)" \
     --volume="${HOME}/.config/asciinema:/run/user/$(id -u)/.config/asciinema:rw" \
     --volume="${PWD}:/data:rw" \
     --workdir='/data' \
-    docker.io/asciinema/asciinema rec
+    ghcr.io/asciinema/asciinema rec
 ```
 
 ## Usage
 
 asciinema is composed of multiple commands, similar to `git`, `apt-get` or
 `brew`.
 
@@ -232,15 +262,15 @@
 - `--rows=<n>` - Override terminal rows for recorded process
 - `-y, --yes` - Answer "yes" to all prompts (e.g. upload confirmation)
 - `-q, --quiet` - Be quiet, suppress all notices/warnings (implies -y)
 
 Stdin recording allows for capturing of all characters typed in by the user in
 the currently recorded shell. This may be used by a player (e.g.
 [asciinema-player](https://github.com/asciinema/asciinema-player)) to display
-pressed keys. Because it's basically a key-logging (scoped to a single shell
+pressed keys. Because it's basically key-logging (scoped to a single shell
 instance), it's disabled by default, and has to be explicitly enabled via
 `--stdin` option.
 
 ### `play <filename>`
 
 **Replay recorded asciicast in a terminal.**
 
@@ -289,14 +319,29 @@
 asciinema play dweb:/ipfs/QmNe7FsYaHc9SaDEAEXbaagAzNw9cH7YbzN4xV7jV1MCzK/ascii.cast
 ```
 
 Available options:
 
 - `-i, --idle-time-limit=<sec>` - Limit replayed terminal inactivity to max `<sec>` seconds
 - `-s, --speed=<factor>` - Playback speed (can be fractional)
+- `-l, --loop` - Play in a loop
+- `-m, --pause-on-markers` - Automatically pause on [markers](#markers)
+- `--stream=<stream>` - Select stream to play (see below)
+- `--out-fmt=<format>` - Select output format (see below)
+
+By default the output stream (`o`) is played. This is what you want in most
+cases.  If you recorded the input stream (`i`) with `asciinema rec --stdin` then
+you can replay it with `asciinema play --stream=i <filename>`.
+
+By default the selected stream is written to stdout in original, raw data form.
+This is also what you want in majority of cases. However you can change the
+output format to asciicast (newline delimited JSON) with `asciinema play
+--out-fmt=asciicast <filename>`. This allows delegating actual rendering to
+another place (e.g. outside of your terminal) by piping output of `asciinema
+play` to a tool of your choice.
 
 > For the best playback experience it is recommended to run `asciinema play` in
 > a terminal of dimensions not smaller than the one used for recording, as
 > there's no "transcoding" of control sequences for new terminal size.
 
 ### `cat <filename>`
 
@@ -341,14 +386,37 @@
 > A new install ID is generated on each machine and system user account you use
 > asciinema on, so in order to keep all recordings under a single asciinema.org
 > account you need to run `asciinema auth` on all of those machines.
 
 > asciinema versions prior to 2.0 confusingly referred to install ID as "API
 > token".
 
+## Markers
+
+Markers allow marking specific time locations in a recording, which can be used
+for navigation, as well as for automatic pausing of the playback.
+
+Markers can be added to a recording in several ways:
+
+- while you are recording, by pressing a configured hotkey, see [add_marker_key
+  config option](#configuration-file)
+- for existing recording, by inserting marker events (`"m"`) in the asciicast
+  file, see [marker event](doc/asciicast-v2.md#m---marker)
+
+When replaying a recording with `asciinema play` you can enable
+auto-pause-on-marker behaviour with `-m`/`--pause-on-markers` option (it's off
+by default). When a marker is encountered, the playback automatically pauses and
+can be resumed by pressing space bar key. The playback continues until next
+marker is encountered. You can also fast-forward to the next marker by pressing
+`]` key (when paused).
+
+Markers can be useful in e.g. live demos: you can create a recording with
+markers, then play it back during presentation, and have it stop wherever you
+want to explain terminal contents in more detail.
+
 ## Hosting the recordings on the web
 
 As mentioned in the `Usage > rec` section above, if the `filename` argument to
 `asciinema rec` is omitted then the recorded asciicast is uploaded to
 [asciinema.org](https://asciinema.org). You can watch it there and share it via
 secret URL.
 
@@ -399,14 +467,17 @@
 ; Be quiet, suppress all notices/warnings, default: no
 quiet = true
 
 ; Define hotkey for pausing recording (suspending capture of output),
 ; default: C-\ (control + backslash)
 pause_key = C-p
 
+; Define hotkey for adding a marker, default: none
+add_marker_key = C-x
+
 ; Define hotkey prefix key - when defined other recording hotkeys must
 ; be preceeded by it, default: no prefix
 prefix_key = C-a
 
 [play]
 
 ; Playback speed (can be fractional), default: 1
@@ -416,16 +487,20 @@
 idle_time_limit = 1
 
 ; Define hotkey for pausing/resuming playback,
 ; default: space
 pause_key = p
 
 ; Define hotkey for stepping through playback, a frame at a time,
-; default: .
-step_key = ]
+; default: . (dot)
+step_key = s
+
+; Define hotkey for jumping to the next marker,
+; default: ]
+next_marker_key = m
 
 [notifications]
 ; Desktop notifications are displayed on certain occasions, e.g. when
 ; pausing/resuming the capture of terminal with C-\ keyboard shortcut.
 
 ; Should desktop notifications be enabled, default: yes
 enabled = no
@@ -451,23 +526,27 @@
 
 If `$XDG_CONFIG_HOME` is set on Linux then asciinema uses
 `$XDG_CONFIG_HOME/asciinema` instead of `$HOME/.config/asciinema`.
 
 > asciinema versions prior to 1.1 used `$HOME/.asciinema`. If you have it
 > there you should `mv $HOME/.asciinema $HOME/.config/asciinema`.
 
+## Consulting
+
+I offer consulting services for asciinema project. See https://asciinema.org/consulting for more information.
+
 ## Contributing
 
 If you want to contribute to this project check out
 [Contributing](https://asciinema.org/contributing) page.
 
 ## Authors
 
 Developed with passion by [Marcin Kulik](http://ku1ik.com) and great open
 source [contributors](https://github.com/asciinema/asciinema/contributors).
 
 ## License
 
-Copyright &copy; 2011–2021 Marcin Kulik.
+© 2011 Marcin Kulik.
 
 All code is licensed under the GPL, v3 or later. See [LICENSE](./LICENSE) file
 for details.
```

### Comparing `asciinema-2.2.0/asciinema/__init__.py` & `asciinema-2.3.0/asciinema/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 __author__ = "Marcin Kulik"
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 if sys.version_info < (3, 6):
     raise ImportError("Python < 3.6 is unsupported.")
 
 # pylint: disable=wrong-import-position
 from typing import Any, Optional
```

### Comparing `asciinema-2.2.0/asciinema/__main__.py` & `asciinema-2.3.0/asciinema/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,29 @@
 from .commands.auth import AuthCommand
 from .commands.cat import CatCommand
 from .commands.play import PlayCommand
 from .commands.record import RecordCommand
 from .commands.upload import UploadCommand
 
 
+def valid_encoding() -> bool:
+    def _locales() -> Optional[str]:
+        try:
+            return locale.nl_langinfo(locale.CODESET)
+        except AttributeError:
+            return locale.getlocale()[-1]
+
+    loc = _locales()
+
+    if loc is None:
+        return False
+    else:
+        return loc.upper() in ("US-ASCII", "UTF-8", "UTF8")
+
+
 def positive_int(value: str) -> int:
     _value = int(value)
     if _value <= 0:
         raise argparse.ArgumentTypeError("must be positive")
 
     return _value
 
@@ -31,19 +46,15 @@
 def maybe_str(v: Any) -> Optional[str]:
     if v is not None:
         return str(v)
     return None
 
 
 def main() -> Any:
-    if locale.nl_langinfo(locale.CODESET).upper() not in [
-        "US-ASCII",
-        "UTF-8",
-        "UTF8",
-    ]:
+    if not valid_encoding():
         sys.stderr.write(
             "asciinema needs an ASCII or UTF-8 character encoding to run. "
             "Check the output of `locale` command.\n"
         )
         return 1
 
     try:
@@ -170,29 +181,57 @@
         help="limit idle time during playback to given number of seconds",
         type=positive_float,
         default=maybe_str(cfg.play_idle_time_limit),
     )
     parser_play.add_argument(
         "-s",
         "--speed",
-        help="playback speedup (can be fractional)",
+        help="set playback speed (can be fractional)",
         type=positive_float,
         default=cfg.play_speed,
     )
     parser_play.add_argument(
+        "-l",
+        "--loop",
+        help="loop loop loop loop",
+        action="store_true",
+        default=False,
+    )
+    parser_play.add_argument(
+        "-m",
+        "--pause-on-markers",
+        help="automatically pause on markers",
+        action="store_true",
+        default=False,
+    )
+    parser_play.add_argument(
+        "--out-fmt",
+        help="select output format",
+        choices=["raw", "asciicast"],
+        default="raw",
+    )
+    parser_play.add_argument(
+        "--stream",
+        help="select stream to play",
+        choices=["o", "i"],
+        default=None,
+    )
+    parser_play.add_argument(
         "filename", help='local path, http/ipfs URL or "-" (read from stdin)'
     )
     parser_play.set_defaults(cmd=PlayCommand)
 
     # create the parser for the `cat` command
     parser_cat = subparsers.add_parser(
-        "cat", help="Print full output of terminal session"
+        "cat", help="Print full output of terminal sessions"
     )
     parser_cat.add_argument(
-        "filename", help='local path, http/ipfs URL or "-" (read from stdin)'
+        "filename",
+        nargs="+",
+        help='local path, http/ipfs URL or "-" (read from stdin)',
     )
     parser_cat.set_defaults(cmd=CatCommand)
 
     # create the parser for the `upload` command
     parser_upload = subparsers.add_parser(
         "upload", help="Upload locally saved terminal session to asciinema.org"
     )
```

### Comparing `asciinema-2.2.0/asciinema/api.py` & `asciinema-2.3.0/asciinema/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 from . import __version__
 from .http_adapter import HTTPConnectionError
 from .urllib_http_adapter import URLLibHttpAdapter
 
 
 class APIError(Exception):
-    pass
+    def __init__(self, e: str, retryable: bool):
+        super().__init__(e)
+        self.retryable = retryable
 
 
 class Api:
     def __init__(
         self,
         url: str,
         user: Optional[str],
@@ -44,15 +46,15 @@
                     self.upload_url(),
                     files={"asciicast": ("ascii.cast", f)},
                     headers=self._headers(),
                     username=self.user,
                     password=self.install_id,
                 )
             except HTTPConnectionError as e:
-                raise APIError(str(e)) from e
+                raise APIError(str(e), True) from e
 
         if status not in (200, 201):
             self._handle_error(status, body)
 
         if (headers.get("content-type") or "")[0:16] == "application/json":
             result = json.loads(body)
         else:
@@ -78,24 +80,24 @@
             400: f"Invalid request: {body.decode('utf-8', 'replace')}",
             401: "Invalid or revoked install ID",
             404: (
                 "API endpoint not found. "
                 "This asciinema version may no longer be supported. "
                 "Please upgrade to the latest version."
             ),
-            413: "Sorry, your asciicast is too big.",
+            413: "Sorry, the size of your recording exceeds the server-configured limit.",
             422: f"Invalid asciicast: {body.decode('utf-8', 'replace')}",
-            503: "The server is down for maintenance. Try again in a minute.",
+            503: "The server is down for maintenance.",
         }
 
         error = errors.get(status)
 
         if not error:
             if status >= 500:
                 error = (
                     "The server is having temporary problems. "
                     "Try again in a minute."
                 )
             else:
                 error = f"HTTP status: {status}"
 
-        raise APIError(error)
+        raise APIError(error, status >= 500)
```

### Comparing `asciinema-2.2.0/asciinema/asciicast/__init__.py` & `asciinema-2.3.0/asciinema/asciicast/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import codecs
 import gzip
 import os
 import sys
 import urllib.error
 from codecs import StreamReader
 from html.parser import HTMLParser
+from io import BytesIO
 from typing import Any, List, TextIO, Union
 from urllib.parse import urlparse, urlunparse
 from urllib.request import Request, urlopen
 
 from . import v1, v2
 
 
@@ -54,54 +55,58 @@
         url = f"https://ipfs.io/ipfs/{url[7:]}"
     elif url.startswith("dweb:/ipfs/"):
         url = f"https://ipfs.io/{url[5:]}"
 
     if url.startswith("http:") or url.startswith("https:"):
         req = Request(url)
         req.add_header("Accept-Encoding", "gzip")
+        body = None
+        content_type = None
+        utf8_reader = codecs.getreader("utf-8")
+
         with urlopen(req) as response:
             body = response
+            content_type = response.headers["Content-Type"]
             url = response.geturl()  # final URL after redirects
 
             if response.headers["Content-Encoding"] == "gzip":
                 body = gzip.open(body)
 
-            utf8_reader = codecs.getreader("utf-8")
-            content_type = response.headers["Content-Type"]
+            body = BytesIO(body.read())
 
-            if content_type and content_type.startswith("text/html"):
-                html = utf8_reader(body, errors="replace").read()
-                parser = Parser()
-                parser.feed(html)
-                new_url = parser.url
-
-                if not new_url:
-                    raise LoadError(
-                        '<link rel="alternate" '
-                        'type="application/x-asciicast" '
-                        'href="..."> '
-                        "not found in fetched HTML document"
+        if content_type and content_type.startswith("text/html"):
+            html = utf8_reader(body, errors="replace").read()
+            parser = Parser()
+            parser.feed(html)
+            new_url = parser.url
+
+            if not new_url:
+                raise LoadError(
+                    '<link rel="alternate" '
+                    'type="application/x-asciicast" '
+                    'href="..."> '
+                    "not found in fetched HTML document"
+                )
+
+            if "://" not in new_url:
+                base_url = urlparse(url)
+
+                if new_url.startswith("/"):
+                    new_url = urlunparse(
+                        (base_url[0], base_url[1], new_url, "", "", "")
+                    )
+                else:
+                    path = f"{os.path.dirname(base_url[2])}/{new_url}"
+                    new_url = urlunparse(
+                        (base_url[0], base_url[1], path, "", "", "")
                     )
 
-                if "://" not in new_url:
-                    base_url = urlparse(url)
-
-                    if new_url.startswith("/"):
-                        new_url = urlunparse(
-                            (base_url[0], base_url[1], new_url, "", "", "")
-                        )
-                    else:
-                        path = f"{os.path.dirname(base_url[2])}/{new_url}"
-                        new_url = urlunparse(
-                            (base_url[0], base_url[1], path, "", "", "")
-                        )
-
-                return open_url(new_url)
+            return open_url(new_url)
 
-            return utf8_reader(body, errors="strict")
+        return utf8_reader(body, errors="strict")
 
     return open(url, mode="rt", encoding="utf-8")
 
 
 class open_from_url:
     FORMAT_ERROR = "only asciicast v1 and v2 formats can be opened"
```

### Comparing `asciinema-2.2.0/asciinema/asciicast/events.py` & `asciinema-2.3.0/asciinema/asciicast/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Any, Generator, List, Optional
+from typing import Any, Generator, Iterable, List, Optional
 
 
 def to_relative_time(
-    events: Generator[List[Any], None, None]
+    events: Iterable[Any],
 ) -> Generator[List[Any], None, None]:
     prev_time = 0
 
     for frame in events:
         time, type_, data = frame
         delay = time - prev_time
         prev_time = time
         yield [delay, type_, data]
 
 
 def to_absolute_time(
-    events: Generator[List[Any], None, None]
+    events: Iterable[Any],
 ) -> Generator[List[Any], None, None]:
     time = 0
 
     for frame in events:
         delay, type_, data = frame
         time = time + delay
         yield [time, type_, data]
 
 
 def cap_relative_time(
-    events: Generator[List[Any], None, None], time_limit: Optional[float]
-) -> Generator[List[Any], None, None]:
+    events: Iterable[Any], time_limit: Optional[float]
+) -> Iterable[Any]:
     if time_limit:
         return (
             [min(delay, time_limit), type_, data]
             for delay, type_, data in events
         )
     return events
 
 
 def adjust_speed(
-    events: Generator[List[Any], None, None], speed: Any
+    events: Iterable[Any], speed: Any
 ) -> Generator[List[Any], None, None]:
     return ([delay / speed, type_, data] for delay, type_, data in events)
```

### Comparing `asciinema-2.2.0/asciinema/asciicast/raw.py` & `asciinema-2.3.0/asciinema/asciicast/raw.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,24 +19,42 @@
 
         if (
             append and path.exists(path_) and os.stat(path_).st_size == 0
         ):  # true for pipes
             append = False
 
         self.buffering = buffering
-        self.mode: str = "ab" if append else "wb"
-        self.metadata = metadata
+
+        if append:
+            self.mode = "ab"
+            self.header = None
+        else:
+            self.mode = "wb"
+            width = metadata["width"]
+            height = metadata["height"]
+            self.header = f"\x1b[8;{height};{width}t".encode("utf-8")
+
+    def __enter__(self) -> Any:
+        super().__enter__()
+
+        if self.header:
+            self._write(self.header)
+
+        return self
 
     def write_stdout(self, _ts: float, data: Any) -> None:
         self._write(data)
 
     # pylint: disable=no-self-use
     def write_stdin(self, ts: float, data: Any) -> None:
         pass
 
+    def write_marker(self, ts: float) -> None:
+        pass
+
     # pylint: disable=consider-using-with
     def _open_file(self) -> None:
         if self.path == "-":
             self.file = os.fdopen(
                 sys.stdout.fileno(),
                 mode=self.mode,
                 buffering=self.buffering,
```

### Comparing `asciinema-2.2.0/asciinema/asciicast/v1.py` & `asciinema-2.3.0/asciinema/asciicast/v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 import json
 from codecs import StreamReader
 from json.decoder import JSONDecodeError
-from typing import Any, Dict, Generator, List, Optional, TextIO, Union
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    TextIO,
+    Union,
+)
 
 from .events import to_absolute_time
 
 
 class LoadError(Exception):
     pass
 
@@ -22,24 +31,24 @@
         header = {
             k: v
             for k, v in self.__attrs.items()
             if k in keys and v is not None
         }
         return header
 
+    def events(self, type_: Optional[str] = None) -> Iterable[List[Any]]:
+        if type_ in [None, "o"]:
+            return to_absolute_time(self.__stdout_events())
+        else:
+            return []
+
     def __stdout_events(self) -> Generator[List[Any], None, None]:
         for time, data in self.__attrs["stdout"]:
             yield [time, "o", data]
 
-    def events(self) -> Any:
-        return self.stdout_events()
-
-    def stdout_events(self) -> Generator[List[Any], None, None]:
-        return to_absolute_time(self.__stdout_events())
-
 
 class open_from_file:
     FORMAT_ERROR: str = "only asciicast v1 format can be opened"
 
     def __init__(
         self, first_line: str, file: Union[TextIO, StreamReader]
     ) -> None:
```

### Comparing `asciinema-2.2.0/asciinema/asciicast/v2.py` & `asciinema-2.3.0/asciinema/asciicast/v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,25 @@
         self, f: Union[TextIO, StreamReader], header: Dict[str, Any]
     ) -> None:
         self.version: int = 2
         self.__file = f
         self.v2_header = header
         self.idle_time_limit = header.get("idle_time_limit")
 
-    def events(self) -> Generator[Any, None, None]:
-        for line in self.__file:
-            yield json.loads(line)
-
-    def stdout_events(self) -> Generator[List[Any], None, None]:
-        for time, type_, data in self.events():
-            if type_ == "o":
-                yield [time, type_, data]
+    def events(
+        self, type_: Optional[str] = None
+    ) -> Generator[List[Any], None, None]:
+        if type_ is None:
+            for line in self.__file:
+                yield json.loads(line)
+        else:
+            for line in self.__file:
+                event = json.loads(line)
+                if event[1] == type_:
+                    yield event
 
 
 def build_from_header_and_file(
     header: Dict[str, Any], f: Union[StreamReader, TextIO]
 ) -> Asciicast:
     return Asciicast(f, header)
 
@@ -72,15 +75,15 @@
 
 
 def get_duration(path_: str) -> Any:
     with open(path_, mode="rt", encoding="utf-8") as f:
         first_line = f.readline()
         with open_from_file(first_line, f) as a:
             last_frame = None
-            for last_frame in a.stdout_events():
+            for last_frame in a.events("o"):
                 pass
             return last_frame[0]
 
 
 def build_header(
     width: Optional[int], height: Optional[int], metadata: Any
 ) -> Dict[str, Any]:
@@ -138,14 +141,17 @@
 
     def write_stdin(self, ts: float, data: Union[str, bytes]) -> None:
         if isinstance(data, str):
             data = data.encode(encoding="utf-8", errors="strict")
         data = self.stdin_decoder.decode(data)
         self.__write_event(ts, "i", data)
 
+    def write_marker(self, ts: float) -> None:
+        self.__write_event(ts, "m", "")
+
     # pylint: disable=consider-using-with
     def _open_file(self) -> None:
         if self.path == "-":
             self.file = os.fdopen(
                 sys.stdout.fileno(),
                 mode=self.mode,
                 buffering=self.buffering,
```

### Comparing `asciinema-2.2.0/asciinema/async_worker.py` & `asciinema-2.3.0/asciinema/async_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,24 @@
 
 class async_worker:
     def __init__(self) -> None:
         self.queue: Queue[Any] = Queue()
         self.process: Optional[Process] = None
 
     def __enter__(self) -> Any:
-        self.process = Process(target=self.run)
+        self.process = Process(target=self._run)
         self.process.start()
         return self
 
+    def _run(self) -> None:
+        try:
+            self.run()
+        except KeyboardInterrupt:
+            pass
+
     def __exit__(
         self, exc_type: str, exc_value: str, exc_traceback: str
     ) -> None:
         self.queue.put(None)
         assert isinstance(self.process, Process)
         self.process.join()
```

### Comparing `asciinema-2.2.0/asciinema/commands/auth.py` & `asciinema-2.3.0/asciinema/commands/auth.py`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/asciinema/commands/cat.py` & `asciinema-2.3.0/asciinema/commands/cat.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 from ..tty_ import raw
 from .command import Command
 
 
 class CatCommand(Command):
     def __init__(self, args: Any, config: Config, env: Dict[str, str]):
         Command.__init__(self, args, config, env)
-        self.filename = args.filename
+        self.filenames = args.filename
 
     def execute(self) -> int:
         try:
             with open("/dev/tty", "rt", encoding="utf-8") as stdin:
                 with raw(stdin.fileno()):
-                    with asciicast.open_from_url(self.filename) as a:
-                        for _, _type, text in a.stdout_events():
-                            sys.stdout.write(text)
-                            sys.stdout.flush()
+                    return self.cat()
+        except OSError:
+            return self.cat()
+
+    def cat(self) -> int:
+        try:
+            for filename in self.filenames:
+                with asciicast.open_from_url(filename) as a:
+                    for _, _type, text in a.events("o"):
+                        sys.stdout.write(text)
+                        sys.stdout.flush()
 
         except asciicast.LoadError as e:
             self.print_error(f"printing failed: {str(e)}")
             return 1
 
         return 0
```

### Comparing `asciinema-2.2.0/asciinema/commands/command.py` & `asciinema-2.3.0/asciinema/commands/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, _args: Any, config: Config, env: Dict[str, str]):
         self.quiet: bool = False
         self.api = Api(config.api_url, env.get("USER"), config.install_id)
 
     def print(
         self,
         text: str,
-        end: str = "\n",
+        end: str = "\r\n",
         color: Optional[int] = None,
         force: bool = False,
     ) -> None:
         if not self.quiet or force:
             if color is not None and os.isatty(sys.stderr.fileno()):
                 text = f"\x1b[0;3{color}m{text}\x1b[0m"
```

### Comparing `asciinema-2.2.0/asciinema/commands/play.py` & `asciinema-2.3.0/asciinema/commands/play.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,45 @@
         env: Dict[str, str],
         player: Optional[Player] = None,
     ) -> None:
         Command.__init__(self, args, config, env)
         self.filename = args.filename
         self.idle_time_limit = args.idle_time_limit
         self.speed = args.speed
+        self.loop = args.loop
+        self.out_fmt = args.out_fmt
+        self.stream = args.stream
+        self.pause_on_markers = args.pause_on_markers
         self.player = player if player is not None else Player()
         self.key_bindings = {
             "pause": config.play_pause_key,
             "step": config.play_step_key,
+            "next_marker": config.play_next_marker_key,
         }
 
     def execute(self) -> int:
+        code = self.play()
+
+        if self.loop:
+            while code == 0:
+                code = self.play()
+
+        return code
+
+    def play(self) -> int:
         try:
             with asciicast.open_from_url(self.filename) as a:
                 self.player.play(
-                    a, self.idle_time_limit, self.speed, self.key_bindings
+                    a,
+                    idle_time_limit=self.idle_time_limit,
+                    speed=self.speed,
+                    key_bindings=self.key_bindings,
+                    out_fmt=self.out_fmt,
+                    stream=self.stream,
+                    pause_on_markers=self.pause_on_markers,
                 )
 
         except asciicast.LoadError as e:
             self.print_error(f"playback failed: {str(e)}")
             return 1
         except KeyboardInterrupt:
             return 1
```

### Comparing `asciinema-2.2.0/asciinema/commands/record.py` & `asciinema-2.3.0/asciinema/commands/record.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.notifier = notifier.get_notifier(
             config.notifications_enabled, config.notifications_command
         )
         self.env = env
         self.key_bindings = {
             "prefix": config.record_prefix_key,
             "pause": config.record_pause_key,
+            "add_marker": config.record_add_marker_key,
         }
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-return-statements
     # pylint: disable=too-many-statements
     def execute(self) -> int:
         upload = False
@@ -49,14 +50,20 @@
                     "filename required when recording in raw mode"
                 )
                 return 1
             self.filename = _tmp_path()
             upload = True
 
         if self.filename == "-":
+            if sys.stdout.isatty():
+                self.print_error(
+                    f"when recording to stdout it must not be TTY - forgot to pipe?"
+                )
+                return 1
+
             append = False
 
         elif os.path.exists(self.filename):
             if not os.access(self.filename, os.W_OK):
                 self.print_error(f"can't write to {self.filename}")
                 return 1
 
@@ -72,24 +79,38 @@
                 )
                 self.print_error(
                     "use --append option "
                     "if you want to append to existing recording"
                 )
                 return 1
 
-        elif append:
-            self.print_warning(
-                f"{self.filename} does not exist, not appending"
-            )
-            append = False
+        else:
+            dir_path = os.path.dirname(os.path.abspath(self.filename))
+
+            if not os.path.exists(dir_path):
+                self.print_error(f"directory {dir_path} doesn't exist")
+                return 1
+
+            if not os.access(dir_path, os.W_OK):
+                self.print_error(f"directory {dir_path} is not writable")
+                return 1
+
+            if append:
+                self.print_warning(
+                    f"{self.filename} does not exist, not appending"
+                )
+                append = False
 
         if append:
             self.print_info(f"appending to asciicast at {self.filename}")
         else:
-            self.print_info(f"recording asciicast to {self.filename}")
+            if self.filename == "-":
+                self.print_info(f"recording asciicast to stdout")
+            else:
+                self.print_info(f"recording asciicast to {self.filename}")
 
         if self.command:
             self.print_info("""exit opened program when you're done""")
         else:
             self.print_info(
                 """press <ctrl-d> or type "exit" when you're done"""
             )
@@ -114,14 +135,17 @@
                 record_stdin=self.record_stdin,
                 writer=self.writer,
                 notify=self.notifier.notify,
                 key_bindings=self.key_bindings,
                 cols_override=self.cols_override,
                 rows_override=self.rows_override,
             )
+        except IOError as e:
+            self.print_error(f"I/O error: {str(e)}")
+            return 1
         except v2.LoadError:
             self.print_error(
                 "can only append to asciicast v2 format recordings"
             )
             return 1
 
         self.print_info("recording finished")
@@ -151,15 +175,15 @@
             except APIError as e:
                 self.print("\r\x1b[A", end="")
                 self.print_error(f"upload failed: {str(e)}")
                 self.print_error(
                     f"retry later by running: asciinema upload {self.filename}"
                 )
                 return 1
-        else:
+        elif self.filename != "-":
             self.print_info(f"asciicast saved to {self.filename}")
 
         return 0
 
 
 def _tmp_path() -> Optional[str]:
     return NamedTemporaryFile(suffix="-ascii.cast", delete=False).name
```

### Comparing `asciinema-2.2.0/asciinema/commands/upload.py` & `asciinema-2.3.0/asciinema/commands/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,16 @@
 
         except OSError as e:
             self.print_error(f"upload failed: {str(e)}")
             return 1
 
         except APIError as e:
             self.print_error(f"upload failed: {str(e)}")
-            self.print_error(
-                f"retry later by running: asciinema upload {self.filename}"
-            )
+
+            if e.retryable:
+                self.print_error(
+                    f"retry later by running: asciinema upload {self.filename}"
+                )
+
             return 1
 
         return 0
```

### Comparing `asciinema-2.2.0/asciinema/config.py` & `asciinema-2.3.0/asciinema/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,18 @@
         return self.__get_key("record", "prefix")
 
     @property
     def record_pause_key(self) -> Any:
         return self.__get_key("record", "pause", "C-\\")
 
     @property
+    def record_add_marker_key(self) -> Any:
+        return self.__get_key("record", "add_marker")
+
+    @property
     def play_idle_time_limit(self) -> Optional[float]:
         fallback = self.config.getfloat(
             "play", "maxwait", fallback=None
         )  # pre 2.0
         return self.config.getfloat(
             "play", "idle_time_limit", fallback=fallback
         )
@@ -154,14 +158,18 @@
         return self.__get_key("play", "pause", " ")
 
     @property
     def play_step_key(self) -> Any:
         return self.__get_key("play", "step", ".")
 
     @property
+    def play_next_marker_key(self) -> Any:
+        return self.__get_key("play", "next_marker", "]")
+
+    @property
     def notifications_enabled(self) -> bool:
         return self.config.getboolean(
             "notifications", "enabled", fallback=True
         )
 
     @property
     def notifications_command(self) -> Optional[str]:
```

### Comparing `asciinema-2.2.0/asciinema/data/icon-256x256.png` & `asciinema-2.3.0/asciinema/data/icon-256x256.png`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/asciinema/file_writer.py` & `asciinema-2.3.0/asciinema/file_writer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-import stat
 from typing import IO, Any, Callable, Optional
 
 
 class file_writer:
     def __init__(
         self,
         path: str,
@@ -25,20 +23,14 @@
 
     def _open_file(self) -> None:
         raise NotImplementedError
 
     def _write(self, data: Any) -> None:
         try:
             self.file.write(data)  # type: ignore
-        except BrokenPipeError as e:
-            if self.path != "-" and stat.S_ISFIFO(os.stat(self.path).st_mode):
-                self.on_error("Broken pipe, reopening...")
-                self._open_file()
-                self.on_error("Output pipe reopened successfully")
-                self.file.write(data)  # type: ignore
-            else:
-                self.on_error("Output pipe broken")
-                raise e
+        except IOError as e:
+            self.on_error("Write error, recording suspended")
+            raise e
 
 
 def noop(_: Any) -> None:
     return None
```

### Comparing `asciinema-2.2.0/asciinema/notifier.py` & `asciinema-2.3.0/asciinema/notifier.py`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/asciinema/pty_.py` & `asciinema-2.3.0/asciinema/pty_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import array
-import errno
 import fcntl
 import os
 import pty
 import select
 import signal
 import struct
 import termios
@@ -15,14 +14,16 @@
 EXIT_SIGNALS = [
     signal.SIGCHLD,
     signal.SIGHUP,
     signal.SIGTERM,
     signal.SIGQUIT,
 ]
 
+READ_LEN = 256 * 1024
+
 
 # pylint: disable=too-many-arguments,too-many-locals,too-many-statements
 def record(
     command: Any,
     env: Dict[str, str],
     writer: Any,
     get_tty_size: Callable[[], Tuple[int, int]],
@@ -33,123 +34,147 @@
 ) -> None:
     pty_fd: Any = None
     start_time: Optional[float] = None
     pause_time: Optional[float] = None
     prefix_mode: bool = False
     prefix_key = key_bindings.get("prefix")
     pause_key = key_bindings.get("pause")
+    add_marker_key = key_bindings.get("add_marker")
+    input_data = bytes()
 
     def set_pty_size() -> None:
         cols, rows = get_tty_size()
         buf = array.array("h", [rows, cols, 0, 0])
         fcntl.ioctl(pty_fd, termios.TIOCSWINSZ, buf)
 
     def handle_master_read(data: Any) -> None:
-        os.write(tty_stdout_fd, data)
+        remaining_data = memoryview(data)
+        while remaining_data:
+            n = os.write(tty_stdout_fd, remaining_data)
+            remaining_data = remaining_data[n:]
 
         if not pause_time:
             assert start_time is not None
-            writer.write_stdout(time.time() - start_time, data)
+            writer.write_stdout(time.perf_counter() - start_time, data)
 
     def handle_stdin_read(data: Any) -> None:
+        nonlocal input_data
         nonlocal pause_time
         nonlocal start_time
         nonlocal prefix_mode
 
         if not prefix_mode and prefix_key and data == prefix_key:
             prefix_mode = True
             return
 
-        if prefix_mode or (not prefix_key and data in [pause_key]):
+        if prefix_mode or (
+            not prefix_key and data in [pause_key, add_marker_key]
+        ):
             prefix_mode = False
 
             if data == pause_key:
                 if pause_time:
                     assert start_time is not None
-                    start_time += time.time() - pause_time
+                    start_time += time.perf_counter() - pause_time
                     pause_time = None
                     notify("Resumed recording")
                 else:
-                    pause_time = time.time()
+                    pause_time = time.perf_counter()
                     notify("Paused recording")
 
+            elif data == add_marker_key:
+                assert start_time is not None
+                writer.write_marker(time.perf_counter() - start_time)
+                notify("Marker added")
+
             return
 
-        remaining_data = data
-        while remaining_data:
-            n = os.write(pty_fd, remaining_data)
-            remaining_data = remaining_data[n:]
+        input_data += data
 
-        if not pause_time:
+        # save stdin unless paused or data is OSC response (e.g. \x1b]11;?\x07)
+        if not pause_time and not (
+            len(data) > 2
+            and data[0] == 0x1B
+            and data[1] == 0x5D
+            and data[-1] == 0x07
+        ):
             assert start_time is not None
-            writer.write_stdin(time.time() - start_time, data)
+            writer.write_stdin(time.perf_counter() - start_time, data)
 
     def copy(signal_fd: int) -> None:  # pylint: disable=too-many-branches
-        fds = [pty_fd, tty_stdin_fd, signal_fd]
-        stdin_fd = pty.STDIN_FILENO
+        nonlocal input_data
 
-        if not os.isatty(stdin_fd):
-            fds.append(stdin_fd)
+        crfds = [pty_fd, tty_stdin_fd, signal_fd]
 
         while True:
+            if len(input_data) > 0:
+                cwfds = [pty_fd]
+            else:
+                cwfds = []
+
             try:
-                rfds, _, _ = select.select(fds, [], [])
-            except OSError as e:  # Python >= 3.3
-                if e.errno == errno.EINTR:
-                    continue
+                rfds, wfds, _ = select.select(crfds, cwfds, [])
+            except KeyboardInterrupt:
+                if tty_stdin_fd in crfds:
+                    crfds.remove(tty_stdin_fd)
+
+                break
 
             if pty_fd in rfds:
-                data = os.read(pty_fd, 1024)
+                try:
+                    data = os.read(pty_fd, READ_LEN)
+                except OSError as e:
+                    data = b""
 
                 if not data:  # Reached EOF.
-                    fds.remove(pty_fd)
+                    break
                 else:
                     handle_master_read(data)
 
             if tty_stdin_fd in rfds:
-                data = os.read(tty_stdin_fd, 1024)
-
-                if not data:
-                    fds.remove(tty_stdin_fd)
-                else:
-                    handle_stdin_read(data)
-
-            if stdin_fd in rfds:
-                data = os.read(stdin_fd, 1024)
+                data = os.read(tty_stdin_fd, READ_LEN)
 
                 if not data:
-                    fds.remove(stdin_fd)
+                    if tty_stdin_fd in crfds:
+                        crfds.remove(tty_stdin_fd)
                 else:
                     handle_stdin_read(data)
 
             if signal_fd in rfds:
-                data = os.read(signal_fd, 1024)
+                data = os.read(signal_fd, READ_LEN)
 
                 if data:
                     signals = struct.unpack(f"{len(data)}B", data)
 
                     for sig in signals:
                         if sig in EXIT_SIGNALS:
-                            os.close(pty_fd)
-                            return None
+                            crfds.remove(signal_fd)
                         if sig == signal.SIGWINCH:
                             set_pty_size()
 
+            if pty_fd in wfds:
+                n = os.write(pty_fd, input_data)
+                input_data = input_data[n:]
+
     pid, pty_fd = pty.fork()
 
     if pid == pty.CHILD:
         os.execvpe(command[0], command, env)
 
-    start_time = time.time()
+    flags = fcntl.fcntl(pty_fd, fcntl.F_GETFL, 0) | os.O_NONBLOCK
+    fcntl.fcntl(pty_fd, fcntl.F_SETFL, flags)
+
+    start_time = time.perf_counter()
     set_pty_size()
 
     with SignalFD(EXIT_SIGNALS + [signal.SIGWINCH]) as sig_fd:
         with raw(tty_stdin_fd):
             try:
                 copy(sig_fd)
+                os.close(pty_fd)
             except (IOError, OSError):
                 pass
 
     os.waitpid(pid, 0)
 
 
 class SignalFD:
```

### Comparing `asciinema-2.2.0/asciinema/recorder.py` & `asciinema-2.3.0/asciinema/recorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import time
 from typing import Any, Callable, Dict, List, Optional, TextIO, Tuple, Type
 
 from . import pty_ as pty  # avoid collisions with standard library `pty`
 from .asciicast import v2
 from .asciicast.v2 import writer as w2
 from .async_worker import async_worker
@@ -74,29 +75,22 @@
 class tty_fds:
     def __init__(self) -> None:
         self.stdin_file: Optional[TextIO] = None
         self.stdout_file: Optional[TextIO] = None
 
     def __enter__(self) -> Tuple[int, int]:
         try:
-            self.stdin_file = open("/dev/tty", "rt", encoding="utf_8")
-        except OSError:
-            self.stdin_file = open("/dev/null", "rt", encoding="utf_8")
-
-        try:
             self.stdout_file = open("/dev/tty", "wt", encoding="utf_8")
         except OSError:
             self.stdout_file = open("/dev/null", "wt", encoding="utf_8")
 
-        return (self.stdin_file.fileno(), self.stdout_file.fileno())
+        return (sys.stdin.fileno(), self.stdout_file.fileno())
 
     def __exit__(self, type_: str, value: str, traceback: str) -> None:
-        assert self.stdin_file is not None
         assert self.stdout_file is not None
-        self.stdin_file.close()
         self.stdout_file.close()
 
 
 def build_metadata(  # pylint: disable=too-many-arguments
     cols: int,
     rows: int,
     idle_time_limit: Optional[float],
@@ -133,25 +127,34 @@
     def write_stdin(self, ts: float, data: Any) -> None:
         if self.record_stdin:
             self.enqueue([ts, "i", data])
 
     def write_stdout(self, ts: float, data: Any) -> None:
         self.enqueue([ts, "o", data])
 
+    def write_marker(self, ts: float) -> None:
+        self.enqueue([ts, "m", None])
+
     def run(self) -> None:
-        with self.writer as w:
-            event: Tuple[float, str, Any]
+        try:
+            with self.writer as w:
+                event: Tuple[float, str, Any]
+                for event in iter(self.queue.get, None):
+                    assert event is not None
+                    ts, etype, data = event
+
+                    if etype == "o":
+                        w.write_stdout(self.time_offset + ts, data)
+                    elif etype == "i":
+                        w.write_stdin(self.time_offset + ts, data)
+                    elif etype == "m":
+                        w.write_marker(self.time_offset + ts)
+        except IOError:
             for event in iter(self.queue.get, None):
-                assert event is not None
-                ts, etype, data = event
-
-                if etype == "o":
-                    w.write_stdout(self.time_offset + ts, data)
-                elif etype == "i":
-                    w.write_stdin(self.time_offset + ts, data)
+                pass
 
 
 class async_notifier(async_worker):
     def __init__(self, notify: Callable[[str], None]) -> None:
         async_worker.__init__(self)
         self._notify = notify
```

### Comparing `asciinema-2.2.0/asciinema/tty_.py` & `asciinema-2.3.0/asciinema/tty_.py`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/asciinema/urllib_http_adapter.py` & `asciinema-2.3.0/asciinema/urllib_http_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         """
         fields: {name: value} for regular form fields.
         files: {name: (filename, file-type)} for data to be uploaded as files
 
         yield body's chunk as bytes
         """
         encoder = codecs.getencoder("utf-8")
-        for (key, value) in fields.items():
+        for key, value in fields.items():
             key = self.u(key)
             yield encoder(f"--{self.boundary}\r\n")
             yield encoder(
                 self.u(f'content-disposition: form-data; name="{key}"\r\n')
             )
             yield encoder("\r\n")
             if isinstance(value, (int, float)):
                 value = str(value)
             yield encoder(self.u(value))
             yield encoder("\r\n")
-        for (key, filename_and_f) in files.items():
+        for key, filename_and_f in files.items():
             filename, f = filename_and_f
             key = self.u(key)
             filename = self.u(filename)
             yield encoder(f"--{self.boundary}\r\n")
             yield encoder(
                 self.u(
                     "content-disposition: form-data"
```

### Comparing `asciinema-2.2.0/asciinema.egg-info/PKG-INFO` & `asciinema-2.3.0/asciinema.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: asciinema
-Version: 2.2.0
+Version: 2.3.0
 Summary: Terminal session recorder
 Home-page: https://asciinema.org
 Download-URL: 
-https://github.com/asciinema/asciinema/archive/v2.2.0.tar.gz
+https://github.com/asciinema/asciinema/archive/v2.3.0.tar.gz
 Author: Marcin Kulik
 Author-email: m@ku1ik.com
 License: GNU GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # asciinema
@@ -158,39 +157,41 @@
 ```sh
 python3 -m asciinema --version
 ```
 
 ### Docker image
 
 asciinema Docker image is based on [Ubuntu
-20.04](https://releases.ubuntu.com/20.04/) and has the latest version of
+22.04](https://releases.ubuntu.com/22.04/) and has the latest version of
 asciinema recorder pre-installed.
 
 ```sh
-docker pull docker.io/asciinema/asciinema
+docker pull ghcr.io/asciinema/asciinema
 ```
 
 When running it don't forget to allocate a pseudo-TTY (`-t`), keep STDIN open
 (`-i`) and mount config directory volume (`-v`):
 
 ```sh
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" ghcr.io/asciinema/asciinema rec
 ```
 
 Container's entrypoint is set to `/usr/local/bin/asciinema` so you can run the
 container with any arguments you would normally pass to `asciinema` binary (see
 Usage section for commands and options).
 
 There's not much software installed in this image though. In most cases you may
 want to install extra programs before recording. One option is to derive new
-image from this one (start your custom Dockerfile with `FROM asciinema/asciinema`). Another option is to start the container with `/bin/bash`
-as the entrypoint, install extra packages and manually start `asciinema rec`:
+image from this one (start your custom Dockerfile with `FROM
+ghcr.io/asciinema/asciinema`). Another option is to start the container with
+`/bin/bash` as the entrypoint, install extra packages and manually start
+`asciinema rec`:
 
 ```console
-docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash docker.io/asciinema/asciinema rec
+docker run --rm -it -v "${HOME}/.config/asciinema:/root/.config/asciinema" --entrypoint=/bin/bash ghcr.io/asciinema/asciinema rec
 root@6689517d99a1:~# apt-get install foobar
 root@6689517d99a1:~# asciinema rec
 ```
 
 It is also possible to run the docker container as a non-root user, which has
 security benefits. You can specify a user and group id at runtime to give the
 application permission similar to the calling user on your host.
@@ -198,15 +199,15 @@
 ```sh
 docker run --rm -it \
     --env=ASCIINEMA_CONFIG_HOME="/run/user/$(id -u)/.config/asciinema" \
     --user="$(id -u):$(id -g)" \
     --volume="${HOME}/.config/asciinema:/run/user/$(id -u)/.config/asciinema:rw" \
     --volume="${PWD}:/data:rw" \
     --workdir='/data' \
-    docker.io/asciinema/asciinema rec
+    ghcr.io/asciinema/asciinema rec
 ```
 
 ## Usage
 
 asciinema is composed of multiple commands, similar to `git`, `apt-get` or
 `brew`.
 
@@ -261,15 +262,15 @@
 - `--rows=<n>` - Override terminal rows for recorded process
 - `-y, --yes` - Answer "yes" to all prompts (e.g. upload confirmation)
 - `-q, --quiet` - Be quiet, suppress all notices/warnings (implies -y)
 
 Stdin recording allows for capturing of all characters typed in by the user in
 the currently recorded shell. This may be used by a player (e.g.
 [asciinema-player](https://github.com/asciinema/asciinema-player)) to display
-pressed keys. Because it's basically a key-logging (scoped to a single shell
+pressed keys. Because it's basically key-logging (scoped to a single shell
 instance), it's disabled by default, and has to be explicitly enabled via
 `--stdin` option.
 
 ### `play <filename>`
 
 **Replay recorded asciicast in a terminal.**
 
@@ -318,14 +319,29 @@
 asciinema play dweb:/ipfs/QmNe7FsYaHc9SaDEAEXbaagAzNw9cH7YbzN4xV7jV1MCzK/ascii.cast
 ```
 
 Available options:
 
 - `-i, --idle-time-limit=<sec>` - Limit replayed terminal inactivity to max `<sec>` seconds
 - `-s, --speed=<factor>` - Playback speed (can be fractional)
+- `-l, --loop` - Play in a loop
+- `-m, --pause-on-markers` - Automatically pause on [markers](#markers)
+- `--stream=<stream>` - Select stream to play (see below)
+- `--out-fmt=<format>` - Select output format (see below)
+
+By default the output stream (`o`) is played. This is what you want in most
+cases.  If you recorded the input stream (`i`) with `asciinema rec --stdin` then
+you can replay it with `asciinema play --stream=i <filename>`.
+
+By default the selected stream is written to stdout in original, raw data form.
+This is also what you want in majority of cases. However you can change the
+output format to asciicast (newline delimited JSON) with `asciinema play
+--out-fmt=asciicast <filename>`. This allows delegating actual rendering to
+another place (e.g. outside of your terminal) by piping output of `asciinema
+play` to a tool of your choice.
 
 > For the best playback experience it is recommended to run `asciinema play` in
 > a terminal of dimensions not smaller than the one used for recording, as
 > there's no "transcoding" of control sequences for new terminal size.
 
 ### `cat <filename>`
 
@@ -370,14 +386,37 @@
 > A new install ID is generated on each machine and system user account you use
 > asciinema on, so in order to keep all recordings under a single asciinema.org
 > account you need to run `asciinema auth` on all of those machines.
 
 > asciinema versions prior to 2.0 confusingly referred to install ID as "API
 > token".
 
+## Markers
+
+Markers allow marking specific time locations in a recording, which can be used
+for navigation, as well as for automatic pausing of the playback.
+
+Markers can be added to a recording in several ways:
+
+- while you are recording, by pressing a configured hotkey, see [add_marker_key
+  config option](#configuration-file)
+- for existing recording, by inserting marker events (`"m"`) in the asciicast
+  file, see [marker event](doc/asciicast-v2.md#m---marker)
+
+When replaying a recording with `asciinema play` you can enable
+auto-pause-on-marker behaviour with `-m`/`--pause-on-markers` option (it's off
+by default). When a marker is encountered, the playback automatically pauses and
+can be resumed by pressing space bar key. The playback continues until next
+marker is encountered. You can also fast-forward to the next marker by pressing
+`]` key (when paused).
+
+Markers can be useful in e.g. live demos: you can create a recording with
+markers, then play it back during presentation, and have it stop wherever you
+want to explain terminal contents in more detail.
+
 ## Hosting the recordings on the web
 
 As mentioned in the `Usage > rec` section above, if the `filename` argument to
 `asciinema rec` is omitted then the recorded asciicast is uploaded to
 [asciinema.org](https://asciinema.org). You can watch it there and share it via
 secret URL.
 
@@ -428,14 +467,17 @@
 ; Be quiet, suppress all notices/warnings, default: no
 quiet = true
 
 ; Define hotkey for pausing recording (suspending capture of output),
 ; default: C-\ (control + backslash)
 pause_key = C-p
 
+; Define hotkey for adding a marker, default: none
+add_marker_key = C-x
+
 ; Define hotkey prefix key - when defined other recording hotkeys must
 ; be preceeded by it, default: no prefix
 prefix_key = C-a
 
 [play]
 
 ; Playback speed (can be fractional), default: 1
@@ -445,16 +487,20 @@
 idle_time_limit = 1
 
 ; Define hotkey for pausing/resuming playback,
 ; default: space
 pause_key = p
 
 ; Define hotkey for stepping through playback, a frame at a time,
-; default: .
-step_key = ]
+; default: . (dot)
+step_key = s
+
+; Define hotkey for jumping to the next marker,
+; default: ]
+next_marker_key = m
 
 [notifications]
 ; Desktop notifications are displayed on certain occasions, e.g. when
 ; pausing/resuming the capture of terminal with C-\ keyboard shortcut.
 
 ; Should desktop notifications be enabled, default: yes
 enabled = no
@@ -480,25 +526,27 @@
 
 If `$XDG_CONFIG_HOME` is set on Linux then asciinema uses
 `$XDG_CONFIG_HOME/asciinema` instead of `$HOME/.config/asciinema`.
 
 > asciinema versions prior to 1.1 used `$HOME/.asciinema`. If you have it
 > there you should `mv $HOME/.asciinema $HOME/.config/asciinema`.
 
+## Consulting
+
+I offer consulting services for asciinema project. See https://asciinema.org/consulting for more information.
+
 ## Contributing
 
 If you want to contribute to this project check out
 [Contributing](https://asciinema.org/contributing) page.
 
 ## Authors
 
 Developed with passion by [Marcin Kulik](http://ku1ik.com) and great open
 source [contributors](https://github.com/asciinema/asciinema/contributors).
 
 ## License
 
-Copyright &copy; 2011–2021 Marcin Kulik.
+© 2011 Marcin Kulik.
 
 All code is licensed under the GPL, v3 or later. See [LICENSE](./LICENSE) file
 for details.
-
-
```

### Comparing `asciinema-2.2.0/asciinema.egg-info/SOURCES.txt` & `asciinema-2.3.0/asciinema.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 asciinema/commands/command.py
 asciinema/commands/play.py
 asciinema/commands/record.py
 asciinema/commands/upload.py
 asciinema/data/icon-256x256.png
 doc/asciicast-v1.md
 doc/asciicast-v2.md
-man/asciinema.1
+man/asciinema.1
+tests/test_helper.py
```

### Comparing `asciinema-2.2.0/doc/asciicast-v1.md` & `asciinema-2.3.0/doc/asciicast-v1.md`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/doc/asciicast-v2.md` & `asciinema-2.3.0/doc/asciicast-v2.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 Example file:
 
 ```json
 {"version": 2, "width": 80, "height": 24, "timestamp": 1504467315, "title": "Demo", "env": {"TERM": "xterm-256color", "SHELL": "/bin/zsh"}}
 [0.248848, "o", "\u001b[1;31mHello \u001b[32mWorld!\u001b[0m\n"]
 [1.001376, "o", "That was ok\rThis is better."]
-[2.143733, "o", " "]
+[1.500000, "m", ""]
+[2.143733, "o", "Now... "]
 [6.541828, "o", "Bye!"]
 ```
 
 Suggested file extension is `.cast`, suggested media type is
 `application/x-asciicast`.
 
 ## Header
@@ -110,62 +111,74 @@
 
     [time, event-type, event-data]
 
 Where:
 
 * `time` (float) - indicates when this event happened, represented as the number
   of seconds since the beginning of the recording session,
-* `event-type` (string) - one of: `"o"`, `"i"`,
+* `event-type` (string) - one of: `"o"`, `"i"`, `"m"`
 * `event-data` (any) - event specific data, described separately for each event
   type.
 
 For example, let's look at the following line:
 
     [1.001376, "o", "Hello world"]
 
 It represents the event which:
 
 * happened 1.001376 sec after the start of the recording session,
-* is of type `"o"` (print to stdout, see below),
+* is of type `"o"` (output, write to a terminal, see below),
 * has data `"Hello world"`.
 
 ### Supported event types
 
 This section describes the event types supported in asciicast v2 format.
 
 The list is open to extension, and new event types may be added in both the
 current and future versions of the format. For example, we may add new event
 type for text overlay (subtitles display).
 
 A tool which interprets the event stream (web/cli player, post-processor) should
 ignore (or pass through) event types it doesn't understand or doesn't care
 about.
 
-#### "o" - data written to stdout
+#### "o" - output, data written to the terminal
 
 Event of type `"o"` represents printing new data to terminal's stdout.
 
-`event-data` is a string containing the data that was printed to a terminal. It
-has to be valid, UTF-8 encoded JSON string as described
-in [JSON RFC section 2.5](http://www.ietf.org/rfc/rfc4627.txt), with all
+`event-data` is a string containing the data that was printed. It must be valid,
+UTF-8 encoded JSON string as described in [JSON RFC section
+2.5](http://www.ietf.org/rfc/rfc4627.txt), with any non-printable Unicode
+codepoints encoded as `\uXXXX`.
+
+#### "i" - input, data read from the terminal
+
+Event of type `"i"` represents character typed in by the user, or more
+specifically, raw data sent from a terminal emulator to stdin of the recorded
+program (usually shell).
+
+`event-data` is a string containing captured ASCII character representing a key,
+or a control character like `"\r"` (enter), `"\u0001"` (ctrl-a), `"\u0003"`
+(ctrl-c), etc. Like with `"o"` event, it's UTF-8 encoded JSON string, with any
 non-printable Unicode codepoints encoded as `\uXXXX`.
 
-#### "i" - data read from stdin
+> Official asciinema recorder doesn't capture keyboard input by default. All
+> implementations of asciicast-compatible terminal recorder should not capture
+> it either unless explicitly permitted by the user.
 
-Event of type `"i"` represents character(s) typed in by the user, or
-more specifically, data sent from terminal emulator to stdin of the recorded
-shell.
+#### "m" - marker
 
-`event-data` is a string containing the captured character(s). Like with `"o"`
-event, it's UTF-8 encoded JSON string, with all non-printable Unicode codepoints
-encoded as `\uXXXX`.
+Event of type `"m"` represents a marker.
 
-> Official asciinema recorder doesn't capture stdin by default. All
-> implementations of asciicast-compatible terminal recorder should not capture
-> it either unless explicitly permitted by the user.
+When marker is encountered in the event stream and "pause on markers"
+functionality of the player is enabled, the playback should pause, and wait for
+the user to resume.
+
+`event-data` can be used to annotate a marker. Annotations may be used to e.g.
+show a list of named "chapters".
 
 ## Notes on compatibility
 
 Version 2 of asciicast file format solves several problems which couldn't be
 easily fixed in the old format:
 
 * minimal memory usage when recording and replaying arbitrarily long sessions -
```

### Comparing `asciinema-2.2.0/man/asciinema.1` & `asciinema-2.3.0/man/asciinema.1`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/pyproject.toml` & `asciinema-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asciinema-2.2.0/setup.cfg` & `asciinema-2.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = asciinema
-version = 2.2.0
+version = 2.3.0
 author = Marcin Kulik
 author_email = m@ku1ik.com
 url = https://asciinema.org
 download_url = 
 	https://github.com/asciinema/asciinema/archive/v%(version)s.tar.gz
 description = Terminal session recorder
 description_file = README.md
@@ -16,19 +16,19 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Natural Language :: English
 	Programming Language :: Python
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Shells
 	Topic :: Terminals
 	Topic :: Utilities
 
 [options]
 include_package_data = True
 packages =
```

