# Comparing `tmp/robingame-0.0.9.tar.gz` & `tmp/robingame-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingame-0.0.9.tar", last modified: Mon Oct 31 15:29:10 2022, max compression
+gzip compressed data, was "robingame-0.1.0.tar", last modified: Wed Jul  5 14:04:27 2023, max compression
```

## Comparing `robingame-0.0.9.tar` & `robingame-0.1.0.tar`

### file list

```diff
@@ -1,105 +1,115 @@
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.330294 robingame-0.0.9/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1070 2022-06-16 13:09:58.000000 robingame-0.0.9/LICENSE
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       30 2022-09-29 14:01:02.000000 robingame-0.0.9/MANIFEST.in
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      588 2022-10-31 15:29:10.330294 robingame-0.0.9/PKG-INFO
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       74 2022-09-29 13:11:16.000000 robingame-0.0.9/README.md
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       85 2022-06-16 13:11:40.000000 robingame-0.0.9/pyproject.toml
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.290295 robingame-0.0.9/robingame/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-04-13 14:09:00.000000 robingame-0.0.9/robingame/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.290295 robingame-0.0.9/robingame/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      142 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1699 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/__pycache__/animation.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     9555 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1094 2022-10-28 12:35:54.000000 robingame-0.0.9/robingame/animation.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.294294 robingame-0.0.9/robingame/examples/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.294294 robingame-0.0.9/robingame/examples/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      151 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/examples/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.294294 robingame-0.0.9/robingame/examples/gui_examples/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/gui_examples/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.294294 robingame-0.0.9/robingame/examples/gui_examples/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      164 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/examples/gui_examples/assets/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      235 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/examples/gui_examples/assets/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      412 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      663 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/button-up.aseprite
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      239 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/button-up.png
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1228 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/flashybutton.aseprite
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      638 2022-07-08 17:55:21.000000 robingame-0.0.9/robingame/examples/gui_examples/assets/flashybutton.png
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4384 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/examples/gui_examples/coloured_button_effects.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1987 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/examples/gui_examples/complicated_on_press_hook.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1816 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/examples/gui_examples/on_press_event.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/gui/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-04-13 14:09:00.000000 robingame-0.0.9/robingame/gui/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/gui/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      146 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/gui/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4755 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/gui/__pycache__/button.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     5043 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/gui/button.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     2960 2022-10-28 12:08:24.000000 robingame-0.0.9/robingame/gui/menu.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/image/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       70 2022-07-04 15:59:47.000000 robingame-0.0.9/robingame/image/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.298294 robingame-0.0.9/robingame/image/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      238 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/image/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     5612 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/image/__pycache__/classes.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     6058 2022-09-29 13:04:56.000000 robingame-0.0.9/robingame/image/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     5751 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/image/classes.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     6229 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/image/utils.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.306295 robingame-0.0.9/robingame/input/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      141 2022-10-31 15:27:34.000000 robingame-0.0.9/robingame/input/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.310294 robingame-0.0.9/robingame/input/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      227 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/input/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     2245 2022-10-23 14:36:20.000000 robingame-0.0.9/robingame/input/__pycache__/event.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)    14616 2022-10-31 15:15:29.000000 robingame-0.0.9/robingame/input/__pycache__/gamecube.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      816 2022-10-31 12:14:48.000000 robingame-0.0.9/robingame/input/__pycache__/keyboard.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4267 2022-10-31 12:14:48.000000 robingame-0.0.9/robingame/input/__pycache__/queue.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1623 2022-09-30 15:38:53.000000 robingame-0.0.9/robingame/input/event.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)    13533 2022-10-31 15:13:45.000000 robingame-0.0.9/robingame/input/gamecube.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      278 2022-10-23 16:14:19.000000 robingame-0.0.9/robingame/input/keyboard.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     3194 2022-10-23 16:14:19.000000 robingame-0.0.9/robingame/input/queue.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     5953 2022-10-31 15:26:24.000000 robingame-0.0.9/robingame/input/visualization.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.314294 robingame-0.0.9/robingame/objects/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      155 2022-10-31 15:24:56.000000 robingame-0.0.9/robingame/objects/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.318294 robingame-0.0.9/robingame/objects/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      246 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     5127 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/entity.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     3265 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/game.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1085 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/group.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1687 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1931 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/objects/__pycache__/particles.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4092 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/objects/entity.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     2711 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/objects/game.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      623 2022-04-26 15:21:33.000000 robingame-0.0.9/robingame/objects/group.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1189 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/objects/helpers.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1680 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/objects/particles.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4341 2022-10-20 20:14:55.000000 robingame-0.0.9/robingame/recording.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      566 2022-09-23 20:04:13.000000 robingame-0.0.9/robingame/sound.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.318294 robingame-0.0.9/robingame/text/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-08-14 15:34:27.000000 robingame-0.0.9/robingame/text/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.322295 robingame-0.0.9/robingame/text/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      147 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/text/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      315 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/text/__pycache__/exceptions.cpython-310.pyc
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.326295 robingame-0.0.9/robingame/text/assets/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        0 2022-08-14 15:34:27.000000 robingame-0.0.9/robingame/text/assets/__init__.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1138 2022-08-15 10:12:50.000000 robingame-0.0.9/robingame/text/assets/cellphone-black.png
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1103 2022-08-15 10:12:50.000000 robingame-0.0.9/robingame/text/assets/cellphone-white.png
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     8303 2022-08-14 15:36:03.000000 robingame-0.0.9/robingame/text/assets/test_font.aseprite
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     2612 2022-08-14 15:34:27.000000 robingame-0.0.9/robingame/text/assets/test_font.png
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       37 2022-08-14 15:34:27.000000 robingame-0.0.9/robingame/text/exceptions.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.326295 robingame-0.0.9/robingame/text/font/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       26 2022-09-19 07:33:39.000000 robingame-0.0.9/robingame/text/font/__init__.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.326295 robingame-0.0.9/robingame/text/font/__pycache__/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      188 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/text/font/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4036 2022-09-29 13:04:57.000000 robingame-0.0.9/robingame/text/font/__pycache__/classes.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1073 2022-10-23 14:36:20.000000 robingame-0.0.9/robingame/text/font/__pycache__/fonts.cpython-310.pyc
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     4112 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/text/font/classes.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1136 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/text/font/font_sandbox.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     1406 2022-09-29 13:48:23.000000 robingame-0.0.9/robingame/text/font/fonts.py
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     9175 2022-09-29 13:02:45.000000 robingame-0.0.9/robingame/utils.py
-drwxrwxr-x   0 binnev    (1000) binnev    (1000)        0 2022-10-31 15:29:10.290295 robingame-0.0.9/robingame.egg-info/
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      588 2022-10-31 15:29:10.000000 robingame-0.0.9/robingame.egg-info/PKG-INFO
--rw-rw-r--   0 binnev    (1000) binnev    (1000)     3165 2022-10-31 15:29:10.000000 robingame-0.0.9/robingame.egg-info/SOURCES.txt
--rw-rw-r--   0 binnev    (1000) binnev    (1000)        1 2022-10-31 15:29:10.000000 robingame-0.0.9/robingame.egg-info/dependency_links.txt
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       39 2022-10-31 15:29:10.000000 robingame-0.0.9/robingame.egg-info/requires.txt
--rw-rw-r--   0 binnev    (1000) binnev    (1000)       10 2022-10-31 15:29:10.000000 robingame-0.0.9/robingame.egg-info/top_level.txt
--rw-rw-r--   0 binnev    (1000) binnev    (1000)      721 2022-10-31 15:29:10.330294 robingame-0.0.9/setup.cfg
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1070 2023-05-14 09:02:00.000000 robingame-0.1.0/LICENSE
+-rw-rw-r--   0 robin     (1000) robin     (1000)       30 2023-05-14 09:02:00.000000 robingame-0.1.0/MANIFEST.in
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1005 2023-07-05 14:04:27.769086 robingame-0.1.0/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      491 2023-07-05 13:47:52.000000 robingame-0.1.0/README.md
+-rw-rw-r--   0 robin     (1000) robin     (1000)       85 2023-05-14 09:02:00.000000 robingame-0.1.0/pyproject.toml
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      141 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1696 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/__pycache__/animation.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7698 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1076 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/animation.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      150 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      163 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6899 2023-07-05 11:38:56.000000 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/assets/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      235 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/assets/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)      663 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)      239 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1228 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)      638 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4884 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/coloured_button_effects.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1836 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/complicated_on_press_hook.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1601 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/on_press_event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1711 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/particle_example.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/gui/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       50 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/gui/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/gui/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      215 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/gui/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4682 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/gui/__pycache__/button.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1563 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/gui/__pycache__/menu.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4973 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/gui/button.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1060 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/gui/menu.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/image/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/image/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      216 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4184 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/classes.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6057 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3928 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/classes.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6228 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/input/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      142 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/input/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      329 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2244 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/event.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)    14615 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/gamecube.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)      815 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/input/__pycache__/keyboard.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4266 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/queue.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1623 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    13533 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/gamecube.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      278 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/keyboard.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3194 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/queue.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5928 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/input/visualization.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/objects/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      139 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/objects/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      338 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3021 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/entity.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2985 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/game.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1668 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/group.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1707 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/helpers.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2105 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/particles.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2755 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/entity.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2526 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/game.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1098 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/group.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1188 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/helpers.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2045 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/particles.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4452 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/recording.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      566 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/sound.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      146 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)      314 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/__pycache__/exceptions.cpython-310.pyc
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/assets/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1138 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/cellphone-black.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1103 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/cellphone-white.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8303 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/test_font.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2612 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/test_font.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)       37 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/exceptions.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/font/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       26 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/font/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/font/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      187 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/font/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4035 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/font/__pycache__/classes.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1073 2023-06-29 14:47:29.000000 robingame-0.1.0/robingame/text/font/__pycache__/fonts.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4112 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/font/classes.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1142 2023-06-29 14:58:35.000000 robingame-0.1.0/robingame/text/font/font_sandbox.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1415 2023-06-29 14:47:25.000000 robingame-0.1.0/robingame/text/font/fonts.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7727 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1005 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3459 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       45 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       10 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)      728 2023-07-05 14:04:27.769086 robingame-0.1.0/setup.cfg
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/tests/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      469 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_animation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2028 2023-07-05 10:07:02.000000 robingame-0.1.0/tests/test_event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7148 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_image.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4392 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_inputs.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1036 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_text.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2289 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_utils.py
```

### Comparing `robingame-0.0.9/LICENSE` & `robingame-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/animation.py` & `robingame-0.1.0/robingame/animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
         raise ValueError(f"{x=} is greater than {num=}")
     distance = stop - start
     progress = x / num
     value = start + function(progress) * distance
     return value
 
 
-def ease_in(x, start, stop, num, power=3) -> numpy.array:
+def ease_in(x, start, stop, num, power=3) -> float:
     f = lambda x: x**power
     return ease(x=x, start=start, stop=stop, num=num, function=f)
 
 
-def ease_out(x, start, stop, num, power=3) -> numpy.array:
+def ease_out(x, start, stop, num, power=3) -> float:
     f = lambda x: 1 - (1 - x) ** power
     return ease(x=x, start=start, stop=stop, num=num, function=f)
 
 
-def ease_in_out(x, start, stop, num, power=3) -> numpy.array:
+def ease_in_out(x, start, stop, num, power=3) -> float:
     f = lambda x: 4 * x**power if x < 0.5 else 1 - (-2 * x + 2) ** power / 2
     return ease(x=x, start=start, stop=stop, num=num, function=f)
 
 
 def damping_response(t, amp=0.5, damping=0.4, phase=0, freq=0.3):
     decay = damping * freq
     return amp * numpy.e ** (-decay * t) * numpy.cos(freq * t - phase)
```

### Comparing `robingame-0.0.9/robingame/examples/gui_examples/assets/button-up.aseprite` & `robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/examples/gui_examples/assets/flashybutton.aseprite` & `robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/examples/gui_examples/assets/flashybutton.png` & `robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.png`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/examples/gui_examples/coloured_button_effects.py` & `robingame-0.1.0/robingame/examples/gui_examples/coloured_button_effects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,41 @@
 import pygame.mouse
+from pygame import Surface, Rect, Color
 
 from robingame.animation import damping_response
 from robingame.examples.gui_examples.assets import button_flash
+from robingame.gui import Menu
 from robingame.gui.button import Button
 from robingame.image import scale_image, brighten, SpriteAnimation
 from robingame.objects import Game, Group, Particle
 from robingame.utils import mouse_hovering_over, random_int
 
 
-class ButtonWithImages(Button):
+class MyButton(Button):
+    image: Surface
+    rect: Rect  # used for collision detection
+    debug_color = Color("red")
+
+    def draw(self, surface: Surface, debug: bool = False):
+        super().draw(surface, debug)
+        image_rect = self.image.get_rect()
+        image_rect.center = self.rect.center
+        surface.blit(self.image, image_rect)
+        if debug:
+            pygame.draw.rect(surface, color=self.debug_color, rect=self.rect, width=1)
+            pygame.draw.rect(surface, color=self.debug_color, rect=(*self.rect.center, 2, 2))
+
+
+class ButtonWithImages(MyButton):
     frame_duration = 3
 
+    @property
+    def animation_frame(self):
+        return self.tick // self.frame_duration
+
     def __init__(self, x: int, y: int, width: int, height: int, **kwargs):
         super().__init__(x, y, width, height, **kwargs)
         self.image_idle = button_flash.images[-1]
         self.image_pressed = brighten(scale_image(self.image_idle.copy(), 0.9), amount=-50)
         self.image = self.image_idle
 
     def state_idle(self):
@@ -34,15 +55,15 @@
         self.animation = button_flash
 
     def on_release(self):
         super().on_release()
         self.animation = SpriteAnimation(images=[self.image_idle])
 
 
-class BouncyButton(Button):
+class BouncyButton(MyButton):
     frame_duration = 3
 
     def __init__(self, x: int, y: int, width: int, height: int, **kwargs):
         super().__init__(x, y, width, height, **kwargs)
         self.image = button_flash.play(0)
         sizes = [damping_response(t) for t in range(20)]
         self.animation = button_flash
@@ -84,46 +105,38 @@
 
     screen_color = (50, 50, 50)
     window_width = 500
     window_height = 500
 
     def __init__(self):
         super().__init__()
-        self.buttons = Group()
+        self.scenes = Group()
         self.particles = Group()
-        self.child_groups += [self.buttons, self.particles]
-        self.buttons.add(
+        self.child_groups += [self.scenes, self.particles]
+        menu = Menu()
+        menu.buttons.add(
             ButtonWithImages(
                 x=200,
                 y=100,
                 width=200,
                 height=100,
                 text="press and hold for smoke",
                 on_release=(
                     lambda button: (
-                        self.particles.add(Flash(x=button.x, y=button.y)),
-                        self.particles.add(Glow(x=button.x, y=button.y) for _ in range(50)),
+                        self.particles.add(Flash(x=button.rect.centerx, y=button.rect.centery)),
+                        self.particles.add(
+                            Glow(x=button.rect.centerx, y=button.rect.centery) for _ in range(50)
+                        ),
                     )
                 ),
                 on_unfocus=(lambda button: self.particles.kill()),
             ),
             BouncyButton(x=200, y=300, width=200, height=100),
         )
-
-    def update(self):
-        super().update()
-
-        # button manager stuff
-        for button in self.buttons:
-            if mouse_hovering_over(button):
-                button.is_focused = True
-                button.is_pressed = pygame.mouse.get_pressed()[0]
-            else:
-                button.is_focused = False
-                button.is_pressed = False
+        self.scenes.add(menu)
 
 
 class Flash(Particle):
     gravity = 0.1
     friction = 0.01
     decay = 20
     color = (150, 200, 150)
```

### Comparing `robingame-0.0.9/robingame/examples/gui_examples/on_press_event.py` & `robingame-0.1.0/robingame/examples/gui_examples/on_press_event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 from dataclasses import dataclass
 
 import pygame.mouse
 
-from robingame.gui.button import Button
+from robingame.examples.gui_examples.coloured_button_effects import MyButton
+from robingame.gui import Menu
 from robingame.input import EventQueue
 from robingame.objects import Game, Group
-from robingame.utils import mouse_hovering_over
 
 
 class OnPressEventExample(Game):
     """
     This is an example where the hooks increment/decrement a value stored on the outer Game class.
     """
 
     screen_color = (50, 50, 50)
 
     def __init__(self):
         super().__init__()
         self.value = 0
-        self.buttons = Group()
+        self.scenes = Group()
         self.particles = Group()
-        self.child_groups += [self.buttons, self.particles]
-        self.buttons.add(
-            Button(
+        self.child_groups += [self.scenes, self.particles]
+        menu = Menu()
+        self.scenes.add(menu)
+        menu.buttons.add(
+            MyButton(
                 x=200,
                 y=100,
                 width=200,
                 height=50,
                 text="change value",
                 on_press=lambda button: EventQueue.add(ChangeValue(amount=5)),
                 on_release=lambda button: EventQueue.add(ChangeValue(amount=-5)),
                 on_focus=lambda button: EventQueue.add(ChangeValue(amount=1)),
                 on_unfocus=lambda button: EventQueue.add(ChangeValue(amount=-1)),
             )
         )
 
     def update(self):
         super().update()
+        self.listen_events()
 
-        # listen for events
+    def listen_events(self):
         if event := EventQueue.get(type=ChangeValue.type):
             self.value += event.amount
-        print(f"{self.value=}")
-
-        # button manager stuff
-        for button in self.buttons:
-            if mouse_hovering_over(button):
-                button.is_focused = True
-                button.is_pressed = pygame.mouse.get_pressed()[0]
-            else:
-                button.is_focused = False
-                button.is_pressed = False
+            print(f"{self.value=}")
 
 
 @dataclass
 class ChangeValue:
     type = pygame.event.custom_type()
     amount: int = 1
```

### Comparing `robingame-0.0.9/robingame/gui/__pycache__/button.cpython-310.pyc` & `robingame-0.1.0/robingame/gui/__pycache__/button.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 5043 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,298 +1,293 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 b313 0000  o.......u.5c....
+00000000: 6f0d 0d0a 0000 0000 8874 a564 6d13 0000  o........t.dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6403 6c02 6d03 5a03 0100 6400  Z.d.d.l.m.Z...d.
+00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
+00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
-00000060: 6d07 5a07 0100 6400 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000070: 0100 4700 6407 6408 8400 6408 6507 8303  ..G.d.d...d.e...
-00000080: 5a0a 4700 6409 640a 8400 640a 650a 8303  Z.G.d.d...d.e...
-00000090: 5a0b 6402 5300 290b e900 0000 0029 01da  Z.d.S.)......)..
-000000a0: 0843 616c 6c61 626c 654e 2901 da05 436f  .CallableN)...Co
-000000b0: 6c6f 7229 01da 0452 6563 7429 01da 0e50  lor)...Rect)...P
-000000c0: 6879 7369 6361 6c45 6e74 6974 7929 01da  hysicalEntity)..
-000000d0: 0d70 756c 7369 6e67 5f76 616c 7565 6300  .pulsing_valuec.
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0009  ................
-000000f0: 0000 0000 0000 0073 b800 0000 6500 5a01  .......s....e.Z.
-00000100: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
-00000110: 3c00 6504 6505 6403 3c00 6404 5a06 6405  <.e.e.d.<.d.Z.d.
-00000120: 5a07 6508 6505 6406 3c00 0907 0907 0907  Z.e.e.d.<.......
-00000130: 0907 0907 6424 6408 6509 6409 6509 640a  ....d$d.e.d.e.d.
-00000140: 6509 640b 6509 6608 8700 6601 640c 640d  e.d.e.f...f.d.d.
-00000150: 840d 5a0a 640e 640f 8400 5a0b 6410 6411  ..Z.d.d...Z.d.d.
-00000160: 8400 5a0c 6412 6413 8400 5a0d 6414 6415  ..Z.d.d...Z.d.d.
-00000170: 8400 5a0e 6416 6417 8400 5a0f 6418 6419  ..Z.d.d...Z.d.d.
-00000180: 8400 5a10 641a 641b 8400 5a11 641c 641d  ..Z.d.d...Z.d.d.
-00000190: 8400 5a12 641e 641f 8400 5a13 6420 6421  ..Z.d.d...Z.d d!
-000001a0: 8400 5a14 6422 6423 8400 5a15 8700 0400  ..Z.d"d#..Z.....
-000001b0: 5a16 5300 2925 da06 4275 7474 6f6e 61e9  Z.S.)%..Buttona.
-000001c0: 0100 000a 2020 2020 4755 4920 6275 7474  ....    GUI butt
-000001d0: 6f6e 2065 6e74 6974 792e 2052 6561 6374  on entity. React
-000001e0: 7320 746f 2063 6861 6e67 6573 2069 6e20  s to changes in 
-000001f0: 7468 6520 6973 5f66 6f63 7573 6564 2061  the is_focused a
-00000200: 6e64 2069 735f 7072 6573 7365 6420 626f  nd is_pressed bo
-00000210: 6f6c 6561 6e73 2c20 6275 7420 646f 6573  oleans, but does
-00000220: 6e27 740a 2020 2020 7365 7420 7468 656d  n't.    set them
-00000230: 2028 6120 7061 7265 6e74 206d 656e 7520   (a parent menu 
-00000240: 636c 6173 7320 6f72 2073 6f6d 6574 6869  class or somethi
-00000250: 6e67 2065 6c73 6520 7368 6f75 6c64 2073  ng else should s
-00000260: 6574 2074 6865 6d29 2e20 5468 6973 2069  et them). This i
-00000270: 7320 736f 2074 6861 7420 6561 6368 2042  s so that each B
-00000280: 7574 746f 6e0a 2020 2020 646f 6573 6e27  utton.    doesn'
-00000290: 7420 6861 7665 2074 6f20 646f 2069 7473  t have to do its
-000002a0: 206f 776e 2069 6e70 7574 2064 6574 6563   own input detec
-000002b0: 7469 6f6e 2e20 4974 2061 6c73 6f20 616c  tion. It also al
-000002c0: 6c6f 7773 2061 2070 6172 656e 7420 6d65  lows a parent me
-000002d0: 6e75 2063 6c61 7373 2074 6f20 7461 6b65  nu class to take
-000002e0: 2069 6e74 6f0a 2020 2020 6163 636f 756e   into.    accoun
-000002f0: 7420 6164 6469 7469 6f6e 616c 2063 6f6e  t additional con
-00000300: 7465 7874 2065 2e67 2e20 7368 6966 7469  text e.g. shifti
-00000310: 6e67 2066 6f63 7573 2066 726f 6d20 6f6e  ng focus from on
-00000320: 6520 6275 7474 6f6e 2074 6f20 616e 6f74  e button to anot
-00000330: 6865 7220 7573 696e 6720 6120 6b65 7962  her using a keyb
-00000340: 6f61 7264 206f 720a 2020 2020 6a6f 7973  oard or.    joys
-00000350: 7469 636b 2069 6e70 7574 2e20 4f70 6572  tick input. Oper
-00000360: 6174 696f 6e73 206c 696b 6520 7468 6973  ations like this
-00000370: 2077 6f75 6c64 2062 6520 6265 796f 6e64   would be beyond
-00000380: 2074 6865 2073 636f 7065 206f 6620 6120   the scope of a 
-00000390: 7369 6e67 6c65 2042 7574 746f 6e20 696e  single Button in
-000003a0: 7374 616e 6365 2e0a 2020 2020 da0a 6973  stance..    ..is
-000003b0: 5f66 6f63 7573 6564 da0a 6973 5f70 7265  _focused..is_pre
-000003c0: 7373 6564 da06 7562 756e 7475 e914 0000  ssed..ubuntu....
-000003d0: 00da 0a74 6578 745f 636f 6c6f 724e da01  ...text_colorN..
-000003e0: 78da 0179 da05 7769 6474 68da 0668 6569  x..y..width..hei
-000003f0: 6768 7463 0a00 0000 0000 0000 0000 0000  ghtc............
-00000400: 0b00 0000 0600 0000 0300 0000 7300 0100  ............s...
-00000410: 007c 037c 005f 007c 047c 005f 017c 057c  .|.|._.|.|._.|.|
-00000420: 005f 0274 0364 0164 017c 037c 0483 047c  ._.t.d.d.|.|...|
-00000430: 005f 047c 017c 0266 027c 006a 045f 0564  ._.|.|.f.|.j._.d
-00000440: 027c 005f 0664 027c 005f 077c 0670 2264  .|._.d.|._.|.p"d
-00000450: 0364 0484 007c 005f 087c 0770 2964 0564  .d...|._.|.p)d.d
-00000460: 0484 007c 005f 097c 0870 3064 0664 0484  ...|._.|.p0d.d..
-00000470: 007c 005f 0a7c 0970 3764 0764 0484 007c  .|._.|.p7d.d...|
-00000480: 005f 0b74 0c6a 0da0 0e74 0c6a 0da0 0fa1  ._.t.j...t.j....
-00000490: 007c 006a 10a1 027c 005f 0d7c 006a 117c  .|.j...|._.|.j.|
-000004a0: 005f 1274 0ca0 137c 006a 046a 14a1 017c  ._.t...|.j.j...|
-000004b0: 005f 157c 006a 15a0 1674 1764 0883 01a1  ._.|.j...t.d....
-000004c0: 0101 007c 006a 0272 797c 006a 0da0 187c  ...|.j.ry|.j...|
-000004d0: 006a 0264 0974 1764 0a83 01a1 037d 057c  .j.d.t.d.....}.|
-000004e0: 05a0 19a1 007d 0a7c 006a 15a0 19a1 006a  .....}.|.j.....j
-000004f0: 057c 0a5f 057c 006a 15a0 1a7c 057c 0aa1  .|._.|.j...|.|..
-00000500: 0201 0074 1b83 00a0 1ca1 0001 0064 0053  ...t.........d.S
-00000510: 0029 0b4e 7201 0000 0046 6301 0000 0000  .).Nr....Fc.....
-00000520: 0000 0000 0000 0001 0000 0001 0000 0053  ...............S
-00000530: 0000 00f3 0400 0000 6400 5300 a901 4ea9  ........d.S...N.
-00000540: 00a9 01da 0662 7574 746f 6e72 1300 0000  .....buttonr....
-00000550: 7213 0000 00fa 332f 686f 6d65 2f62 696e  r.....3/home/bin
-00000560: 6e65 762f 636f 6465 2f72 6f62 696e 6761  nev/code/robinga
-00000570: 6d65 2f72 6f62 696e 6761 6d65 2f67 7569  me/robingame/gui
-00000580: 2f62 7574 746f 6e2e 7079 da08 3c6c 616d  /button.py..<lam
-00000590: 6264 613e 2d00 0000 f302 0000 0004 007a  bda>-..........z
-000005a0: 2142 7574 746f 6e2e 5f5f 696e 6974 5f5f  !Button.__init__
-000005b0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000005c0: 613e 6301 0000 0000 0000 0000 0000 0001  a>c.............
-000005d0: 0000 0001 0000 0053 0000 0072 1100 0000  .......S...r....
-000005e0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-000005f0: 1300 0000 7213 0000 0072 1600 0000 7217  ....r....r....r.
-00000600: 0000 002e 0000 0072 1800 0000 6301 0000  .......r....c...
-00000610: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000620: 0053 0000 0072 1100 0000 7212 0000 0072  .S...r....r....r
-00000630: 1300 0000 7214 0000 0072 1300 0000 7213  ....r....r....r.
-00000640: 0000 0072 1600 0000 7217 0000 002f 0000  ...r....r..../..
-00000650: 0072 1800 0000 6301 0000 0000 0000 0000  .r....c.........
-00000660: 0000 0001 0000 0001 0000 0053 0000 0072  ...........S...r
-00000670: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00000680: 0000 0072 1300 0000 7213 0000 0072 1600  ...r....r....r..
-00000690: 0000 7217 0000 0030 0000 0072 1800 0000  ..r....0...r....
-000006a0: da03 7265 6454 da05 626c 6163 6b29 1d72  ..redT..black).r
-000006b0: 0f00 0000 7210 0000 00da 0474 6578 7472  ....r......textr
-000006c0: 0400 0000 da04 7265 6374 da06 6365 6e74  ......rect..cent
-000006d0: 6572 7208 0000 0072 0900 0000 da09 5f6f  err....r......_o
-000006e0: 6e5f 7072 6573 73da 095f 6f6e 5f66 6f63  n_press.._on_foc
-000006f0: 7573 da0b 5f6f 6e5f 7265 6c65 6173 65da  us.._on_release.
-00000700: 0b5f 6f6e 5f75 6e66 6f63 7573 da06 7079  ._on_unfocus..py
-00000710: 6761 6d65 da04 666f 6e74 da04 466f 6e74  game..font..Font
-00000720: da10 6765 745f 6465 6661 756c 745f 666f  ..get_default_fo
-00000730: 6e74 da09 666f 6e74 5f73 697a 65da 0a73  nt..font_size..s
-00000740: 7461 7465 5f69 646c 65da 0573 7461 7465  tate_idle..state
-00000750: da07 5375 7266 6163 65da 0473 697a 65da  ..Surface..size.
-00000760: 0569 6d61 6765 da04 6669 6c6c 7203 0000  .image..fillr...
-00000770: 00da 0672 656e 6465 72da 0867 6574 5f72  ...render..get_r
-00000780: 6563 74da 0462 6c69 74da 0573 7570 6572  ect..blit..super
-00000790: da08 5f5f 696e 6974 5f5f 290b da04 7365  ..__init__)...se
-000007a0: 6c66 720d 0000 0072 0e00 0000 720f 0000  lfr....r....r...
-000007b0: 0072 1000 0000 721b 0000 00da 086f 6e5f  .r....r......on_
-000007c0: 7072 6573 73da 086f 6e5f 666f 6375 73da  press..on_focus.
-000007d0: 0a6f 6e5f 7265 6c65 6173 65da 0a6f 6e5f  .on_release..on_
-000007e0: 756e 666f 6375 735a 0874 6578 7452 6563  unfocusZ.textRec
-000007f0: 74a9 01da 095f 5f63 6c61 7373 5f5f 7213  t....__class__r.
-00000800: 0000 0072 1600 0000 7231 0000 001a 0000  ...r....r1......
-00000810: 0073 2a00 0000 060c 0601 0601 1001 0c01  .s*.............
-00000820: 0601 0601 0e01 0e01 0e01 0e01 1801 0801  ................
-00000830: 1001 1001 0601 1601 0801 0e01 0e01 0e01  ................
-00000840: 7a0f 4275 7474 6f6e 2e5f 5f69 6e69 745f  z.Button.__init_
-00000850: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000860: 0000 0200 0000 4300 0000 7324 0000 007c  ......C...s$...|
-00000870: 006a 0072 077c 00a0 01a1 0001 007c 006a  .j.r.|.......|.j
-00000880: 0272 107c 00a0 03a1 0001 0064 0053 0064  .r.|.......d.S.d
-00000890: 0053 0072 1200 0000 2904 7208 0000 00da  .S.r....).r.....
-000008a0: 0566 6f63 7573 7209 0000 00da 0570 7265  .focusr......pre
-000008b0: 7373 a901 7232 0000 0072 1300 0000 7213  ss..r2...r....r.
-000008c0: 0000 0072 1600 0000 7227 0000 003f 0000  ...r....r'...?..
-000008d0: 00f3 0a00 0000 0601 0801 0601 0c01 04ff  ................
-000008e0: 7a11 4275 7474 6f6e 2e73 7461 7465 5f69  z.Button.state_i
-000008f0: 646c 6563 0100 0000 0000 0000 0000 0000  dlec............
-00000900: 0100 0000 0200 0000 4300 0000 7324 0000  ........C...s$..
-00000910: 007c 006a 0073 077c 00a0 01a1 0001 007c  .|.j.s.|.......|
-00000920: 006a 0272 107c 00a0 03a1 0001 0064 0053  .j.r.|.......d.S
-00000930: 0064 0053 0072 1200 0000 2904 7208 0000  .d.S.r....).r...
-00000940: 00da 0775 6e66 6f63 7573 7209 0000 0072  ...unfocusr....r
-00000950: 3a00 0000 723b 0000 0072 1300 0000 7213  :...r;...r....r.
-00000960: 0000 0072 1600 0000 da0b 7374 6174 655f  ...r......state_
-00000970: 666f 6375 7345 0000 0072 3c00 0000 7a12  focusE...r<...z.
-00000980: 4275 7474 6f6e 2e73 7461 7465 5f66 6f63  Button.state_foc
-00000990: 7573 6301 0000 0000 0000 0000 0000 0001  usc.............
-000009a0: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
-000009b0: 7c00 6a00 7309 7c00 a001 a100 0100 6400  |.j.s.|.......d.
-000009c0: 5300 6400 5300 7212 0000 0029 0272 0900  S.d.S.r....).r..
-000009d0: 0000 da07 7265 6c65 6173 6572 3b00 0000  ....releaser;...
-000009e0: 7213 0000 0072 1300 0000 7216 0000 00da  r....r....r.....
-000009f0: 0b73 7461 7465 5f70 7265 7373 4b00 0000  .state_pressK...
-00000a00: 7306 0000 0006 010c 0104 ff7a 1242 7574  s..........z.But
-00000a10: 746f 6e2e 7374 6174 655f 7072 6573 7363  ton.state_pressc
-00000a20: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000a30: 0300 0000 4300 0000 f30e 0000 007c 00a0  ....C........|..
-00000a40: 007c 00a1 0101 0064 0053 0072 1200 0000  .|.....d.S.r....
-00000a50: 2901 721e 0000 0072 3b00 0000 7213 0000  ).r....r;...r...
-00000a60: 0072 1300 0000 7216 0000 0072 3300 0000  .r....r....r3...
-00000a70: 5900 0000 f302 0000 000e 017a 0f42 7574  Y..........z.But
-00000a80: 746f 6e2e 6f6e 5f70 7265 7373 6301 0000  ton.on_pressc...
-00000a90: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000aa0: 0043 0000 0072 4100 0000 7212 0000 0029  .C...rA...r....)
-00000ab0: 0172 2000 0000 723b 0000 0072 1300 0000  .r ...r;...r....
-00000ac0: 7213 0000 0072 1600 0000 7235 0000 005c  r....r....r5...\
-00000ad0: 0000 0072 4200 0000 7a11 4275 7474 6f6e  ...rB...z.Button
-00000ae0: 2e6f 6e5f 7265 6c65 6173 6563 0100 0000  .on_releasec....
-00000af0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000b00: 4300 0000 7241 0000 0072 1200 0000 2901  C...rA...r....).
-00000b10: 721f 0000 0072 3b00 0000 7213 0000 0072  r....r;...r....r
-00000b20: 1300 0000 7216 0000 0072 3400 0000 5f00  ....r....r4..._.
-00000b30: 0000 7242 0000 007a 0f42 7574 746f 6e2e  ..rB...z.Button.
-00000b40: 6f6e 5f66 6f63 7573 6301 0000 0000 0000  on_focusc.......
-00000b50: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000b60: 0072 4100 0000 7212 0000 0029 0172 2100  .rA...r....).r!.
-00000b70: 0000 723b 0000 0072 1300 0000 7213 0000  ..r;...r....r...
-00000b80: 0072 1600 0000 7236 0000 0062 0000 0072  .r....r6...b...r
-00000b90: 4200 0000 7a11 4275 7474 6f6e 2e6f 6e5f  B...z.Button.on_
-00000ba0: 756e 666f 6375 7363 0100 0000 0000 0000  unfocusc........
-00000bb0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000bc0: f314 0000 007c 00a0 00a1 0001 007c 006a  .....|.......|.j
-00000bd0: 017c 005f 0264 0053 0072 1200 0000 2903  .|._.d.S.r....).
-00000be0: 7233 0000 0072 4000 0000 7228 0000 0072  r3...r@...r(...r
-00000bf0: 3b00 0000 7213 0000 0072 1300 0000 7216  ;...r....r....r.
-00000c00: 0000 0072 3a00 0000 6900 0000 f304 0000  ...r:...i.......
-00000c10: 0008 010c 017a 0c42 7574 746f 6e2e 7072  .....z.Button.pr
-00000c20: 6573 7363 0100 0000 0000 0000 0000 0000  essc............
-00000c30: 0100 0000 0200 0000 4300 0000 7243 0000  ........C...rC..
-00000c40: 0072 1200 0000 2903 7234 0000 0072 3e00  .r....).r4...r>.
-00000c50: 0000 7228 0000 0072 3b00 0000 7213 0000  ..r(...r;...r...
-00000c60: 0072 1300 0000 7216 0000 0072 3900 0000  .r....r....r9...
-00000c70: 6d00 0000 7244 0000 007a 0c42 7574 746f  m...rD...z.Butto
-00000c80: 6e2e 666f 6375 7363 0100 0000 0000 0000  n.focusc........
-00000c90: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000ca0: 7326 0000 007c 00a0 00a1 0001 007c 006a  s&...|.......|.j
-00000cb0: 0172 0d7c 006a 027c 005f 0464 0053 007c  .r.|.j.|._.d.S.|
-00000cc0: 006a 037c 005f 0464 0053 0072 1200 0000  .j.|._.d.S.r....
-00000cd0: 2905 7235 0000 0072 0800 0000 723e 0000  ).r5...r....r>..
-00000ce0: 0072 2700 0000 7228 0000 0072 3b00 0000  .r'...r(...r;...
-00000cf0: 7213 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
-00000d00: 3f00 0000 7100 0000 7304 0000 0008 011e  ?...q...s.......
-00000d10: 017a 0e42 7574 746f 6e2e 7265 6c65 6173  .z.Button.releas
-00000d20: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000d30: 0000 0200 0000 4300 0000 7243 0000 0072  ......C...rC...r
-00000d40: 1200 0000 2903 7236 0000 0072 2700 0000  ....).r6...r'...
-00000d50: 7228 0000 0072 3b00 0000 7213 0000 0072  r(...r;...r....r
-00000d60: 1300 0000 7216 0000 0072 3d00 0000 7500  ....r....r=...u.
-00000d70: 0000 7244 0000 007a 0e42 7574 746f 6e2e  ..rD...z.Button.
-00000d80: 756e 666f 6375 7329 054e 4e4e 4e4e 2917  unfocus).NNNNN).
-00000d90: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000da0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000db0: 6d65 5f5f da07 5f5f 646f 635f 5fda 0462  me__..__doc__..b
-00000dc0: 6f6f 6cda 0f5f 5f61 6e6e 6f74 6174 696f  ool..__annotatio
-00000dd0: 6e73 5f5f 5a09 666f 6e74 5f6e 616d 6572  ns__Z.font_namer
-00000de0: 2600 0000 7203 0000 00da 0369 6e74 7231  &...r......intr1
-00000df0: 0000 0072 2700 0000 723e 0000 0072 4000  ...r'...r>...r@.
-00000e00: 0000 7233 0000 0072 3500 0000 7234 0000  ..r3...r5...r4..
-00000e10: 0072 3600 0000 723a 0000 0072 3900 0000  .r6...r:...r9...
-00000e20: 723f 0000 0072 3d00 0000 da0d 5f5f 636c  r?...r=.....__cl
-00000e30: 6173 7363 656c 6c5f 5f72 1300 0000 7213  asscell__r....r.
-00000e40: 0000 0072 3700 0000 7216 0000 0072 0700  ...r7...r....r..
-00000e50: 0000 0b00 0000 7340 0000 000a 0004 0108  ......s@........
-00000e60: 0808 0104 0104 0108 0102 0802 0102 0102  ................
-00000e70: 0102 0104 f602 0202 fe02 0302 fd02 0402  ................
-00000e80: fc02 050e fb08 2508 0608 0608 0e08 0308  ......%.........
-00000e90: 0308 0308 0708 0408 0410 0472 0700 0000  ...........r....
-00000ea0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000eb0: 0003 0000 0000 0000 0073 5000 0000 6500  .........sP...e.
-00000ec0: 5a01 6400 5a02 6401 5a03 6504 6402 8301  Z.d.Z.d.Z.e.d...
-00000ed0: 5a05 6504 6403 8301 5a06 6504 6404 8301  Z.e.d...Z.e.d...
-00000ee0: 5a07 8700 6601 6405 6406 8408 5a08 8700  Z...f.d.d...Z...
-00000ef0: 6601 6407 6408 8408 5a09 8700 6601 6409  f.d.d...Z...f.d.
-00000f00: 640a 8408 5a0a 8700 0400 5a0b 5300 290b  d...Z.....Z.S.).
-00000f10: da0d 436f 6c6f 7265 6442 7574 746f 6e29  ..ColoredButton)
-00000f20: 03e9 6400 0000 7201 0000 0072 4e00 0000  ..d...r....rN...
-00000f30: da06 6f72 616e 6765 7219 0000 00da 0577  ..oranger......w
-00000f40: 6869 7465 6301 0000 0000 0000 0000 0000  hitec...........
-00000f50: 0001 0000 0005 0000 0003 0000 0073 2600  .............s&.
-00000f60: 0000 7400 8300 a001 a100 0100 7402 7c00  ..t.........t.|.
-00000f70: 6a03 6401 6402 6403 8304 6404 6405 6603  j.d.d.d...d.d.f.
-00000f80: 7c00 5f04 6400 5300 2906 4ee9 5000 0000  |._.d.S.).N.P...
-00000f90: e996 0000 0067 b81e 85eb 51b8 9e3f e91e  .....g....Q..?..
-00000fa0: 0000 00e9 4b00 0000 2905 7230 0000 0072  ....K...).r0...r
-00000fb0: 2700 0000 7206 0000 00da 0474 6963 6bda  '...r......tick.
-00000fc0: 0563 6f6c 6f72 723b 0000 0072 3700 0000  .colorr;...r7...
-00000fd0: 7213 0000 0072 1600 0000 7227 0000 0080  r....r....r'....
-00000fe0: 0000 0073 0400 0000 0a01 1c01 7a18 436f  ...s........z.Co
-00000ff0: 6c6f 7265 6442 7574 746f 6e2e 7374 6174  loredButton.stat
-00001000: 655f 6964 6c65 6301 0000 0000 0000 0000  e_idlec.........
-00001010: 0000 0001 0000 0006 0000 0003 0000 0073  ...............s
-00001020: 3200 0000 7400 8300 a001 a100 0100 7402  2...t.........t.
-00001030: 7c00 6a03 6401 6402 6403 8304 7402 7c00  |.j.d.d.d...t.|.
-00001040: 6a03 6404 6405 6403 8304 6406 6603 7c00  j.d.d.d...d.f.|.
-00001050: 5f04 6400 5300 2907 4ee9 b400 0000 e9ff  _.d.S.).N.......
-00001060: 0000 0067 3333 3333 3333 d33f 724e 0000  ...g333333.?rN..
-00001070: 00e9 a300 0000 7201 0000 0029 0572 3000  ......r....).r0.
-00001080: 0000 723e 0000 0072 0600 0000 7255 0000  ..r>...r....rU..
-00001090: 0072 5600 0000 723b 0000 0072 3700 0000  .rV...r;...r7...
-000010a0: 7213 0000 0072 1600 0000 723e 0000 0084  r....r....r>....
-000010b0: 0000 0073 0a00 0000 0a01 0e02 0e01 0201  ...s............
-000010c0: 0afd 7a19 436f 6c6f 7265 6442 7574 746f  ..z.ColoredButto
-000010d0: 6e2e 7374 6174 655f 666f 6375 7363 0100  n.state_focusc..
-000010e0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000010f0: 0000 0300 0000 7316 0000 0074 0083 00a0  ......s....t....
-00001100: 01a1 0001 007c 006a 027c 005f 0364 0053  .....|.j.|._.d.S
-00001110: 0072 1200 0000 2904 7230 0000 0072 4000  .r....).r0...r@.
-00001120: 0000 da0b 7072 6573 735f 636f 6c6f 7272  ....press_colorr
-00001130: 5600 0000 723b 0000 0072 3700 0000 7213  V...r;...r7...r.
-00001140: 0000 0072 1600 0000 7240 0000 008c 0000  ...r....r@......
-00001150: 0073 0400 0000 0a01 0c01 7a19 436f 6c6f  .s........z.Colo
-00001160: 7265 6442 7574 746f 6e2e 7374 6174 655f  redButton.state_
-00001170: 7072 6573 7329 0c72 4500 0000 7246 0000  press).rE...rF..
-00001180: 0072 4700 0000 5a0a 6964 6c65 5f63 6f6c  .rG...Z.idle_col
-00001190: 6f72 7203 0000 005a 0b66 6f63 7573 5f63  orr....Z.focus_c
-000011a0: 6f6c 6f72 725a 0000 0072 0c00 0000 7227  olorrZ...r....r'
-000011b0: 0000 0072 3e00 0000 7240 0000 0072 4c00  ...r>...r@...rL.
-000011c0: 0000 7213 0000 0072 1300 0000 7237 0000  ..r....r....r7..
-000011d0: 0072 1600 0000 724d 0000 007a 0000 0073  .r....rM...z...s
-000011e0: 1000 0000 0800 0401 0801 0801 0801 0c02  ................
-000011f0: 0c04 1408 724d 0000 0029 0cda 0674 7970  ....rM...)...typ
-00001200: 696e 6772 0200 0000 7222 0000 0072 0300  ingr....r"...r..
-00001210: 0000 da0b 7079 6761 6d65 2e72 6563 7472  ....pygame.rectr
-00001220: 0400 0000 da11 726f 6269 6e67 616d 652e  ......robingame.
-00001230: 6f62 6a65 6374 7372 0500 0000 da0f 726f  objectsr......ro
-00001240: 6269 6e67 616d 652e 7574 696c 7372 0600  bingame.utilsr..
-00001250: 0000 7207 0000 0072 4d00 0000 7213 0000  ..r....rM...r...
-00001260: 0072 1300 0000 7213 0000 0072 1600 0000  .r....r....r....
-00001270: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
-00001280: 0000 000c 0008 020c 010c 010c 020c 0110  ................
-00001290: 0314 6f                                  ..o
+00000060: 6d07 5a07 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
+00000070: 6505 8303 5a08 4700 6408 6409 8400 6409  e...Z.G.d.d...d.
+00000080: 6508 8303 5a09 6401 5300 290a e900 0000  e...Z.d.S.).....
+00000090: 004e 2901 da05 436f 6c6f 7229 01da 0452  .N)...Color)...R
+000000a0: 6563 7429 01da 0645 6e74 6974 7929 01da  ect)...Entity)..
+000000b0: 0d70 756c 7369 6e67 5f76 616c 7565 6300  .pulsing_valuec.
+000000c0: 0000 0000 0000 0000 0000 0000 0000 0009  ................
+000000d0: 0000 0000 0000 0073 b400 0000 6500 5a01  .......s....e.Z.
+000000e0: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+000000f0: 3c00 6504 6505 6403 3c00 6404 5a06 6507  <.e.e.d.<.d.Z.e.
+00000100: 6505 6405 3c00 0906 0906 0906 0906 0906  e.d.<...........
+00000110: 6423 6407 6508 6408 6508 6409 6508 640a  d#d.e.d.e.d.e.d.
+00000120: 6508 6608 8700 6601 640b 640c 840d 5a09  e.f...f.d.d...Z.
+00000130: 640d 640e 8400 5a0a 640f 6410 8400 5a0b  d.d...Z.d.d...Z.
+00000140: 6411 6412 8400 5a0c 6413 6414 8400 5a0d  d.d...Z.d.d...Z.
+00000150: 6415 6416 8400 5a0e 6417 6418 8400 5a0f  d.d...Z.d.d...Z.
+00000160: 6419 641a 8400 5a10 641b 641c 8400 5a11  d.d...Z.d.d...Z.
+00000170: 641d 641e 8400 5a12 641f 6420 8400 5a13  d.d...Z.d.d ..Z.
+00000180: 6421 6422 8400 5a14 8700 0400 5a15 5300  d!d"..Z.....Z.S.
+00000190: 2924 da06 4275 7474 6f6e 61e9 0100 000a  )$..Buttona.....
+000001a0: 2020 2020 4755 4920 6275 7474 6f6e 2065      GUI button e
+000001b0: 6e74 6974 792e 2052 6561 6374 7320 746f  ntity. Reacts to
+000001c0: 2063 6861 6e67 6573 2069 6e20 7468 6520   changes in the 
+000001d0: 6973 5f66 6f63 7573 6564 2061 6e64 2069  is_focused and i
+000001e0: 735f 7072 6573 7365 6420 626f 6f6c 6561  s_pressed boolea
+000001f0: 6e73 2c20 6275 7420 646f 6573 6e27 740a  ns, but doesn't.
+00000200: 2020 2020 7365 7420 7468 656d 2028 6120      set them (a 
+00000210: 7061 7265 6e74 206d 656e 7520 636c 6173  parent menu clas
+00000220: 7320 6f72 2073 6f6d 6574 6869 6e67 2065  s or something e
+00000230: 6c73 6520 7368 6f75 6c64 2073 6574 2074  lse should set t
+00000240: 6865 6d29 2e20 5468 6973 2069 7320 736f  hem). This is so
+00000250: 2074 6861 7420 6561 6368 2042 7574 746f   that each Butto
+00000260: 6e0a 2020 2020 646f 6573 6e27 7420 6861  n.    doesn't ha
+00000270: 7665 2074 6f20 646f 2069 7473 206f 776e  ve to do its own
+00000280: 2069 6e70 7574 2064 6574 6563 7469 6f6e   input detection
+00000290: 2e20 4974 2061 6c73 6f20 616c 6c6f 7773  . It also allows
+000002a0: 2061 2070 6172 656e 7420 6d65 6e75 2063   a parent menu c
+000002b0: 6c61 7373 2074 6f20 7461 6b65 2069 6e74  lass to take int
+000002c0: 6f0a 2020 2020 6163 636f 756e 7420 6164  o.    account ad
+000002d0: 6469 7469 6f6e 616c 2063 6f6e 7465 7874  ditional context
+000002e0: 2065 2e67 2e20 7368 6966 7469 6e67 2066   e.g. shifting f
+000002f0: 6f63 7573 2066 726f 6d20 6f6e 6520 6275  ocus from one bu
+00000300: 7474 6f6e 2074 6f20 616e 6f74 6865 7220  tton to another 
+00000310: 7573 696e 6720 6120 6b65 7962 6f61 7264  using a keyboard
+00000320: 206f 720a 2020 2020 6a6f 7973 7469 636b   or.    joystick
+00000330: 2069 6e70 7574 2e20 4f70 6572 6174 696f   input. Operatio
+00000340: 6e73 206c 696b 6520 7468 6973 2077 6f75  ns like this wou
+00000350: 6c64 2062 6520 6265 796f 6e64 2074 6865  ld be beyond the
+00000360: 2073 636f 7065 206f 6620 6120 7369 6e67   scope of a sing
+00000370: 6c65 2042 7574 746f 6e20 696e 7374 616e  le Button instan
+00000380: 6365 2e0a 2020 2020 da0a 6973 5f66 6f63  ce..    ..is_foc
+00000390: 7573 6564 da0a 6973 5f70 7265 7373 6564  used..is_pressed
+000003a0: e914 0000 00da 0a74 6578 745f 636f 6c6f  .......text_colo
+000003b0: 724e da01 78da 0179 da05 7769 6474 68da  rN..x..y..width.
+000003c0: 0668 6569 6768 7463 0a00 0000 0000 0000  .heightc........
+000003d0: 0000 0000 0b00 0000 0600 0000 0300 0000  ................
+000003e0: 7300 0100 007c 037c 005f 007c 047c 005f  s....|.|._.|.|._
+000003f0: 017c 057c 005f 0274 0364 0164 017c 037c  .|.|._.t.d.d.|.|
+00000400: 0483 047c 005f 047c 017c 0266 027c 006a  ...|._.|.|.f.|.j
+00000410: 045f 0564 027c 005f 0664 027c 005f 077c  ._.d.|._.d.|._.|
+00000420: 0670 2264 0364 0484 007c 005f 087c 0770  .p"d.d...|._.|.p
+00000430: 2964 0564 0484 007c 005f 097c 0870 3064  )d.d...|._.|.p0d
+00000440: 0664 0484 007c 005f 0a7c 0970 3764 0764  .d...|._.|.p7d.d
+00000450: 0484 007c 005f 0b74 0c6a 0da0 0e74 0c6a  ...|._.t.j...t.j
+00000460: 0da0 0fa1 007c 006a 10a1 027c 005f 0d7c  .....|.j...|._.|
+00000470: 006a 117c 005f 1274 0ca0 137c 006a 046a  .j.|._.t...|.j.j
+00000480: 14a1 017c 005f 157c 006a 15a0 1674 1764  ...|._.|.j...t.d
+00000490: 0883 01a1 0101 007c 006a 0272 797c 006a  .......|.j.ry|.j
+000004a0: 0da0 187c 006a 0264 0974 1764 0a83 01a1  ...|.j.d.t.d....
+000004b0: 037d 057c 05a0 19a1 007d 0a7c 006a 15a0  .}.|.....}.|.j..
+000004c0: 19a1 006a 057c 0a5f 057c 006a 15a0 1a7c  ...j.|._.|.j...|
+000004d0: 057c 0aa1 0201 0074 1b83 00a0 1ca1 0001  .|.....t........
+000004e0: 0064 0053 0029 0b4e 7201 0000 0046 6301  .d.S.).Nr....Fc.
+000004f0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000500: 0000 0053 0000 00f3 0400 0000 6400 5300  ...S........d.S.
+00000510: a901 4ea9 00a9 01da 0662 7574 746f 6e72  ..N......buttonr
+00000520: 1100 0000 7211 0000 00fa 322f 686f 6d65  ....r.....2/home
+00000530: 2f72 6f62 696e 2f63 6f64 652f 726f 6269  /robin/code/robi
+00000540: 6e67 616d 652f 726f 6269 6e67 616d 652f  ngame/robingame/
+00000550: 6775 692f 6275 7474 6f6e 2e70 79da 083c  gui/button.py..<
+00000560: 6c61 6d62 6461 3e2a 0000 00f3 0200 0000  lambda>*........
+00000570: 0400 7a21 4275 7474 6f6e 2e5f 5f69 6e69  ..z!Button.__ini
+00000580: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6c61  t__.<locals>.<la
+00000590: 6d62 6461 3e63 0100 0000 0000 0000 0000  mbda>c..........
+000005a0: 0000 0100 0000 0100 0000 5300 0000 720f  ..........S...r.
+000005b0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+000005c0: 0000 7211 0000 0072 1100 0000 7214 0000  ..r....r....r...
+000005d0: 0072 1500 0000 2b00 0000 7216 0000 0063  .r....+...r....c
+000005e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000005f0: 0100 0000 5300 0000 720f 0000 0072 1000  ....S...r....r..
+00000600: 0000 7211 0000 0072 1200 0000 7211 0000  ..r....r....r...
+00000610: 0072 1100 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000620: 2c00 0000 7216 0000 0063 0100 0000 0000  ,...r....c......
+00000630: 0000 0000 0000 0100 0000 0100 0000 5300  ..............S.
+00000640: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000650: 0072 1200 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000660: 7214 0000 0072 1500 0000 2d00 0000 7216  r....r....-...r.
+00000670: 0000 00da 0372 6564 54da 0562 6c61 636b  .....redT..black
+00000680: 291d 720d 0000 0072 0e00 0000 da04 7465  ).r....r......te
+00000690: 7874 7203 0000 00da 0472 6563 74da 0663  xtr......rect..c
+000006a0: 656e 7465 7272 0700 0000 7208 0000 00da  enterr....r.....
+000006b0: 095f 6f6e 5f70 7265 7373 da09 5f6f 6e5f  ._on_press.._on_
+000006c0: 666f 6375 73da 0b5f 6f6e 5f72 656c 6561  focus.._on_relea
+000006d0: 7365 da0b 5f6f 6e5f 756e 666f 6375 73da  se.._on_unfocus.
+000006e0: 0670 7967 616d 65da 0466 6f6e 74da 0446  .pygame..font..F
+000006f0: 6f6e 74da 1067 6574 5f64 6566 6175 6c74  ont..get_default
+00000700: 5f66 6f6e 74da 0966 6f6e 745f 7369 7a65  _font..font_size
+00000710: da0a 7374 6174 655f 6964 6c65 da05 7374  ..state_idle..st
+00000720: 6174 65da 0753 7572 6661 6365 da04 7369  ate..Surface..si
+00000730: 7a65 da05 696d 6167 65da 0466 696c 6c72  ze..image..fillr
+00000740: 0200 0000 da06 7265 6e64 6572 da08 6765  ......render..ge
+00000750: 745f 7265 6374 da04 626c 6974 da05 7375  t_rect..blit..su
+00000760: 7065 72da 085f 5f69 6e69 745f 5f29 0bda  per..__init__)..
+00000770: 0473 656c 6672 0b00 0000 720c 0000 0072  .selfr....r....r
+00000780: 0d00 0000 720e 0000 0072 1900 0000 da08  ....r....r......
+00000790: 6f6e 5f70 7265 7373 da08 6f6e 5f66 6f63  on_press..on_foc
+000007a0: 7573 da0a 6f6e 5f72 656c 6561 7365 da0a  us..on_release..
+000007b0: 6f6e 5f75 6e66 6f63 7573 da08 7465 7874  on_unfocus..text
+000007c0: 5265 6374 a901 da09 5f5f 636c 6173 735f  Rect....__class_
+000007d0: 5f72 1100 0000 7214 0000 0072 2f00 0000  _r....r....r/...
+000007e0: 1700 0000 732a 0000 0006 0c06 0106 0110  ....s*..........
+000007f0: 010c 0106 0106 010e 010e 010e 010e 0118  ................
+00000800: 0108 0110 0110 0106 0116 0108 010e 010e  ................
+00000810: 010e 017a 0f42 7574 746f 6e2e 5f5f 696e  ...z.Button.__in
+00000820: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00000830: 0001 0000 0002 0000 0043 0000 0073 2400  .........C...s$.
+00000840: 0000 7c00 6a00 7207 7c00 a001 a100 0100  ..|.j.r.|.......
+00000850: 7c00 6a02 7210 7c00 a003 a100 0100 6400  |.j.r.|.......d.
+00000860: 5300 6400 5300 7210 0000 0029 0472 0700  S.d.S.r....).r..
+00000870: 0000 da05 666f 6375 7372 0800 0000 da05  ....focusr......
+00000880: 7072 6573 73a9 0172 3000 0000 7211 0000  press..r0...r...
+00000890: 0072 1100 0000 7214 0000 0072 2500 0000  .r....r....r%...
+000008a0: 3c00 0000 f30a 0000 0006 0108 0106 010c  <...............
+000008b0: 0104 ff7a 1142 7574 746f 6e2e 7374 6174  ...z.Button.stat
+000008c0: 655f 6964 6c65 6301 0000 0000 0000 0000  e_idlec.........
+000008d0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000008e0: 2400 0000 7c00 6a00 7307 7c00 a001 a100  $...|.j.s.|.....
+000008f0: 0100 7c00 6a02 7210 7c00 a003 a100 0100  ..|.j.r.|.......
+00000900: 6400 5300 6400 5300 7210 0000 0029 0472  d.S.d.S.r....).r
+00000910: 0700 0000 da07 756e 666f 6375 7372 0800  ......unfocusr..
+00000920: 0000 7239 0000 0072 3a00 0000 7211 0000  ..r9...r:...r...
+00000930: 0072 1100 0000 7214 0000 00da 0b73 7461  .r....r......sta
+00000940: 7465 5f66 6f63 7573 4200 0000 723b 0000  te_focusB...r;..
+00000950: 007a 1242 7574 746f 6e2e 7374 6174 655f  .z.Button.state_
+00000960: 666f 6375 7363 0100 0000 0000 0000 0000  focusc..........
+00000970: 0000 0100 0000 0200 0000 4300 0000 7316  ..........C...s.
+00000980: 0000 007c 006a 0073 097c 00a0 01a1 0001  ...|.j.s.|......
+00000990: 0064 0053 0064 0053 0072 1000 0000 2902  .d.S.d.S.r....).
+000009a0: 7208 0000 00da 0772 656c 6561 7365 723a  r......releaser:
+000009b0: 0000 0072 1100 0000 7211 0000 0072 1400  ...r....r....r..
+000009c0: 0000 da0b 7374 6174 655f 7072 6573 7348  ....state_pressH
+000009d0: 0000 0073 0600 0000 0601 0c01 04ff 7a12  ...s..........z.
+000009e0: 4275 7474 6f6e 2e73 7461 7465 5f70 7265  Button.state_pre
+000009f0: 7373 6301 0000 0000 0000 0000 0000 0001  ssc.............
+00000a00: 0000 0003 0000 0043 0000 00f3 0e00 0000  .......C........
+00000a10: 7c00 a000 7c00 a101 0100 6400 5300 7210  |...|.....d.S.r.
+00000a20: 0000 0029 0172 1c00 0000 723a 0000 0072  ...).r....r:...r
+00000a30: 1100 0000 7211 0000 0072 1400 0000 7231  ....r....r....r1
+00000a40: 0000 0056 0000 00f3 0200 0000 0e01 7a0f  ...V..........z.
+00000a50: 4275 7474 6f6e 2e6f 6e5f 7072 6573 7363  Button.on_pressc
+00000a60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000a70: 0300 0000 4300 0000 7240 0000 0072 1000  ....C...r@...r..
+00000a80: 0000 2901 721e 0000 0072 3a00 0000 7211  ..).r....r:...r.
+00000a90: 0000 0072 1100 0000 7214 0000 0072 3300  ...r....r....r3.
+00000aa0: 0000 5900 0000 7241 0000 007a 1142 7574  ..Y...rA...z.But
+00000ab0: 746f 6e2e 6f6e 5f72 656c 6561 7365 6301  ton.on_releasec.
+00000ac0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000ad0: 0000 0043 0000 0072 4000 0000 7210 0000  ...C...r@...r...
+00000ae0: 0029 0172 1d00 0000 723a 0000 0072 1100  .).r....r:...r..
+00000af0: 0000 7211 0000 0072 1400 0000 7232 0000  ..r....r....r2..
+00000b00: 005c 0000 0072 4100 0000 7a0f 4275 7474  .\...rA...z.Butt
+00000b10: 6f6e 2e6f 6e5f 666f 6375 7363 0100 0000  on.on_focusc....
+00000b20: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000b30: 4300 0000 7240 0000 0072 1000 0000 2901  C...r@...r....).
+00000b40: 721f 0000 0072 3a00 0000 7211 0000 0072  r....r:...r....r
+00000b50: 1100 0000 7214 0000 0072 3400 0000 5f00  ....r....r4..._.
+00000b60: 0000 7241 0000 007a 1142 7574 746f 6e2e  ..rA...z.Button.
+00000b70: 6f6e 5f75 6e66 6f63 7573 6301 0000 0000  on_unfocusc.....
+00000b80: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000b90: 0000 00f3 1400 0000 7c00 a000 a100 0100  ........|.......
+00000ba0: 7c00 6a01 7c00 5f02 6400 5300 7210 0000  |.j.|._.d.S.r...
+00000bb0: 0029 0372 3100 0000 723f 0000 0072 2600  .).r1...r?...r&.
+00000bc0: 0000 723a 0000 0072 1100 0000 7211 0000  ..r:...r....r...
+00000bd0: 0072 1400 0000 7239 0000 0066 0000 00f3  .r....r9...f....
+00000be0: 0400 0000 0801 0c01 7a0c 4275 7474 6f6e  ........z.Button
+00000bf0: 2e70 7265 7373 6301 0000 0000 0000 0000  .pressc.........
+00000c00: 0000 0001 0000 0002 0000 0043 0000 0072  ...........C...r
+00000c10: 4200 0000 7210 0000 0029 0372 3200 0000  B...r....).r2...
+00000c20: 723d 0000 0072 2600 0000 723a 0000 0072  r=...r&...r:...r
+00000c30: 1100 0000 7211 0000 0072 1400 0000 7238  ....r....r....r8
+00000c40: 0000 006a 0000 0072 4300 0000 7a0c 4275  ...j...rC...z.Bu
+00000c50: 7474 6f6e 2e66 6f63 7573 6301 0000 0000  tton.focusc.....
+00000c60: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000c70: 0000 0073 2600 0000 7c00 a000 a100 0100  ...s&...|.......
+00000c80: 7c00 6a01 720d 7c00 6a02 7c00 5f04 6400  |.j.r.|.j.|._.d.
+00000c90: 5300 7c00 6a03 7c00 5f04 6400 5300 7210  S.|.j.|._.d.S.r.
+00000ca0: 0000 0029 0572 3300 0000 7207 0000 0072  ...).r3...r....r
+00000cb0: 3d00 0000 7225 0000 0072 2600 0000 723a  =...r%...r&...r:
+00000cc0: 0000 0072 1100 0000 7211 0000 0072 1400  ...r....r....r..
+00000cd0: 0000 723e 0000 006e 0000 0073 0400 0000  ..r>...n...s....
+00000ce0: 0801 1e01 7a0e 4275 7474 6f6e 2e72 656c  ....z.Button.rel
+00000cf0: 6561 7365 6301 0000 0000 0000 0000 0000  easec...........
+00000d00: 0001 0000 0002 0000 0043 0000 0072 4200  .........C...rB.
+00000d10: 0000 7210 0000 0029 0372 3400 0000 7225  ..r....).r4...r%
+00000d20: 0000 0072 2600 0000 723a 0000 0072 1100  ...r&...r:...r..
+00000d30: 0000 7211 0000 0072 1400 0000 723c 0000  ..r....r....r<..
+00000d40: 0072 0000 0072 4300 0000 7a0e 4275 7474  .r...rC...z.Butt
+00000d50: 6f6e 2e75 6e66 6f63 7573 2905 4e4e 4e4e  on.unfocus).NNNN
+00000d60: 4e29 16da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000d70: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000d80: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000d90: da04 626f 6f6c da0f 5f5f 616e 6e6f 7461  ..bool..__annota
+00000da0: 7469 6f6e 735f 5f72 2400 0000 7202 0000  tions__r$...r...
+00000db0: 00da 0369 6e74 722f 0000 0072 2500 0000  ...intr/...r%...
+00000dc0: 723d 0000 0072 3f00 0000 7231 0000 0072  r=...r?...r1...r
+00000dd0: 3300 0000 7232 0000 0072 3400 0000 7239  3...r2...r4...r9
+00000de0: 0000 0072 3800 0000 723e 0000 0072 3c00  ...r8...r>...r<.
+00000df0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00000e00: 5f72 1100 0000 7211 0000 0072 3600 0000  _r....r....r6...
+00000e10: 7214 0000 0072 0600 0000 0900 0000 733e  r....r........s>
+00000e20: 0000 000a 0004 0108 0808 0104 0108 0102  ................
+00000e30: 0802 0102 0102 0102 0104 f602 0202 fe02  ................
+00000e40: 0302 fd02 0402 fc02 050e fb08 2508 0608  ............%...
+00000e50: 0608 0e08 0308 0308 0308 0708 0408 0410  ................
+00000e60: 0472 0600 0000 6300 0000 0000 0000 0000  .r....c.........
+00000e70: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+00000e80: 5000 0000 6500 5a01 6400 5a02 6401 5a03  P...e.Z.d.Z.d.Z.
+00000e90: 6504 6402 8301 5a05 6504 6403 8301 5a06  e.d...Z.e.d...Z.
+00000ea0: 6504 6404 8301 5a07 8700 6601 6405 6406  e.d...Z...f.d.d.
+00000eb0: 8408 5a08 8700 6601 6407 6408 8408 5a09  ..Z...f.d.d...Z.
+00000ec0: 8700 6601 6409 640a 8408 5a0a 8700 0400  ..f.d.d...Z.....
+00000ed0: 5a0b 5300 290b da0d 436f 6c6f 7265 6442  Z.S.)...ColoredB
+00000ee0: 7574 746f 6e29 03e9 6400 0000 7201 0000  utton)..d...r...
+00000ef0: 0072 4d00 0000 da06 6f72 616e 6765 7217  .rM.....oranger.
+00000f00: 0000 00da 0577 6869 7465 6301 0000 0000  .....whitec.....
+00000f10: 0000 0000 0000 0001 0000 0005 0000 0003  ................
+00000f20: 0000 0073 2600 0000 7400 8300 a001 a100  ...s&...t.......
+00000f30: 0100 7402 7c00 6a03 6401 6402 6403 8304  ..t.|.j.d.d.d...
+00000f40: 6404 6405 6603 7c00 5f04 6400 5300 2906  d.d.f.|._.d.S.).
+00000f50: 4ee9 5000 0000 e996 0000 0067 b81e 85eb  N.P........g....
+00000f60: 51b8 9e3f e91e 0000 00e9 4b00 0000 2905  Q..?......K...).
+00000f70: 722e 0000 0072 2500 0000 7205 0000 00da  r....r%...r.....
+00000f80: 0474 6963 6bda 0563 6f6c 6f72 723a 0000  .tick..colorr:..
+00000f90: 0072 3600 0000 7211 0000 0072 1400 0000  .r6...r....r....
+00000fa0: 7225 0000 007d 0000 0073 0400 0000 0a01  r%...}...s......
+00000fb0: 1c01 7a18 436f 6c6f 7265 6442 7574 746f  ..z.ColoredButto
+00000fc0: 6e2e 7374 6174 655f 6964 6c65 6301 0000  n.state_idlec...
+00000fd0: 0000 0000 0000 0000 0001 0000 0006 0000  ................
+00000fe0: 0003 0000 0073 3200 0000 7400 8300 a001  .....s2...t.....
+00000ff0: a100 0100 7402 7c00 6a03 6401 6402 6403  ....t.|.j.d.d.d.
+00001000: 8304 7402 7c00 6a03 6404 6405 6403 8304  ..t.|.j.d.d.d...
+00001010: 6406 6603 7c00 5f04 6400 5300 2907 4ee9  d.f.|._.d.S.).N.
+00001020: b400 0000 e9ff 0000 0067 3333 3333 3333  .........g333333
+00001030: d33f 724d 0000 00e9 a300 0000 7201 0000  .?rM........r...
+00001040: 0029 0572 2e00 0000 723d 0000 0072 0500  .).r....r=...r..
+00001050: 0000 7254 0000 0072 5500 0000 723a 0000  ..rT...rU...r:..
+00001060: 0072 3600 0000 7211 0000 0072 1400 0000  .r6...r....r....
+00001070: 723d 0000 0081 0000 0073 0a00 0000 0a01  r=.......s......
+00001080: 0e02 0e01 0201 0afd 7a19 436f 6c6f 7265  ........z.Colore
+00001090: 6442 7574 746f 6e2e 7374 6174 655f 666f  dButton.state_fo
+000010a0: 6375 7363 0100 0000 0000 0000 0000 0000  cusc............
+000010b0: 0100 0000 0200 0000 0300 0000 7316 0000  ............s...
+000010c0: 0074 0083 00a0 01a1 0001 007c 006a 027c  .t.........|.j.|
+000010d0: 005f 0364 0053 0072 1000 0000 2904 722e  ._.d.S.r....).r.
+000010e0: 0000 0072 3f00 0000 da0b 7072 6573 735f  ...r?.....press_
+000010f0: 636f 6c6f 7272 5500 0000 723a 0000 0072  colorrU...r:...r
+00001100: 3600 0000 7211 0000 0072 1400 0000 723f  6...r....r....r?
+00001110: 0000 0089 0000 0073 0400 0000 0a01 0c01  .......s........
+00001120: 7a19 436f 6c6f 7265 6442 7574 746f 6e2e  z.ColoredButton.
+00001130: 7374 6174 655f 7072 6573 7329 0c72 4400  state_press).rD.
+00001140: 0000 7245 0000 0072 4600 0000 da0a 6964  ..rE...rF.....id
+00001150: 6c65 5f63 6f6c 6f72 7202 0000 00da 0b66  le_colorr......f
+00001160: 6f63 7573 5f63 6f6c 6f72 7259 0000 0072  ocus_colorrY...r
+00001170: 0a00 0000 7225 0000 0072 3d00 0000 723f  ....r%...r=...r?
+00001180: 0000 0072 4b00 0000 7211 0000 0072 1100  ...rK...r....r..
+00001190: 0000 7236 0000 0072 1400 0000 724c 0000  ..r6...r....rL..
+000011a0: 0077 0000 0073 1000 0000 0800 0401 0801  .w...s..........
+000011b0: 0801 0801 0c02 0c04 1408 724c 0000 0029  ..........rL...)
+000011c0: 0a72 2000 0000 7202 0000 00da 0b70 7967  .r ...r......pyg
+000011d0: 616d 652e 7265 6374 7203 0000 00da 1172  ame.rectr......r
+000011e0: 6f62 696e 6761 6d65 2e6f 626a 6563 7473  obingame.objects
+000011f0: 7204 0000 00da 0f72 6f62 696e 6761 6d65  r......robingame
+00001200: 2e75 7469 6c73 7205 0000 0072 0600 0000  .utilsr....r....
+00001210: 724c 0000 0072 1100 0000 7211 0000 0072  rL...r....r....r
+00001220: 1100 0000 7214 0000 00da 083c 6d6f 6475  ....r......<modu
+00001230: 6c65 3e01 0000 0073 0e00 0000 0800 0c01  le>....s........
+00001240: 0c01 0c02 0c01 1003 146e                 .........n
```

### Comparing `robingame-0.0.9/robingame/gui/button.py` & `robingame-0.1.0/robingame/gui/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from typing import Callable
-
 import pygame
 from pygame import Color
 from pygame.rect import Rect
 
-from robingame.objects import PhysicalEntity
+from robingame.objects import Entity
 from robingame.utils import pulsing_value
 
 
-class Button(PhysicalEntity):
+class Button(Entity):
     """
     GUI button entity. Reacts to changes in the is_focused and is_pressed booleans, but doesn't
     set them (a parent menu class or something else should set them). This is so that each Button
     doesn't have to do its own input detection. It also allows a parent menu class to take into
     account additional context e.g. shifting focus from one button to another using a keyboard or
     joystick input. Operations like this would be beyond the scope of a single Button instance.
     """
 
     is_focused: bool  # does the button have focus? (e.g. mouse hovering over)
     is_pressed: bool  # is the button down right now
-    font_name = "ubuntu"
     font_size = 20
     text_color: Color
 
     def __init__(
         self,
         x: int,
         y: int,
```

### Comparing `robingame-0.0.9/robingame/image/__pycache__/utils.cpython-310.pyc` & `robingame-0.1.0/robingame/image/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 6229 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 5518 0000  o.......u.5cU...
+00000000: 6f0d 0d0a 0000 0000 8874 a564 5418 0000  o........t.dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6400 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6506 6602 6407 6408 8404 5a09 6435 6406  e.f.d.d...Z.d5d.
@@ -35,345 +35,345 @@
 00000220: 0073 1074 006a 01a0 03a1 0001 0074 006a  .s.t.j.......t.j
 00000230: 01a0 0464 01a1 0153 0074 006a 01a0 05a1  ...d...S.t.j....
 00000240: 0053 0029 024e 2902 e901 0000 0072 0700  .S.).N)......r..
 00000250: 0000 2906 da06 7079 6761 6d65 da07 6469  ..)...pygame..di
 00000260: 7370 6c61 79da 0867 6574 5f69 6e69 74da  splay..get_init.
 00000270: 0469 6e69 74da 0873 6574 5f6d 6f64 65da  .init..set_mode.
 00000280: 0b67 6574 5f73 7572 6661 6365 a900 720e  .get_surface..r.
-00000290: 0000 0072 0e00 0000 fa34 2f68 6f6d 652f  ...r.....4/home/
-000002a0: 6269 6e6e 6576 2f63 6f64 652f 726f 6269  binnev/code/robi
-000002b0: 6e67 616d 652f 726f 6269 6e67 616d 652f  ngame/robingame/
-000002c0: 696d 6167 652f 7574 696c 732e 7079 da0c  image/utils.py..
-000002d0: 696e 6974 5f64 6973 706c 6179 0b00 0000  init_display....
-000002e0: 7308 0000 000a 010a 010c 010a 0272 1000  s............r..
-000002f0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000300: 0000 0008 0000 0043 0000 0073 6800 0000  .......C...sh...
-00000310: 7400 8300 0100 7a08 7401 6a02 a003 7c00  t.....z.t.j...|.
-00000320: a101 7d02 5700 6e0e 0400 7401 6a04 7919  ..}.W.n...t.j.y.
-00000330: 0100 0100 0100 7405 6401 7c00 8302 0100  ......t.d.|.....
-00000340: 8200 7700 7c01 6400 7501 722e 7c01 6402  ..w.|.d.u.r.|.d.
-00000350: 6b02 7227 7c02 a006 6403 a101 7d01 7c02  k.r'|...d...}.|.
-00000360: a007 7c01 7401 6a08 a102 0100 7c02 a009  ..|.t.j.....|...
-00000370: a100 7d02 7c02 5300 2904 4e7a 1555 6e61  ..}.|.S.).Nz.Una
-00000380: 626c 6520 746f 206c 6f61 6420 696d 6167  ble to load imag
-00000390: 653a e9ff ffff ff29 0272 0100 0000 7201  e:.....).r....r.
-000003a0: 0000 0029 0a72 1000 0000 7208 0000 00da  ...).r....r.....
-000003b0: 0569 6d61 6765 da04 6c6f 6164 da05 6572  .image..load..er
-000003c0: 726f 72da 0570 7269 6e74 da06 6765 745f  ror..print..get_
-000003d0: 6174 da0c 7365 745f 636f 6c6f 726b 6579  at..set_colorkey
-000003e0: da08 524c 4541 4343 454c da0d 636f 6e76  ..RLEACCEL..conv
-000003f0: 6572 745f 616c 7068 6129 03da 0866 696c  ert_alpha)...fil
-00000400: 656e 616d 65da 0863 6f6c 6f72 6b65 7972  ename..colorkeyr
-00000410: 1200 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000420: 0000 00da 0a6c 6f61 645f 696d 6167 6513  .....load_image.
-00000430: 0000 0073 1a00 0000 0601 0201 1001 0e01  ...s............
-00000440: 0a01 0201 02fe 0806 0801 0a01 0e01 0802  ................
-00000450: 0401 721c 0000 00da 0773 7572 6661 6365  ..r......surface
-00000460: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000470: 0003 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-00000480: 7c00 a001 a100 8301 5300 2901 7ae8 4368  |.......S.).z.Ch
-00000490: 6563 6b20 6966 2061 2073 7572 6661 6365  eck if a surface
-000004a0: 2068 6173 2061 6e79 206e 6f6e 2d7a 6572   has any non-zer
-000004b0: 6f20 7069 7865 6c73 2e20 6053 7572 6661  o pixels. `Surfa
-000004c0: 6365 2e67 6574 5f62 6f75 6e64 696e 675f  ce.get_bounding_
-000004d0: 7265 6374 2829 6020 7265 7475 726e 7320  rect()` returns 
-000004e0: 7468 650a 2020 2020 736d 616c 6c65 7374  the.    smallest
-000004f0: 2072 6563 7461 6e67 6c65 206f 6e20 7468   rectangle on th
-00000500: 6520 7375 7266 6163 6520 636f 6e74 6169  e surface contai
-00000510: 6e69 6e67 2064 6174 612e 2049 6620 7468  ning data. If th
-00000520: 6520 7375 7266 6163 6520 6973 2065 6d70  e surface is emp
-00000530: 7479 2c20 6974 2077 696c 6c20 7265 7475  ty, it will retu
-00000540: 726e 0a20 2020 2052 6563 7428 302c 2030  rn.    Rect(0, 0
-00000550: 2c20 302c 2030 292c 2066 6f72 2077 6869  , 0, 0), for whi
-00000560: 6368 2060 616e 7960 2072 6574 7572 6e73  ch `any` returns
-00000570: 2046 616c 7365 2902 da03 616e 79da 1167   False)...any..g
-00000580: 6574 5f62 6f75 6e64 696e 675f 7265 6374  et_bounding_rect
-00000590: 2901 721d 0000 0072 0e00 0000 720e 0000  ).r....r....r...
-000005a0: 0072 0f00 0000 da09 6e6f 745f 656d 7074  .r......not_empt
-000005b0: 7926 0000 0073 0200 0000 0c04 7220 0000  y&...s......r ..
-000005c0: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
-000005d0: 0000 0400 0000 4f00 0000 7320 0000 0074  ......O...s ...t
-000005e0: 007c 0069 007c 01a4 018e 01a0 01a1 007d  .|.i.|.........}
-000005f0: 027c 02a0 0264 01a1 0101 007c 0253 0029  .|...d.....|.S.)
-00000600: 024e 2904 7201 0000 0072 0100 0000 7201  .N).r....r....r.
-00000610: 0000 0072 0100 0000 2903 7204 0000 0072  ...r....).r....r
-00000620: 1900 0000 da04 6669 6c6c 2903 da04 6172  ......fill)...ar
-00000630: 6773 da06 6b77 6172 6773 5a03 696d 6772  gs..kwargsZ.imgr
-00000640: 0e00 0000 720e 0000 0072 0f00 0000 da0b  ....r....r......
-00000650: 656d 7074 795f 696d 6167 652d 0000 0073  empty_image-...s
-00000660: 0600 0000 1201 0a01 0401 7224 0000 00da  ..........r$....
-00000670: 0c63 7572 7265 6e74 5f66 696c 65da 0666  .current_file..f
-00000680: 6f6c 6465 7263 0200 0000 0000 0000 0000  olderc..........
-00000690: 0000 0200 0000 0200 0000 4300 0000 7312  ..........C...s.
-000006a0: 0000 0074 007c 0083 016a 01a0 02a1 007c  ...t.|...j.....|
-000006b0: 011b 0053 00a9 014e 2903 7203 0000 00da  ...S...N).r.....
-000006c0: 0670 6172 656e 74da 0861 6273 6f6c 7574  .parent..absolut
-000006d0: 6529 0272 2500 0000 7226 0000 0072 0e00  e).r%...r&...r..
-000006e0: 0000 720e 0000 0072 0f00 0000 da0f 7265  ..r....r......re
-000006f0: 6c61 7469 7665 5f66 6f6c 6465 7233 0000  lative_folder3..
-00000700: 00f3 0200 0000 1201 722a 0000 0063 0100  ........r*...c..
-00000710: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000720: 0000 4300 0000 7332 0000 0074 007c 0083  ..C...s2...t.|..
-00000730: 0164 016b 0272 0d67 007c 00a2 0164 0291  .d.k.r.g.|...d..
-00000740: 0152 0053 0074 007c 0083 0164 036b 0272  .R.S.t.|...d.k.r
-00000750: 157c 0053 0074 0164 0483 0182 0129 054e  .|.S.t.d.....).N
-00000760: e903 0000 00e9 ff00 0000 e904 0000 007a  ...............z
-00000770: 1162 6f67 7573 2063 6f6c 6f75 722c 206d  .bogus colour, m
-00000780: 616e 2902 da03 6c65 6eda 0945 7863 6570  an)...len..Excep
-00000790: 7469 6f6e 2901 5a0c 636f 6c6f 7572 5f74  tion).Z.colour_t
-000007a0: 7570 6c65 720e 0000 0072 0e00 0000 720f  upler....r....r.
-000007b0: 0000 00da 0970 6164 5f61 6c70 6861 3700  .....pad_alpha7.
-000007c0: 0000 730a 0000 000c 010e 020c 0104 0108  ..s.............
-000007d0: 0272 3100 0000 da05 636f 6c6f 72da 0661  .r1.....color..a
-000007e0: 6d6f 756e 7463 0200 0000 0000 0000 0000  mountc..........
-000007f0: 0000 0500 0000 0500 0000 4300 0000 734e  ..........C...sN
-00000800: 0000 0074 007c 0083 017d 0074 017c 006a  ...t.|...}.t.|.j
-00000810: 027c 0117 0064 0164 028d 027d 0274 017c  .|...d.d...}.t.|
-00000820: 006a 037c 0117 0064 0164 028d 027d 0374  .j.|...d.d...}.t
-00000830: 017c 006a 047c 0117 0064 0164 028d 027d  .|.j.|...d.d...}
-00000840: 0474 007c 027c 037c 047c 006a 0583 0453  .t.|.|.|.|.j...S
-00000850: 0029 034e 2902 7201 0000 0072 2d00 0000  .).N).r....r-...
-00000860: 2901 5a07 6265 7477 6565 6e29 0672 0200  ).Z.between).r..
-00000870: 0000 7205 0000 00da 0172 da01 67da 0162  ..r......r..g..b
-00000880: da01 6129 0572 3200 0000 7233 0000 0072  ..a).r2...r3...r
-00000890: 3400 0000 7235 0000 0072 3600 0000 720e  4...r5...r6...r.
-000008a0: 0000 0072 0e00 0000 720f 0000 00da 0e62  ...r....r......b
-000008b0: 7269 6768 7465 6e5f 636f 6c6f 7241 0000  righten_colorA..
-000008c0: 0073 0a00 0000 0801 1201 1201 1201 1001  .s..............
-000008d0: 7238 0000 0072 1200 0000 6302 0000 0000  r8...r....c.....
-000008e0: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
-000008f0: 0000 0073 8600 0000 7c00 a000 a100 5c02  ...s....|.....\.
-00000900: 7d02 7d03 7c00 a001 a100 7d04 7402 7c02  }.}.|.....}.t.|.
-00000910: 8301 4400 5d32 7d05 7402 7c03 8301 4400  ..D.]2}.t.|...D.
-00000920: 5d2b 7d06 7c00 a003 7c05 7c06 6602 a101  ]+}.|...|.|.f...
-00000930: 6400 6400 8502 1900 7d07 7404 7c07 7c01  d.d.....}.t.|.|.
-00000940: 8302 7d08 7c08 7234 7c04 a005 7c05 7c06  ..}.|.r4|...|.|.
-00000950: 6602 7406 6a07 7c08 8e00 a102 0100 7114  f.t.j.|.......q.
-00000960: 7c04 a005 7c05 7c06 6602 7406 6a07 7c07  |...|.|.f.t.j.|.
-00000970: 8e00 a102 0100 7114 710e 7c04 5300 7227  ......q.q.|.S.r'
-00000980: 0000 0029 08da 0867 6574 5f73 697a 65da  ...)...get_size.
-00000990: 0463 6f70 79da 0572 616e 6765 7216 0000  .copy..ranger...
-000009a0: 0072 3800 0000 da06 7365 745f 6174 7208  .r8.....set_atr.
-000009b0: 0000 0072 0200 0000 2909 7212 0000 0072  ...r....).r....r
-000009c0: 3300 0000 da05 7769 6474 68da 0668 6569  3.....width..hei
-000009d0: 6768 745a 096e 6577 5f69 6d61 6765 da01  ghtZ.new_image..
-000009e0: 78da 0179 7232 0000 00da 096e 6577 5f63  x..yr2.....new_c
-000009f0: 6f6c 6f72 720e 0000 0072 0e00 0000 720f  olorr....r....r.
-00000a00: 0000 00da 0862 7269 6768 7465 6e49 0000  .....brightenI..
-00000a10: 0073 1600 0000 0c01 0802 0c05 0c01 1601  .s..............
-00000a20: 0a01 0401 1801 1802 02fa 0408 7242 0000  ............rB..
-00000a30: 00da 0573 6361 6c65 6302 0000 0000 0000  ...scalec.......
-00000a40: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00000a50: 0073 3200 0000 7c00 a000 a100 6a01 7c01  .s2...|.....j.|.
-00000a60: 1400 7d02 7c00 a000 a100 6a02 7c01 1400  ..}.|.....j.|...
-00000a70: 7d03 7403 6a04 a005 7c00 7c02 7c03 6602  }.t.j...|.|.|.f.
-00000a80: a102 7d00 7c00 5300 7227 0000 0029 06da  ..}.|.S.r'...)..
-00000a90: 0867 6574 5f72 6563 7472 3d00 0000 723e  .get_rectr=...r>
-00000aa0: 0000 0072 0800 0000 da09 7472 616e 7366  ...r......transf
-00000ab0: 6f72 6d72 4300 0000 2904 7212 0000 0072  ormrC...).r....r
-00000ac0: 4300 0000 da07 785f 7363 616c 65da 0779  C.....x_scale..y
-00000ad0: 5f73 6361 6c65 720e 0000 0072 0e00 0000  _scaler....r....
-00000ae0: 720f 0000 00da 0b73 6361 6c65 5f69 6d61  r......scale_ima
-00000af0: 6765 5d00 0000 7308 0000 000e 010e 0112  ge]...s.........
-00000b00: 0104 0172 4800 0000 da06 696d 6167 6573  ...rH.....images
-00000b10: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b20: 0003 0000 0003 0000 00f3 1200 0000 8700  ................
-00000b30: 6601 6401 6402 8408 7c00 4400 8301 5300  f.d.d...|.D...S.
-00000b40: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000b50: 0200 0000 0500 0000 1300 0000 f316 0000  ................
-00000b60: 0067 007c 005d 077d 0174 007c 0188 0083  .g.|.].}.t.|....
-00000b70: 0291 0271 0253 0072 0e00 0000 2901 7248  ...q.S.r....).rH
-00000b80: 0000 00a9 02da 022e 3072 1200 0000 a901  ........0r......
-00000b90: 7243 0000 0072 0e00 0000 720f 0000 00da  rC...r....r.....
-00000ba0: 0a3c 6c69 7374 636f 6d70 3e65 0000 00f3  .<listcomp>e....
-00000bb0: 0200 0000 1600 7a20 7363 616c 655f 696d  ......z scale_im
-00000bc0: 6167 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ages.<locals>.<l
-00000bd0: 6973 7463 6f6d 703e 720e 0000 0029 0272  istcomp>r....).r
-00000be0: 4900 0000 7243 0000 0072 0e00 0000 724e  I...rC...r....rN
-00000bf0: 0000 0072 0f00 0000 da0c 7363 616c 655f  ...r......scale_
-00000c00: 696d 6167 6573 6400 0000 722b 0000 0072  imagesd...r+...r
-00000c10: 5100 0000 4663 0300 0000 0000 0000 0000  Q...Fc..........
-00000c20: 0000 0300 0000 0600 0000 4300 0000 7318  ..........C...s.
-00000c30: 0000 0074 006a 01a0 027c 0074 037c 0183  ...t.j...|.t.|..
-00000c40: 0174 037c 0283 01a1 0353 0072 2700 0000  .t.|.....S.r'...
-00000c50: 2904 7208 0000 0072 4500 0000 da04 666c  ).r....rE.....fl
-00000c60: 6970 da04 626f 6f6c 2903 7212 0000 00da  ip..bool).r.....
-00000c70: 0666 6c69 705f 78da 0666 6c69 705f 7972  .flip_x..flip_yr
-00000c80: 0e00 0000 720e 0000 0072 0f00 0000 da0a  ....r....r......
-00000c90: 666c 6970 5f69 6d61 6765 6800 0000 7302  flip_imageh...s.
-00000ca0: 0000 0018 0172 5600 0000 6303 0000 0000  .....rV...c.....
-00000cb0: 0000 0000 0000 0003 0000 0003 0000 0003  ................
-00000cc0: 0000 0073 1400 0000 8700 8701 6602 6401  ...s........f.d.
-00000cd0: 6402 8408 7c00 4400 8301 5300 2903 4e63  d...|.D...S.).Nc
-00000ce0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000cf0: 0600 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
-00000d00: 005d 087d 0174 007c 0188 0088 0183 0391  .].}.t.|........
-00000d10: 0271 0253 0072 0e00 0000 2901 7256 0000  .q.S.r....).rV..
-00000d20: 0072 4c00 0000 a902 7254 0000 0072 5500  .rL.....rT...rU.
-00000d30: 0000 720e 0000 0072 0f00 0000 724f 0000  ..r....r....rO..
-00000d40: 006d 0000 0073 0200 0000 1800 7a1f 666c  .m...s......z.fl
-00000d50: 6970 5f69 6d61 6765 732e 3c6c 6f63 616c  ip_images.<local
-00000d60: 733e 2e3c 6c69 7374 636f 6d70 3e72 0e00  s>.<listcomp>r..
-00000d70: 0000 2903 7249 0000 0072 5400 0000 7255  ..).rI...rT...rU
-00000d80: 0000 0072 0e00 0000 7257 0000 0072 0f00  ...r....rW...r..
-00000d90: 0000 da0b 666c 6970 5f69 6d61 6765 736c  ....flip_imagesl
-00000da0: 0000 0073 0200 0000 1401 7258 0000 00da  ...s......rX....
-00000db0: 0d63 6f6c 6f72 5f6d 6170 7069 6e67 6302  .color_mappingc.
-00000dc0: 0000 0000 0000 0000 0000 0009 0000 0007  ................
-00000dd0: 0000 0043 0000 0073 9800 0000 6401 6402  ...C...s....d.d.
-00000de0: 8400 7c01 a000 a100 4400 8301 7d01 7c00  ..|.....D...}.|.
-00000df0: a001 a100 5c02 7d02 7d03 7c00 a002 a100  ....\.}.}.|.....
-00000e00: 7d04 7403 7c02 8301 4400 5d32 7d05 7403  }.t.|...D.]2}.t.
-00000e10: 7c03 8301 4400 5d2b 7d06 7c00 a004 7c05  |...D.]+}.|...|.
-00000e20: 7c06 6602 a101 6400 6400 8502 1900 7d07  |.f...d.d.....}.
-00000e30: 7c01 a005 7c07 a101 7d08 7c08 723d 7c04  |...|...}.|.r=|.
-00000e40: a006 7c05 7c06 6602 7407 6a08 7c08 8e00  ..|.|.f.t.j.|...
-00000e50: a102 0100 711d 7c04 a006 7c05 7c06 6602  ....q.|...|.|.f.
-00000e60: 7407 6a08 7c07 8e00 a102 0100 711d 7117  t.j.|.......q.q.
-00000e70: 7c04 5300 2903 4e63 0100 0000 0000 0000  |.S.).Nc........
-00000e80: 0000 0000 0300 0000 0500 0000 5300 0000  ............S...
-00000e90: 731e 0000 0069 007c 005d 0b5c 027d 017d  s....i.|.].\.}.}
-00000ea0: 0274 007c 0183 0174 007c 0283 0193 0271  .t.|...t.|.....q
-00000eb0: 0253 0072 0e00 0000 2901 7231 0000 0029  .S.r....).r1...)
-00000ec0: 0372 4d00 0000 da01 6bda 0176 720e 0000  .rM.....k..vr...
-00000ed0: 0072 0e00 0000 720f 0000 00da 0a3c 6469  .r....r......<di
-00000ee0: 6374 636f 6d70 3e73 0000 0073 0200 0000  ctcomp>s...s....
-00000ef0: 1e00 7a21 7265 636f 6c6f 725f 696d 6167  ..z!recolor_imag
-00000f00: 652e 3c6c 6f63 616c 733e 2e3c 6469 6374  e.<locals>.<dict
-00000f10: 636f 6d70 3e29 09da 0569 7465 6d73 7239  comp>)...itemsr9
-00000f20: 0000 0072 3a00 0000 723b 0000 0072 1600  ...r:...r;...r..
-00000f30: 0000 da03 6765 7472 3c00 0000 7208 0000  ....getr<...r...
-00000f40: 0072 0200 0000 2909 721d 0000 0072 5900  .r....).r....rY.
-00000f50: 0000 723d 0000 0072 3e00 0000 5a0b 6e65  ..r=...r>...Z.ne
-00000f60: 775f 7375 7266 6163 6572 3f00 0000 7240  w_surfacer?...r@
-00000f70: 0000 0072 3200 0000 7241 0000 0072 0e00  ...r2...rA...r..
-00000f80: 0000 720e 0000 0072 0f00 0000 da0d 7265  ..r....r......re
-00000f90: 636f 6c6f 725f 696d 6167 6570 0000 0073  color_imagep...s
-00000fa0: 1800 0000 1203 0c01 0802 0c05 0c01 1601  ................
-00000fb0: 0a01 0401 1801 1802 02fa 0408 725f 0000  ............r_..
-00000fc0: 00da 0863 6f6c 6f72 6d61 7063 0200 0000  ...colormapc....
-00000fd0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000fe0: 0300 0000 724a 0000 0029 034e 6301 0000  ....rJ...).Nc...
-00000ff0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001000: 0013 0000 0072 4b00 0000 720e 0000 0029  .....rK...r....)
-00001010: 0172 5f00 0000 724c 0000 00a9 0172 6000  .r_...rL.....r`.
-00001020: 0000 720e 0000 0072 0f00 0000 724f 0000  ..r....r....rO..
-00001030: 0088 0000 0072 5000 0000 7a22 7265 636f  .....rP...z"reco
-00001040: 6c6f 725f 696d 6167 6573 2e3c 6c6f 6361  lor_images.<loca
-00001050: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 720e  ls>.<listcomp>r.
-00001060: 0000 0029 0272 4900 0000 7260 0000 0072  ...).rI...r`...r
-00001070: 0e00 0000 7261 0000 0072 0f00 0000 da0e  ....ra...r......
-00001080: 7265 636f 6c6f 725f 696d 6167 6573 8700  recolor_images..
-00001090: 0000 722b 0000 0072 6200 0000 721a 0000  ..r+...rb...r...
-000010a0: 00da 0a69 6d61 6765 5f73 697a 65da 0a6e  ...image_size..n
-000010b0: 756d 5f69 6d61 6765 7363 0400 0000 0000  um_imagesc......
-000010c0: 0000 0000 0000 0700 0000 0400 0000 0300  ................
-000010d0: 0000 73ac 0000 0074 007c 0083 017d 007c  ..s....t.|...}.|
-000010e0: 00a0 01a1 0073 0f74 0264 017c 009b 009d  .....s.t.d.|....
-000010f0: 0283 0182 0174 037c 00a0 04a1 007c 0283  .....t.|.....|..
-00001100: 0289 027c 0172 517c 015c 0289 0389 0088  ...|.rQ|.\......
-00001110: 02a0 05a1 006a 0688 031a 0089 0188 02a0  .....j..........
-00001120: 05a1 006a 0788 001a 007d 0487 0087 0187  ...j.....}......
-00001130: 0366 0364 0264 0384 0874 087c 0483 0144  .f.d.d...t.|...D
-00001140: 0083 017d 0587 0266 0164 0464 0384 087c  ...}...f.d.d...|
-00001150: 0544 0083 017d 0674 0974 0a74 0b7c 0683  .D...}.t.t.t.|..
-00001160: 0283 017d 067c 0372 4f7c 0664 057c 0385  ...}.|.rO|.d.|..
-00001170: 0219 007d 067c 0653 0088 0267 017d 067c  ...}.|.S...g.}.|
-00001180: 0653 0029 067a db4c 6f61 6420 7468 6520  .S.).z.Load the 
-00001190: 696d 6167 6520 6669 6c65 2e20 446f 6e27  image file. Don'
-000011a0: 7420 6361 6c6c 2074 6869 7320 756e 7469  t call this unti
-000011b0: 6c20 7079 6761 6d65 2e64 6973 706c 6179  l pygame.display
-000011c0: 2068 6173 2062 6565 6e20 696e 6974 6961   has been initia
-000011d0: 7465 642e 2053 706c 6974 0a20 2020 2074  ted. Split.    t
-000011e0: 6865 2073 7072 6974 6573 6865 6574 2069  he spritesheet i
-000011f0: 6e74 6f20 696d 6167 6573 2061 6e64 2072  nto images and r
-00001200: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
-00001210: 696d 6167 6573 2e0a 0a20 2020 2049 6620  images...    If 
-00001220: 696d 6167 655f 7369 7a65 2069 7320 4e6f  image_size is No
-00001230: 6e65 2c20 6c6f 6164 2074 6865 2077 686f  ne, load the who
-00001240: 6c65 2073 7072 6974 6573 6865 6574 2061  le spritesheet a
-00001250: 7320 6f6e 6520 7370 7269 7465 2e0a 2020  s one sprite..  
-00001260: 2020 fa0e 436f 756c 646e 2774 2066 696e    ..Couldn't fin
-00001270: 6420 6301 0000 0000 0000 0000 0000 0003  d c.............
-00001280: 0000 0009 0000 0013 0000 0073 3400 0000  ...........s4...
-00001290: 6700 7c00 5d16 7d01 7400 8801 8301 4400  g.|.].}.t.....D.
-000012a0: 5d0f 7d02 7401 a002 8802 7c02 1400 8800  ].}.t.....|.....
-000012b0: 7c01 1400 8802 8800 6604 a101 9103 7108  |.......f.....q.
-000012c0: 7102 5300 720e 0000 0029 0372 3b00 0000  q.S.r....).r;...
-000012d0: 7208 0000 00da 0452 6563 7429 0372 4d00  r......Rect).rM.
-000012e0: 0000 da01 6ada 0169 2903 723e 0000 00da  ....j..i).r>....
-000012f0: 0e6e 756d 5f68 6f72 697a 6f6e 7461 6c72  .num_horizontalr
-00001300: 3d00 0000 720e 0000 0072 0f00 0000 724f  =...r....r....rO
-00001310: 0000 009f 0000 0073 0e00 0000 0600 0202  .......s........
-00001320: 0601 04fd 0203 18fe 08ff 7a24 6c6f 6164  ..........z$load
-00001330: 5f73 7072 6974 6573 6865 6574 2e3c 6c6f  _spritesheet.<lo
-00001340: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001350: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001360: 0005 0000 0013 0000 0073 1600 0000 6700  .........s....g.
-00001370: 7c00 5d07 7d01 8800 a000 7c01 a101 9102  |.].}.....|.....
-00001380: 7102 5300 720e 0000 0029 01da 0a73 7562  q.S.r....)...sub
-00001390: 7375 7266 6163 6529 0272 4d00 0000 da04  surface).rM.....
-000013a0: 7265 6374 2901 da05 7368 6565 7472 0e00  rect)...sheetr..
-000013b0: 0000 720f 0000 0072 4f00 0000 a400 0000  ..r....rO.......
-000013c0: 7250 0000 004e 290c 7203 0000 00da 0665  rP...N).r......e
-000013d0: 7869 7374 73da 1146 696c 654e 6f74 466f  xists..FileNotFo
-000013e0: 756e 6445 7272 6f72 721c 0000 00da 0861  undErrorr......a
-000013f0: 735f 706f 7369 7872 4400 0000 723d 0000  s_posixrD...r=..
-00001400: 0072 3e00 0000 723b 0000 00da 046c 6973  .r>...r;.....lis
-00001410: 74da 0666 696c 7465 7272 2000 0000 2907  t..filterr ...).
-00001420: 721a 0000 0072 6300 0000 721b 0000 0072  r....rc...r....r
-00001430: 6400 0000 5a0c 6e75 6d5f 7665 7274 6963  d...Z.num_vertic
-00001440: 616c 5a05 7265 6374 7372 4900 0000 720e  alZ.rectsrI...r.
-00001450: 0000 0029 0472 3e00 0000 7269 0000 0072  ...).r>...ri...r
-00001460: 6c00 0000 723d 0000 0072 0f00 0000 da10  l...r=...r......
-00001470: 6c6f 6164 5f73 7072 6974 6573 6865 6574  load_spritesheet
-00001480: 8b00 0000 7324 0000 0008 0b08 010e 010e  ....s$..........
-00001490: 0104 0208 010e 010e 010e 0106 0206 fe12  ................
-000014a0: 050e 0104 010c 0104 0306 ff04 0172 7200  .............rr.
-000014b0: 0000 6303 0000 0000 0000 0000 0000 0007  ..c.............
-000014c0: 0000 0006 0000 0003 0000 0073 6200 0000  ...........sb...
-000014d0: 7400 7c00 8301 7d00 7c00 6a01 7d03 7c00  t.|...}.|.j.}.|.
-000014e0: 6a02 7d04 7403 a003 7c03 9b00 6401 7c04  j.}.t...|...d.|.
-000014f0: 9b00 6402 9d04 a101 7d05 7c05 731e 7404  ..d.....}.|.s.t.
-00001500: 6403 7c00 9b00 9d02 8301 8201 8700 6601  d.|...........f.
-00001510: 6404 6405 8408 7c05 4400 8301 7d06 7c02  d.d...|.D...}.|.
-00001520: 722f 7c06 6406 7c02 8502 1900 7d06 7c06  r/|.d.|.....}.|.
-00001530: 5300 2907 7a1a 4c6f 6164 2061 2073 6571  S.).z.Load a seq
-00001540: 7565 6e63 6520 6f66 2069 6d61 6765 732e  uence of images.
-00001550: fa01 2fda 012a 7265 0000 0063 0100 0000  ../..*re...c....
-00001560: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001570: 1300 0000 724b 0000 0072 0e00 0000 2901  ....rK...r....).
-00001580: 721c 0000 0029 0272 4d00 0000 da04 6669  r....).rM.....fi
-00001590: 6c65 a901 721b 0000 0072 0e00 0000 720f  le..r....r....r.
-000015a0: 0000 0072 4f00 0000 b500 0000 7250 0000  ...rO.......rP..
-000015b0: 007a 276c 6f61 645f 696d 6167 655f 7365  .z'load_image_se
-000015c0: 7175 656e 6365 2e3c 6c6f 6361 6c73 3e2e  quence.<locals>.
-000015d0: 3c6c 6973 7463 6f6d 703e 4e29 0572 0300  <listcomp>N).r..
-000015e0: 0000 7228 0000 00da 0473 7465 6dda 0467  ..r(.....stem..g
-000015f0: 6c6f 6272 6e00 0000 2907 721a 0000 0072  lobrn...).r....r
-00001600: 1b00 0000 7264 0000 005a 0d70 6172 656e  ....rd...Z.paren
-00001610: 745f 666f 6c64 6572 da07 7061 7474 6572  t_folder..patter
-00001620: 6eda 0566 696c 6573 7249 0000 0072 0e00  n..filesrI...r..
-00001630: 0000 7276 0000 0072 0f00 0000 da13 6c6f  ..rv...r......lo
-00001640: 6164 5f69 6d61 6765 5f73 6571 7565 6e63  ad_image_sequenc
-00001650: 65ad 0000 0073 1400 0000 0802 0601 0601  e....s..........
-00001660: 1601 0401 0e01 1201 0401 0c01 0401 727b  ..............r{
-00001670: 0000 0072 2700 0000 2902 4646 2903 4e4e  ...r'...).FF).NN
-00001680: 7201 0000 0029 024e 7201 0000 0029 1eda  r....).Nr....)..
-00001690: 0c70 7967 616d 652e 636f 6c6f 7272 0200  .pygame.colorr..
-000016a0: 0000 7278 0000 00da 0770 6174 686c 6962  ..rx.....pathlib
-000016b0: 7203 0000 0072 0800 0000 7204 0000 00da  r....r....r.....
-000016c0: 0f72 6f62 696e 6761 6d65 2e75 7469 6c73  .robingame.utils
-000016d0: 7205 0000 0072 1000 0000 721c 0000 0072  r....r....r....r
-000016e0: 5300 0000 7220 0000 0072 2400 0000 da03  S...r ...r$.....
-000016f0: 7374 7272 2a00 0000 7231 0000 00da 0369  strr*...r1.....i
-00001700: 6e74 7238 0000 0072 4200 0000 da05 666c  ntr8...rB.....fl
-00001710: 6f61 7472 4800 0000 7251 0000 0072 5600  oatrH...rQ...rV.
-00001720: 0000 7258 0000 00da 0464 6963 7472 5f00  ..rX.....dictr_.
-00001730: 0000 7262 0000 0072 7200 0000 727b 0000  ..rb...rr...r{..
-00001740: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00001750: 720f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001760: 0000 0073 4200 0000 0c00 0801 0c01 0802  ...sB...........
-00001770: 0c01 0c02 0e03 1008 1213 0e07 1606 0804  ................
-00001780: 160a 1208 1214 1a07 1004 1204 1804 1a17  ................
-00001790: 0206 0201 0201 04fc 0601 02ff 0602 02fe  ................
-000017a0: 0204 02fc 0405 0afb 2222                 ........""
+00000290: 0000 0072 0e00 0000 fa33 2f68 6f6d 652f  ...r.....3/home/
+000002a0: 726f 6269 6e2f 636f 6465 2f72 6f62 696e  robin/code/robin
+000002b0: 6761 6d65 2f72 6f62 696e 6761 6d65 2f69  game/robingame/i
+000002c0: 6d61 6765 2f75 7469 6c73 2e70 79da 0c69  mage/utils.py..i
+000002d0: 6e69 745f 6469 7370 6c61 790b 0000 0073  nit_display....s
+000002e0: 0800 0000 0a01 0a01 0c01 0a02 7210 0000  ............r...
+000002f0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00000300: 0000 0800 0000 4300 0000 7368 0000 0074  ......C...sh...t
+00000310: 0083 0001 007a 0874 016a 02a0 037c 00a1  .....z.t.j...|..
+00000320: 017d 0257 006e 0e04 0074 016a 0479 1901  .}.W.n...t.j.y..
+00000330: 0001 0001 0074 0564 017c 0083 0201 0082  .....t.d.|......
+00000340: 0077 007c 0164 0075 0172 2e7c 0164 026b  .w.|.d.u.r.|.d.k
+00000350: 0272 277c 02a0 0664 03a1 017d 017c 02a0  .r'|...d...}.|..
+00000360: 077c 0174 016a 08a1 0201 007c 02a0 09a1  .|.t.j.....|....
+00000370: 007d 027c 0253 0029 044e 7a15 556e 6162  .}.|.S.).Nz.Unab
+00000380: 6c65 2074 6f20 6c6f 6164 2069 6d61 6765  le to load image
+00000390: 3ae9 ffff ffff 2902 7201 0000 0072 0100  :.....).r....r..
+000003a0: 0000 290a 7210 0000 0072 0800 0000 da05  ..).r....r......
+000003b0: 696d 6167 65da 046c 6f61 64da 0565 7272  image..load..err
+000003c0: 6f72 da05 7072 696e 74da 0667 6574 5f61  or..print..get_a
+000003d0: 74da 0c73 6574 5f63 6f6c 6f72 6b65 79da  t..set_colorkey.
+000003e0: 0852 4c45 4143 4345 4cda 0d63 6f6e 7665  .RLEACCEL..conve
+000003f0: 7274 5f61 6c70 6861 2903 da08 6669 6c65  rt_alpha)...file
+00000400: 6e61 6d65 da08 636f 6c6f 726b 6579 7212  name..colorkeyr.
+00000410: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000420: 0000 da0a 6c6f 6164 5f69 6d61 6765 1300  ....load_image..
+00000430: 0000 731a 0000 0006 0102 0110 010e 010a  ..s.............
+00000440: 0102 0102 fe08 0608 010a 010e 0108 0204  ................
+00000450: 0172 1c00 0000 da07 7375 7266 6163 6563  .r......surfacec
+00000460: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000470: 0300 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
+00000480: 00a0 01a1 0083 0153 0029 017a e843 6865  .......S.).z.Che
+00000490: 636b 2069 6620 6120 7375 7266 6163 6520  ck if a surface 
+000004a0: 6861 7320 616e 7920 6e6f 6e2d 7a65 726f  has any non-zero
+000004b0: 2070 6978 656c 732e 2060 5375 7266 6163   pixels. `Surfac
+000004c0: 652e 6765 745f 626f 756e 6469 6e67 5f72  e.get_bounding_r
+000004d0: 6563 7428 2960 2072 6574 7572 6e73 2074  ect()` returns t
+000004e0: 6865 0a20 2020 2073 6d61 6c6c 6573 7420  he.    smallest 
+000004f0: 7265 6374 616e 676c 6520 6f6e 2074 6865  rectangle on the
+00000500: 2073 7572 6661 6365 2063 6f6e 7461 696e   surface contain
+00000510: 696e 6720 6461 7461 2e20 4966 2074 6865  ing data. If the
+00000520: 2073 7572 6661 6365 2069 7320 656d 7074   surface is empt
+00000530: 792c 2069 7420 7769 6c6c 2072 6574 7572  y, it will retur
+00000540: 6e0a 2020 2020 5265 6374 2830 2c20 302c  n.    Rect(0, 0,
+00000550: 2030 2c20 3029 2c20 666f 7220 7768 6963   0, 0), for whic
+00000560: 6820 6061 6e79 6020 7265 7475 726e 7320  h `any` returns 
+00000570: 4661 6c73 6529 02da 0361 6e79 da11 6765  False)...any..ge
+00000580: 745f 626f 756e 6469 6e67 5f72 6563 7429  t_bounding_rect)
+00000590: 0172 1d00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000005a0: 720f 0000 00da 096e 6f74 5f65 6d70 7479  r......not_empty
+000005b0: 2600 0000 7302 0000 000c 0472 2000 0000  &...s......r ...
+000005c0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+000005d0: 0004 0000 004f 0000 0073 2000 0000 7400  .....O...s ...t.
+000005e0: 7c00 6900 7c01 a401 8e01 a001 a100 7d02  |.i.|.........}.
+000005f0: 7c02 a002 6401 a101 0100 7c02 5300 2902  |...d.....|.S.).
+00000600: 4e29 0472 0100 0000 7201 0000 0072 0100  N).r....r....r..
+00000610: 0000 7201 0000 0029 0372 0400 0000 7219  ..r....).r....r.
+00000620: 0000 00da 0466 696c 6c29 03da 0461 7267  .....fill)...arg
+00000630: 73da 066b 7761 7267 73da 0369 6d67 720e  s..kwargs..imgr.
+00000640: 0000 0072 0e00 0000 720f 0000 00da 0b65  ...r....r......e
+00000650: 6d70 7479 5f69 6d61 6765 2d00 0000 7306  mpty_image-...s.
+00000660: 0000 0012 010a 0104 0172 2500 0000 da0c  .........r%.....
+00000670: 6375 7272 656e 745f 6669 6c65 da06 666f  current_file..fo
+00000680: 6c64 6572 6302 0000 0000 0000 0000 0000  lderc...........
+00000690: 0002 0000 0002 0000 0043 0000 0073 1200  .........C...s..
+000006a0: 0000 7400 7c00 8301 6a01 a002 a100 7c01  ..t.|...j.....|.
+000006b0: 1b00 5300 a901 4e29 0372 0300 0000 da06  ..S...N).r......
+000006c0: 7061 7265 6e74 da08 6162 736f 6c75 7465  parent..absolute
+000006d0: 2902 7226 0000 0072 2700 0000 720e 0000  ).r&...r'...r...
+000006e0: 0072 0e00 0000 720f 0000 00da 0f72 656c  .r....r......rel
+000006f0: 6174 6976 655f 666f 6c64 6572 3300 0000  ative_folder3...
+00000700: f302 0000 0012 0172 2b00 0000 6301 0000  .......r+...c...
+00000710: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000720: 0043 0000 0073 3200 0000 7400 7c00 8301  .C...s2...t.|...
+00000730: 6401 6b02 720d 6700 7c00 a201 6402 9101  d.k.r.g.|...d...
+00000740: 5200 5300 7400 7c00 8301 6403 6b02 7215  R.S.t.|...d.k.r.
+00000750: 7c00 5300 7401 6404 8301 8201 2905 4ee9  |.S.t.d.....).N.
+00000760: 0300 0000 e9ff 0000 00e9 0400 0000 7a11  ..............z.
+00000770: 626f 6775 7320 636f 6c6f 7572 2c20 6d61  bogus colour, ma
+00000780: 6e29 02da 036c 656e da09 4578 6365 7074  n)...len..Except
+00000790: 696f 6e29 01da 0c63 6f6c 6f75 725f 7475  ion)...colour_tu
+000007a0: 706c 6572 0e00 0000 720e 0000 0072 0f00  pler....r....r..
+000007b0: 0000 da09 7061 645f 616c 7068 6137 0000  ....pad_alpha7..
+000007c0: 0073 0a00 0000 0c01 0e02 0c01 0401 0802  .s..............
+000007d0: 7233 0000 00da 0563 6f6c 6f72 da06 616d  r3.....color..am
+000007e0: 6f75 6e74 6302 0000 0000 0000 0000 0000  ountc...........
+000007f0: 0005 0000 0005 0000 0043 0000 0073 4e00  .........C...sN.
+00000800: 0000 7400 7c00 8301 7d00 7401 7c00 6a02  ..t.|...}.t.|.j.
+00000810: 7c01 1700 6401 6402 8d02 7d02 7401 7c00  |...d.d...}.t.|.
+00000820: 6a03 7c01 1700 6401 6402 8d02 7d03 7401  j.|...d.d...}.t.
+00000830: 7c00 6a04 7c01 1700 6401 6402 8d02 7d04  |.j.|...d.d...}.
+00000840: 7400 7c02 7c03 7c04 7c00 6a05 8304 5300  t.|.|.|.|.j...S.
+00000850: 2903 4e29 0272 0100 0000 722e 0000 0029  ).N).r....r....)
+00000860: 01da 0762 6574 7765 656e 2906 7202 0000  ...between).r...
+00000870: 0072 0500 0000 da01 72da 0167 da01 62da  .r......r..g..b.
+00000880: 0161 2905 7234 0000 0072 3500 0000 7237  .a).r4...r5...r7
+00000890: 0000 0072 3800 0000 7239 0000 0072 0e00  ...r8...r9...r..
+000008a0: 0000 720e 0000 0072 0f00 0000 da0e 6272  ..r....r......br
+000008b0: 6967 6874 656e 5f63 6f6c 6f72 4100 0000  ighten_colorA...
+000008c0: 730a 0000 0008 0112 0112 0112 0110 0172  s..............r
+000008d0: 3b00 0000 7212 0000 0063 0200 0000 0000  ;...r....c......
+000008e0: 0000 0000 0000 0900 0000 0700 0000 4300  ..............C.
+000008f0: 0000 7386 0000 007c 00a0 00a1 005c 027d  ..s....|.....\.}
+00000900: 027d 037c 00a0 01a1 007d 0474 027c 0283  .}.|.....}.t.|..
+00000910: 0144 005d 327d 0574 027c 0383 0144 005d  .D.]2}.t.|...D.]
+00000920: 2b7d 067c 00a0 037c 057c 0666 02a1 0164  +}.|...|.|.f...d
+00000930: 0064 0085 0219 007d 0774 047c 077c 0183  .d.....}.t.|.|..
+00000940: 027d 087c 0872 347c 04a0 057c 057c 0666  .}.|.r4|...|.|.f
+00000950: 0274 066a 077c 088e 00a1 0201 0071 147c  .t.j.|.......q.|
+00000960: 04a0 057c 057c 0666 0274 066a 077c 078e  ...|.|.f.t.j.|..
+00000970: 00a1 0201 0071 1471 0e7c 0453 0072 2800  .....q.q.|.S.r(.
+00000980: 0000 2908 da08 6765 745f 7369 7a65 da04  ..)...get_size..
+00000990: 636f 7079 da05 7261 6e67 6572 1600 0000  copy..ranger....
+000009a0: 723b 0000 00da 0673 6574 5f61 7472 0800  r;.....set_atr..
+000009b0: 0000 7202 0000 0029 0972 1200 0000 7235  ..r....).r....r5
+000009c0: 0000 00da 0577 6964 7468 da06 6865 6967  .....width..heig
+000009d0: 6874 da09 6e65 775f 696d 6167 65da 0178  ht..new_image..x
+000009e0: da01 7972 3400 0000 da09 6e65 775f 636f  ..yr4.....new_co
+000009f0: 6c6f 7272 0e00 0000 720e 0000 0072 0f00  lorr....r....r..
+00000a00: 0000 da08 6272 6967 6874 656e 4900 0000  ....brightenI...
+00000a10: 7316 0000 000c 0108 020c 050c 0116 010a  s...............
+00000a20: 0104 0118 0118 0202 fa04 0872 4600 0000  ...........rF...
+00000a30: da05 7363 616c 6563 0200 0000 0000 0000  ..scalec........
+00000a40: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+00000a50: 7332 0000 007c 00a0 00a1 006a 017c 0114  s2...|.....j.|..
+00000a60: 007d 027c 00a0 00a1 006a 027c 0114 007d  .}.|.....j.|...}
+00000a70: 0374 036a 04a0 057c 007c 027c 0366 02a1  .t.j...|.|.|.f..
+00000a80: 027d 007c 0053 0072 2800 0000 2906 da08  .}.|.S.r(...)...
+00000a90: 6765 745f 7265 6374 7240 0000 0072 4100  get_rectr@...rA.
+00000aa0: 0000 7208 0000 00da 0974 7261 6e73 666f  ..r......transfo
+00000ab0: 726d 7247 0000 0029 0472 1200 0000 7247  rmrG...).r....rG
+00000ac0: 0000 00da 0778 5f73 6361 6c65 da07 795f  .....x_scale..y_
+00000ad0: 7363 616c 6572 0e00 0000 720e 0000 0072  scaler....r....r
+00000ae0: 0f00 0000 da0b 7363 616c 655f 696d 6167  ......scale_imag
+00000af0: 655d 0000 0073 0800 0000 0e01 0e01 1201  e]...s..........
+00000b00: 0401 724c 0000 00da 0669 6d61 6765 7363  ..rL.....imagesc
+00000b10: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000b20: 0300 0000 0300 0000 f312 0000 0087 0066  ...............f
+00000b30: 0164 0164 0284 087c 0044 0083 0153 0029  .d.d...|.D...S.)
+00000b40: 034e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000b50: 0000 0005 0000 0013 0000 00f3 1600 0000  ................
+00000b60: 6700 7c00 5d07 7d01 7400 7c01 8800 8302  g.|.].}.t.|.....
+00000b70: 9102 7102 5300 720e 0000 0029 0172 4c00  ..q.S.r....).rL.
+00000b80: 0000 a902 da02 2e30 7212 0000 00a9 0172  .......0r......r
+00000b90: 4700 0000 720e 0000 0072 0f00 0000 da0a  G...r....r......
+00000ba0: 3c6c 6973 7463 6f6d 703e 6500 0000 f302  <listcomp>e.....
+00000bb0: 0000 0016 007a 2073 6361 6c65 5f69 6d61  .....z scale_ima
+00000bc0: 6765 732e 3c6c 6f63 616c 733e 2e3c 6c69  ges.<locals>.<li
+00000bd0: 7374 636f 6d70 3e72 0e00 0000 2902 724d  stcomp>r....).rM
+00000be0: 0000 0072 4700 0000 720e 0000 0072 5200  ...rG...r....rR.
+00000bf0: 0000 720f 0000 00da 0c73 6361 6c65 5f69  ..r......scale_i
+00000c00: 6d61 6765 7364 0000 0072 2c00 0000 7255  magesd...r,...rU
+00000c10: 0000 0046 6303 0000 0000 0000 0000 0000  ...Fc...........
+00000c20: 0003 0000 0006 0000 0043 0000 0073 1800  .........C...s..
+00000c30: 0000 7400 6a01 a002 7c00 7403 7c01 8301  ..t.j...|.t.|...
+00000c40: 7403 7c02 8301 a103 5300 7228 0000 0029  t.|.....S.r(...)
+00000c50: 0472 0800 0000 7249 0000 00da 0466 6c69  .r....rI.....fli
+00000c60: 70da 0462 6f6f 6c29 0372 1200 0000 da06  p..bool).r......
+00000c70: 666c 6970 5f78 da06 666c 6970 5f79 720e  flip_x..flip_yr.
+00000c80: 0000 0072 0e00 0000 720f 0000 00da 0a66  ...r....r......f
+00000c90: 6c69 705f 696d 6167 6568 0000 0073 0200  lip_imageh...s..
+00000ca0: 0000 1801 725a 0000 0063 0300 0000 0000  ....rZ...c......
+00000cb0: 0000 0000 0000 0300 0000 0300 0000 0300  ................
+00000cc0: 0000 7314 0000 0087 0087 0166 0264 0164  ..s........f.d.d
+00000cd0: 0284 087c 0044 0083 0153 0029 034e 6301  ...|.D...S.).Nc.
+00000ce0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00000cf0: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
+00000d00: 5d08 7d01 7400 7c01 8800 8801 8303 9102  ].}.t.|.........
+00000d10: 7102 5300 720e 0000 0029 0172 5a00 0000  q.S.r....).rZ...
+00000d20: 7250 0000 00a9 0272 5800 0000 7259 0000  rP.....rX...rY..
+00000d30: 0072 0e00 0000 720f 0000 0072 5300 0000  .r....r....rS...
+00000d40: 6d00 0000 7302 0000 0018 007a 1f66 6c69  m...s......z.fli
+00000d50: 705f 696d 6167 6573 2e3c 6c6f 6361 6c73  p_images.<locals
+00000d60: 3e2e 3c6c 6973 7463 6f6d 703e 720e 0000  >.<listcomp>r...
+00000d70: 0029 0372 4d00 0000 7258 0000 0072 5900  .).rM...rX...rY.
+00000d80: 0000 720e 0000 0072 5b00 0000 720f 0000  ..r....r[...r...
+00000d90: 00da 0b66 6c69 705f 696d 6167 6573 6c00  ...flip_imagesl.
+00000da0: 0000 7302 0000 0014 0172 5c00 0000 da0d  ..s......r\.....
+00000db0: 636f 6c6f 725f 6d61 7070 696e 6763 0200  color_mappingc..
+00000dc0: 0000 0000 0000 0000 0000 0900 0000 0700  ................
+00000dd0: 0000 4300 0000 7398 0000 0064 0164 0284  ..C...s....d.d..
+00000de0: 007c 01a0 00a1 0044 0083 017d 017c 00a0  .|.....D...}.|..
+00000df0: 01a1 005c 027d 027d 037c 00a0 02a1 007d  ...\.}.}.|.....}
+00000e00: 0474 037c 0283 0144 005d 327d 0574 037c  .t.|...D.]2}.t.|
+00000e10: 0383 0144 005d 2b7d 067c 00a0 047c 057c  ...D.]+}.|...|.|
+00000e20: 0666 02a1 0164 0064 0085 0219 007d 077c  .f...d.d.....}.|
+00000e30: 01a0 057c 07a1 017d 087c 0872 3d7c 04a0  ...|...}.|.r=|..
+00000e40: 067c 057c 0666 0274 076a 087c 088e 00a1  .|.|.f.t.j.|....
+00000e50: 0201 0071 1d7c 04a0 067c 057c 0666 0274  ...q.|...|.|.f.t
+00000e60: 076a 087c 078e 00a1 0201 0071 1d71 177c  .j.|.......q.q.|
+00000e70: 0453 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000e80: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
+00000e90: 1e00 0000 6900 7c00 5d0b 5c02 7d01 7d02  ....i.|.].\.}.}.
+00000ea0: 7400 7c01 8301 7400 7c02 8301 9302 7102  t.|...t.|.....q.
+00000eb0: 5300 720e 0000 0029 0172 3300 0000 2903  S.r....).r3...).
+00000ec0: 7251 0000 00da 016b da01 7672 0e00 0000  rQ.....k..vr....
+00000ed0: 720e 0000 0072 0f00 0000 da0a 3c64 6963  r....r......<dic
+00000ee0: 7463 6f6d 703e 7200 0000 7302 0000 001e  tcomp>r...s.....
+00000ef0: 007a 2172 6563 6f6c 6f72 5f69 6d61 6765  .z!recolor_image
+00000f00: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000f10: 6f6d 703e 2909 da05 6974 656d 7372 3c00  omp>)...itemsr<.
+00000f20: 0000 723d 0000 0072 3e00 0000 7216 0000  ..r=...r>...r...
+00000f30: 00da 0367 6574 723f 0000 0072 0800 0000  ...getr?...r....
+00000f40: 7202 0000 0029 0972 1d00 0000 725d 0000  r....).r....r]..
+00000f50: 0072 4000 0000 7241 0000 00da 0b6e 6577  .r@...rA.....new
+00000f60: 5f73 7572 6661 6365 7243 0000 0072 4400  _surfacerC...rD.
+00000f70: 0000 7234 0000 0072 4500 0000 720e 0000  ..r4...rE...r...
+00000f80: 0072 0e00 0000 720f 0000 00da 0d72 6563  .r....r......rec
+00000f90: 6f6c 6f72 5f69 6d61 6765 7000 0000 7318  olor_imagep...s.
+00000fa0: 0000 0012 020c 0108 020c 050c 0116 010a  ................
+00000fb0: 0104 0118 0118 0202 fa04 0872 6400 0000  ...........rd...
+00000fc0: da08 636f 6c6f 726d 6170 6302 0000 0000  ..colormapc.....
+00000fd0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
+00000fe0: 0000 0072 4e00 0000 2903 4e63 0100 0000  ...rN...).Nc....
+00000ff0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00001000: 1300 0000 724f 0000 0072 0e00 0000 2901  ....rO...r....).
+00001010: 7264 0000 0072 5000 0000 a901 7265 0000  rd...rP.....re..
+00001020: 0072 0e00 0000 720f 0000 0072 5300 0000  .r....r....rS...
+00001030: 8700 0000 7254 0000 007a 2272 6563 6f6c  ....rT...z"recol
+00001040: 6f72 5f69 6d61 6765 732e 3c6c 6f63 616c  or_images.<local
+00001050: 733e 2e3c 6c69 7374 636f 6d70 3e72 0e00  s>.<listcomp>r..
+00001060: 0000 2902 724d 0000 0072 6500 0000 720e  ..).rM...re...r.
+00001070: 0000 0072 6600 0000 720f 0000 00da 0e72  ...rf...r......r
+00001080: 6563 6f6c 6f72 5f69 6d61 6765 7386 0000  ecolor_images...
+00001090: 0072 2c00 0000 7267 0000 0072 1a00 0000  .r,...rg...r....
+000010a0: da0a 696d 6167 655f 7369 7a65 da0a 6e75  ..image_size..nu
+000010b0: 6d5f 696d 6167 6573 6304 0000 0000 0000  m_imagesc.......
+000010c0: 0000 0000 0007 0000 0004 0000 0003 0000  ................
+000010d0: 0073 ac00 0000 7400 7c00 8301 7d00 7c00  .s....t.|...}.|.
+000010e0: a001 a100 730f 7402 6401 7c00 9b00 9d02  ....s.t.d.|.....
+000010f0: 8301 8201 7403 7c00 a004 a100 7c02 8302  ....t.|.....|...
+00001100: 8902 7c01 7251 7c01 5c02 8903 8900 8802  ..|.rQ|.\.......
+00001110: a005 a100 6a06 8803 1a00 8901 8802 a005  ....j...........
+00001120: a100 6a07 8800 1a00 7d04 8700 8701 8703  ..j.....}.......
+00001130: 6603 6402 6403 8408 7408 7c04 8301 4400  f.d.d...t.|...D.
+00001140: 8301 7d05 8702 6601 6404 6403 8408 7c05  ..}...f.d.d...|.
+00001150: 4400 8301 7d06 7409 740a 740b 7c06 8302  D...}.t.t.t.|...
+00001160: 8301 7d06 7c03 724f 7c06 6405 7c03 8502  ..}.|.rO|.d.|...
+00001170: 1900 7d06 7c06 5300 8802 6701 7d06 7c06  ..}.|.S...g.}.|.
+00001180: 5300 2906 7adb 4c6f 6164 2074 6865 2069  S.).z.Load the i
+00001190: 6d61 6765 2066 696c 652e 2044 6f6e 2774  mage file. Don't
+000011a0: 2063 616c 6c20 7468 6973 2075 6e74 696c   call this until
+000011b0: 2070 7967 616d 652e 6469 7370 6c61 7920   pygame.display 
+000011c0: 6861 7320 6265 656e 2069 6e69 7469 6174  has been initiat
+000011d0: 6564 2e20 5370 6c69 740a 2020 2020 7468  ed. Split.    th
+000011e0: 6520 7370 7269 7465 7368 6565 7420 696e  e spritesheet in
+000011f0: 746f 2069 6d61 6765 7320 616e 6420 7265  to images and re
+00001200: 7475 726e 2061 206c 6973 7420 6f66 2069  turn a list of i
+00001210: 6d61 6765 732e 0a0a 2020 2020 4966 2069  mages...    If i
+00001220: 6d61 6765 5f73 697a 6520 6973 204e 6f6e  mage_size is Non
+00001230: 652c 206c 6f61 6420 7468 6520 7768 6f6c  e, load the whol
+00001240: 6520 7370 7269 7465 7368 6565 7420 6173  e spritesheet as
+00001250: 206f 6e65 2073 7072 6974 652e 0a20 2020   one sprite..   
+00001260: 20fa 0e43 6f75 6c64 6e27 7420 6669 6e64   ..Couldn't find
+00001270: 2063 0100 0000 0000 0000 0000 0000 0300   c..............
+00001280: 0000 0900 0000 1300 0000 7334 0000 0067  ..........s4...g
+00001290: 007c 005d 167d 0174 0088 0183 0144 005d  .|.].}.t.....D.]
+000012a0: 0f7d 0274 01a0 0288 027c 0214 0088 007c  .}.t.....|.....|
+000012b0: 0114 0088 0288 0066 04a1 0191 0371 0871  .......f.....q.q
+000012c0: 0253 0072 0e00 0000 2903 723e 0000 0072  .S.r....).r>...r
+000012d0: 0800 0000 da04 5265 6374 2903 7251 0000  ......Rect).rQ..
+000012e0: 00da 016a da01 6929 0372 4100 0000 da0e  ...j..i).rA.....
+000012f0: 6e75 6d5f 686f 7269 7a6f 6e74 616c 7240  num_horizontalr@
+00001300: 0000 0072 0e00 0000 720f 0000 0072 5300  ...r....r....rS.
+00001310: 0000 9e00 0000 730e 0000 0006 0002 0206  ......s.........
+00001320: 0104 fd02 0318 fe08 ff7a 246c 6f61 645f  .........z$load_
+00001330: 7370 7269 7465 7368 6565 742e 3c6c 6f63  spritesheet.<loc
+00001340: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
+00001350: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001360: 0500 0000 1300 0000 7316 0000 0067 007c  ........s....g.|
+00001370: 005d 077d 0188 00a0 007c 01a1 0191 0271  .].}.....|.....q
+00001380: 0253 0072 0e00 0000 2901 da0a 7375 6273  .S.r....)...subs
+00001390: 7572 6661 6365 2902 7251 0000 00da 0472  urface).rQ.....r
+000013a0: 6563 7429 01da 0573 6865 6574 720e 0000  ect)...sheetr...
+000013b0: 0072 0f00 0000 7253 0000 00a3 0000 0072  .r....rS.......r
+000013c0: 5400 0000 4e29 0c72 0300 0000 da06 6578  T...N).r......ex
+000013d0: 6973 7473 da11 4669 6c65 4e6f 7446 6f75  ists..FileNotFou
+000013e0: 6e64 4572 726f 7272 1c00 0000 da08 6173  ndErrorr......as
+000013f0: 5f70 6f73 6978 7248 0000 0072 4000 0000  _posixrH...r@...
+00001400: 7241 0000 0072 3e00 0000 da04 6c69 7374  rA...r>.....list
+00001410: da06 6669 6c74 6572 7220 0000 0029 0772  ..filterr ...).r
+00001420: 1a00 0000 7268 0000 0072 1b00 0000 7269  ....rh...r....ri
+00001430: 0000 00da 0c6e 756d 5f76 6572 7469 6361  .....num_vertica
+00001440: 6cda 0572 6563 7473 724d 0000 0072 0e00  l..rectsrM...r..
+00001450: 0000 2904 7241 0000 0072 6e00 0000 7271  ..).rA...rn...rq
+00001460: 0000 0072 4000 0000 720f 0000 00da 106c  ...r@...r......l
+00001470: 6f61 645f 7370 7269 7465 7368 6565 748a  oad_spritesheet.
+00001480: 0000 0073 2400 0000 080b 0801 0e01 0e01  ...s$...........
+00001490: 0402 0801 0e01 0e01 0e01 0602 06fe 1205  ................
+000014a0: 0e01 0401 0c01 0403 06ff 0401 7279 0000  ............ry..
+000014b0: 0063 0300 0000 0000 0000 0000 0000 0700  .c..............
+000014c0: 0000 0600 0000 0300 0000 7362 0000 0074  ..........sb...t
+000014d0: 007c 0083 017d 007c 006a 017d 037c 006a  .|...}.|.j.}.|.j
+000014e0: 027d 0474 03a0 037c 039b 0064 017c 049b  .}.t...|...d.|..
+000014f0: 0064 029d 04a1 017d 057c 0573 1e74 0464  .d.....}.|.s.t.d
+00001500: 037c 009b 009d 0283 0182 0187 0066 0164  .|...........f.d
+00001510: 0464 0584 087c 0544 0083 017d 067c 0272  .d...|.D...}.|.r
+00001520: 2f7c 0664 067c 0285 0219 007d 067c 0653  /|.d.|.....}.|.S
+00001530: 0029 077a 1a4c 6f61 6420 6120 7365 7175  .).z.Load a sequ
+00001540: 656e 6365 206f 6620 696d 6167 6573 2efa  ence of images..
+00001550: 012f da01 2a72 6a00 0000 6301 0000 0000  ./..*rj...c.....
+00001560: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001570: 0000 0072 4f00 0000 720e 0000 0029 0172  ...rO...r....).r
+00001580: 1c00 0000 2902 7251 0000 00da 0466 696c  ....).rQ.....fil
+00001590: 65a9 0172 1b00 0000 720e 0000 0072 0f00  e..r....r....r..
+000015a0: 0000 7253 0000 00b4 0000 0072 5400 0000  ..rS.......rT...
+000015b0: 7a27 6c6f 6164 5f69 6d61 6765 5f73 6571  z'load_image_seq
+000015c0: 7565 6e63 652e 3c6c 6f63 616c 733e 2e3c  uence.<locals>.<
+000015d0: 6c69 7374 636f 6d70 3e4e 2905 7203 0000  listcomp>N).r...
+000015e0: 0072 2900 0000 da04 7374 656d da04 676c  .r).....stem..gl
+000015f0: 6f62 7273 0000 0029 0772 1a00 0000 721b  obrs...).r....r.
+00001600: 0000 0072 6900 0000 da0d 7061 7265 6e74  ...ri.....parent
+00001610: 5f66 6f6c 6465 72da 0770 6174 7465 726e  _folder..pattern
+00001620: da05 6669 6c65 7372 4d00 0000 720e 0000  ..filesrM...r...
+00001630: 0072 7d00 0000 720f 0000 00da 136c 6f61  .r}...r......loa
+00001640: 645f 696d 6167 655f 7365 7175 656e 6365  d_image_sequence
+00001650: ac00 0000 7314 0000 0008 0206 0106 0116  ....s...........
+00001660: 0104 010e 0112 0104 010c 0104 0172 8300  .............r..
+00001670: 0000 7228 0000 0029 0246 4629 034e 4e72  ..r(...).FF).NNr
+00001680: 0100 0000 2902 4e72 0100 0000 291e da0c  ....).Nr....)...
+00001690: 7079 6761 6d65 2e63 6f6c 6f72 7202 0000  pygame.colorr...
+000016a0: 0072 7f00 0000 da07 7061 7468 6c69 6272  .r......pathlibr
+000016b0: 0300 0000 7208 0000 0072 0400 0000 da0f  ....r....r......
+000016c0: 726f 6269 6e67 616d 652e 7574 696c 7372  robingame.utilsr
+000016d0: 0500 0000 7210 0000 0072 1c00 0000 7257  ....r....r....rW
+000016e0: 0000 0072 2000 0000 7225 0000 00da 0373  ...r ...r%.....s
+000016f0: 7472 722b 0000 0072 3300 0000 da03 696e  trr+...r3.....in
+00001700: 7472 3b00 0000 7246 0000 00da 0566 6c6f  tr;...rF.....flo
+00001710: 6174 724c 0000 0072 5500 0000 725a 0000  atrL...rU...rZ..
+00001720: 0072 5c00 0000 da04 6469 6374 7264 0000  .r\.....dictrd..
+00001730: 0072 6700 0000 7279 0000 0072 8300 0000  .rg...ry...r....
+00001740: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00001750: 0f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001760: 0000 7342 0000 000c 0008 010c 0108 020c  ..sB............
+00001770: 010c 020e 0310 0812 130e 0716 0608 0416  ................
+00001780: 0a12 0812 141a 0710 0412 0418 041a 1602  ................
+00001790: 0602 0102 0104 fc06 0102 ff06 0202 fe02  ................
+000017a0: 0402 fc04 050a fb22 22                   .......""
```

### Comparing `robingame-0.0.9/robingame/image/classes.py` & `robingame-0.1.0/robingame/image/classes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from typing import Callable
 
 from pygame import Surface
 
 from robingame.image.utils import (
     load_spritesheet,
     load_image_sequence,
     flip_images,
@@ -15,19 +14,18 @@
 class SpriteAnimation:
     """
     Animates a sequence of images.
     Can scale, flip, and recolor itself.
     """
 
     images: list[Surface] | None
-    source: Callable | None
 
     def __init__(
         self,
-        images: [Surface] = None,
+        images: list[Surface] = None,
         scale: float = None,
         flip_x: bool = False,
         flip_y: bool = False,
         colormap: dict = None,
     ):
         self.images = images
         if scale:
@@ -129,58 +127,7 @@
         return self.__class__(images=recolor_images(self.images, colormap))
 
     def scaled_copy(self, scale: float):
         return self.__class__(images=scale_images(self.images, scale))
 
     def __len__(self):
         return len(self.images)
-
-
-class SpriteDict(dict):
-    """
-    Takes a folder and list of files as input, and handles the creation of SpriteAnimations.
-    """
-
-    def __init__(
-        self,
-        folder: Path | str,
-        size: (int, int) = None,
-        file_mapping: dict = None,
-        scale: int = 1,
-        colormap: dict = None,
-        create_flipped_versions: bool = False,
-        type="spritesheet",
-    ):
-        """
-        Create SpriteSheet for each file, but don't trigger .load() yet.
-        """
-        super().__init__()
-        self.scale = scale
-        self.image_size = size
-        self.colormap = colormap
-        self.create_flipped_versions = create_flipped_versions
-        folder = Path(folder)
-        self.folder = folder
-        self.type = type
-        self.sprite_sheets = dict()
-        if file_mapping:
-            for key, filename in file_mapping.items():
-                self.register(**{key: filename})
-
-    def register(self, **kwargs):
-        for key, filename in kwargs.items():
-            if self.type == "spritesheet":  # todo: add other options
-                self[key] = unflipped = SpriteAnimation.from_spritesheet(
-                    self.folder / filename,
-                    image_size=self.image_size,
-                    colormap=self.colormap,
-                    scale=self.scale,
-                )
-                if self.create_flipped_versions:
-                    self[f"{key}_right"] = unflipped
-                    self[f"{key}_left"] = SpriteAnimation.from_spritesheet(
-                        self.folder / filename,
-                        image_size=self.image_size,
-                        colormap=self.colormap,
-                        scale=self.scale,
-                        flip_x=True,
-                    )
```

### Comparing `robingame-0.0.9/robingame/image/utils.py` & `robingame-0.1.0/robingame/image/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 
 
 def flip_images(images: [Surface], flip_x=False, flip_y=False):
     return [flip_image(image, flip_x, flip_y) for image in images]
 
 
 def recolor_image(surface: Surface, color_mapping: dict) -> [Surface]:
-
     # make sure the colourmap has alpha channel on all colours
     color_mapping = {pad_alpha(k): pad_alpha(v) for k, v in color_mapping.items()}
     width, height = surface.get_size()
     # surface.copy() inherits surface's colorkey; preserving transparency
     new_surface = surface.copy()
 
     # iterate over all the pixels in the old surface, and write a pixel to the new surface in the
```

### Comparing `robingame-0.0.9/robingame/input/__pycache__/event.cpython-310.pyc` & `robingame-0.1.0/robingame/input/__pycache__/event.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 15:38:53 2022 UTC, .py size: 1623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8d0d 3763 5706 0000  o.........7cW...
+00000000: 6f0d 0d0a 0000 0000 88a3 6064 5706 0000  o.........`dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 650b 8300 0100 4700 6406 6407 8400  ..e.....G.d.d...
@@ -51,91 +51,91 @@
 00000320: 2020 2020 7175 6575 6520 616e 6420 7072      queue and pr
 00000330: 6f63 6573 7365 6420 696e 2074 6865 2073  ocessed in the s
 00000340: 616d 6520 7469 636b 2e0a 2020 2020 2020  ame tick..      
 00000350: 2020 4e29 0772 0300 0000 7207 0000 00da    N).r....r.....
 00000360: 0474 7970 6572 0400 0000 da06 7079 6761  .typer......pyga
 00000370: 6d65 720a 0000 00da 0470 6f73 7429 02da  mer......post)..
 00000380: 0363 6c73 720a 0000 00a9 0072 0f00 0000  .clsr......r....
-00000390: fa34 2f68 6f6d 652f 6269 6e6e 6576 2f63  .4/home/binnev/c
-000003a0: 6f64 652f 726f 6269 6e67 616d 652f 726f  ode/robingame/ro
-000003b0: 6269 6e67 616d 652f 696e 7075 742f 6576  bingame/input/ev
-000003c0: 656e 742e 7079 da03 6164 6414 0000 0073  ent.py..add....s
-000003d0: 0600 0000 0809 1601 1001 7a0e 4576 656e  ..........z.Even
-000003e0: 7451 7565 7565 2e61 6464 6301 0000 0000  tQueue.addc.....
-000003f0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000400: 0000 0073 1000 0000 7400 6a01 a002 a100  ...s....t.j.....
-00000410: 7c00 5f03 6401 5300 2902 7a7a 0a20 2020  |._.d.S.).zz.   
-00000420: 2020 2020 2052 6561 6420 616c 6c20 7468       Read all th
-00000430: 6520 6576 656e 7473 2066 726f 6d20 7079  e events from py
-00000440: 6761 6d65 2773 2065 7665 6e74 2071 7565  game's event que
-00000450: 7565 2069 6e74 6f20 636c 732e 6576 656e  ue into cls.even
-00000460: 7473 0a20 2020 2020 2020 2028 616c 736f  ts.        (also
-00000470: 2063 6c65 6172 7320 7079 6761 6d65 2773   clears pygame's
-00000480: 2065 7665 6e74 2071 7565 7565 290a 2020   event queue).  
-00000490: 2020 2020 2020 4e29 0472 0c00 0000 720a        N).r....r.
-000004a0: 0000 00da 0367 6574 da06 6576 656e 7473  .....get..events
-000004b0: 2901 720e 0000 0072 0f00 0000 720f 0000  ).r....r....r...
-000004c0: 0072 1000 0000 da06 7570 6461 7465 2100  .r......update!.
-000004d0: 0000 7302 0000 0010 067a 1145 7665 6e74  ..s......z.Event
-000004e0: 5175 6575 652e 7570 6461 7465 6301 0000  Queue.updatec...
-000004f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000500: 000b 0000 0073 1400 0000 8700 6601 6401  .....s......f.d.
-00000510: 6402 8408 7c00 6a00 4400 8301 5300 2903  d...|.j.D...S.).
-00000520: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00000530: 0000 0600 0000 1300 0000 732a 0000 0067  ..........s*...g
-00000540: 007c 005d 1189 0074 0087 0066 0164 0064  .|.]...t...f.d.d
-00000550: 0184 0888 01a0 01a1 0044 0083 0183 0172  .........D.....r
-00000560: 0288 0091 0271 0253 0029 0263 0100 0000  .....q.S.).c....
-00000570: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000580: 3300 0000 7324 0000 0081 007c 005d 0d5c  3...s$.....|.].\
-00000590: 027d 017d 0274 0088 007c 0164 0083 037c  .}.}.t...|.d...|
-000005a0: 026b 0256 0001 0071 0264 0053 0029 014e  .k.V...q.d.S.).N
-000005b0: 2901 da07 6765 7461 7474 7229 03da 022e  )...getattr)....
-000005c0: 30da 0961 7474 7269 6275 7465 da05 7661  0..attribute..va
-000005d0: 6c75 65a9 0172 0a00 0000 720f 0000 0072  lue..r....r....r
-000005e0: 1000 0000 da09 3c67 656e 6578 7072 3e2e  ......<genexpr>.
-000005f0: 0000 0073 0400 0000 0280 2200 7a2f 4576  ...s......".z/Ev
-00000600: 656e 7451 7565 7565 2e66 696c 7465 722e  entQueue.filter.
-00000610: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000620: 6d70 3e2e 3c67 656e 6578 7072 3e29 02da  mp>.<genexpr>)..
-00000630: 0361 6c6c da05 6974 656d 7329 0172 1600  .all..items).r..
-00000640: 0000 a901 da06 6b77 6172 6773 7219 0000  ......kwargsr...
-00000650: 0072 1000 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000660: 703e 2b00 0000 730c 0000 0006 0002 0218  p>+...s.........
-00000670: 0102 fd02 0106 ff7a 2545 7665 6e74 5175  .......z%EventQu
-00000680: 6575 652e 6669 6c74 6572 2e3c 6c6f 6361  eue.filter.<loca
-00000690: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2901  ls>.<listcomp>).
-000006a0: 7213 0000 00a9 0272 0e00 0000 721e 0000  r......r....r...
-000006b0: 0072 0f00 0000 721d 0000 0072 1000 0000  .r....r....r....
-000006c0: da06 6669 6c74 6572 2900 0000 7306 0000  ..filter)...s...
-000006d0: 000a 0204 0206 fe7a 1145 7665 6e74 5175  .......z.EventQu
-000006e0: 6575 652e 6669 6c74 6572 6301 0000 0000  eue.filterc.....
-000006f0: 0000 0000 0000 0002 0000 0008 0000 004b  ...............K
-00000700: 0000 0073 2c00 0000 7a0b 7c00 6a00 6402  ...s,...z.|.j.d.
-00000710: 6900 7c01 a401 8e01 6401 1900 5700 5300  i.|.....d...W.S.
-00000720: 0400 7401 7915 0100 0100 0100 5900 6400  ..t.y.......Y.d.
-00000730: 5300 7700 2903 4e72 0100 0000 720f 0000  S.w.).Nr....r...
-00000740: 0029 0272 2100 0000 da0a 496e 6465 7845  .).r!.....IndexE
-00000750: 7272 6f72 7220 0000 0072 0f00 0000 720f  rrorr ...r....r.
-00000760: 0000 0072 1000 0000 7212 0000 0031 0000  ...r....r....1..
-00000770: 0073 0a00 0000 0202 1601 0c01 0601 02ff  .s..............
-00000780: 7a0e 4576 656e 7451 7565 7565 2e67 6574  z.EventQueue.get
-00000790: 4e29 0cda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000007a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000007b0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-000007c0: 7213 0000 00da 0b63 6c61 7373 6d65 7468  r......classmeth
-000007d0: 6f64 7205 0000 0072 0600 0000 7211 0000  odr....r....r...
-000007e0: 0072 1400 0000 7221 0000 0072 1200 0000  .r....r!...r....
-000007f0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000800: 1000 0000 7209 0000 000c 0000 0073 1600  ....r........s..
-00000810: 0000 0800 0401 0405 0202 1801 020c 0a01  ................
-00000820: 0207 0a01 0207 0e01 7209 0000 0029 0dda  ........r....)..
-00000830: 0b64 6174 6163 6c61 7373 6573 7202 0000  .dataclassesr...
-00000840: 0072 0300 0000 7204 0000 00da 0674 7970  .r....r......typ
-00000850: 696e 6772 0500 0000 720c 0000 00da 0c70  ingr....r......p
-00000860: 7967 616d 652e 6576 656e 7472 0600 0000  ygame.eventr....
-00000870: 7207 0000 005a 0f72 6f62 696e 6761 6d65  r....Z.robingame
-00000880: 2e69 6d61 6765 7208 0000 0072 0900 0000  .imager....r....
-00000890: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000008a0: 1000 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000008b0: 0000 730e 0000 0014 000c 0108 0210 010c  ..s.............
-000008c0: 0206 0212 03                             .....
+00000390: fa33 2f68 6f6d 652f 726f 6269 6e2f 636f  .3/home/robin/co
+000003a0: 6465 2f72 6f62 696e 6761 6d65 2f72 6f62  de/robingame/rob
+000003b0: 696e 6761 6d65 2f69 6e70 7574 2f65 7665  ingame/input/eve
+000003c0: 6e74 2e70 79da 0361 6464 1400 0000 7306  nt.py..add....s.
+000003d0: 0000 0008 0916 0110 017a 0e45 7665 6e74  .........z.Event
+000003e0: 5175 6575 652e 6164 6463 0100 0000 0000  Queue.addc......
+000003f0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000400: 0000 7310 0000 0074 006a 01a0 02a1 007c  ..s....t.j.....|
+00000410: 005f 0364 0153 0029 027a 7a0a 2020 2020  ._.d.S.).zz.    
+00000420: 2020 2020 5265 6164 2061 6c6c 2074 6865      Read all the
+00000430: 2065 7665 6e74 7320 6672 6f6d 2070 7967   events from pyg
+00000440: 616d 6527 7320 6576 656e 7420 7175 6575  ame's event queu
+00000450: 6520 696e 746f 2063 6c73 2e65 7665 6e74  e into cls.event
+00000460: 730a 2020 2020 2020 2020 2861 6c73 6f20  s.        (also 
+00000470: 636c 6561 7273 2070 7967 616d 6527 7320  clears pygame's 
+00000480: 6576 656e 7420 7175 6575 6529 0a20 2020  event queue).   
+00000490: 2020 2020 204e 2904 720c 0000 0072 0a00       N).r....r..
+000004a0: 0000 da03 6765 74da 0665 7665 6e74 7329  ....get..events)
+000004b0: 0172 0e00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+000004c0: 7210 0000 00da 0675 7064 6174 6521 0000  r......update!..
+000004d0: 0073 0200 0000 1006 7a11 4576 656e 7451  .s......z.EventQ
+000004e0: 7565 7565 2e75 7064 6174 6563 0100 0000  ueue.updatec....
+000004f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000500: 0b00 0000 7314 0000 0087 0066 0164 0164  ....s......f.d.d
+00000510: 0284 087c 006a 0044 0083 0153 0029 034e  ...|.j.D...S.).N
+00000520: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000530: 0006 0000 0013 0000 0073 2a00 0000 6700  .........s*...g.
+00000540: 7c00 5d11 8900 7400 8700 6601 6400 6401  |.]...t...f.d.d.
+00000550: 8408 8801 a001 a100 4400 8301 8301 7202  ........D.....r.
+00000560: 8800 9102 7102 5300 2902 6301 0000 0000  ....q.S.).c.....
+00000570: 0000 0000 0000 0003 0000 0005 0000 0033  ...............3
+00000580: 0000 0073 2400 0000 8100 7c00 5d0d 5c02  ...s$.....|.].\.
+00000590: 7d01 7d02 7400 8800 7c01 6400 8303 7c02  }.}.t...|.d...|.
+000005a0: 6b02 5600 0100 7102 6400 5300 2901 4e29  k.V...q.d.S.).N)
+000005b0: 01da 0767 6574 6174 7472 2903 da02 2e30  ...getattr)....0
+000005c0: da09 6174 7472 6962 7574 65da 0576 616c  ..attribute..val
+000005d0: 7565 a901 720a 0000 0072 0f00 0000 7210  ue..r....r....r.
+000005e0: 0000 00da 093c 6765 6e65 7870 723e 2e00  .....<genexpr>..
+000005f0: 0000 7304 0000 0002 8022 007a 2f45 7665  ..s......".z/Eve
+00000600: 6e74 5175 6575 652e 6669 6c74 6572 2e3c  ntQueue.filter.<
+00000610: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000620: 703e 2e3c 6765 6e65 7870 723e 2902 da03  p>.<genexpr>)...
+00000630: 616c 6cda 0569 7465 6d73 2901 7216 0000  all..items).r...
+00000640: 00a9 01da 066b 7761 7267 7372 1900 0000  .....kwargsr....
+00000650: 7210 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00000660: 3e2b 0000 0073 0c00 0000 0600 0202 1801  >+...s..........
+00000670: 02fd 0201 06ff 7a25 4576 656e 7451 7565  ......z%EventQue
+00000680: 7565 2e66 696c 7465 722e 3c6c 6f63 616c  ue.filter.<local
+00000690: 733e 2e3c 6c69 7374 636f 6d70 3e29 0172  s>.<listcomp>).r
+000006a0: 1300 0000 a902 720e 0000 0072 1e00 0000  ......r....r....
+000006b0: 720f 0000 0072 1d00 0000 7210 0000 00da  r....r....r.....
+000006c0: 0666 696c 7465 7229 0000 0073 0600 0000  .filter)...s....
+000006d0: 0a02 0402 06fe 7a11 4576 656e 7451 7565  ......z.EventQue
+000006e0: 7565 2e66 696c 7465 7263 0100 0000 0000  ue.filterc......
+000006f0: 0000 0000 0000 0200 0000 0800 0000 4b00  ..............K.
+00000700: 0000 732c 0000 007a 0b7c 006a 0064 0269  ..s,...z.|.j.d.i
+00000710: 007c 01a4 018e 0164 0119 0057 0053 0004  .|.....d...W.S..
+00000720: 0074 0179 1501 0001 0001 0059 0064 0053  .t.y.......Y.d.S
+00000730: 0077 0029 034e 7201 0000 0072 0f00 0000  .w.).Nr....r....
+00000740: 2902 7221 0000 00da 0a49 6e64 6578 4572  ).r!.....IndexEr
+00000750: 726f 7272 2000 0000 720f 0000 0072 0f00  rorr ...r....r..
+00000760: 0000 7210 0000 0072 1200 0000 3100 0000  ..r....r....1...
+00000770: 730a 0000 0002 0216 010c 0106 0102 ff7a  s..............z
+00000780: 0e45 7665 6e74 5175 6575 652e 6765 744e  .EventQueue.getN
+00000790: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000007a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000007b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+000007c0: 1300 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+000007d0: 6472 0500 0000 7206 0000 0072 1100 0000  dr....r....r....
+000007e0: 7214 0000 0072 2100 0000 7212 0000 0072  r....r!...r....r
+000007f0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00000800: 0000 0072 0900 0000 0c00 0000 7316 0000  ...r........s...
+00000810: 0008 0004 0104 0502 0218 0102 0c0a 0102  ................
+00000820: 070a 0102 070e 0172 0900 0000 290d da0b  .......r....)...
+00000830: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
+00000840: 7203 0000 0072 0400 0000 da06 7479 7069  r....r......typi
+00000850: 6e67 7205 0000 0072 0c00 0000 da0c 7079  ngr....r......py
+00000860: 6761 6d65 2e65 7665 6e74 7206 0000 0072  game.eventr....r
+00000870: 0700 0000 da0f 726f 6269 6e67 616d 652e  ......robingame.
+00000880: 696d 6167 6572 0800 0000 7209 0000 0072  imager....r....r
+00000890: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+000008a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000008b0: 0073 0e00 0000 1400 0c01 0802 1001 0c02  .s..............
+000008c0: 0602 1203                                ....
```

### Comparing `robingame-0.0.9/robingame/input/__pycache__/gamecube.cpython-310.pyc` & `robingame-0.1.0/robingame/input/__pycache__/gamecube.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Oct 31 15:13:45 2022 UTC, .py size: 13533 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 29e6 5f63 dd34 0000  o.......)._c.4..
+00000000: 6f0d 0d0a 0000 0000 88a3 6064 dd34 0000  o.........`d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 b602 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 5a04 6404 5a05 6405  m.Z...d.Z.d.Z.d.
 00000050: 5a06 6406 5a07 6407 5a08 6408 5a09 6409  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0a 640a 5a0b 640b 5a0c 640c 5a0d 640d  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a0e 640e 5a0f 640f 5a10 6410 5a11 6411  Z.d.Z.d.Z.d.Z.d.
@@ -79,836 +79,836 @@
 000004e0: 7574 2061 6e79 0a20 2020 2076 616c 7565  ut any.    value
 000004f0: 7320 6f75 7473 6964 6520 7468 6520 6f75  s outside the ou
 00000500: 7470 7574 2072 616e 6765 2e20 5769 6c6c  tput range. Will
 00000510: 2073 7469 6c6c 2061 6c6c 6f77 2069 6e70   still allow inp
 00000520: 7574 7320 6f75 7473 6964 6520 7468 6520  uts outside the 
 00000530: 696e 7075 7420 7261 6e67 652e 2902 da03  input range.)...
 00000540: 6d61 78da 036d 696e 290d da0b 696e 7075  max..min)...inpu
-00000550: 745f 7661 6c75 655a 0b69 6e70 7574 5f72  t_valueZ.input_r
-00000560: 616e 6765 5a0c 6f75 7470 7574 5f72 616e  angeZ.output_ran
-00000570: 6765 5a0c 6c69 6d69 745f 6f75 7470 7574  geZ.limit_output
-00000580: 5a09 696e 7075 745f 6d69 6e5a 0969 6e70  Z.input_minZ.inp
-00000590: 7574 5f6d 6178 5a0a 6f75 7470 7574 5f6d  ut_maxZ.output_m
-000005a0: 696e 5a0a 6f75 7470 7574 5f6d 6178 5a02  inZ.output_maxZ.
-000005b0: 6469 5a02 646f da08 6772 6164 6965 6e74  diZ.do..gradient
+00000550: 745f 7661 6c75 65da 0b69 6e70 7574 5f72  t_value..input_r
+00000560: 616e 6765 da0c 6f75 7470 7574 5f72 616e  ange..output_ran
+00000570: 6765 da0c 6c69 6d69 745f 6f75 7470 7574  ge..limit_output
+00000580: da09 696e 7075 745f 6d69 6eda 0969 6e70  ..input_min..inp
+00000590: 7574 5f6d 6178 da0a 6f75 7470 7574 5f6d  ut_max..output_m
+000005a0: 696e da0a 6f75 7470 7574 5f6d 6178 da02  in..output_max..
+000005b0: 6469 da02 646f da08 6772 6164 6965 6e74  di..do..gradient
 000005c0: da06 6f66 6673 6574 da0c 6f75 7470 7574  ..offset..output
-000005d0: 5f76 616c 7565 a900 721e 0000 00fa 372f  _value..r.....7/
-000005e0: 686f 6d65 2f62 696e 6e65 762f 636f 6465  home/binnev/code
-000005f0: 2f72 6f62 696e 6761 6d65 2f72 6f62 696e  /robingame/robin
-00000600: 6761 6d65 2f69 6e70 7574 2f67 616d 6563  game/input/gamec
-00000610: 7562 652e 7079 da0a 6c69 6e65 6172 5f6d  ube.py..linear_m
-00000620: 6170 2a00 0000 7316 0000 0008 0308 0108  ap*...s.........
-00000630: 0208 0108 010c 010c 0304 020a 010a 0104  ................
-00000640: 0272 2000 0000 6300 0000 0000 0000 0000  .r ...c.........
-00000650: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000660: be01 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000670: 6402 5a04 6403 5a05 6404 5a06 6405 6507  d.Z.d.Z.d.Z.d.e.
-00000680: 6602 6406 6407 8404 5a08 6408 6409 8400  f.d.d...Z.d.d...
-00000690: 5a09 640a 640b 8400 5a0a 640c 640d 8400  Z.d.d...Z.d.d...
-000006a0: 5a0b 640e 640f 8400 5a0c 650d 6410 6411  Z.d.d...Z.e.d.d.
-000006b0: 8400 8301 5a0e 650d 6412 6413 8400 8301  ....Z.e.d.d.....
-000006c0: 5a0f 650d 6414 6415 8400 8301 5a10 650d  Z.e.d.d.....Z.e.
-000006d0: 6416 6417 8400 8301 5a11 650d 6418 6419  d.d.....Z.e.d.d.
-000006e0: 8400 8301 5a12 650d 641a 641b 8400 8301  ....Z.e.d.d.....
-000006f0: 5a13 650d 641c 641d 8400 8301 5a14 650d  Z.e.d.d.....Z.e.
-00000700: 641e 641f 8400 8301 5a15 650d 6420 6421  d.d.....Z.e.d d!
-00000710: 8400 8301 5a16 650d 6422 6423 8400 8301  ....Z.e.d"d#....
-00000720: 5a17 650d 6424 6425 8400 8301 5a18 650d  Z.e.d$d%....Z.e.
-00000730: 6426 6427 8400 8301 5a19 650d 6428 6429  d&d'....Z.e.d(d)
-00000740: 8400 8301 5a1a 650d 642a 642b 8400 8301  ....Z.e.d*d+....
-00000750: 5a1b 650d 642c 642d 8400 8301 5a1c 650d  Z.e.d,d-....Z.e.
-00000760: 642e 642f 8400 8301 5a1d 650d 6430 6431  d.d/....Z.e.d0d1
-00000770: 8400 8301 5a1e 650d 6432 6433 8400 8301  ....Z.e.d2d3....
-00000780: 5a1f 650d 6434 6435 8400 8301 5a20 650d  Z.e.d4d5....Z e.
-00000790: 6436 6437 8400 8301 5a21 650d 6438 6439  d6d7....Z!e.d8d9
-000007a0: 8400 8301 5a22 650d 643a 643b 8400 8301  ....Z"e.d:d;....
-000007b0: 5a23 650d 643c 643d 8400 8301 5a24 650d  Z#e.d<d=....Z$e.
-000007c0: 643e 643f 8400 8301 5a25 650d 6440 6441  d>d?....Z%e.d@dA
-000007d0: 8400 8301 5a26 650d 6442 6443 8400 8301  ....Z&e.dBdC....
-000007e0: 5a27 650d 6444 6445 8400 8301 5a28 650d  Z'e.dDdE....Z(e.
-000007f0: 6446 6447 8400 8301 5a29 650d 6448 6449  dFdG....Z)e.dHdI
-00000800: 8400 8301 5a2a 650d 644a 644b 8400 8301  ....Z*e.dJdK....
-00000810: 5a2b 650d 644c 644d 8400 8301 5a2c 644e  Z+e.dLdM....Z,dN
-00000820: 5300 294f da18 4761 6d65 6375 6265 436f  S.)O..GamecubeCo
-00000830: 6e74 726f 6c6c 6572 5265 6164 6572 6148  ntrollerReaderaH
-00000840: 0200 0043 6c61 7373 2074 6f20 7265 6164  ...Class to read
-00000850: 2074 6865 2069 6e70 7574 7320 6f66 2061   the inputs of a
-00000860: 2047 616d 6543 7562 6520 636f 6e74 726f   GameCube contro
-00000870: 6c6c 6572 2070 6c75 6767 6564 2069 6e74  ller plugged int
-00000880: 6f20 7468 6520 4d61 7966 6c61 7368 2022  o the Mayflash "
-00000890: 4761 6d65 4375 6265 0a20 2020 2043 6f6e  GameCube.    Con
-000008a0: 7472 6f6c 6c65 7220 4164 6170 7465 7220  troller Adapter 
-000008b0: 666f 7220 5769 6920 5520 2620 5043 2055  for Wii U & PC U
-000008c0: 5342 220a 0a20 2020 2054 6869 7320 636c  SB"..    This cl
-000008d0: 6173 730a 2020 2020 2d20 7265 6164 7320  ass.    - reads 
-000008e0: 7468 6520 7661 6c75 6573 2066 726f 6d20  the values from 
-000008f0: 7468 6520 636f 6e74 726f 6c6c 6572 2773  the controller's
-00000900: 2062 7574 746f 6e73 2028 6269 6e61 7279   buttons (binary
-00000910: 2076 616c 7565 7329 2061 7865 7320 2861   values) axes (a
-00000920: 6e61 6c6f 6720 696e 7075 7473 2073 7563  nalog inputs suc
-00000930: 6820 6173 0a20 2020 2063 6f6e 7472 6f6c  h as.    control
-00000940: 2073 7469 636b 7320 616e 6420 7472 6967   sticks and trig
-00000950: 6765 7273 2920 616e 6420 6861 7473 2028  gers) and hats (
-00000960: 7468 6520 342d 7761 7920 4420 7061 6429  the 4-way D pad)
-00000970: 0a20 2020 202d 206d 6170 7320 7468 6520  .    - maps the 
-00000980: 7661 6c75 6573 206f 6620 7468 6520 696e  values of the in
-00000990: 7075 7473 2074 6f20 6120 302d 3120 7261  puts to a 0-1 ra
-000009a0: 6e67 6520 616e 6420 6578 706f 7365 7320  nge and exposes 
-000009b0: 7468 6573 6520 6173 206e 616d 6564 2070  these as named p
-000009c0: 726f 7065 7274 6965 7320 6966 2074 6865  roperties if the
-000009d0: 0a20 2020 2075 7365 7220 7761 6e74 7320  .    user wants 
-000009e0: 746f 2061 6363 6573 7320 6120 7369 6e67  to access a sing
-000009f0: 6c65 2076 616c 7565 2e0a 2020 2020 2d20  le value..    - 
-00000a00: 6578 706f 7365 7320 6120 2e67 6574 5f76  exposes a .get_v
-00000a10: 616c 7565 7328 2920 6d65 7468 6f64 2077  alues() method w
-00000a20: 6869 6368 2072 6574 7572 6e73 2061 2074  hich returns a t
-00000a30: 7570 6c65 206f 6620 616c 6c20 7468 6520  uple of all the 
-00000a40: 696e 7075 7473 2028 7369 6d69 6c61 7220  inputs (similar 
-00000a50: 746f 2068 6f77 0a20 2020 2070 7967 616d  to how.    pygam
-00000a60: 6520 6465 616c 7320 7769 7468 206b 6579  e deals with key
-00000a70: 626f 6172 6420 616e 6420 6d6f 7573 6520  board and mouse 
-00000a80: 696e 7075 742e 0a20 2020 2029 02e7 9a99  input..    )....
-00000a90: 9999 9999 b93f 67a4 703d 0ad7 a3e8 3f29  .....?g.p=....?)
-00000aa0: 0272 2200 0000 6771 3d0a d7a3 70e5 3f29  .r"...gq=...p.?)
-00000ab0: 0267 0000 0000 0000 e0bf 7203 0000 00da  .g........r.....
-00000ac0: 0b6a 6f79 7374 6963 6b5f 6964 6302 0000  .joystick_idc...
-00000ad0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000ae0: 0043 0000 0073 1c00 0000 7400 6a01 a002  .C...s....t.j...
-00000af0: 7c01 a101 7c00 5f01 7c00 6a01 a003 a100  |...|._.|.j.....
-00000b00: 0100 6400 5300 a901 4e29 04da 0670 7967  ..d.S...N)...pyg
-00000b10: 616d 65da 086a 6f79 7374 6963 6bda 084a  ame..joystick..J
-00000b20: 6f79 7374 6963 6bda 0469 6e69 7429 02da  oystick..init)..
-00000b30: 0473 656c 6672 2300 0000 721e 0000 0072  .selfr#...r....r
-00000b40: 1e00 0000 721f 0000 00da 085f 5f69 6e69  ....r......__ini
-00000b50: 745f 5f51 0000 0073 0400 0000 0e01 0e01  t__Q...s........
-00000b60: 7a21 4761 6d65 6375 6265 436f 6e74 726f  z!GamecubeContro
-00000b70: 6c6c 6572 5265 6164 6572 2e5f 5f69 6e69  llerReader.__ini
-00000b80: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000b90: 0100 0000 1600 0000 4300 0000 735c 0000  ........C...s\..
-00000ba0: 007c 006a 007c 006a 017c 006a 027c 006a  .|.j.|.j.|.j.|.j
-00000bb0: 037c 006a 047c 006a 057c 006a 067c 006a  .|.j.|.j.|.j.|.j
-00000bc0: 077c 006a 087c 006a 097c 006a 0a7c 006a  .|.j.|.j.|.j.|.j
-00000bd0: 0b7c 006a 0c7c 006a 0d7c 006a 0e7c 006a  .|.j.|.j.|.j.|.j
-00000be0: 0f7c 006a 107c 006a 117c 006a 127c 006a  .|.j.|.j.|.j.|.j
-00000bf0: 137c 006a 147c 006a 1566 1653 0029 017a  .|.j.|.j.f.S.).z
-00000c00: a147 6574 2074 6865 2063 7572 7265 6e74  .Get the current
-00000c10: 2073 7461 7465 206f 6620 616c 6c20 7468   state of all th
-00000c20: 6520 696e 7075 7473 2e20 5468 6973 2069  e inputs. This i
-00000c30: 7320 696e 7465 6e64 6564 2074 6f20 6265  s intended to be
-00000c40: 2065 7175 6976 616c 656e 7420 746f 0a20   equivalent to. 
-00000c50: 2020 2020 2020 2070 7967 616d 652e 6b65         pygame.ke
-00000c60: 792e 6765 745f 7072 6573 7365 6420 736f  y.get_pressed so
-00000c70: 2074 6861 7420 7468 6520 696e 7075 7473   that the inputs
-00000c80: 2063 616e 2062 6520 7072 6f63 6573 7365   can be processe
-00000c90: 6420 696e 2074 6865 2073 616d 6520 7761  d in the same wa
-00000ca0: 792e 2916 da01 41da 0142 da01 58da 0159  y.)...A..B..X..Y
-00000cb0: da01 5ada 014c da01 52da 0553 5441 5254  ..Z..L..R..START
-00000cc0: da04 4c45 4654 da05 5249 4748 54da 0255  ..LEFT..RIGHT..U
-00000cd0: 50da 0444 4f57 4eda 0643 5f4c 4546 54da  P..DOWN..C_LEFT.
-00000ce0: 0743 5f52 4947 4854 da04 435f 5550 da06  .C_RIGHT..C_UP..
-00000cf0: 435f 444f 574e da06 525f 4158 4953 da06  C_DOWN..R_AXIS..
-00000d00: 4c5f 4158 4953 da06 445f 4c45 4654 da07  L_AXIS..D_LEFT..
-00000d10: 445f 5249 4748 54da 0444 5f55 50da 0644  D_RIGHT..D_UP..D
-00000d20: 5f44 4f57 4ea9 0172 2900 0000 721e 0000  _DOWN..r)...r...
-00000d30: 0072 1e00 0000 721f 0000 00da 0a67 6574  .r....r......get
-00000d40: 5f76 616c 7565 7355 0000 0073 2e00 0000  _valuesU...s....
-00000d50: 0407 0401 0401 0401 0401 0401 0401 0401  ................
-00000d60: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-00000d70: 0401 0401 0401 0401 0401 0401 04ea 7a23  ..............z#
-00000d80: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
-00000d90: 6572 5265 6164 6572 2e67 6574 5f76 616c  erReader.get_val
-00000da0: 7565 7363 0200 0000 0000 0000 0000 0000  uesc............
-00000db0: 0200 0000 0400 0000 4300 0000 f30e 0000  ........C.......
-00000dc0: 0074 007c 017c 006a 0164 0183 0353 00a9  .t.|.|.j.d...S..
-00000dd0: 024e 2902 7201 0000 0072 0300 0000 2902  .N).r....r....).
-00000de0: 7220 0000 00da 1647 5245 595f 5354 4943  r .....GREY_STIC
-00000df0: 4b5f 494e 5055 545f 5241 4e47 45a9 0272  K_INPUT_RANGE..r
-00000e00: 2900 0000 721a 0000 0072 1e00 0000 721e  )...r....r....r.
-00000e10: 0000 0072 1f00 0000 da0e 6772 6579 5f73  ...r......grey_s
-00000e20: 7469 636b 5f6d 6170 7400 0000 f302 0000  tick_mapt.......
-00000e30: 000e 017a 2747 616d 6563 7562 6543 6f6e  ...z'GamecubeCon
-00000e40: 7472 6f6c 6c65 7252 6561 6465 722e 6772  trollerReader.gr
-00000e50: 6579 5f73 7469 636b 5f6d 6170 6302 0000  ey_stick_mapc...
-00000e60: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000e70: 0043 0000 0072 4300 0000 7244 0000 0029  .C...rC...rD...)
-00000e80: 0272 2000 0000 da18 5945 4c4c 4f57 5f53  .r .....YELLOW_S
-00000e90: 5449 434b 5f49 4e50 5554 5f52 414e 4745  TICK_INPUT_RANGE
-00000ea0: 7246 0000 0072 1e00 0000 721e 0000 0072  rF...r....r....r
-00000eb0: 1f00 0000 da10 7965 6c6c 6f77 5f73 7469  ......yellow_sti
-00000ec0: 636b 5f6d 6170 7700 0000 7248 0000 007a  ck_mapw...rH...z
-00000ed0: 2947 616d 6563 7562 6543 6f6e 7472 6f6c  )GamecubeControl
-00000ee0: 6c65 7252 6561 6465 722e 7965 6c6c 6f77  lerReader.yellow
-00000ef0: 5f73 7469 636b 5f6d 6170 6302 0000 0000  _stick_mapc.....
-00000f00: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000f10: 0000 0072 4300 0000 7244 0000 0029 0272  ...rC...rD...).r
-00000f20: 2000 0000 da13 5452 4947 4745 525f 494e   .....TRIGGER_IN
-00000f30: 5055 545f 5241 4e47 4572 4600 0000 721e  PUT_RANGErF...r.
-00000f40: 0000 0072 1e00 0000 721f 0000 00da 0b74  ...r....r......t
-00000f50: 7269 6767 6572 5f6d 6170 7a00 0000 7248  rigger_mapz...rH
-00000f60: 0000 007a 2447 616d 6563 7562 6543 6f6e  ...z$GamecubeCon
-00000f70: 7472 6f6c 6c65 7252 6561 6465 722e 7472  trollerReader.tr
-00000f80: 6967 6765 725f 6d61 7063 0100 0000 0000  igger_mapc......
-00000f90: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000fa0: 0000 f30c 0000 007c 006a 00a0 0164 01a1  .......|.j...d..
-00000fb0: 0153 00a9 024e 7201 0000 00a9 0272 2600  .S...Nr......r&.
-00000fc0: 0000 da08 6765 745f 6178 6973 7241 0000  ....get_axisrA..
-00000fd0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000fe0: da12 5f47 5245 595f 5354 4943 4b5f 585f  .._GREY_STICK_X_
-00000ff0: 4158 4953 8100 0000 f302 0000 000c 027a  AXIS...........z
-00001000: 2b47 616d 6563 7562 6543 6f6e 7472 6f6c  +GamecubeControl
-00001010: 6c65 7252 6561 6465 722e 5f47 5245 595f  lerReader._GREY_
-00001020: 5354 4943 4b5f 585f 4158 4953 6301 0000  STICK_X_AXISc...
-00001030: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001040: 0043 0000 0072 4d00 0000 a902 4e72 0300  .C...rM.....Nr..
-00001050: 0000 724f 0000 0072 4100 0000 721e 0000  ..rO...rA...r...
-00001060: 0072 1e00 0000 721f 0000 00da 125f 4752  .r....r......_GR
-00001070: 4559 5f53 5449 434b 5f59 5f41 5849 5385  EY_STICK_Y_AXIS.
-00001080: 0000 0072 5200 0000 7a2b 4761 6d65 6375  ...rR...z+Gamecu
-00001090: 6265 436f 6e74 726f 6c6c 6572 5265 6164  beControllerRead
-000010a0: 6572 2e5f 4752 4559 5f53 5449 434b 5f59  er._GREY_STICK_Y
-000010b0: 5f41 5849 5363 0100 0000 0000 0000 0000  _AXISc..........
-000010c0: 0000 0100 0000 0300 0000 4300 0000 724d  ..........C...rM
-000010d0: 0000 00a9 024e 7207 0000 0072 4f00 0000  .....Nr....rO...
-000010e0: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
-000010f0: 1f00 0000 da14 5f59 454c 4c4f 575f 5354  ......_YELLOW_ST
-00001100: 4943 4b5f 585f 4158 4953 8900 0000 7252  ICK_X_AXIS....rR
-00001110: 0000 007a 2d47 616d 6563 7562 6543 6f6e  ...z-GamecubeCon
-00001120: 7472 6f6c 6c65 7252 6561 6465 722e 5f59  trollerReader._Y
-00001130: 454c 4c4f 575f 5354 4943 4b5f 585f 4158  ELLOW_STICK_X_AX
-00001140: 4953 6301 0000 0000 0000 0000 0000 0001  ISc.............
-00001150: 0000 0003 0000 0043 0000 0072 4d00 0000  .......C...rM...
-00001160: a902 4e72 0400 0000 724f 0000 0072 4100  ..Nr....rO...rA.
-00001170: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00001180: 00da 145f 5945 4c4c 4f57 5f53 5449 434b  ..._YELLOW_STICK
-00001190: 5f59 5f41 5849 538d 0000 0072 5200 0000  _Y_AXIS....rR...
-000011a0: 7a2d 4761 6d65 6375 6265 436f 6e74 726f  z-GamecubeContro
-000011b0: 6c6c 6572 5265 6164 6572 2e5f 5945 4c4c  llerReader._YELL
-000011c0: 4f57 5f53 5449 434b 5f59 5f41 5849 5363  OW_STICK_Y_AXISc
-000011d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000011e0: 0300 0000 4300 0000 724d 0000 00a9 024e  ....C...rM.....N
-000011f0: 7205 0000 0072 4f00 0000 7241 0000 0072  r....rO...rA...r
-00001200: 1e00 0000 721e 0000 0072 1f00 0000 da0f  ....r....r......
-00001210: 5f4c 5f54 5249 4747 4552 5f41 5849 5391  _L_TRIGGER_AXIS.
-00001220: 0000 0072 5200 0000 7a28 4761 6d65 6375  ...rR...z(Gamecu
-00001230: 6265 436f 6e74 726f 6c6c 6572 5265 6164  beControllerRead
-00001240: 6572 2e5f 4c5f 5452 4947 4745 525f 4158  er._L_TRIGGER_AX
-00001250: 4953 6301 0000 0000 0000 0000 0000 0001  ISc.............
-00001260: 0000 0003 0000 0043 0000 0072 4d00 0000  .......C...rM...
-00001270: a902 4e72 0600 0000 724f 0000 0072 4100  ..Nr....rO...rA.
-00001280: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00001290: 00da 0f5f 525f 5452 4947 4745 525f 4158  ..._R_TRIGGER_AX
-000012a0: 4953 9500 0000 7252 0000 007a 2847 616d  IS....rR...z(Gam
-000012b0: 6563 7562 6543 6f6e 7472 6f6c 6c65 7252  ecubeControllerR
-000012c0: 6561 6465 722e 5f52 5f54 5249 4747 4552  eader._R_TRIGGER
-000012d0: 5f41 5849 5363 0100 0000 0000 0000 0000  _AXISc..........
-000012e0: 0000 0100 0000 0300 0000 4300 0000 f30e  ..........C.....
-000012f0: 0000 007c 00a0 007c 006a 010b 00a1 0153  ...|...|.j.....S
-00001300: 0072 2400 0000 a902 7247 0000 0072 5100  .r$.....rG...rQ.
-00001310: 0000 7241 0000 0072 1e00 0000 721e 0000  ..rA...r....r...
-00001320: 0072 1f00 0000 7233 0000 009b 0000 00f3  .r....r3........
-00001330: 0200 0000 0e02 7a1d 4761 6d65 6375 6265  ......z.Gamecube
-00001340: 436f 6e74 726f 6c6c 6572 5265 6164 6572  ControllerReader
-00001350: 2e4c 4546 5463 0100 0000 0000 0000 0000  .LEFTc..........
-00001360: 0000 0100 0000 0300 0000 4300 0000 f30c  ..........C.....
-00001370: 0000 007c 00a0 007c 006a 01a1 0153 0072  ...|...|.j...S.r
-00001380: 2400 0000 725e 0000 0072 4100 0000 721e  $...r^...rA...r.
-00001390: 0000 0072 1e00 0000 721f 0000 0072 3400  ...r....r....r4.
-000013a0: 0000 9f00 0000 7252 0000 007a 1e47 616d  ......rR...z.Gam
-000013b0: 6563 7562 6543 6f6e 7472 6f6c 6c65 7252  ecubeControllerR
-000013c0: 6561 6465 722e 5249 4748 5463 0100 0000  eader.RIGHTc....
-000013d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000013e0: 4300 0000 725d 0000 0072 2400 0000 a902  C...r]...r$.....
-000013f0: 7247 0000 0072 5400 0000 7241 0000 0072  rG...rT...rA...r
-00001400: 1e00 0000 721e 0000 0072 1f00 0000 7235  ....r....r....r5
-00001410: 0000 00a3 0000 0072 5f00 0000 7a1b 4761  .......r_...z.Ga
-00001420: 6d65 6375 6265 436f 6e74 726f 6c6c 6572  mecubeController
-00001430: 5265 6164 6572 2e55 5063 0100 0000 0000  Reader.UPc......
-00001440: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001450: 0000 7260 0000 0072 2400 0000 7261 0000  ..r`...r$...ra..
-00001460: 0072 4100 0000 721e 0000 0072 1e00 0000  .rA...r....r....
-00001470: 721f 0000 0072 3600 0000 a700 0000 7252  r....r6.......rR
-00001480: 0000 007a 1d47 616d 6563 7562 6543 6f6e  ...z.GamecubeCon
-00001490: 7472 6f6c 6c65 7252 6561 6465 722e 444f  trollerReader.DO
-000014a0: 574e 6301 0000 0000 0000 0000 0000 0001  WNc.............
-000014b0: 0000 0003 0000 0043 0000 0072 5d00 0000  .......C...r]...
-000014c0: 7224 0000 00a9 0272 4a00 0000 7256 0000  r$.....rJ...rV..
-000014d0: 0072 4100 0000 721e 0000 0072 1e00 0000  .rA...r....r....
-000014e0: 721f 0000 0072 3700 0000 ab00 0000 725f  r....r7.......r_
-000014f0: 0000 007a 1f47 616d 6563 7562 6543 6f6e  ...z.GamecubeCon
-00001500: 7472 6f6c 6c65 7252 6561 6465 722e 435f  trollerReader.C_
-00001510: 4c45 4654 6301 0000 0000 0000 0000 0000  LEFTc...........
-00001520: 0001 0000 0003 0000 0043 0000 0072 6000  .........C...r`.
-00001530: 0000 7224 0000 0072 6200 0000 7241 0000  ..r$...rb...rA..
-00001540: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001550: 7238 0000 00af 0000 0072 5200 0000 7a20  r8.......rR...z 
-00001560: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
-00001570: 6572 5265 6164 6572 2e43 5f52 4947 4854  erReader.C_RIGHT
-00001580: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001590: 0003 0000 0043 0000 0072 5d00 0000 7224  .....C...r]...r$
-000015a0: 0000 00a9 0272 4a00 0000 7258 0000 0072  .....rJ...rX...r
-000015b0: 4100 0000 721e 0000 0072 1e00 0000 721f  A...r....r....r.
-000015c0: 0000 0072 3900 0000 b300 0000 725f 0000  ...r9.......r_..
-000015d0: 007a 1d47 616d 6563 7562 6543 6f6e 7472  .z.GamecubeContr
-000015e0: 6f6c 6c65 7252 6561 6465 722e 435f 5550  ollerReader.C_UP
-000015f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001600: 0003 0000 0043 0000 0072 6000 0000 7224  .....C...r`...r$
-00001610: 0000 0072 6300 0000 7241 0000 0072 1e00  ...rc...rA...r..
-00001620: 0000 721e 0000 0072 1f00 0000 723a 0000  ..r....r....r:..
-00001630: 00b7 0000 0072 5200 0000 7a1f 4761 6d65  .....rR...z.Game
-00001640: 6375 6265 436f 6e74 726f 6c6c 6572 5265  cubeControllerRe
-00001650: 6164 6572 2e43 5f44 4f57 4e63 0100 0000  ader.C_DOWNc....
-00001660: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001670: 4300 0000 7260 0000 0072 2400 0000 2902  C...r`...r$...).
-00001680: 724c 0000 0072 5c00 0000 7241 0000 0072  rL...r\...rA...r
-00001690: 1e00 0000 721e 0000 0072 1f00 0000 723b  ....r....r....r;
-000016a0: 0000 00bb 0000 0072 5200 0000 7a1f 4761  .......rR...z.Ga
-000016b0: 6d65 6375 6265 436f 6e74 726f 6c6c 6572  mecubeController
-000016c0: 5265 6164 6572 2e52 5f41 5849 5363 0100  Reader.R_AXISc..
-000016d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000016e0: 0000 4300 0000 7260 0000 0072 2400 0000  ..C...r`...r$...
-000016f0: 2902 724c 0000 0072 5a00 0000 7241 0000  ).rL...rZ...rA..
-00001700: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001710: 723c 0000 00bf 0000 0072 5200 0000 7a1f  r<.......rR...z.
-00001720: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
-00001730: 6572 5265 6164 6572 2e4c 5f41 5849 5363  erReader.L_AXISc
-00001740: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001750: 0300 0000 4300 0000 724d 0000 0072 4e00  ....C...rM...rN.
-00001760: 0000 2902 7226 0000 00da 0767 6574 5f68  ..).r&.....get_h
-00001770: 6174 7241 0000 0072 1e00 0000 721e 0000  atrA...r....r...
-00001780: 0072 1f00 0000 da06 5f44 5f50 4144 c700  .r......_D_PAD..
-00001790: 0000 7252 0000 007a 1f47 616d 6563 7562  ..rR...z.Gamecub
-000017a0: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
-000017b0: 722e 5f44 5f50 4144 6301 0000 0000 0000  r._D_PADc.......
-000017c0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-000017d0: 00f3 0a00 0000 7c00 6a00 6401 1900 5300  ......|.j.d...S.
-000017e0: 724e 0000 00a9 0172 6500 0000 7241 0000  rN.....re...rA..
-000017f0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001800: da08 5f44 5f50 4144 5f58 cb00 0000 f302  .._D_PAD_X......
-00001810: 0000 000a 027a 2147 616d 6563 7562 6543  .....z!GamecubeC
-00001820: 6f6e 7472 6f6c 6c65 7252 6561 6465 722e  ontrollerReader.
-00001830: 5f44 5f50 4144 5f58 6301 0000 0000 0000  _D_PAD_Xc.......
-00001840: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001850: 0072 6600 0000 7253 0000 0072 6700 0000  .rf...rS...rg...
-00001860: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
-00001870: 1f00 0000 da08 5f44 5f50 4144 5f59 cf00  ......_D_PAD_Y..
-00001880: 0000 7269 0000 007a 2147 616d 6563 7562  ..ri...z!Gamecub
-00001890: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
-000018a0: 722e 5f44 5f50 4144 5f59 6301 0000 0000  r._D_PAD_Yc.....
-000018b0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-000018c0: 0000 00f3 0e00 0000 7400 7c00 6a01 6401  ........t.|.j.d.
-000018d0: 6b00 8301 5300 724e 0000 00a9 02da 0369  k...S.rN.......i
-000018e0: 6e74 7268 0000 0072 4100 0000 721e 0000  ntrh...rA...r...
-000018f0: 0072 1e00 0000 721f 0000 0072 3d00 0000  .r....r....r=...
-00001900: d500 0000 725f 0000 007a 1f47 616d 6563  ....r_...z.Gamec
-00001910: 7562 6543 6f6e 7472 6f6c 6c65 7252 6561  ubeControllerRea
-00001920: 6465 722e 445f 4c45 4654 6301 0000 0000  der.D_LEFTc.....
-00001930: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00001940: 0000 00f3 0e00 0000 7400 7c00 6a01 6401  ........t.|.j.d.
-00001950: 6b04 8301 5300 724e 0000 0072 6c00 0000  k...S.rN...rl...
-00001960: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
-00001970: 1f00 0000 723e 0000 00d9 0000 0072 5f00  ....r>.......r_.
-00001980: 0000 7a20 4761 6d65 6375 6265 436f 6e74  ..z GamecubeCont
-00001990: 726f 6c6c 6572 5265 6164 6572 2e44 5f52  rollerReader.D_R
-000019a0: 4947 4854 6301 0000 0000 0000 0000 0000  IGHTc...........
-000019b0: 0001 0000 0003 0000 0043 0000 0072 6e00  .........C...rn.
-000019c0: 0000 724e 0000 00a9 0272 6d00 0000 726a  ..rN.....rm...rj
-000019d0: 0000 0072 4100 0000 721e 0000 0072 1e00  ...rA...r....r..
-000019e0: 0000 721f 0000 0072 3f00 0000 dd00 0000  ..r....r?.......
-000019f0: 725f 0000 007a 1d47 616d 6563 7562 6543  r_...z.GamecubeC
-00001a00: 6f6e 7472 6f6c 6c65 7252 6561 6465 722e  ontrollerReader.
-00001a10: 445f 5550 6301 0000 0000 0000 0000 0000  D_UPc...........
-00001a20: 0001 0000 0003 0000 0043 0000 0072 6b00  .........C...rk.
-00001a30: 0000 724e 0000 0072 6f00 0000 7241 0000  ..rN...ro...rA..
-00001a40: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001a50: 7240 0000 00e1 0000 0072 5f00 0000 7a1f  r@.......r_...z.
-00001a60: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
-00001a70: 6572 5265 6164 6572 2e44 5f44 4f57 4e63  erReader.D_DOWNc
-00001a80: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001a90: 0300 0000 4300 0000 724d 0000 0072 4e00  ....C...rM...rN.
-00001aa0: 0000 a902 7226 0000 00da 0a67 6574 5f62  ....r&.....get_b
-00001ab0: 7574 746f 6e72 4100 0000 721e 0000 0072  uttonrA...r....r
-00001ac0: 1e00 0000 721f 0000 0072 2d00 0000 e900  ....r....r-.....
-00001ad0: 0000 7252 0000 007a 1a47 616d 6563 7562  ..rR...z.Gamecub
-00001ae0: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
-00001af0: 722e 5863 0100 0000 0000 0000 0000 0000  r.Xc............
-00001b00: 0100 0000 0300 0000 4300 0000 724d 0000  ........C...rM..
-00001b10: 0072 5300 0000 7270 0000 0072 4100 0000  .rS...rp...rA...
-00001b20: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00001b30: 2b00 0000 ed00 0000 7252 0000 007a 1a47  +.......rR...z.G
-00001b40: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
-00001b50: 7252 6561 6465 722e 4163 0100 0000 0000  rReader.Ac......
-00001b60: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001b70: 0000 724d 0000 0072 5700 0000 7270 0000  ..rM...rW...rp..
-00001b80: 0072 4100 0000 721e 0000 0072 1e00 0000  .rA...r....r....
-00001b90: 721f 0000 0072 2c00 0000 f100 0000 7252  r....r,.......rR
-00001ba0: 0000 007a 1a47 616d 6563 7562 6543 6f6e  ...z.GamecubeCon
-00001bb0: 7472 6f6c 6c65 7252 6561 6465 722e 4263  trollerReader.Bc
-00001bc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001bd0: 0300 0000 4300 0000 724d 0000 0072 5900  ....C...rM...rY.
-00001be0: 0000 7270 0000 0072 4100 0000 721e 0000  ..rp...rA...r...
-00001bf0: 0072 1e00 0000 721f 0000 0072 2e00 0000  .r....r....r....
-00001c00: f500 0000 7252 0000 007a 1a47 616d 6563  ....rR...z.Gamec
-00001c10: 7562 6543 6f6e 7472 6f6c 6c65 7252 6561  ubeControllerRea
-00001c20: 6465 722e 5963 0100 0000 0000 0000 0000  der.Yc..........
-00001c30: 0000 0100 0000 0300 0000 4300 0000 724d  ..........C...rM
-00001c40: 0000 0072 5b00 0000 7270 0000 0072 4100  ...r[...rp...rA.
-00001c50: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00001c60: 0072 3000 0000 f900 0000 7252 0000 007a  .r0.......rR...z
-00001c70: 1a47 616d 6563 7562 6543 6f6e 7472 6f6c  .GamecubeControl
-00001c80: 6c65 7252 6561 6465 722e 4c63 0100 0000  lerReader.Lc....
-00001c90: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001ca0: 4300 0000 724d 0000 0072 5500 0000 7270  C...rM...rU...rp
-00001cb0: 0000 0072 4100 0000 721e 0000 0072 1e00  ...rA...r....r..
-00001cc0: 0000 721f 0000 0072 3100 0000 fd00 0000  ..r....r1.......
-00001cd0: 7252 0000 007a 1a47 616d 6563 7562 6543  rR...z.GamecubeC
-00001ce0: 6f6e 7472 6f6c 6c65 7252 6561 6465 722e  ontrollerReader.
-00001cf0: 5263 0100 0000 0000 0000 0000 0000 0100  Rc..............
-00001d00: 0000 0300 0000 4300 0000 724d 0000 0029  ......C...rM...)
-00001d10: 024e 7209 0000 0072 7000 0000 7241 0000  .Nr....rp...rA..
-00001d20: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001d30: 722f 0000 0001 0100 0072 5200 0000 7a1a  r/.......rR...z.
-00001d40: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
-00001d50: 6572 5265 6164 6572 2e5a 6301 0000 0000  erReader.Zc.....
-00001d60: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00001d70: 0000 0072 4d00 0000 2902 4e72 0b00 0000  ...rM...).Nr....
-00001d80: 7270 0000 0072 4100 0000 721e 0000 0072  rp...rA...r....r
-00001d90: 1e00 0000 721f 0000 0072 3200 0000 0501  ....r....r2.....
-00001da0: 0000 7252 0000 007a 1e47 616d 6563 7562  ..rR...z.Gamecub
-00001db0: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
-00001dc0: 722e 5354 4152 544e 292d da08 5f5f 6e61  r.STARTN)-..__na
-00001dd0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001de0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00001df0: 5f5f 646f 635f 5f72 4500 0000 7249 0000  __doc__rE...rI..
-00001e00: 0072 4b00 0000 726d 0000 0072 2a00 0000  .rK...rm...r*...
-00001e10: 7242 0000 0072 4700 0000 724a 0000 0072  rB...rG...rJ...r
-00001e20: 4c00 0000 da08 7072 6f70 6572 7479 7251  L.....propertyrQ
-00001e30: 0000 0072 5400 0000 7256 0000 0072 5800  ...rT...rV...rX.
-00001e40: 0000 725a 0000 0072 5c00 0000 7233 0000  ..rZ...r\...r3..
-00001e50: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
-00001e60: 7237 0000 0072 3800 0000 7239 0000 0072  r7...r8...r9...r
-00001e70: 3a00 0000 723b 0000 0072 3c00 0000 7265  :...r;...r<...re
-00001e80: 0000 0072 6800 0000 726a 0000 0072 3d00  ...rh...rj...r=.
-00001e90: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
-00001ea0: 0072 2d00 0000 722b 0000 0072 2c00 0000  .r-...r+...r,...
-00001eb0: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00001ec0: 2f00 0000 7232 0000 0072 1e00 0000 721e  /...r2...r....r.
-00001ed0: 0000 0072 1e00 0000 721f 0000 0072 2100  ...r....r....r!.
-00001ee0: 0000 3f00 0000 7390 0000 0008 0004 0104  ..?...s.........
-00001ef0: 0d04 0104 010e 0208 0408 1f08 0308 0302  ................
-00001f00: 070a 0102 030a 0102 030a 0102 030a 0102  ................
-00001f10: 030a 0102 030a 0102 050a 0102 030a 0102  ................
-00001f20: 030a 0102 030a 0102 030a 0102 030a 0102  ................
-00001f30: 030a 0102 030a 0102 030a 0102 030a 0102  ................
-00001f40: 070a 0102 030a 0102 030a 0102 050a 0102  ................
-00001f50: 030a 0102 030a 0102 030a 0102 070a 0102  ................
-00001f60: 030a 0102 030a 0102 030a 0102 030a 0102  ................
-00001f70: 030a 0102 030a 0102 030e 0172 2100 0000  ...........r!...
-00001f80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001f90: 0005 0000 0040 0000 0073 7800 0000 6500  .....@...sx...e.
-00001fa0: 5a01 6400 5a02 6418 6402 6503 6403 6504  Z.d.Z.d.d.e.d.e.
-00001fb0: 6604 6404 6405 8405 5a05 6506 6406 6407  f.d.d...Z.e.d.d.
-00001fc0: 8400 8301 5a07 6506 6408 6409 8400 8301  ....Z.e.d.d.....
-00001fd0: 5a08 6506 640a 640b 8400 8301 5a09 6506  Z.e.d.d.....Z.e.
-00001fe0: 640c 640d 8400 8301 5a0a 640e 640f 8400  d.d.....Z.d.d...
-00001ff0: 5a0b 6410 6411 8400 5a0c 6412 6413 8400  Z.d.d...Z.d.d...
-00002000: 5a0d 6414 6415 8400 5a0e 6416 6417 8400  Z.d.d...Z.d.d...
-00002010: 5a0f 6401 5300 2919 da0b 4275 7474 6f6e  Z.d.S.)...Button
-00002020: 496e 7075 744e da02 6964 da06 7061 7265  InputN..id..pare
-00002030: 6e74 6303 0000 0000 0000 0000 0000 0003  ntc.............
-00002040: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-00002050: 7c01 7c00 5f00 7c02 7c00 5f01 6401 5300  |.|._.|.|._.d.S.
-00002060: 2902 61e6 0100 000a 2020 2020 2020 2020  ).a.....        
-00002070: 436c 6173 7320 746f 2064 6573 6372 6962  Class to describ
-00002080: 6520 6120 7369 6e67 6c65 2069 6e70 7574  e a single input
-00002090: 2063 6861 6e6e 656c 206f 6e20 6120 6a6f   channel on a jo
-000020a0: 7973 7469 636b 2f63 6f6e 7472 6f6c 6c65  ystick/controlle
-000020b0: 7220 2d2d 2065 2e67 2e20 7468 6520 2241  r -- e.g. the "A
-000020c0: 2220 6275 7474 6f6e 0a20 2020 2020 2020  " button.       
-000020d0: 206f 6e20 6120 6761 6d65 6375 6265 2063   on a gamecube c
-000020e0: 6f6e 7472 6f6c 6c65 722e 2049 6d70 6c65  ontroller. Imple
-000020f0: 6d65 6e74 7320 6d65 7468 6f64 7320 7768  ments methods wh
-00002100: 6963 6820 6368 6563 6b20 7769 7468 2074  ich check with t
-00002110: 6865 2070 6172 656e 7420 696e 7075 7420  he parent input 
-00002120: 6465 7669 6365 0a20 2020 2020 2020 2077  device.        w
-00002130: 6865 7468 6572 2074 6869 7320 6275 7474  hether this butt
-00002140: 6f6e 2069 7320 7072 6573 7365 642c 2072  on is pressed, r
-00002150: 656c 6561 7365 642c 2065 7463 2e20 5468  eleased, etc. Th
-00002160: 6973 2061 6c6c 6f77 7320 666f 7220 7468  is allows for th
-00002170: 6520 6d6f 7265 2070 6c65 6173 616e 7420  e more pleasant 
-00002180: 7368 6f72 7468 616e 643a 0a20 2020 2020  shorthand:.     
-00002190: 2020 2060 636f 6e74 726f 6c6c 6572 2e61     `controller.a
-000021a0: 5f62 7574 746f 6e2e 6973 5f70 7265 7373  _button.is_press
-000021b0: 6564 6020 696e 7374 6561 6420 6f66 2060  ed` instead of `
-000021c0: 636f 6e74 726f 6c6c 6572 2e69 735f 7072  controller.is_pr
-000021d0: 6573 7365 6428 636f 6e74 726f 6c6c 6572  essed(controller
-000021e0: 2e61 5f62 7574 746f 6e29 600a 0a20 2020  .a_button)`..   
-000021f0: 2020 2020 203a 7061 7261 6d20 696e 7420       :param int 
-00002200: 6964 3a20 696e 6465 7820 6f66 2074 6869  id: index of thi
-00002210: 7320 696e 7075 7420 6368 616e 6e65 6c20  s input channel 
-00002220: 696e 2074 6865 2063 6f6e 7472 6f6c 6c65  in the controlle
-00002230: 722e 6765 745f 7661 6c75 6573 2829 2074  r.get_values() t
-00002240: 7570 6c65 0a20 2020 2020 2020 204e 2902  uple.        N).
-00002250: 7278 0000 0072 7900 0000 2903 7229 0000  rx...ry...).r)..
-00002260: 0072 7800 0000 7279 0000 0072 1e00 0000  .rx...ry...r....
-00002270: 721e 0000 0072 1f00 0000 722a 0000 000b  r....r....r*....
-00002280: 0100 0073 0400 0000 0609 0a01 7a14 4275  ...s........z.Bu
-00002290: 7474 6f6e 496e 7075 742e 5f5f 696e 6974  ttonInput.__init
-000022a0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-000022b0: 0000 0003 0000 0043 0000 00f3 0e00 0000  .......C........
-000022c0: 7c00 6a00 a001 7c00 6a02 a101 5300 7224  |.j...|.j...S.r$
-000022d0: 0000 0029 0372 7900 0000 da07 6973 5f64  ...).ry.....is_d
-000022e0: 6f77 6e72 7800 0000 7241 0000 0072 1e00  ownrx...rA...r..
-000022f0: 0000 721e 0000 0072 1f00 0000 727b 0000  ..r....r....r{..
-00002300: 0017 0100 0072 5f00 0000 7a13 4275 7474  .....r_...z.Butt
-00002310: 6f6e 496e 7075 742e 6973 5f64 6f77 6e63  onInput.is_downc
-00002320: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002330: 0300 0000 4300 0000 727a 0000 0072 2400  ....C...rz...r$.
-00002340: 0000 2903 7279 0000 00da 0a69 735f 7072  ..).ry.....is_pr
-00002350: 6573 7365 6472 7800 0000 7241 0000 0072  essedrx...rA...r
-00002360: 1e00 0000 721e 0000 0072 1f00 0000 727c  ....r....r....r|
-00002370: 0000 001b 0100 0072 5f00 0000 7a16 4275  .......r_...z.Bu
-00002380: 7474 6f6e 496e 7075 742e 6973 5f70 7265  ttonInput.is_pre
-00002390: 7373 6564 6301 0000 0000 0000 0000 0000  ssedc...........
-000023a0: 0001 0000 0003 0000 0043 0000 0072 7a00  .........C...rz.
-000023b0: 0000 7224 0000 0029 0372 7900 0000 da0b  ..r$...).ry.....
-000023c0: 6973 5f72 656c 6561 7365 6472 7800 0000  is_releasedrx...
-000023d0: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
-000023e0: 1f00 0000 727d 0000 001f 0100 0072 5f00  ....r}.......r_.
-000023f0: 0000 7a17 4275 7474 6f6e 496e 7075 742e  ..z.ButtonInput.
-00002400: 6973 5f72 656c 6561 7365 6463 0100 0000  is_releasedc....
-00002410: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00002420: 4300 0000 7306 0000 007c 006a 0053 0029  C...s....|.j.S.)
-00002430: 017a 8c44 6f65 7320 7468 6520 7361 6d65  .z.Does the same
-00002440: 2074 6869 6e67 2061 7320 6973 5f64 6f77   thing as is_dow
-00002450: 6e20 6275 7420 6d61 6b65 7320 736f 6d65  n but makes some
-00002460: 2070 6172 7473 206f 6620 7468 6520 636f   parts of the co
-00002470: 6465 206d 6f72 6520 7265 6164 6162 6c65  de more readable
-00002480: 2c0a 2020 2020 2020 2020 6573 7065 6369  ,.        especi
-00002490: 616c 6c79 2066 6f72 2061 6e61 6c6f 6720  ally for analog 
-000024a0: 696e 7075 7473 2074 6861 7420 6361 6e20  inputs that can 
-000024b0: 6265 2062 6574 7765 656e 2030 2d31 2e29  be between 0-1.)
-000024c0: 0172 7b00 0000 7241 0000 0072 1e00 0000  .r{...rA...r....
-000024d0: 721e 0000 0072 1f00 0000 da05 7661 6c75  r....r......valu
-000024e0: 6523 0100 0073 0200 0000 0604 7a11 4275  e#...s......z.Bu
-000024f0: 7474 6f6e 496e 7075 742e 7661 6c75 6563  ttonInput.valuec
-00002500: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002510: 0400 0000 4300 0000 f310 0000 007c 006a  ....C........|.j
-00002520: 00a0 017c 006a 027c 01a1 0253 0072 2400  ...|.j.|...S.r$.
-00002530: 0000 2903 7279 0000 00da 1062 7566 6665  ..).ry.....buffe
-00002540: 7265 645f 7072 6573 7365 7372 7800 0000  red_pressesrx...
-00002550: a902 7229 0000 00da 0d62 7566 6665 725f  ..r).....buffer_
-00002560: 6c65 6e67 7468 721e 0000 0072 1e00 0000  lengthr....r....
-00002570: 721f 0000 0072 8000 0000 2901 0000 f302  r....r....).....
-00002580: 0000 0010 017a 1c42 7574 746f 6e49 6e70  .....z.ButtonInp
-00002590: 7574 2e62 7566 6665 7265 645f 7072 6573  ut.buffered_pres
-000025a0: 7365 7363 0200 0000 0000 0000 0000 0000  sesc............
-000025b0: 0200 0000 0400 0000 4300 0000 727f 0000  ........C...r...
-000025c0: 0072 2400 0000 2903 7279 0000 00da 1162  .r$...).ry.....b
-000025d0: 7566 6665 7265 645f 7265 6c65 6173 6573  uffered_releases
-000025e0: 7278 0000 0072 8100 0000 721e 0000 0072  rx...r....r....r
-000025f0: 1e00 0000 721f 0000 0072 8400 0000 2c01  ....r....r....,.
-00002600: 0000 7283 0000 007a 1d42 7574 746f 6e49  ..r....z.ButtonI
-00002610: 6e70 7574 2e62 7566 6665 7265 645f 7265  nput.buffered_re
-00002620: 6c65 6173 6573 6302 0000 0000 0000 0000  leasesc.........
-00002630: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00002640: 1c00 0000 7c00 6a00 7401 7c01 7402 8302  ....|.j.t.|.t...
-00002650: 720b 7c01 6a00 1800 5300 7c01 1800 5300  r.|.j...S.|...S.
-00002660: 7224 0000 00a9 0372 7e00 0000 da0a 6973  r$.....r~.....is
-00002670: 696e 7374 616e 6365 7277 0000 00a9 0272  instancerw.....r
-00002680: 2900 0000 da05 6f74 6865 7272 1e00 0000  ).....otherr....
-00002690: 721e 0000 0072 1f00 0000 da07 5f5f 7375  r....r......__su
-000026a0: 625f 5f2f 0100 00f3 0200 0000 1c01 7a13  b__/..........z.
-000026b0: 4275 7474 6f6e 496e 7075 742e 5f5f 7375  ButtonInput.__su
-000026c0: 625f 5f63 0200 0000 0000 0000 0000 0000  b__c............
-000026d0: 0200 0000 0400 0000 4300 0000 731c 0000  ........C...s...
-000026e0: 007c 006a 0074 017c 0174 0283 0272 0b7c  .|.j.t.|.t...r.|
-000026f0: 016a 0017 0053 007c 0117 0053 0072 2400  .j...S.|...S.r$.
-00002700: 0000 7285 0000 0072 8700 0000 721e 0000  ..r....r....r...
-00002710: 0072 1e00 0000 721f 0000 00da 075f 5f61  .r....r......__a
-00002720: 6464 5f5f 3201 0000 728a 0000 007a 1342  dd__2...r....z.B
-00002730: 7574 746f 6e49 6e70 7574 2e5f 5f61 6464  uttonInput.__add
-00002740: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00002750: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00002760: 7400 7c00 6a01 8301 5300 2901 7a43 5468  t.|.j...S.).zCTh
-00002770: 6973 2061 6c6c 6f77 7320 7573 2074 6f20  is allows us to 
-00002780: 646f 2060 6966 2069 6e70 7574 2e55 5060  do `if input.UP`
-00002790: 2069 6e73 7465 6164 206f 6620 6069 6620   instead of `if 
-000027a0: 696e 7075 742e 5550 2e69 735f 646f 776e  input.UP.is_down
-000027b0: 6029 02da 0462 6f6f 6c72 7e00 0000 7241  `)...boolr~...rA
-000027c0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-000027d0: 0000 da08 5f5f 626f 6f6c 5f5f 3501 0000  ....__bool__5...
-000027e0: 7269 0000 007a 1442 7574 746f 6e49 6e70  ri...z.ButtonInp
-000027f0: 7574 2e5f 5f62 6f6f 6c5f 5f72 2400 0000  ut.__bool__r$...
-00002800: 2910 7272 0000 0072 7300 0000 7274 0000  ).rr...rs...rt..
-00002810: 0072 6d00 0000 7202 0000 0072 2a00 0000  .rm...r....r*...
-00002820: 7276 0000 0072 7b00 0000 727c 0000 0072  rv...r{...r|...r
-00002830: 7d00 0000 727e 0000 0072 8000 0000 7284  }...r~...r....r.
-00002840: 0000 0072 8900 0000 728b 0000 0072 8d00  ...r....r....r..
-00002850: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00002860: 0072 1f00 0000 7277 0000 000a 0100 0073  .r....rw.......s
-00002870: 1e00 0000 0800 1401 020c 0a01 0203 0a01  ................
-00002880: 0203 0a01 0203 0a01 0805 0803 0803 0803  ................
-00002890: 0c03 7277 0000 0063 0000 0000 0000 0000  ..rw...c........
-000028a0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-000028b0: 7326 0000 0065 005a 0164 005a 0264 015a  s&...e.Z.d.Z.d.Z
-000028c0: 0364 025a 0465 0564 0365 0666 0264 0464  .d.Z.e.d.e.f.d.d
-000028d0: 0584 0483 015a 0764 0653 0029 07da 0941  .....Z.d.S.)...A
-000028e0: 7869 7349 6e70 7574 67cd cccc cccc ccec  xisInputg.......
-000028f0: 3f72 0500 0000 da06 7265 7475 726e 6301  ?r......returnc.
-00002900: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00002910: 0000 0003 0000 0073 4c00 0000 7400 8800  .......sL...t...
-00002920: 6a01 8301 6401 8800 6a02 1800 6400 8502  j...d...j...d...
-00002930: 1900 7d01 8700 6601 6402 6403 8408 7c01  ..}...f.d.d...|.
-00002940: 4400 8301 7d01 7c01 7224 7c01 6401 1900  D...}.|.r$|.d...
-00002950: 8800 6a03 6b05 6f23 7c01 6404 1900 6405  ..j.k.o#|.d...d.
-00002960: 6b01 5300 6406 5300 2907 4ee9 ffff ffff  k.S.d.S.).N.....
-00002970: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002980: 0004 0000 0013 0000 0073 1600 0000 6700  .........s....g.
-00002990: 7c00 5d07 7d01 7c01 8800 6a00 1900 9102  |.].}.|...j.....
-000029a0: 7102 5300 721e 0000 0029 0172 7800 0000  q.S.r....).rx...
-000029b0: 2902 da02 2e30 da06 696e 7075 7473 7241  )....0..inputsrA
-000029c0: 0000 0072 1e00 0000 721f 0000 00da 0a3c  ...r....r......<
-000029d0: 6c69 7374 636f 6d70 3e41 0100 0073 0200  listcomp>A...s..
-000029e0: 0000 1600 7a28 4178 6973 496e 7075 742e  ....z(AxisInput.
-000029f0: 6973 5f73 6d61 7368 6564 2e3c 6c6f 6361  is_smashed.<loca
-00002a00: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
-00002a10: 0000 0072 2200 0000 4629 04da 046c 6973  ...r"...F)...lis
-00002a20: 7472 7900 0000 da0c 736d 6173 685f 7769  try.....smash_wi
-00002a30: 6e64 6f77 da0f 736d 6173 685f 7468 7265  ndow..smash_thre
-00002a40: 7368 6f6c 6429 0272 2900 0000 da07 6869  shold).r).....hi
-00002a50: 7374 6f72 7972 1e00 0000 7241 0000 0072  storyr....rA...r
-00002a60: 1f00 0000 da0a 6973 5f73 6d61 7368 6564  ......is_smashed
-00002a70: 3e01 0000 730a 0000 0018 0212 0104 011a  >...s...........
-00002a80: 0104 027a 1441 7869 7349 6e70 7574 2e69  ...z.AxisInput.i
-00002a90: 735f 736d 6173 6865 644e 2908 7272 0000  s_smashedN).rr..
-00002aa0: 0072 7300 0000 7274 0000 0072 9600 0000  .rs...rt...r....
-00002ab0: 7295 0000 0072 7600 0000 728c 0000 0072  r....rv...r....r
-00002ac0: 9800 0000 721e 0000 0072 1e00 0000 721e  ....r....r....r.
-00002ad0: 0000 0072 1f00 0000 728e 0000 003a 0100  ...r....r....:..
-00002ae0: 0073 0a00 0000 0800 0401 0401 0202 1401  .s..............
-00002af0: 728e 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002b00: 0000 0000 0000 0500 0000 0000 0000 73e0  ..............s.
-00002b10: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
-00002b20: 0465 0583 015a 0565 0465 0683 015a 0665  .e...Z.e.e...Z.e
-00002b30: 0465 0783 015a 0765 0465 0883 015a 0865  .e...Z.e.e...Z.e
-00002b40: 0965 0a83 015a 0a65 0965 0b83 015a 0b65  .e...Z.e.e...Z.e
-00002b50: 0965 0c83 015a 0c65 0965 0d83 015a 0d65  .e...Z.e.e...Z.e
-00002b60: 0965 0e83 015a 0e65 0465 0f83 015a 0f65  .e...Z.e.e...Z.e
-00002b70: 0465 1083 015a 1065 0465 1183 015a 1165  .e...Z.e.e...Z.e
-00002b80: 0465 1283 015a 1265 0965 1383 015a 1365  .e...Z.e.e...Z.e
-00002b90: 0965 1483 015a 1565 0965 1683 015a 1765  .e...Z.e.e...Z.e
-00002ba0: 0965 1883 015a 1965 0965 1a83 015a 1b65  .e...Z.e.e...Z.e
-00002bb0: 0965 1c83 015a 1c65 0965 1d83 015a 1d65  .e...Z.e.e...Z.e
-00002bc0: 0965 1e83 015a 1e65 0965 1f83 015a 1f64  .e...Z.e.e...Z.d
-00002bd0: 0864 0365 2066 0287 0066 0164 0464 0584  .d.e f...f.d.d..
-00002be0: 0d5a 2164 0664 0784 005a 2287 0004 005a  .Z!d.d...Z"....Z
-00002bf0: 2353 0029 09da 1247 616d 6563 7562 6543  #S.)...GamecubeC
-00002c00: 6f6e 7472 6f6c 6c65 7261 3e01 0000 0a20  ontrollera>.... 
-00002c10: 2020 2041 2077 7261 7070 6572 2061 726f     A wrapper aro
-00002c20: 756e 6420 4761 6d65 6375 6265 436f 6e74  und GamecubeCont
-00002c30: 726f 6c6c 6572 5265 6164 6572 2061 6e64  rollerReader and
-00002c40: 2049 6e70 7574 5175 6575 6520 7768 6963   InputQueue whic
-00002c50: 6820 6c65 6176 6573 2061 6c6c 2074 6865  h leaves all the
-00002c60: 2066 6964 646c 790a 2020 2020 696e 7075   fiddly.    inpu
-00002c70: 742d 7265 6164 696e 6720 6c6f 6769 6320  t-reading logic 
-00002c80: 746f 2047 616d 6563 7562 6543 6f6e 7472  to GamecubeContr
-00002c90: 6f6c 6c65 7252 6561 6465 722c 2061 6e64  ollerReader, and
-00002ca0: 2070 726f 7669 6465 7320 6120 636f 6e76   provides a conv
-00002cb0: 656e 6965 6e74 2069 6e74 6572 6661 6365  enient interface
-00002cc0: 2066 6f72 0a20 2020 2061 6363 6573 7369   for.    accessi
-00002cd0: 6e67 2074 6865 2071 7565 7565 206f 6620  ng the queue of 
-00002ce0: 696e 7075 7473 2e0a 0a20 2020 2054 6869  inputs...    Thi
-00002cf0: 7320 616c 6c6f 7773 2067 616d 6573 2074  s allows games t
-00002d00: 6f20 7375 6263 6c61 7373 2074 6869 7320  o subclass this 
-00002d10: 636c 6173 7320 616e 6420 6465 6669 6e65  class and define
-00002d20: 206e 6577 206b 6579 206d 6170 7069 6e67   new key mapping
-00002d30: 7320 652e 672e 2022 4122 202d 2d3e 2022  s e.g. "A" --> "
-00002d40: 6174 7461 636b 220a 2020 2020 e93c 0000  attack".    .<..
-00002d50: 00da 0d63 6f6e 7472 6f6c 6c65 725f 6964  ...controller_id
-00002d60: 6303 0000 0000 0000 0000 0000 0008 0000  c...............
-00002d70: 0005 0000 0003 0000 0073 6400 0000 7400  .........sd...t.
-00002d80: 7c01 8301 7d03 7c01 7c00 5f01 7c03 7c00  |...}.|.|._.|.|.
-00002d90: 5f02 7403 8300 a004 7c02 a101 0100 6401  _.t.....|.....d.
-00002da0: 6402 8400 7c00 6a05 6a06 4400 8301 7d04  d...|.j.j.D...}.
-00002db0: 7c04 a007 a100 4400 5d12 5c02 7d05 7d06  |.....D.].\.}.}.
-00002dc0: 7c06 6a05 7c06 6a08 7c00 6403 8d02 7d07  |.j.|.j.|.d...}.
-00002dd0: 7409 7c00 7c05 7c07 8303 0100 711d 6400  t.|.|.|.....q.d.
-00002de0: 5300 2904 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00002df0: 0000 0400 0000 0600 0000 5300 0000 733a  ..........S...s:
-00002e00: 0000 0069 007c 005d 197d 017c 016a 00a0  ...i.|.].}.|.j..
-00002e10: 01a1 0044 005d 115c 027d 027d 0374 027c  ...D.].\.}.}.t.|
-00002e20: 0174 0383 0272 0974 047c 0374 0583 0272  .t...r.t.|.t...r
-00002e30: 097c 027c 0393 0371 0971 0253 0072 1e00  .|.|...q.q.S.r..
-00002e40: 0000 2906 da08 5f5f 6469 6374 5f5f da05  ..)...__dict__..
-00002e50: 6974 656d 73da 0a69 7373 7562 636c 6173  items..issubclas
-00002e60: 7372 9900 0000 7286 0000 0072 7700 0000  sr....r....rw...
-00002e70: 2904 7291 0000 005a 065f 636c 6173 73da  ).r....Z._class.
-00002e80: 046e 616d 65da 0461 7474 7272 1e00 0000  .name..attrr....
-00002e90: 721e 0000 0072 1f00 0000 da0a 3c64 6963  r....r......<dic
-00002ea0: 7463 6f6d 703e 7101 0000 7316 0000 0006  tcomp>q...s.....
-00002eb0: 0002 0208 0104 fd06 0308 0102 fc08 0402  ................
-00002ec0: fc04 0108 ff7a 2f47 616d 6563 7562 6543  .....z/GamecubeC
-00002ed0: 6f6e 7472 6f6c 6c65 722e 5f5f 696e 6974  ontroller.__init
-00002ee0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  __.<locals>.<dic
-00002ef0: 7463 6f6d 703e 2901 7279 0000 0029 0a72  tcomp>).ry...).r
-00002f00: 2100 0000 729b 0000 00da 0a63 6f6e 7472  !...r......contr
-00002f10: 6f6c 6c65 72da 0573 7570 6572 722a 0000  oller..superr*..
-00002f20: 00da 095f 5f63 6c61 7373 5f5f da07 5f5f  ...__class__..__
-00002f30: 6d72 6f5f 5f72 9d00 0000 7278 0000 00da  mro__r....rx....
-00002f40: 0773 6574 6174 7472 2908 7229 0000 0072  .setattr).r)...r
-00002f50: 9b00 0000 da0c 7175 6575 655f 6c65 6e67  ......queue_leng
-00002f60: 7468 72a2 0000 005a 0d62 7574 746f 6e5f  thr....Z.button_
-00002f70: 696e 7075 7473 729f 0000 0072 a000 0000  inputsr....r....
-00002f80: da03 696e 70a9 0172 a400 0000 721e 0000  ..inp..r....r...
-00002f90: 0072 1f00 0000 722a 0000 0069 0100 0073  .r....r*...i...s
-00002fa0: 1600 0000 0801 0601 0601 0c01 0604 0602  ................
-00002fb0: 06fe 1006 1001 0e01 04fe 7a1b 4761 6d65  ..........z.Game
-00002fc0: 6375 6265 436f 6e74 726f 6c6c 6572 2e5f  cubeController._
-00002fd0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00002fe0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00002ff0: 730a 0000 007c 006a 00a0 01a1 0053 0072  s....|.j.....S.r
-00003000: 2400 0000 2902 72a2 0000 0072 4200 0000  $...).r....rB...
-00003010: 7241 0000 0072 1e00 0000 721e 0000 0072  rA...r....r....r
-00003020: 1f00 0000 da0e 6765 745f 6e65 775f 7661  ......get_new_va
-00003030: 6c75 6573 7b01 0000 7302 0000 000a 017a  lues{...s......z
-00003040: 2147 616d 6563 7562 6543 6f6e 7472 6f6c  !GamecubeControl
-00003050: 6c65 722e 6765 745f 6e65 775f 7661 6c75  ler.get_new_valu
-00003060: 6573 2901 729a 0000 0029 2472 7200 0000  es).r....)$rr...
-00003070: 7273 0000 0072 7400 0000 7275 0000 0072  rs...rt...ru...r
-00003080: 8e00 0000 7233 0000 0072 3400 0000 7235  ....r3...r4...r5
-00003090: 0000 0072 3600 0000 7277 0000 0072 2b00  ...r6...rw...r+.
-000030a0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-000030b0: 0072 2f00 0000 7239 0000 0072 3a00 0000  .r/...r9...r:...
-000030c0: 7237 0000 0072 3800 0000 7232 0000 0072  r7...r8...r2...r
-000030d0: 3f00 0000 da08 445f 5041 445f 5550 723d  ?.....D_PAD_UPr=
-000030e0: 0000 00da 0a44 5f50 4144 5f4c 4546 5472  .....D_PAD_LEFTr
-000030f0: 3e00 0000 da0b 445f 5041 445f 5249 4748  >.....D_PAD_RIGH
-00003100: 5472 4000 0000 da0a 445f 5041 445f 444f  Tr@.....D_PAD_DO
-00003110: 574e 7230 0000 0072 3100 0000 723c 0000  WNr0...r1...r<..
-00003120: 0072 3b00 0000 726d 0000 0072 2a00 0000  .r;...rm...r*...
-00003130: 72aa 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00003140: 6c6c 5f5f 721e 0000 0072 1e00 0000 72a9  ll__r....r....r.
-00003150: 0000 0072 1f00 0000 7299 0000 0048 0100  ...r....r....H..
-00003160: 0073 3400 0000 0800 0401 0809 0801 0801  .s4.............
-00003170: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003180: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003190: 0801 0801 0801 1402 1012 7299 0000 00da  ..........r.....
-000031a0: 085f 5f6d 6169 6e5f 5f63 0000 0000 0000  .__main__c......
-000031b0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-000031c0: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
-000031d0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
-000031e0: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
-000031f0: 0964 0a84 005a 0764 0b53 0029 0cda 0954  .d...Z.d.S.)...T
-00003200: 6578 7450 7269 6e74 6301 0000 0000 0000  extPrintc.......
-00003210: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00003220: 0073 2600 0000 7c00 a000 a100 0100 7401  .s&...|.......t.
-00003230: 6a02 a003 a100 0100 7401 6a02 a004 6400  j.......t.j...d.
-00003240: 6401 a102 7c00 5f02 6400 5300 2902 4ee9  d...|._.d.S.).N.
-00003250: 1e00 0000 2905 da05 7265 7365 7472 2500  ....)...resetr%.
-00003260: 0000 da04 666f 6e74 7228 0000 00da 0446  ....fontr(.....F
-00003270: 6f6e 7472 4100 0000 721e 0000 0072 1e00  ontrA...r....r..
-00003280: 0000 721f 0000 0072 2a00 0000 8301 0000  ..r....r*.......
-00003290: 7306 0000 0008 010a 0114 017a 1254 6578  s..........z.Tex
-000032a0: 7450 7269 6e74 2e5f 5f69 6e69 745f 5f63  tPrint.__init__c
-000032b0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-000032c0: 0500 0000 4300 0000 7338 0000 007c 006a  ....C...s8...|.j
-000032d0: 00a0 017c 0264 0174 02a1 037d 037c 01a0  ...|.d.t...}.|..
-000032e0: 037c 037c 006a 047c 006a 0566 02a1 0201  .|.|.j.|.j.f....
-000032f0: 007c 0004 006a 057c 006a 0637 0002 005f  .|...j.|.j.7..._
-00003300: 0564 0053 0029 024e 5429 0772 b400 0000  .d.S.).NT).r....
-00003310: da06 7265 6e64 6572 da05 424c 4143 4bda  ..render..BLACK.
-00003320: 0462 6c69 74da 0178 da01 79da 0b6c 696e  .blit..x..y..lin
-00003330: 655f 6865 6967 6874 2904 7229 0000 00da  e_height).r)....
-00003340: 0673 6372 6565 6e5a 0a74 6578 7453 7472  .screenZ.textStr
-00003350: 696e 675a 0a74 6578 7442 6974 6d61 7072  ingZ.textBitmapr
-00003360: 1e00 0000 721e 0000 0072 1f00 0000 da06  ....r....r......
-00003370: 7470 7269 6e74 8801 0000 7306 0000 0010  tprint....s.....
-00003380: 0114 0114 017a 1054 6578 7450 7269 6e74  .....z.TextPrint
-00003390: 2e74 7072 696e 7463 0100 0000 0000 0000  .tprintc........
-000033a0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-000033b0: 7316 0000 0064 017c 005f 0064 017c 005f  s....d.|._.d.|._
-000033c0: 0164 027c 005f 0264 0053 0029 034e 720c  .d.|._.d.S.).Nr.
-000033d0: 0000 0072 1600 0000 2903 72b9 0000 0072  ...r....).r....r
-000033e0: ba00 0000 72bb 0000 0072 4100 0000 721e  ....r....rA...r.
-000033f0: 0000 0072 1e00 0000 721f 0000 0072 b300  ...r....r....r..
-00003400: 0000 8d01 0000 7306 0000 0006 0106 010a  ......s.........
-00003410: 017a 0f54 6578 7450 7269 6e74 2e72 6573  .z.TextPrint.res
-00003420: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
-00003430: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
-00003440: 7c00 0400 6a00 6401 3700 0200 5f00 6400  |...j.d.7..._.d.
-00003450: 5300 a902 4e72 0c00 0000 a901 72b9 0000  S...Nr......r...
-00003460: 0072 4100 0000 721e 0000 0072 1e00 0000  .rA...r....r....
-00003470: 721f 0000 00da 0669 6e64 656e 7492 0100  r......indent...
-00003480: 00f3 0200 0000 1201 7a10 5465 7874 5072  ........z.TextPr
-00003490: 696e 742e 696e 6465 6e74 6301 0000 0000  int.indentc.....
-000034a0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-000034b0: 0000 0073 1200 0000 7c00 0400 6a00 6401  ...s....|...j.d.
-000034c0: 3800 0200 5f00 6400 5300 72be 0000 0072  8..._.d.S.r....r
-000034d0: bf00 0000 7241 0000 0072 1e00 0000 721e  ....rA...r....r.
-000034e0: 0000 0072 1f00 0000 da08 756e 696e 6465  ...r......uninde
-000034f0: 6e74 9501 0000 72c1 0000 007a 1254 6578  nt....r....z.Tex
-00003500: 7450 7269 6e74 2e75 6e69 6e64 656e 744e  tPrint.unindentN
-00003510: 2908 7272 0000 0072 7300 0000 7274 0000  ).rr...rs...rt..
-00003520: 0072 2a00 0000 72bd 0000 0072 b300 0000  .r*...r....r....
-00003530: 72c0 0000 0072 c200 0000 721e 0000 0072  r....r....r....r
-00003540: 1e00 0000 721e 0000 0072 1f00 0000 72b1  ....r....r....r.
-00003550: 0000 0082 0100 0073 0c00 0000 0800 0801  .......s........
-00003560: 0805 0805 0805 0c03 72b1 0000 00da 0562  ........r......b
-00003570: 6c61 636b da05 7768 6974 6529 0269 f401  lack..white).i..
-00003580: 0000 69bc 0200 007a 074d 7920 4761 6d65  ..i....z.My Game
-00003590: 4629 0172 2300 0000 7a15 4761 6d65 6375  F).r#...z.Gamecu
-000035a0: 6265 2063 6f6e 7472 6f6c 6c65 7220 307a  be controller 0z
-000035b0: 0842 7574 746f 6e73 3a7a 1341 2042 2058  .Buttons:z.A B X
-000035c0: 2059 205a 204c 2052 2053 5441 5254 7a02   Y Z L R STARTz.
-000035d0: 3a20 7a05 4178 6573 3a7a 705f 4c5f 5452  : z.Axes:zp_L_TR
-000035e0: 4947 4745 525f 4158 4953 205f 525f 5452  IGGER_AXIS _R_TR
-000035f0: 4947 4745 525f 4158 4953 205f 4752 4559  IGGER_AXIS _GREY
-00003600: 5f53 5449 434b 5f58 5f41 5849 5320 5f47  _STICK_X_AXIS _G
-00003610: 5245 595f 5354 4943 4b5f 595f 4158 4953  REY_STICK_Y_AXIS
-00003620: 205f 5945 4c4c 4f57 5f53 5449 434b 5f58   _YELLOW_STICK_X
-00003630: 5f41 5849 5320 5f59 454c 4c4f 575f 5354  _AXIS _YELLOW_ST
-00003640: 4943 4b5f 595f 4158 4953 207a 0548 6174  ICK_Y_AXIS z.Hat
-00003650: 733a 7265 0000 007a 1150 524f 4345 5353  s:re...z.PROCESS
-00003660: 4544 2049 4e50 5554 533a 7a57 4c45 4654  ED INPUTS:zWLEFT
-00003670: 2052 4947 4854 2055 5020 444f 574e 2043   RIGHT UP DOWN C
-00003680: 5f4c 4546 5420 435f 5249 4748 5420 435f  _LEFT C_RIGHT C_
-00003690: 5550 2043 5f44 4f57 4e20 525f 4158 4953  UP C_DOWN R_AXIS
-000036a0: 204c 5f41 5849 5320 445f 4c45 4654 2044   L_AXIS D_LEFT D
-000036b0: 5f52 4947 4854 2044 5f55 5020 445f 444f  _RIGHT D_UP D_DO
-000036c0: 574e 2029 0154 2940 7275 0000 0072 2500  WN ).T)@ru...r%.
-000036d0: 0000 5a15 726f 6269 6e67 616d 652e 696e  ..Z.robingame.in
-000036e0: 7075 742e 7175 6575 6572 0200 0000 722b  put.queuer....r+
-000036f0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00003700: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00003710: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00003720: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00003730: 3800 0000 7239 0000 0072 3a00 0000 723b  8...r9...r:...r;
-00003740: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
-00003750: 0000 723f 0000 0072 4000 0000 7220 0000  ..r?...r@...r ..
-00003760: 0072 2100 0000 7277 0000 0072 8e00 0000  .r!...rw...r....
-00003770: 7299 0000 0072 7200 0000 da06 6f62 6a65  r....rr.....obje
-00003780: 6374 72b1 0000 00da 0543 6f6c 6f72 72b7  ctr......Colorr.
-00003790: 0000 005a 0557 4849 5445 7226 0000 0072  ...Z.WHITEr&...r
-000037a0: 2800 0000 5a09 7465 7874 5072 696e 74da  (...Z.textPrint.
-000037b0: 0764 6973 706c 6179 da08 7365 745f 6d6f  .display..set_mo
-000037c0: 6465 72bc 0000 00da 0b73 6574 5f63 6170  der......set_cap
-000037d0: 7469 6f6e da04 7469 6d65 da05 436c 6f63  tion..time..Cloc
-000037e0: 6b5a 0563 6c6f 636b 5a04 646f 6e65 da05  kZ.clockZ.done..
-000037f0: 6576 656e 74da 0367 6574 da04 7479 7065  event..get..type
-00003800: da04 5155 4954 da04 6669 6c6c 72b3 0000  ..QUIT..fillr...
-00003810: 0072 a200 0000 72c0 0000 0072 bd00 0000  .r....r....r....
-00003820: da05 7370 6c69 74da 0662 7574 746f 6eda  ..split..button.
-00003830: 0767 6574 6174 7472 72c2 0000 00da 0466  .getattrr......f
-00003840: 6c69 70da 0474 6963 6bda 0471 7569 7472  lip..tick..quitr
-00003850: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
-00003860: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00003870: 0073 a200 0000 0400 080a 0c02 0405 0401  .s..............
-00003880: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-00003890: 0401 0401 0401 0401 0401 0401 0401 0401  ................
-000038a0: 0401 0401 0401 0401 0a03 0e15 007f 0e4c  ...............L
-000038b0: 1030 100e 0a37 0201 1002 0a16 0a01 0a02  .0...7..........
-000038c0: 0601 0c02 0c01 0a01 0401 0601 0e01 0c01  ................
-000038d0: 0401 0280 0a02 0801 0a01 0802 0c01 0c02  ................
-000038e0: 0801 0c01 1e01 0801 0c02 0801 0202 0404  ................
-000038f0: 06fb 1e06 0801 0c02 0801 0c01 2001 0801  ............ ...
-00003900: 0c02 0801 0202 0404 06fb 2006 0801 0a03  .......... .....
-00003910: 0a03 04ce 0c34 04a9                      .....4..
+000005d0: 5f76 616c 7565 a900 7227 0000 00fa 362f  _value..r'....6/
+000005e0: 686f 6d65 2f72 6f62 696e 2f63 6f64 652f  home/robin/code/
+000005f0: 726f 6269 6e67 616d 652f 726f 6269 6e67  robingame/robing
+00000600: 616d 652f 696e 7075 742f 6761 6d65 6375  ame/input/gamecu
+00000610: 6265 2e70 79da 0a6c 696e 6561 725f 6d61  be.py..linear_ma
+00000620: 702a 0000 0073 1600 0000 0803 0801 0802  p*...s..........
+00000630: 0801 0801 0c01 0c03 0402 0a01 0a01 0402  ................
+00000640: 7229 0000 0063 0000 0000 0000 0000 0000  r)...c..........
+00000650: 0000 0000 0000 0300 0000 4000 0000 73be  ..........@...s.
+00000660: 0100 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00000670: 025a 0464 035a 0564 045a 0664 0565 0766  .Z.d.Z.d.Z.d.e.f
+00000680: 0264 0664 0784 045a 0864 0864 0984 005a  .d.d...Z.d.d...Z
+00000690: 0964 0a64 0b84 005a 0a64 0c64 0d84 005a  .d.d...Z.d.d...Z
+000006a0: 0b64 0e64 0f84 005a 0c65 0d64 1064 1184  .d.d...Z.e.d.d..
+000006b0: 0083 015a 0e65 0d64 1264 1384 0083 015a  ...Z.e.d.d.....Z
+000006c0: 0f65 0d64 1464 1584 0083 015a 1065 0d64  .e.d.d.....Z.e.d
+000006d0: 1664 1784 0083 015a 1165 0d64 1864 1984  .d.....Z.e.d.d..
+000006e0: 0083 015a 1265 0d64 1a64 1b84 0083 015a  ...Z.e.d.d.....Z
+000006f0: 1365 0d64 1c64 1d84 0083 015a 1465 0d64  .e.d.d.....Z.e.d
+00000700: 1e64 1f84 0083 015a 1565 0d64 2064 2184  .d.....Z.e.d d!.
+00000710: 0083 015a 1665 0d64 2264 2384 0083 015a  ...Z.e.d"d#....Z
+00000720: 1765 0d64 2464 2584 0083 015a 1865 0d64  .e.d$d%....Z.e.d
+00000730: 2664 2784 0083 015a 1965 0d64 2864 2984  &d'....Z.e.d(d).
+00000740: 0083 015a 1a65 0d64 2a64 2b84 0083 015a  ...Z.e.d*d+....Z
+00000750: 1b65 0d64 2c64 2d84 0083 015a 1c65 0d64  .e.d,d-....Z.e.d
+00000760: 2e64 2f84 0083 015a 1d65 0d64 3064 3184  .d/....Z.e.d0d1.
+00000770: 0083 015a 1e65 0d64 3264 3384 0083 015a  ...Z.e.d2d3....Z
+00000780: 1f65 0d64 3464 3584 0083 015a 2065 0d64  .e.d4d5....Z e.d
+00000790: 3664 3784 0083 015a 2165 0d64 3864 3984  6d7....Z!e.d8d9.
+000007a0: 0083 015a 2265 0d64 3a64 3b84 0083 015a  ...Z"e.d:d;....Z
+000007b0: 2365 0d64 3c64 3d84 0083 015a 2465 0d64  #e.d<d=....Z$e.d
+000007c0: 3e64 3f84 0083 015a 2565 0d64 4064 4184  >d?....Z%e.d@dA.
+000007d0: 0083 015a 2665 0d64 4264 4384 0083 015a  ...Z&e.dBdC....Z
+000007e0: 2765 0d64 4464 4584 0083 015a 2865 0d64  'e.dDdE....Z(e.d
+000007f0: 4664 4784 0083 015a 2965 0d64 4864 4984  FdG....Z)e.dHdI.
+00000800: 0083 015a 2a65 0d64 4a64 4b84 0083 015a  ...Z*e.dJdK....Z
+00000810: 2b65 0d64 4c64 4d84 0083 015a 2c64 4e53  +e.dLdM....Z,dNS
+00000820: 0029 4fda 1847 616d 6563 7562 6543 6f6e  .)O..GamecubeCon
+00000830: 7472 6f6c 6c65 7252 6561 6465 7261 4802  trollerReaderaH.
+00000840: 0000 436c 6173 7320 746f 2072 6561 6420  ..Class to read 
+00000850: 7468 6520 696e 7075 7473 206f 6620 6120  the inputs of a 
+00000860: 4761 6d65 4375 6265 2063 6f6e 7472 6f6c  GameCube control
+00000870: 6c65 7220 706c 7567 6765 6420 696e 746f  ler plugged into
+00000880: 2074 6865 204d 6179 666c 6173 6820 2247   the Mayflash "G
+00000890: 616d 6543 7562 650a 2020 2020 436f 6e74  ameCube.    Cont
+000008a0: 726f 6c6c 6572 2041 6461 7074 6572 2066  roller Adapter f
+000008b0: 6f72 2057 6969 2055 2026 2050 4320 5553  or Wii U & PC US
+000008c0: 4222 0a0a 2020 2020 5468 6973 2063 6c61  B"..    This cla
+000008d0: 7373 0a20 2020 202d 2072 6561 6473 2074  ss.    - reads t
+000008e0: 6865 2076 616c 7565 7320 6672 6f6d 2074  he values from t
+000008f0: 6865 2063 6f6e 7472 6f6c 6c65 7227 7320  he controller's 
+00000900: 6275 7474 6f6e 7320 2862 696e 6172 7920  buttons (binary 
+00000910: 7661 6c75 6573 2920 6178 6573 2028 616e  values) axes (an
+00000920: 616c 6f67 2069 6e70 7574 7320 7375 6368  alog inputs such
+00000930: 2061 730a 2020 2020 636f 6e74 726f 6c20   as.    control 
+00000940: 7374 6963 6b73 2061 6e64 2074 7269 6767  sticks and trigg
+00000950: 6572 7329 2061 6e64 2068 6174 7320 2874  ers) and hats (t
+00000960: 6865 2034 2d77 6179 2044 2070 6164 290a  he 4-way D pad).
+00000970: 2020 2020 2d20 6d61 7073 2074 6865 2076      - maps the v
+00000980: 616c 7565 7320 6f66 2074 6865 2069 6e70  alues of the inp
+00000990: 7574 7320 746f 2061 2030 2d31 2072 616e  uts to a 0-1 ran
+000009a0: 6765 2061 6e64 2065 7870 6f73 6573 2074  ge and exposes t
+000009b0: 6865 7365 2061 7320 6e61 6d65 6420 7072  hese as named pr
+000009c0: 6f70 6572 7469 6573 2069 6620 7468 650a  operties if the.
+000009d0: 2020 2020 7573 6572 2077 616e 7473 2074      user wants t
+000009e0: 6f20 6163 6365 7373 2061 2073 696e 676c  o access a singl
+000009f0: 6520 7661 6c75 652e 0a20 2020 202d 2065  e value..    - e
+00000a00: 7870 6f73 6573 2061 202e 6765 745f 7661  xposes a .get_va
+00000a10: 6c75 6573 2829 206d 6574 686f 6420 7768  lues() method wh
+00000a20: 6963 6820 7265 7475 726e 7320 6120 7475  ich returns a tu
+00000a30: 706c 6520 6f66 2061 6c6c 2074 6865 2069  ple of all the i
+00000a40: 6e70 7574 7320 2873 696d 696c 6172 2074  nputs (similar t
+00000a50: 6f20 686f 770a 2020 2020 7079 6761 6d65  o how.    pygame
+00000a60: 2064 6561 6c73 2077 6974 6820 6b65 7962   deals with keyb
+00000a70: 6f61 7264 2061 6e64 206d 6f75 7365 2069  oard and mouse i
+00000a80: 6e70 7574 2e0a 2020 2020 2902 e79a 9999  nput..    ).....
+00000a90: 9999 99b9 3f67 a470 3d0a d7a3 e83f 2902  ....?g.p=....?).
+00000aa0: 722b 0000 0067 713d 0ad7 a370 e53f 2902  r+...gq=...p.?).
+00000ab0: 6700 0000 0000 00e0 bf72 0300 0000 da0b  g........r......
+00000ac0: 6a6f 7973 7469 636b 5f69 6463 0200 0000  joystick_idc....
+00000ad0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000ae0: 4300 0000 731c 0000 0074 006a 01a0 027c  C...s....t.j...|
+00000af0: 01a1 017c 005f 017c 006a 01a0 03a1 0001  ...|._.|.j......
+00000b00: 0064 0053 00a9 014e 2904 da06 7079 6761  .d.S...N)...pyga
+00000b10: 6d65 da08 6a6f 7973 7469 636b da08 4a6f  me..joystick..Jo
+00000b20: 7973 7469 636b da04 696e 6974 2902 da04  ystick..init)...
+00000b30: 7365 6c66 722c 0000 0072 2700 0000 7227  selfr,...r'...r'
+00000b40: 0000 0072 2800 0000 da08 5f5f 696e 6974  ...r(.....__init
+00000b50: 5f5f 5100 0000 7304 0000 000e 010e 017a  __Q...s........z
+00000b60: 2147 616d 6563 7562 6543 6f6e 7472 6f6c  !GamecubeControl
+00000b70: 6c65 7252 6561 6465 722e 5f5f 696e 6974  lerReader.__init
+00000b80: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000b90: 0000 0016 0000 0043 0000 0073 5c00 0000  .......C...s\...
+00000ba0: 7c00 6a00 7c00 6a01 7c00 6a02 7c00 6a03  |.j.|.j.|.j.|.j.
+00000bb0: 7c00 6a04 7c00 6a05 7c00 6a06 7c00 6a07  |.j.|.j.|.j.|.j.
+00000bc0: 7c00 6a08 7c00 6a09 7c00 6a0a 7c00 6a0b  |.j.|.j.|.j.|.j.
+00000bd0: 7c00 6a0c 7c00 6a0d 7c00 6a0e 7c00 6a0f  |.j.|.j.|.j.|.j.
+00000be0: 7c00 6a10 7c00 6a11 7c00 6a12 7c00 6a13  |.j.|.j.|.j.|.j.
+00000bf0: 7c00 6a14 7c00 6a15 6616 5300 2901 7aa1  |.j.|.j.f.S.).z.
+00000c00: 4765 7420 7468 6520 6375 7272 656e 7420  Get the current 
+00000c10: 7374 6174 6520 6f66 2061 6c6c 2074 6865  state of all the
+00000c20: 2069 6e70 7574 732e 2054 6869 7320 6973   inputs. This is
+00000c30: 2069 6e74 656e 6465 6420 746f 2062 6520   intended to be 
+00000c40: 6571 7569 7661 6c65 6e74 2074 6f0a 2020  equivalent to.  
+00000c50: 2020 2020 2020 7079 6761 6d65 2e6b 6579        pygame.key
+00000c60: 2e67 6574 5f70 7265 7373 6564 2073 6f20  .get_pressed so 
+00000c70: 7468 6174 2074 6865 2069 6e70 7574 7320  that the inputs 
+00000c80: 6361 6e20 6265 2070 726f 6365 7373 6564  can be processed
+00000c90: 2069 6e20 7468 6520 7361 6d65 2077 6179   in the same way
+00000ca0: 2e29 16da 0141 da01 42da 0158 da01 59da  .)...A..B..X..Y.
+00000cb0: 015a da01 4cda 0152 da05 5354 4152 54da  .Z..L..R..START.
+00000cc0: 044c 4546 54da 0552 4947 4854 da02 5550  .LEFT..RIGHT..UP
+00000cd0: da04 444f 574e da06 435f 4c45 4654 da07  ..DOWN..C_LEFT..
+00000ce0: 435f 5249 4748 54da 0443 5f55 50da 0643  C_RIGHT..C_UP..C
+00000cf0: 5f44 4f57 4eda 0652 5f41 5849 53da 064c  _DOWN..R_AXIS..L
+00000d00: 5f41 5849 53da 0644 5f4c 4546 54da 0744  _AXIS..D_LEFT..D
+00000d10: 5f52 4947 4854 da04 445f 5550 da06 445f  _RIGHT..D_UP..D_
+00000d20: 444f 574e a901 7232 0000 0072 2700 0000  DOWN..r2...r'...
+00000d30: 7227 0000 0072 2800 0000 da0a 6765 745f  r'...r(.....get_
+00000d40: 7661 6c75 6573 5500 0000 732e 0000 0004  valuesU...s.....
+00000d50: 0704 0104 0104 0104 0104 0104 0104 0104  ................
+00000d60: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00000d70: 0104 0104 0104 0104 0104 0104 ea7a 2347  .............z#G
+00000d80: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
+00000d90: 7252 6561 6465 722e 6765 745f 7661 6c75  rReader.get_valu
+00000da0: 6573 6302 0000 0000 0000 0000 0000 0002  esc.............
+00000db0: 0000 0004 0000 0043 0000 00f3 0e00 0000  .......C........
+00000dc0: 7400 7c01 7c00 6a01 6401 8303 5300 a902  t.|.|.j.d...S...
+00000dd0: 4e29 0272 0100 0000 7203 0000 0029 0272  N).r....r....).r
+00000de0: 2900 0000 da16 4752 4559 5f53 5449 434b  ).....GREY_STICK
+00000df0: 5f49 4e50 5554 5f52 414e 4745 a902 7232  _INPUT_RANGE..r2
+00000e00: 0000 0072 1a00 0000 7227 0000 0072 2700  ...r....r'...r'.
+00000e10: 0000 7228 0000 00da 0e67 7265 795f 7374  ..r(.....grey_st
+00000e20: 6963 6b5f 6d61 7074 0000 00f3 0200 0000  ick_mapt........
+00000e30: 0e01 7a27 4761 6d65 6375 6265 436f 6e74  ..z'GamecubeCont
+00000e40: 726f 6c6c 6572 5265 6164 6572 2e67 7265  rollerReader.gre
+00000e50: 795f 7374 6963 6b5f 6d61 7063 0200 0000  y_stick_mapc....
+00000e60: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000e70: 4300 0000 724c 0000 0072 4d00 0000 2902  C...rL...rM...).
+00000e80: 7229 0000 00da 1859 454c 4c4f 575f 5354  r).....YELLOW_ST
+00000e90: 4943 4b5f 494e 5055 545f 5241 4e47 4572  ICK_INPUT_RANGEr
+00000ea0: 4f00 0000 7227 0000 0072 2700 0000 7228  O...r'...r'...r(
+00000eb0: 0000 00da 1079 656c 6c6f 775f 7374 6963  .....yellow_stic
+00000ec0: 6b5f 6d61 7077 0000 0072 5100 0000 7a29  k_mapw...rQ...z)
+00000ed0: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
+00000ee0: 6572 5265 6164 6572 2e79 656c 6c6f 775f  erReader.yellow_
+00000ef0: 7374 6963 6b5f 6d61 7063 0200 0000 0000  stick_mapc......
+00000f00: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00000f10: 0000 724c 0000 0072 4d00 0000 2902 7229  ..rL...rM...).r)
+00000f20: 0000 00da 1354 5249 4747 4552 5f49 4e50  .....TRIGGER_INP
+00000f30: 5554 5f52 414e 4745 724f 0000 0072 2700  UT_RANGErO...r'.
+00000f40: 0000 7227 0000 0072 2800 0000 da0b 7472  ..r'...r(.....tr
+00000f50: 6967 6765 725f 6d61 707a 0000 0072 5100  igger_mapz...rQ.
+00000f60: 0000 7a24 4761 6d65 6375 6265 436f 6e74  ..z$GamecubeCont
+00000f70: 726f 6c6c 6572 5265 6164 6572 2e74 7269  rollerReader.tri
+00000f80: 6767 6572 5f6d 6170 6301 0000 0000 0000  gger_mapc.......
+00000f90: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000fa0: 00f3 0c00 0000 7c00 6a00 a001 6401 a101  ......|.j...d...
+00000fb0: 5300 a902 4e72 0100 0000 a902 722f 0000  S...Nr......r/..
+00000fc0: 00da 0867 6574 5f61 7869 7372 4a00 0000  ...get_axisrJ...
+00000fd0: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
+00000fe0: 125f 4752 4559 5f53 5449 434b 5f58 5f41  ._GREY_STICK_X_A
+00000ff0: 5849 5381 0000 00f3 0200 0000 0c02 7a2b  XIS...........z+
+00001000: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
+00001010: 6572 5265 6164 6572 2e5f 4752 4559 5f53  erReader._GREY_S
+00001020: 5449 434b 5f58 5f41 5849 5363 0100 0000  TICK_X_AXISc....
+00001030: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001040: 4300 0000 7256 0000 00a9 024e 7203 0000  C...rV.....Nr...
+00001050: 0072 5800 0000 724a 0000 0072 2700 0000  .rX...rJ...r'...
+00001060: 7227 0000 0072 2800 0000 da12 5f47 5245  r'...r(....._GRE
+00001070: 595f 5354 4943 4b5f 595f 4158 4953 8500  Y_STICK_Y_AXIS..
+00001080: 0000 725b 0000 007a 2b47 616d 6563 7562  ..r[...z+Gamecub
+00001090: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
+000010a0: 722e 5f47 5245 595f 5354 4943 4b5f 595f  r._GREY_STICK_Y_
+000010b0: 4158 4953 6301 0000 0000 0000 0000 0000  AXISc...........
+000010c0: 0001 0000 0003 0000 0043 0000 0072 5600  .........C...rV.
+000010d0: 0000 a902 4e72 0700 0000 7258 0000 0072  ....Nr....rX...r
+000010e0: 4a00 0000 7227 0000 0072 2700 0000 7228  J...r'...r'...r(
+000010f0: 0000 00da 145f 5945 4c4c 4f57 5f53 5449  ....._YELLOW_STI
+00001100: 434b 5f58 5f41 5849 5389 0000 0072 5b00  CK_X_AXIS....r[.
+00001110: 0000 7a2d 4761 6d65 6375 6265 436f 6e74  ..z-GamecubeCont
+00001120: 726f 6c6c 6572 5265 6164 6572 2e5f 5945  rollerReader._YE
+00001130: 4c4c 4f57 5f53 5449 434b 5f58 5f41 5849  LLOW_STICK_X_AXI
+00001140: 5363 0100 0000 0000 0000 0000 0000 0100  Sc..............
+00001150: 0000 0300 0000 4300 0000 7256 0000 00a9  ......C...rV....
+00001160: 024e 7204 0000 0072 5800 0000 724a 0000  .Nr....rX...rJ..
+00001170: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
+00001180: da14 5f59 454c 4c4f 575f 5354 4943 4b5f  .._YELLOW_STICK_
+00001190: 595f 4158 4953 8d00 0000 725b 0000 007a  Y_AXIS....r[...z
+000011a0: 2d47 616d 6563 7562 6543 6f6e 7472 6f6c  -GamecubeControl
+000011b0: 6c65 7252 6561 6465 722e 5f59 454c 4c4f  lerReader._YELLO
+000011c0: 575f 5354 4943 4b5f 595f 4158 4953 6301  W_STICK_Y_AXISc.
+000011d0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000011e0: 0000 0043 0000 0072 5600 0000 a902 4e72  ...C...rV.....Nr
+000011f0: 0500 0000 7258 0000 0072 4a00 0000 7227  ....rX...rJ...r'
+00001200: 0000 0072 2700 0000 7228 0000 00da 0f5f  ...r'...r(....._
+00001210: 4c5f 5452 4947 4745 525f 4158 4953 9100  L_TRIGGER_AXIS..
+00001220: 0000 725b 0000 007a 2847 616d 6563 7562  ..r[...z(Gamecub
+00001230: 6543 6f6e 7472 6f6c 6c65 7252 6561 6465  eControllerReade
+00001240: 722e 5f4c 5f54 5249 4747 4552 5f41 5849  r._L_TRIGGER_AXI
+00001250: 5363 0100 0000 0000 0000 0000 0000 0100  Sc..............
+00001260: 0000 0300 0000 4300 0000 7256 0000 00a9  ......C...rV....
+00001270: 024e 7206 0000 0072 5800 0000 724a 0000  .Nr....rX...rJ..
+00001280: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
+00001290: da0f 5f52 5f54 5249 4747 4552 5f41 5849  .._R_TRIGGER_AXI
+000012a0: 5395 0000 0072 5b00 0000 7a28 4761 6d65  S....r[...z(Game
+000012b0: 6375 6265 436f 6e74 726f 6c6c 6572 5265  cubeControllerRe
+000012c0: 6164 6572 2e5f 525f 5452 4947 4745 525f  ader._R_TRIGGER_
+000012d0: 4158 4953 6301 0000 0000 0000 0000 0000  AXISc...........
+000012e0: 0001 0000 0003 0000 0043 0000 00f3 0e00  .........C......
+000012f0: 0000 7c00 a000 7c00 6a01 0b00 a101 5300  ..|...|.j.....S.
+00001300: 722d 0000 00a9 0272 5000 0000 725a 0000  r-.....rP...rZ..
+00001310: 0072 4a00 0000 7227 0000 0072 2700 0000  .rJ...r'...r'...
+00001320: 7228 0000 0072 3c00 0000 9b00 0000 f302  r(...r<.........
+00001330: 0000 000e 027a 1d47 616d 6563 7562 6543  .....z.GamecubeC
+00001340: 6f6e 7472 6f6c 6c65 7252 6561 6465 722e  ontrollerReader.
+00001350: 4c45 4654 6301 0000 0000 0000 0000 0000  LEFTc...........
+00001360: 0001 0000 0003 0000 0043 0000 00f3 0c00  .........C......
+00001370: 0000 7c00 a000 7c00 6a01 a101 5300 722d  ..|...|.j...S.r-
+00001380: 0000 0072 6700 0000 724a 0000 0072 2700  ...rg...rJ...r'.
+00001390: 0000 7227 0000 0072 2800 0000 723d 0000  ..r'...r(...r=..
+000013a0: 009f 0000 0072 5b00 0000 7a1e 4761 6d65  .....r[...z.Game
+000013b0: 6375 6265 436f 6e74 726f 6c6c 6572 5265  cubeControllerRe
+000013c0: 6164 6572 2e52 4947 4854 6301 0000 0000  ader.RIGHTc.....
+000013d0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000013e0: 0000 0072 6600 0000 722d 0000 00a9 0272  ...rf...r-.....r
+000013f0: 5000 0000 725d 0000 0072 4a00 0000 7227  P...r]...rJ...r'
+00001400: 0000 0072 2700 0000 7228 0000 0072 3e00  ...r'...r(...r>.
+00001410: 0000 a300 0000 7268 0000 007a 1b47 616d  ......rh...z.Gam
+00001420: 6563 7562 6543 6f6e 7472 6f6c 6c65 7252  ecubeControllerR
+00001430: 6561 6465 722e 5550 6301 0000 0000 0000  eader.UPc.......
+00001440: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00001450: 0072 6900 0000 722d 0000 0072 6a00 0000  .ri...r-...rj...
+00001460: 724a 0000 0072 2700 0000 7227 0000 0072  rJ...r'...r'...r
+00001470: 2800 0000 723f 0000 00a7 0000 0072 5b00  (...r?.......r[.
+00001480: 0000 7a1d 4761 6d65 6375 6265 436f 6e74  ..z.GamecubeCont
+00001490: 726f 6c6c 6572 5265 6164 6572 2e44 4f57  rollerReader.DOW
+000014a0: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
+000014b0: 0000 0300 0000 4300 0000 7266 0000 0072  ......C...rf...r
+000014c0: 2d00 0000 a902 7253 0000 0072 5f00 0000  -.....rS...r_...
+000014d0: 724a 0000 0072 2700 0000 7227 0000 0072  rJ...r'...r'...r
+000014e0: 2800 0000 7240 0000 00ab 0000 0072 6800  (...r@.......rh.
+000014f0: 0000 7a1f 4761 6d65 6375 6265 436f 6e74  ..z.GamecubeCont
+00001500: 726f 6c6c 6572 5265 6164 6572 2e43 5f4c  rollerReader.C_L
+00001510: 4546 5463 0100 0000 0000 0000 0000 0000  EFTc............
+00001520: 0100 0000 0300 0000 4300 0000 7269 0000  ........C...ri..
+00001530: 0072 2d00 0000 726b 0000 0072 4a00 0000  .r-...rk...rJ...
+00001540: 7227 0000 0072 2700 0000 7228 0000 0072  r'...r'...r(...r
+00001550: 4100 0000 af00 0000 725b 0000 007a 2047  A.......r[...z G
+00001560: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
+00001570: 7252 6561 6465 722e 435f 5249 4748 5463  rReader.C_RIGHTc
+00001580: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001590: 0300 0000 4300 0000 7266 0000 0072 2d00  ....C...rf...r-.
+000015a0: 0000 a902 7253 0000 0072 6100 0000 724a  ....rS...ra...rJ
+000015b0: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+000015c0: 0000 7242 0000 00b3 0000 0072 6800 0000  ..rB.......rh...
+000015d0: 7a1d 4761 6d65 6375 6265 436f 6e74 726f  z.GamecubeContro
+000015e0: 6c6c 6572 5265 6164 6572 2e43 5f55 5063  llerReader.C_UPc
+000015f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001600: 0300 0000 4300 0000 7269 0000 0072 2d00  ....C...ri...r-.
+00001610: 0000 726c 0000 0072 4a00 0000 7227 0000  ..rl...rJ...r'..
+00001620: 0072 2700 0000 7228 0000 0072 4300 0000  .r'...r(...rC...
+00001630: b700 0000 725b 0000 007a 1f47 616d 6563  ....r[...z.Gamec
+00001640: 7562 6543 6f6e 7472 6f6c 6c65 7252 6561  ubeControllerRea
+00001650: 6465 722e 435f 444f 574e 6301 0000 0000  der.C_DOWNc.....
+00001660: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00001670: 0000 0072 6900 0000 722d 0000 0029 0272  ...ri...r-...).r
+00001680: 5500 0000 7265 0000 0072 4a00 0000 7227  U...re...rJ...r'
+00001690: 0000 0072 2700 0000 7228 0000 0072 4400  ...r'...r(...rD.
+000016a0: 0000 bb00 0000 725b 0000 007a 1f47 616d  ......r[...z.Gam
+000016b0: 6563 7562 6543 6f6e 7472 6f6c 6c65 7252  ecubeControllerR
+000016c0: 6561 6465 722e 525f 4158 4953 6301 0000  eader.R_AXISc...
+000016d0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000016e0: 0043 0000 0072 6900 0000 722d 0000 0029  .C...ri...r-...)
+000016f0: 0272 5500 0000 7263 0000 0072 4a00 0000  .rU...rc...rJ...
+00001700: 7227 0000 0072 2700 0000 7228 0000 0072  r'...r'...r(...r
+00001710: 4500 0000 bf00 0000 725b 0000 007a 1f47  E.......r[...z.G
+00001720: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
+00001730: 7252 6561 6465 722e 4c5f 4158 4953 6301  rReader.L_AXISc.
+00001740: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001750: 0000 0043 0000 0072 5600 0000 7257 0000  ...C...rV...rW..
+00001760: 0029 0272 2f00 0000 da07 6765 745f 6861  .).r/.....get_ha
+00001770: 7472 4a00 0000 7227 0000 0072 2700 0000  trJ...r'...r'...
+00001780: 7228 0000 00da 065f 445f 5041 44c7 0000  r(....._D_PAD...
+00001790: 0072 5b00 0000 7a1f 4761 6d65 6375 6265  .r[...z.Gamecube
+000017a0: 436f 6e74 726f 6c6c 6572 5265 6164 6572  ControllerReader
+000017b0: 2e5f 445f 5041 4463 0100 0000 0000 0000  ._D_PADc........
+000017c0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000017d0: f30a 0000 007c 006a 0064 0119 0053 0072  .....|.j.d...S.r
+000017e0: 5700 0000 a901 726e 0000 0072 4a00 0000  W.....rn...rJ...
+000017f0: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
+00001800: 085f 445f 5041 445f 58cb 0000 00f3 0200  ._D_PAD_X.......
+00001810: 0000 0a02 7a21 4761 6d65 6375 6265 436f  ....z!GamecubeCo
+00001820: 6e74 726f 6c6c 6572 5265 6164 6572 2e5f  ntrollerReader._
+00001830: 445f 5041 445f 5863 0100 0000 0000 0000  D_PAD_Xc........
+00001840: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001850: 726f 0000 0072 5c00 0000 7270 0000 0072  ro...r\...rp...r
+00001860: 4a00 0000 7227 0000 0072 2700 0000 7228  J...r'...r'...r(
+00001870: 0000 00da 085f 445f 5041 445f 59cf 0000  ....._D_PAD_Y...
+00001880: 0072 7200 0000 7a21 4761 6d65 6375 6265  .rr...z!Gamecube
+00001890: 436f 6e74 726f 6c6c 6572 5265 6164 6572  ControllerReader
+000018a0: 2e5f 445f 5041 445f 5963 0100 0000 0000  ._D_PAD_Yc......
+000018b0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000018c0: 0000 f30e 0000 0074 007c 006a 0164 016b  .......t.|.j.d.k
+000018d0: 0083 0153 0072 5700 0000 a902 da03 696e  ...S.rW.......in
+000018e0: 7472 7100 0000 724a 0000 0072 2700 0000  trq...rJ...r'...
+000018f0: 7227 0000 0072 2800 0000 7246 0000 00d5  r'...r(...rF....
+00001900: 0000 0072 6800 0000 7a1f 4761 6d65 6375  ...rh...z.Gamecu
+00001910: 6265 436f 6e74 726f 6c6c 6572 5265 6164  beControllerRead
+00001920: 6572 2e44 5f4c 4546 5463 0100 0000 0000  er.D_LEFTc......
+00001930: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001940: 0000 f30e 0000 0074 007c 006a 0164 016b  .......t.|.j.d.k
+00001950: 0483 0153 0072 5700 0000 7275 0000 0072  ...S.rW...ru...r
+00001960: 4a00 0000 7227 0000 0072 2700 0000 7228  J...r'...r'...r(
+00001970: 0000 0072 4700 0000 d900 0000 7268 0000  ...rG.......rh..
+00001980: 007a 2047 616d 6563 7562 6543 6f6e 7472  .z GamecubeContr
+00001990: 6f6c 6c65 7252 6561 6465 722e 445f 5249  ollerReader.D_RI
+000019a0: 4748 5463 0100 0000 0000 0000 0000 0000  GHTc............
+000019b0: 0100 0000 0300 0000 4300 0000 7277 0000  ........C...rw..
+000019c0: 0072 5700 0000 a902 7276 0000 0072 7300  .rW.....rv...rs.
+000019d0: 0000 724a 0000 0072 2700 0000 7227 0000  ..rJ...r'...r'..
+000019e0: 0072 2800 0000 7248 0000 00dd 0000 0072  .r(...rH.......r
+000019f0: 6800 0000 7a1d 4761 6d65 6375 6265 436f  h...z.GamecubeCo
+00001a00: 6e74 726f 6c6c 6572 5265 6164 6572 2e44  ntrollerReader.D
+00001a10: 5f55 5063 0100 0000 0000 0000 0000 0000  _UPc............
+00001a20: 0100 0000 0300 0000 4300 0000 7274 0000  ........C...rt..
+00001a30: 0072 5700 0000 7278 0000 0072 4a00 0000  .rW...rx...rJ...
+00001a40: 7227 0000 0072 2700 0000 7228 0000 0072  r'...r'...r(...r
+00001a50: 4900 0000 e100 0000 7268 0000 007a 1f47  I.......rh...z.G
+00001a60: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
+00001a70: 7252 6561 6465 722e 445f 444f 574e 6301  rReader.D_DOWNc.
+00001a80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001a90: 0000 0043 0000 0072 5600 0000 7257 0000  ...C...rV...rW..
+00001aa0: 00a9 0272 2f00 0000 da0a 6765 745f 6275  ...r/.....get_bu
+00001ab0: 7474 6f6e 724a 0000 0072 2700 0000 7227  ttonrJ...r'...r'
+00001ac0: 0000 0072 2800 0000 7236 0000 00e9 0000  ...r(...r6......
+00001ad0: 0072 5b00 0000 7a1a 4761 6d65 6375 6265  .r[...z.Gamecube
+00001ae0: 436f 6e74 726f 6c6c 6572 5265 6164 6572  ControllerReader
+00001af0: 2e58 6301 0000 0000 0000 0000 0000 0001  .Xc.............
+00001b00: 0000 0003 0000 0043 0000 0072 5600 0000  .......C...rV...
+00001b10: 725c 0000 0072 7900 0000 724a 0000 0072  r\...ry...rJ...r
+00001b20: 2700 0000 7227 0000 0072 2800 0000 7234  '...r'...r(...r4
+00001b30: 0000 00ed 0000 0072 5b00 0000 7a1a 4761  .......r[...z.Ga
+00001b40: 6d65 6375 6265 436f 6e74 726f 6c6c 6572  mecubeController
+00001b50: 5265 6164 6572 2e41 6301 0000 0000 0000  Reader.Ac.......
+00001b60: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00001b70: 0072 5600 0000 7260 0000 0072 7900 0000  .rV...r`...ry...
+00001b80: 724a 0000 0072 2700 0000 7227 0000 0072  rJ...r'...r'...r
+00001b90: 2800 0000 7235 0000 00f1 0000 0072 5b00  (...r5.......r[.
+00001ba0: 0000 7a1a 4761 6d65 6375 6265 436f 6e74  ..z.GamecubeCont
+00001bb0: 726f 6c6c 6572 5265 6164 6572 2e42 6301  rollerReader.Bc.
+00001bc0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001bd0: 0000 0043 0000 0072 5600 0000 7262 0000  ...C...rV...rb..
+00001be0: 0072 7900 0000 724a 0000 0072 2700 0000  .ry...rJ...r'...
+00001bf0: 7227 0000 0072 2800 0000 7237 0000 00f5  r'...r(...r7....
+00001c00: 0000 0072 5b00 0000 7a1a 4761 6d65 6375  ...r[...z.Gamecu
+00001c10: 6265 436f 6e74 726f 6c6c 6572 5265 6164  beControllerRead
+00001c20: 6572 2e59 6301 0000 0000 0000 0000 0000  er.Yc...........
+00001c30: 0001 0000 0003 0000 0043 0000 0072 5600  .........C...rV.
+00001c40: 0000 7264 0000 0072 7900 0000 724a 0000  ..rd...ry...rJ..
+00001c50: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
+00001c60: 7239 0000 00f9 0000 0072 5b00 0000 7a1a  r9.......r[...z.
+00001c70: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
+00001c80: 6572 5265 6164 6572 2e4c 6301 0000 0000  erReader.Lc.....
+00001c90: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00001ca0: 0000 0072 5600 0000 725e 0000 0072 7900  ...rV...r^...ry.
+00001cb0: 0000 724a 0000 0072 2700 0000 7227 0000  ..rJ...r'...r'..
+00001cc0: 0072 2800 0000 723a 0000 00fd 0000 0072  .r(...r:.......r
+00001cd0: 5b00 0000 7a1a 4761 6d65 6375 6265 436f  [...z.GamecubeCo
+00001ce0: 6e74 726f 6c6c 6572 5265 6164 6572 2e52  ntrollerReader.R
+00001cf0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001d00: 0003 0000 0043 0000 0072 5600 0000 2902  .....C...rV...).
+00001d10: 4e72 0900 0000 7279 0000 0072 4a00 0000  Nr....ry...rJ...
+00001d20: 7227 0000 0072 2700 0000 7228 0000 0072  r'...r'...r(...r
+00001d30: 3800 0000 0101 0000 725b 0000 007a 1a47  8.......r[...z.G
+00001d40: 616d 6563 7562 6543 6f6e 7472 6f6c 6c65  amecubeControlle
+00001d50: 7252 6561 6465 722e 5a63 0100 0000 0000  rReader.Zc......
+00001d60: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001d70: 0000 7256 0000 0029 024e 720b 0000 0072  ..rV...).Nr....r
+00001d80: 7900 0000 724a 0000 0072 2700 0000 7227  y...rJ...r'...r'
+00001d90: 0000 0072 2800 0000 723b 0000 0005 0100  ...r(...r;......
+00001da0: 0072 5b00 0000 7a1e 4761 6d65 6375 6265  .r[...z.Gamecube
+00001db0: 436f 6e74 726f 6c6c 6572 5265 6164 6572  ControllerReader
+00001dc0: 2e53 5441 5254 4e29 2dda 085f 5f6e 616d  .STARTN)-..__nam
+00001dd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001de0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00001df0: 5f64 6f63 5f5f 724e 0000 0072 5200 0000  _doc__rN...rR...
+00001e00: 7254 0000 0072 7600 0000 7233 0000 0072  rT...rv...r3...r
+00001e10: 4b00 0000 7250 0000 0072 5300 0000 7255  K...rP...rS...rU
+00001e20: 0000 00da 0870 726f 7065 7274 7972 5a00  .....propertyrZ.
+00001e30: 0000 725d 0000 0072 5f00 0000 7261 0000  ..r]...r_...ra..
+00001e40: 0072 6300 0000 7265 0000 0072 3c00 0000  .rc...re...r<...
+00001e50: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
+00001e60: 4000 0000 7241 0000 0072 4200 0000 7243  @...rA...rB...rC
+00001e70: 0000 0072 4400 0000 7245 0000 0072 6e00  ...rD...rE...rn.
+00001e80: 0000 7271 0000 0072 7300 0000 7246 0000  ..rq...rs...rF..
+00001e90: 0072 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
+00001ea0: 7236 0000 0072 3400 0000 7235 0000 0072  r6...r4...r5...r
+00001eb0: 3700 0000 7239 0000 0072 3a00 0000 7238  7...r9...r:...r8
+00001ec0: 0000 0072 3b00 0000 7227 0000 0072 2700  ...r;...r'...r'.
+00001ed0: 0000 7227 0000 0072 2800 0000 722a 0000  ..r'...r(...r*..
+00001ee0: 003f 0000 0073 9000 0000 0800 0401 040d  .?...s..........
+00001ef0: 0401 0401 0e02 0804 081f 0803 0803 0207  ................
+00001f00: 0a01 0203 0a01 0203 0a01 0203 0a01 0203  ................
+00001f10: 0a01 0203 0a01 0205 0a01 0203 0a01 0203  ................
+00001f20: 0a01 0203 0a01 0203 0a01 0203 0a01 0203  ................
+00001f30: 0a01 0203 0a01 0203 0a01 0203 0a01 0207  ................
+00001f40: 0a01 0203 0a01 0203 0a01 0205 0a01 0203  ................
+00001f50: 0a01 0203 0a01 0203 0a01 0207 0a01 0203  ................
+00001f60: 0a01 0203 0a01 0203 0a01 0203 0a01 0203  ................
+00001f70: 0a01 0203 0a01 0203 0e01 722a 0000 0063  ..........r*...c
+00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f90: 0500 0000 4000 0000 7378 0000 0065 005a  ....@...sx...e.Z
+00001fa0: 0164 005a 0264 1864 0265 0364 0365 0466  .d.Z.d.d.e.d.e.f
+00001fb0: 0464 0464 0584 055a 0565 0664 0664 0784  .d.d...Z.e.d.d..
+00001fc0: 0083 015a 0765 0664 0864 0984 0083 015a  ...Z.e.d.d.....Z
+00001fd0: 0865 0664 0a64 0b84 0083 015a 0965 0664  .e.d.d.....Z.e.d
+00001fe0: 0c64 0d84 0083 015a 0a64 0e64 0f84 005a  .d.....Z.d.d...Z
+00001ff0: 0b64 1064 1184 005a 0c64 1264 1384 005a  .d.d...Z.d.d...Z
+00002000: 0d64 1464 1584 005a 0e64 1664 1784 005a  .d.d...Z.d.d...Z
+00002010: 0f64 0153 0029 19da 0b42 7574 746f 6e49  .d.S.)...ButtonI
+00002020: 6e70 7574 4eda 0269 64da 0670 6172 656e  nputN..id..paren
+00002030: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
+00002040: 0000 0200 0000 4300 0000 7310 0000 007c  ......C...s....|
+00002050: 017c 005f 007c 027c 005f 0164 0153 0029  .|._.|.|._.d.S.)
+00002060: 0261 e601 0000 0a20 2020 2020 2020 2043  .a.....        C
+00002070: 6c61 7373 2074 6f20 6465 7363 7269 6265  lass to describe
+00002080: 2061 2073 696e 676c 6520 696e 7075 7420   a single input 
+00002090: 6368 616e 6e65 6c20 6f6e 2061 206a 6f79  channel on a joy
+000020a0: 7374 6963 6b2f 636f 6e74 726f 6c6c 6572  stick/controller
+000020b0: 202d 2d20 652e 672e 2074 6865 2022 4122   -- e.g. the "A"
+000020c0: 2062 7574 746f 6e0a 2020 2020 2020 2020   button.        
+000020d0: 6f6e 2061 2067 616d 6563 7562 6520 636f  on a gamecube co
+000020e0: 6e74 726f 6c6c 6572 2e20 496d 706c 656d  ntroller. Implem
+000020f0: 656e 7473 206d 6574 686f 6473 2077 6869  ents methods whi
+00002100: 6368 2063 6865 636b 2077 6974 6820 7468  ch check with th
+00002110: 6520 7061 7265 6e74 2069 6e70 7574 2064  e parent input d
+00002120: 6576 6963 650a 2020 2020 2020 2020 7768  evice.        wh
+00002130: 6574 6865 7220 7468 6973 2062 7574 746f  ether this butto
+00002140: 6e20 6973 2070 7265 7373 6564 2c20 7265  n is pressed, re
+00002150: 6c65 6173 6564 2c20 6574 632e 2054 6869  leased, etc. Thi
+00002160: 7320 616c 6c6f 7773 2066 6f72 2074 6865  s allows for the
+00002170: 206d 6f72 6520 706c 6561 7361 6e74 2073   more pleasant s
+00002180: 686f 7274 6861 6e64 3a0a 2020 2020 2020  horthand:.      
+00002190: 2020 6063 6f6e 7472 6f6c 6c65 722e 615f    `controller.a_
+000021a0: 6275 7474 6f6e 2e69 735f 7072 6573 7365  button.is_presse
+000021b0: 6460 2069 6e73 7465 6164 206f 6620 6063  d` instead of `c
+000021c0: 6f6e 7472 6f6c 6c65 722e 6973 5f70 7265  ontroller.is_pre
+000021d0: 7373 6564 2863 6f6e 7472 6f6c 6c65 722e  ssed(controller.
+000021e0: 615f 6275 7474 6f6e 2960 0a0a 2020 2020  a_button)`..    
+000021f0: 2020 2020 3a70 6172 616d 2069 6e74 2069      :param int i
+00002200: 643a 2069 6e64 6578 206f 6620 7468 6973  d: index of this
+00002210: 2069 6e70 7574 2063 6861 6e6e 656c 2069   input channel i
+00002220: 6e20 7468 6520 636f 6e74 726f 6c6c 6572  n the controller
+00002230: 2e67 6574 5f76 616c 7565 7328 2920 7475  .get_values() tu
+00002240: 706c 650a 2020 2020 2020 2020 4e29 0272  ple.        N).r
+00002250: 8100 0000 7282 0000 0029 0372 3200 0000  ....r....).r2...
+00002260: 7281 0000 0072 8200 0000 7227 0000 0072  r....r....r'...r
+00002270: 2700 0000 7228 0000 0072 3300 0000 0b01  '...r(...r3.....
+00002280: 0000 7304 0000 0006 090a 017a 1442 7574  ..s........z.But
+00002290: 746f 6e49 6e70 7574 2e5f 5f69 6e69 745f  tonInput.__init_
+000022a0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000022b0: 0000 0300 0000 4300 0000 f30e 0000 007c  ......C........|
+000022c0: 006a 00a0 017c 006a 02a1 0153 0072 2d00  .j...|.j...S.r-.
+000022d0: 0000 2903 7282 0000 00da 0769 735f 646f  ..).r......is_do
+000022e0: 776e 7281 0000 0072 4a00 0000 7227 0000  wnr....rJ...r'..
+000022f0: 0072 2700 0000 7228 0000 0072 8400 0000  .r'...r(...r....
+00002300: 1701 0000 7268 0000 007a 1342 7574 746f  ....rh...z.Butto
+00002310: 6e49 6e70 7574 2e69 735f 646f 776e 6301  nInput.is_downc.
+00002320: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00002330: 0000 0043 0000 0072 8300 0000 722d 0000  ...C...r....r-..
+00002340: 0029 0372 8200 0000 da0a 6973 5f70 7265  .).r......is_pre
+00002350: 7373 6564 7281 0000 0072 4a00 0000 7227  ssedr....rJ...r'
+00002360: 0000 0072 2700 0000 7228 0000 0072 8500  ...r'...r(...r..
+00002370: 0000 1b01 0000 7268 0000 007a 1642 7574  ......rh...z.But
+00002380: 746f 6e49 6e70 7574 2e69 735f 7072 6573  tonInput.is_pres
+00002390: 7365 6463 0100 0000 0000 0000 0000 0000  sedc............
+000023a0: 0100 0000 0300 0000 4300 0000 7283 0000  ........C...r...
+000023b0: 0072 2d00 0000 2903 7282 0000 00da 0b69  .r-...).r......i
+000023c0: 735f 7265 6c65 6173 6564 7281 0000 0072  s_releasedr....r
+000023d0: 4a00 0000 7227 0000 0072 2700 0000 7228  J...r'...r'...r(
+000023e0: 0000 0072 8600 0000 1f01 0000 7268 0000  ...r........rh..
+000023f0: 007a 1742 7574 746f 6e49 6e70 7574 2e69  .z.ButtonInput.i
+00002400: 735f 7265 6c65 6173 6564 6301 0000 0000  s_releasedc.....
+00002410: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00002420: 0000 0073 0600 0000 7c00 6a00 5300 2901  ...s....|.j.S.).
+00002430: 7a8c 446f 6573 2074 6865 2073 616d 6520  z.Does the same 
+00002440: 7468 696e 6720 6173 2069 735f 646f 776e  thing as is_down
+00002450: 2062 7574 206d 616b 6573 2073 6f6d 6520   but makes some 
+00002460: 7061 7274 7320 6f66 2074 6865 2063 6f64  parts of the cod
+00002470: 6520 6d6f 7265 2072 6561 6461 626c 652c  e more readable,
+00002480: 0a20 2020 2020 2020 2065 7370 6563 6961  .        especia
+00002490: 6c6c 7920 666f 7220 616e 616c 6f67 2069  lly for analog i
+000024a0: 6e70 7574 7320 7468 6174 2063 616e 2062  nputs that can b
+000024b0: 6520 6265 7477 6565 6e20 302d 312e 2901  e between 0-1.).
+000024c0: 7284 0000 0072 4a00 0000 7227 0000 0072  r....rJ...r'...r
+000024d0: 2700 0000 7228 0000 00da 0576 616c 7565  '...r(.....value
+000024e0: 2301 0000 7302 0000 0006 047a 1142 7574  #...s......z.But
+000024f0: 746f 6e49 6e70 7574 2e76 616c 7565 6302  tonInput.valuec.
+00002500: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002510: 0000 0043 0000 00f3 1000 0000 7c00 6a00  ...C........|.j.
+00002520: a001 7c00 6a02 7c01 a102 5300 722d 0000  ..|.j.|...S.r-..
+00002530: 0029 0372 8200 0000 da10 6275 6666 6572  .).r......buffer
+00002540: 6564 5f70 7265 7373 6573 7281 0000 00a9  ed_pressesr.....
+00002550: 0272 3200 0000 da0d 6275 6666 6572 5f6c  .r2.....buffer_l
+00002560: 656e 6774 6872 2700 0000 7227 0000 0072  engthr'...r'...r
+00002570: 2800 0000 7289 0000 0029 0100 00f3 0200  (...r....)......
+00002580: 0000 1001 7a1c 4275 7474 6f6e 496e 7075  ....z.ButtonInpu
+00002590: 742e 6275 6666 6572 6564 5f70 7265 7373  t.buffered_press
+000025a0: 6573 6302 0000 0000 0000 0000 0000 0002  esc.............
+000025b0: 0000 0004 0000 0043 0000 0072 8800 0000  .......C...r....
+000025c0: 722d 0000 0029 0372 8200 0000 da11 6275  r-...).r......bu
+000025d0: 6666 6572 6564 5f72 656c 6561 7365 7372  ffered_releasesr
+000025e0: 8100 0000 728a 0000 0072 2700 0000 7227  ....r....r'...r'
+000025f0: 0000 0072 2800 0000 728d 0000 002c 0100  ...r(...r....,..
+00002600: 0072 8c00 0000 7a1d 4275 7474 6f6e 496e  .r....z.ButtonIn
+00002610: 7075 742e 6275 6666 6572 6564 5f72 656c  put.buffered_rel
+00002620: 6561 7365 7363 0200 0000 0000 0000 0000  easesc..........
+00002630: 0000 0200 0000 0400 0000 4300 0000 731c  ..........C...s.
+00002640: 0000 007c 006a 0074 017c 0174 0283 0272  ...|.j.t.|.t...r
+00002650: 0b7c 016a 0018 0053 007c 0118 0053 0072  .|.j...S.|...S.r
+00002660: 2d00 0000 a903 7287 0000 00da 0a69 7369  -.....r......isi
+00002670: 6e73 7461 6e63 6572 8000 0000 a902 7232  nstancer......r2
+00002680: 0000 00da 056f 7468 6572 7227 0000 0072  .....otherr'...r
+00002690: 2700 0000 7228 0000 00da 075f 5f73 7562  '...r(.....__sub
+000026a0: 5f5f 2f01 0000 f302 0000 001c 017a 1342  __/..........z.B
+000026b0: 7574 746f 6e49 6e70 7574 2e5f 5f73 7562  uttonInput.__sub
+000026c0: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
+000026d0: 0000 0004 0000 0043 0000 0073 1c00 0000  .......C...s....
+000026e0: 7c00 6a00 7401 7c01 7402 8302 720b 7c01  |.j.t.|.t...r.|.
+000026f0: 6a00 1700 5300 7c01 1700 5300 722d 0000  j...S.|...S.r-..
+00002700: 0072 8e00 0000 7290 0000 0072 2700 0000  .r....r....r'...
+00002710: 7227 0000 0072 2800 0000 da07 5f5f 6164  r'...r(.....__ad
+00002720: 645f 5f32 0100 0072 9300 0000 7a13 4275  d__2...r....z.Bu
+00002730: 7474 6f6e 496e 7075 742e 5f5f 6164 645f  ttonInput.__add_
+00002740: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00002750: 0000 0200 0000 4300 0000 730a 0000 0074  ......C...s....t
+00002760: 007c 006a 0183 0153 0029 017a 4354 6869  .|.j...S.).zCThi
+00002770: 7320 616c 6c6f 7773 2075 7320 746f 2064  s allows us to d
+00002780: 6f20 6069 6620 696e 7075 742e 5550 6020  o `if input.UP` 
+00002790: 696e 7374 6561 6420 6f66 2060 6966 2069  instead of `if i
+000027a0: 6e70 7574 2e55 502e 6973 5f64 6f77 6e60  nput.UP.is_down`
+000027b0: 2902 da04 626f 6f6c 7287 0000 0072 4a00  )...boolr....rJ.
+000027c0: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
+000027d0: 00da 085f 5f62 6f6f 6c5f 5f35 0100 0072  ...__bool__5...r
+000027e0: 7200 0000 7a14 4275 7474 6f6e 496e 7075  r...z.ButtonInpu
+000027f0: 742e 5f5f 626f 6f6c 5f5f 722d 0000 0029  t.__bool__r-...)
+00002800: 1072 7b00 0000 727c 0000 0072 7d00 0000  .r{...r|...r}...
+00002810: 7276 0000 0072 0200 0000 7233 0000 0072  rv...r....r3...r
+00002820: 7f00 0000 7284 0000 0072 8500 0000 7286  ....r....r....r.
+00002830: 0000 0072 8700 0000 7289 0000 0072 8d00  ...r....r....r..
+00002840: 0000 7292 0000 0072 9400 0000 7296 0000  ..r....r....r...
+00002850: 0072 2700 0000 7227 0000 0072 2700 0000  .r'...r'...r'...
+00002860: 7228 0000 0072 8000 0000 0a01 0000 731e  r(...r........s.
+00002870: 0000 0008 0014 0102 0c0a 0102 030a 0102  ................
+00002880: 030a 0102 030a 0108 0508 0308 0308 030c  ................
+00002890: 0372 8000 0000 6300 0000 0000 0000 0000  .r....c.........
+000028a0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+000028b0: 2600 0000 6500 5a01 6400 5a02 6401 5a03  &...e.Z.d.Z.d.Z.
+000028c0: 6402 5a04 6505 6403 6506 6602 6404 6405  d.Z.e.d.e.f.d.d.
+000028d0: 8404 8301 5a07 6406 5300 2907 da09 4178  ....Z.d.S.)...Ax
+000028e0: 6973 496e 7075 7467 cdcc cccc cccc ec3f  isInputg.......?
+000028f0: 7205 0000 00da 0672 6574 7572 6e63 0100  r......returnc..
+00002900: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002910: 0000 0300 0000 734c 0000 0074 0088 006a  ......sL...t...j
+00002920: 0183 0164 0188 006a 0218 0064 0085 0219  ...d...j...d....
+00002930: 007d 0187 0066 0164 0264 0384 087c 0144  .}...f.d.d...|.D
+00002940: 0083 017d 017c 0172 247c 0164 0119 0088  ...}.|.r$|.d....
+00002950: 006a 036b 056f 237c 0164 0419 0064 056b  .j.k.o#|.d...d.k
+00002960: 0153 0064 0653 0029 074e e9ff ffff ff63  .S.d.S.).N.....c
+00002970: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002980: 0400 0000 1300 0000 7316 0000 0067 007c  ........s....g.|
+00002990: 005d 077d 017c 0188 006a 0019 0091 0271  .].}.|...j.....q
+000029a0: 0253 0072 2700 0000 2901 7281 0000 0029  .S.r'...).r....)
+000029b0: 02da 022e 30da 0669 6e70 7574 7372 4a00  ....0..inputsrJ.
+000029c0: 0000 7227 0000 0072 2800 0000 da0a 3c6c  ..r'...r(.....<l
+000029d0: 6973 7463 6f6d 703e 4101 0000 7302 0000  istcomp>A...s...
+000029e0: 0016 007a 2841 7869 7349 6e70 7574 2e69  ...z(AxisInput.i
+000029f0: 735f 736d 6173 6865 642e 3c6c 6f63 616c  s_smashed.<local
+00002a00: 733e 2e3c 6c69 7374 636f 6d70 3e72 0100  s>.<listcomp>r..
+00002a10: 0000 722b 0000 0046 2904 da04 6c69 7374  ..r+...F)...list
+00002a20: 7282 0000 00da 0c73 6d61 7368 5f77 696e  r......smash_win
+00002a30: 646f 77da 0f73 6d61 7368 5f74 6872 6573  dow..smash_thres
+00002a40: 686f 6c64 2902 7232 0000 00da 0768 6973  hold).r2.....his
+00002a50: 746f 7279 7227 0000 0072 4a00 0000 7228  toryr'...rJ...r(
+00002a60: 0000 00da 0a69 735f 736d 6173 6865 643e  .....is_smashed>
+00002a70: 0100 0073 0a00 0000 1802 1201 0401 1a01  ...s............
+00002a80: 0402 7a14 4178 6973 496e 7075 742e 6973  ..z.AxisInput.is
+00002a90: 5f73 6d61 7368 6564 4e29 0872 7b00 0000  _smashedN).r{...
+00002aa0: 727c 0000 0072 7d00 0000 729f 0000 0072  r|...r}...r....r
+00002ab0: 9e00 0000 727f 0000 0072 9500 0000 72a1  ....r....r....r.
+00002ac0: 0000 0072 2700 0000 7227 0000 0072 2700  ...r'...r'...r'.
+00002ad0: 0000 7228 0000 0072 9700 0000 3a01 0000  ..r(...r....:...
+00002ae0: 730a 0000 0008 0004 0104 0102 0214 0172  s..............r
+00002af0: 9700 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00002b00: 0000 0000 0005 0000 0000 0000 0073 e000  .............s..
+00002b10: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00002b20: 6505 8301 5a05 6504 6506 8301 5a06 6504  e...Z.e.e...Z.e.
+00002b30: 6507 8301 5a07 6504 6508 8301 5a08 6509  e...Z.e.e...Z.e.
+00002b40: 650a 8301 5a0a 6509 650b 8301 5a0b 6509  e...Z.e.e...Z.e.
+00002b50: 650c 8301 5a0c 6509 650d 8301 5a0d 6509  e...Z.e.e...Z.e.
+00002b60: 650e 8301 5a0e 6504 650f 8301 5a0f 6504  e...Z.e.e...Z.e.
+00002b70: 6510 8301 5a10 6504 6511 8301 5a11 6504  e...Z.e.e...Z.e.
+00002b80: 6512 8301 5a12 6509 6513 8301 5a13 6509  e...Z.e.e...Z.e.
+00002b90: 6514 8301 5a15 6509 6516 8301 5a17 6509  e...Z.e.e...Z.e.
+00002ba0: 6518 8301 5a19 6509 651a 8301 5a1b 6509  e...Z.e.e...Z.e.
+00002bb0: 651c 8301 5a1c 6509 651d 8301 5a1d 6509  e...Z.e.e...Z.e.
+00002bc0: 651e 8301 5a1e 6509 651f 8301 5a1f 6408  e...Z.e.e...Z.d.
+00002bd0: 6403 6520 6602 8700 6601 6404 6405 840d  d.e f...f.d.d...
+00002be0: 5a21 6406 6407 8400 5a22 8700 0400 5a23  Z!d.d...Z"....Z#
+00002bf0: 5300 2909 da12 4761 6d65 6375 6265 436f  S.)...GamecubeCo
+00002c00: 6e74 726f 6c6c 6572 613e 0100 000a 2020  ntrollera>....  
+00002c10: 2020 4120 7772 6170 7065 7220 6172 6f75    A wrapper arou
+00002c20: 6e64 2047 616d 6563 7562 6543 6f6e 7472  nd GamecubeContr
+00002c30: 6f6c 6c65 7252 6561 6465 7220 616e 6420  ollerReader and 
+00002c40: 496e 7075 7451 7565 7565 2077 6869 6368  InputQueue which
+00002c50: 206c 6561 7665 7320 616c 6c20 7468 6520   leaves all the 
+00002c60: 6669 6464 6c79 0a20 2020 2069 6e70 7574  fiddly.    input
+00002c70: 2d72 6561 6469 6e67 206c 6f67 6963 2074  -reading logic t
+00002c80: 6f20 4761 6d65 6375 6265 436f 6e74 726f  o GamecubeContro
+00002c90: 6c6c 6572 5265 6164 6572 2c20 616e 6420  llerReader, and 
+00002ca0: 7072 6f76 6964 6573 2061 2063 6f6e 7665  provides a conve
+00002cb0: 6e69 656e 7420 696e 7465 7266 6163 6520  nient interface 
+00002cc0: 666f 720a 2020 2020 6163 6365 7373 696e  for.    accessin
+00002cd0: 6720 7468 6520 7175 6575 6520 6f66 2069  g the queue of i
+00002ce0: 6e70 7574 732e 0a0a 2020 2020 5468 6973  nputs...    This
+00002cf0: 2061 6c6c 6f77 7320 6761 6d65 7320 746f   allows games to
+00002d00: 2073 7562 636c 6173 7320 7468 6973 2063   subclass this c
+00002d10: 6c61 7373 2061 6e64 2064 6566 696e 6520  lass and define 
+00002d20: 6e65 7720 6b65 7920 6d61 7070 696e 6773  new key mappings
+00002d30: 2065 2e67 2e20 2241 2220 2d2d 3e20 2261   e.g. "A" --> "a
+00002d40: 7474 6163 6b22 0a20 2020 20e9 3c00 0000  ttack".    .<...
+00002d50: da0d 636f 6e74 726f 6c6c 6572 5f69 6463  ..controller_idc
+00002d60: 0300 0000 0000 0000 0000 0000 0800 0000  ................
+00002d70: 0500 0000 0300 0000 7364 0000 0074 007c  ........sd...t.|
+00002d80: 0183 017d 037c 017c 005f 017c 037c 005f  ...}.|.|._.|.|._
+00002d90: 0274 0383 00a0 047c 02a1 0101 0064 0164  .t.....|.....d.d
+00002da0: 0284 007c 006a 056a 0644 0083 017d 047c  ...|.j.j.D...}.|
+00002db0: 04a0 07a1 0044 005d 125c 027d 057d 067c  .....D.].\.}.}.|
+00002dc0: 066a 057c 066a 087c 0064 038d 027d 0774  .j.|.j.|.d...}.t
+00002dd0: 097c 007c 057c 0783 0301 0071 1d64 0053  .|.|.|.....q.d.S
+00002de0: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00002df0: 0004 0000 0006 0000 0053 0000 0073 3a00  .........S...s:.
+00002e00: 0000 6900 7c00 5d19 7d01 7c01 6a00 a001  ..i.|.].}.|.j...
+00002e10: a100 4400 5d11 5c02 7d02 7d03 7402 7c01  ..D.].\.}.}.t.|.
+00002e20: 7403 8302 7209 7404 7c03 7405 8302 7209  t...r.t.|.t...r.
+00002e30: 7c02 7c03 9303 7109 7102 5300 7227 0000  |.|...q.q.S.r'..
+00002e40: 0029 06da 085f 5f64 6963 745f 5fda 0569  .)...__dict__..i
+00002e50: 7465 6d73 da0a 6973 7375 6263 6c61 7373  tems..issubclass
+00002e60: 72a2 0000 0072 8f00 0000 7280 0000 0029  r....r....r....)
+00002e70: 0472 9a00 0000 da06 5f63 6c61 7373 da04  .r......_class..
+00002e80: 6e61 6d65 da04 6174 7472 7227 0000 0072  name..attrr'...r
+00002e90: 2700 0000 7228 0000 00da 0a3c 6469 6374  '...r(.....<dict
+00002ea0: 636f 6d70 3e71 0100 0073 1600 0000 0600  comp>q...s......
+00002eb0: 0202 0801 04fd 0603 0801 02fc 0804 02fc  ................
+00002ec0: 0401 08ff 7a2f 4761 6d65 6375 6265 436f  ....z/GamecubeCo
+00002ed0: 6e74 726f 6c6c 6572 2e5f 5f69 6e69 745f  ntroller.__init_
+00002ee0: 5f2e 3c6c 6f63 616c 733e 2e3c 6469 6374  _.<locals>.<dict
+00002ef0: 636f 6d70 3e29 0172 8200 0000 290a 722a  comp>).r....).r*
+00002f00: 0000 0072 a400 0000 da0a 636f 6e74 726f  ...r......contro
+00002f10: 6c6c 6572 da05 7375 7065 7272 3300 0000  ller..superr3...
+00002f20: da09 5f5f 636c 6173 735f 5fda 075f 5f6d  ..__class__..__m
+00002f30: 726f 5f5f 72a6 0000 0072 8100 0000 da07  ro__r....r......
+00002f40: 7365 7461 7474 7229 0872 3200 0000 72a4  setattr).r2...r.
+00002f50: 0000 00da 0c71 7565 7565 5f6c 656e 6774  .....queue_lengt
+00002f60: 6872 ac00 0000 da0d 6275 7474 6f6e 5f69  hr......button_i
+00002f70: 6e70 7574 7372 a900 0000 72aa 0000 00da  nputsr....r.....
+00002f80: 0369 6e70 a901 72ae 0000 0072 2700 0000  .inp..r....r'...
+00002f90: 7228 0000 0072 3300 0000 6901 0000 7316  r(...r3...i...s.
+00002fa0: 0000 0008 0106 0106 010c 0106 0406 0206  ................
+00002fb0: fe10 0610 010e 0104 fe7a 1b47 616d 6563  .........z.Gamec
+00002fc0: 7562 6543 6f6e 7472 6f6c 6c65 722e 5f5f  ubeController.__
+00002fd0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00002fe0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00002ff0: 0a00 0000 7c00 6a00 a001 a100 5300 722d  ....|.j.....S.r-
+00003000: 0000 0029 0272 ac00 0000 724b 0000 0072  ...).r....rK...r
+00003010: 4a00 0000 7227 0000 0072 2700 0000 7228  J...r'...r'...r(
+00003020: 0000 00da 0e67 6574 5f6e 6577 5f76 616c  .....get_new_val
+00003030: 7565 737b 0100 0073 0200 0000 0a01 7a21  ues{...s......z!
+00003040: 4761 6d65 6375 6265 436f 6e74 726f 6c6c  GamecubeControll
+00003050: 6572 2e67 6574 5f6e 6577 5f76 616c 7565  er.get_new_value
+00003060: 7329 0172 a300 0000 2924 727b 0000 0072  s).r....)$r{...r
+00003070: 7c00 0000 727d 0000 0072 7e00 0000 7297  |...r}...r~...r.
+00003080: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
+00003090: 0000 723f 0000 0072 8000 0000 7234 0000  ..r?...r....r4..
+000030a0: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+000030b0: 7238 0000 0072 4200 0000 7243 0000 0072  r8...rB...rC...r
+000030c0: 4000 0000 7241 0000 0072 3b00 0000 7248  @...rA...r;...rH
+000030d0: 0000 00da 0844 5f50 4144 5f55 5072 4600  .....D_PAD_UPrF.
+000030e0: 0000 da0a 445f 5041 445f 4c45 4654 7247  ....D_PAD_LEFTrG
+000030f0: 0000 00da 0b44 5f50 4144 5f52 4947 4854  .....D_PAD_RIGHT
+00003100: 7249 0000 00da 0a44 5f50 4144 5f44 4f57  rI.....D_PAD_DOW
+00003110: 4e72 3900 0000 723a 0000 0072 4500 0000  Nr9...r:...rE...
+00003120: 7244 0000 0072 7600 0000 7233 0000 0072  rD...rv...r3...r
+00003130: b500 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00003140: 6c5f 5f72 2700 0000 7227 0000 0072 b400  l__r'...r'...r..
+00003150: 0000 7228 0000 0072 a200 0000 4801 0000  ..r(...r....H...
+00003160: 7334 0000 0008 0004 0108 0908 0108 0108  s4..............
+00003170: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003180: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003190: 0108 0108 0114 0210 1272 a200 0000 da08  .........r......
+000031a0: 5f5f 6d61 696e 5f5f 6300 0000 0000 0000  __main__c.......
+000031b0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+000031c0: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
+000031d0: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+000031e0: 6406 8400 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
+000031f0: 640a 8400 5a07 640b 5300 290c da09 5465  d...Z.d.S.)...Te
+00003200: 7874 5072 696e 7463 0100 0000 0000 0000  xtPrintc........
+00003210: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00003220: 7326 0000 007c 00a0 00a1 0001 0074 016a  s&...|.......t.j
+00003230: 02a0 03a1 0001 0074 016a 02a0 0464 0064  .......t.j...d.d
+00003240: 01a1 027c 005f 0264 0053 0029 024e e91e  ...|._.d.S.).N..
+00003250: 0000 0029 05da 0572 6573 6574 722e 0000  ...)...resetr...
+00003260: 00da 0466 6f6e 7472 3100 0000 da04 466f  ...fontr1.....Fo
+00003270: 6e74 724a 0000 0072 2700 0000 7227 0000  ntrJ...r'...r'..
+00003280: 0072 2800 0000 7233 0000 0083 0100 0073  .r(...r3.......s
+00003290: 0600 0000 0801 0a01 1401 7a12 5465 7874  ..........z.Text
+000032a0: 5072 696e 742e 5f5f 696e 6974 5f5f 6303  Print.__init__c.
+000032b0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000032c0: 0000 0043 0000 0073 3800 0000 7c00 6a00  ...C...s8...|.j.
+000032d0: a001 7c02 6401 7402 a103 7d03 7c01 a003  ..|.d.t...}.|...
+000032e0: 7c03 7c00 6a04 7c00 6a05 6602 a102 0100  |.|.j.|.j.f.....
+000032f0: 7c00 0400 6a05 7c00 6a06 3700 0200 5f05  |...j.|.j.7..._.
+00003300: 6400 5300 2902 4e54 2907 72bf 0000 00da  d.S.).NT).r.....
+00003310: 0672 656e 6465 72da 0542 4c41 434b da04  .render..BLACK..
+00003320: 626c 6974 da01 78da 0179 da0b 6c69 6e65  blit..x..y..line
+00003330: 5f68 6569 6768 7429 0472 3200 0000 da06  _height).r2.....
+00003340: 7363 7265 656e da0a 7465 7874 5374 7269  screen..textStri
+00003350: 6e67 da0a 7465 7874 4269 746d 6170 7227  ng..textBitmapr'
+00003360: 0000 0072 2700 0000 7228 0000 00da 0674  ...r'...r(.....t
+00003370: 7072 696e 7488 0100 0073 0600 0000 1001  print....s......
+00003380: 1401 1401 7a10 5465 7874 5072 696e 742e  ....z.TextPrint.
+00003390: 7470 7269 6e74 6301 0000 0000 0000 0000  tprintc.........
+000033a0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000033b0: 1600 0000 6401 7c00 5f00 6401 7c00 5f01  ....d.|._.d.|._.
+000033c0: 6402 7c00 5f02 6400 5300 2903 4e72 0c00  d.|._.d.S.).Nr..
+000033d0: 0000 7216 0000 0029 0372 c400 0000 72c5  ..r....).r....r.
+000033e0: 0000 0072 c600 0000 724a 0000 0072 2700  ...r....rJ...r'.
+000033f0: 0000 7227 0000 0072 2800 0000 72be 0000  ..r'...r(...r...
+00003400: 008d 0100 0073 0600 0000 0601 0601 0a01  .....s..........
+00003410: 7a0f 5465 7874 5072 696e 742e 7265 7365  z.TextPrint.rese
+00003420: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00003430: 0000 0300 0000 4300 0000 7312 0000 007c  ......C...s....|
+00003440: 0004 006a 0064 0137 0002 005f 0064 0053  ...j.d.7..._.d.S
+00003450: 00a9 024e 720c 0000 00a9 0172 c400 0000  ...Nr......r....
+00003460: 724a 0000 0072 2700 0000 7227 0000 0072  rJ...r'...r'...r
+00003470: 2800 0000 da06 696e 6465 6e74 9201 0000  (.....indent....
+00003480: f302 0000 0012 017a 1054 6578 7450 7269  .......z.TextPri
+00003490: 6e74 2e69 6e64 656e 7463 0100 0000 0000  nt.indentc......
+000034a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000034b0: 0000 7312 0000 007c 0004 006a 0064 0138  ..s....|...j.d.8
+000034c0: 0002 005f 0064 0053 0072 cb00 0000 72cc  ..._.d.S.r....r.
+000034d0: 0000 0072 4a00 0000 7227 0000 0072 2700  ...rJ...r'...r'.
+000034e0: 0000 7228 0000 00da 0875 6e69 6e64 656e  ..r(.....uninden
+000034f0: 7495 0100 0072 ce00 0000 7a12 5465 7874  t....r....z.Text
+00003500: 5072 696e 742e 756e 696e 6465 6e74 4e29  Print.unindentN)
+00003510: 0872 7b00 0000 727c 0000 0072 7d00 0000  .r{...r|...r}...
+00003520: 7233 0000 0072 ca00 0000 72be 0000 0072  r3...r....r....r
+00003530: cd00 0000 72cf 0000 0072 2700 0000 7227  ....r....r'...r'
+00003540: 0000 0072 2700 0000 7228 0000 0072 bc00  ...r'...r(...r..
+00003550: 0000 8201 0000 730c 0000 0008 0008 0108  ......s.........
+00003560: 0508 0508 050c 0372 bc00 0000 da05 626c  .......r......bl
+00003570: 6163 6bda 0577 6869 7465 2902 69f4 0100  ack..white).i...
+00003580: 0069 bc02 0000 7a07 4d79 2047 616d 6546  .i....z.My GameF
+00003590: 2901 722c 0000 007a 1547 616d 6563 7562  ).r,...z.Gamecub
+000035a0: 6520 636f 6e74 726f 6c6c 6572 2030 7a08  e controller 0z.
+000035b0: 4275 7474 6f6e 733a 7a13 4120 4220 5820  Buttons:z.A B X 
+000035c0: 5920 5a20 4c20 5220 5354 4152 547a 023a  Y Z L R STARTz.:
+000035d0: 207a 0541 7865 733a 7a70 5f4c 5f54 5249   z.Axes:zp_L_TRI
+000035e0: 4747 4552 5f41 5849 5320 5f52 5f54 5249  GGER_AXIS _R_TRI
+000035f0: 4747 4552 5f41 5849 5320 5f47 5245 595f  GGER_AXIS _GREY_
+00003600: 5354 4943 4b5f 585f 4158 4953 205f 4752  STICK_X_AXIS _GR
+00003610: 4559 5f53 5449 434b 5f59 5f41 5849 5320  EY_STICK_Y_AXIS 
+00003620: 5f59 454c 4c4f 575f 5354 4943 4b5f 585f  _YELLOW_STICK_X_
+00003630: 4158 4953 205f 5945 4c4c 4f57 5f53 5449  AXIS _YELLOW_STI
+00003640: 434b 5f59 5f41 5849 5320 7a05 4861 7473  CK_Y_AXIS z.Hats
+00003650: 3a72 6e00 0000 7a11 5052 4f43 4553 5345  :rn...z.PROCESSE
+00003660: 4420 494e 5055 5453 3a7a 574c 4546 5420  D INPUTS:zWLEFT 
+00003670: 5249 4748 5420 5550 2044 4f57 4e20 435f  RIGHT UP DOWN C_
+00003680: 4c45 4654 2043 5f52 4947 4854 2043 5f55  LEFT C_RIGHT C_U
+00003690: 5020 435f 444f 574e 2052 5f41 5849 5320  P C_DOWN R_AXIS 
+000036a0: 4c5f 4158 4953 2044 5f4c 4546 5420 445f  L_AXIS D_LEFT D_
+000036b0: 5249 4748 5420 445f 5550 2044 5f44 4f57  RIGHT D_UP D_DOW
+000036c0: 4e20 2901 5429 4072 7e00 0000 722e 0000  N ).T)@r~...r...
+000036d0: 00da 1572 6f62 696e 6761 6d65 2e69 6e70  ...robingame.inp
+000036e0: 7574 2e71 7565 7565 7202 0000 0072 3400  ut.queuer....r4.
+000036f0: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
+00003700: 0072 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
+00003710: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
+00003720: 3e00 0000 723f 0000 0072 4000 0000 7241  >...r?...r@...rA
+00003730: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00003740: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
+00003750: 0072 4800 0000 7249 0000 0072 2900 0000  .rH...rI...r)...
+00003760: 722a 0000 0072 8000 0000 7297 0000 0072  r*...r....r....r
+00003770: a200 0000 727b 0000 00da 066f 626a 6563  ....r{.....objec
+00003780: 7472 bc00 0000 da05 436f 6c6f 7272 c200  tr......Colorr..
+00003790: 0000 da05 5748 4954 4572 2f00 0000 7231  ....WHITEr/...r1
+000037a0: 0000 00da 0974 6578 7450 7269 6e74 da07  .....textPrint..
+000037b0: 6469 7370 6c61 79da 0873 6574 5f6d 6f64  display..set_mod
+000037c0: 6572 c700 0000 da0b 7365 745f 6361 7074  er......set_capt
+000037d0: 696f 6eda 0474 696d 65da 0543 6c6f 636b  ion..time..Clock
+000037e0: da05 636c 6f63 6bda 0464 6f6e 65da 0565  ..clock..done..e
+000037f0: 7665 6e74 da03 6765 74da 0474 7970 65da  vent..get..type.
+00003800: 0451 5549 54da 0466 696c 6c72 be00 0000  .QUIT..fillr....
+00003810: 72ac 0000 0072 cd00 0000 72ca 0000 00da  r....r....r.....
+00003820: 0573 706c 6974 da06 6275 7474 6f6e da07  .split..button..
+00003830: 6765 7461 7474 7272 cf00 0000 da04 666c  getattrr......fl
+00003840: 6970 da04 7469 636b da04 7175 6974 7227  ip..tick..quitr'
+00003850: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+00003860: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00003870: 73a2 0000 0004 0008 0a0c 0204 0504 0104  s...............
+00003880: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003890: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+000038a0: 0104 0104 0104 010a 030e 1500 7f0e 4c10  ..............L.
+000038b0: 3010 0e0a 3702 0110 020a 160a 010a 0206  0...7...........
+000038c0: 010c 020c 010a 0104 0106 010e 010c 0104  ................
+000038d0: 0102 800a 0208 010a 0108 020c 010c 0208  ................
+000038e0: 010c 011e 0108 010c 0208 0102 0204 0406  ................
+000038f0: fb1e 0608 010c 0208 010c 0120 0108 010c  ........... ....
+00003900: 0208 0102 0204 0406 fb20 0608 010a 030a  ......... ......
+00003910: 0304 ce0c 3404 a9                        ....4..
```

### Comparing `robingame-0.0.9/robingame/input/__pycache__/keyboard.cpython-310.pyc` & `robingame-0.1.0/robingame/input/__pycache__/keyboard.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Oct 23 16:14:19 2022 UTC, .py size: 278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5b68 5563 1601 0000  o.......[hUc....
+00000000: 6f0d 0d0a 0000 0000 88a3 6064 1601 0000  o.........`d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da0a 496e 7075 7451 7565 7565 6300 0000  ..InputQueuec...
 00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
@@ -15,37 +15,37 @@
 000000e0: 2800 0000 7400 6a01 a002 a100 8900 7403  (...t.j.......t.
 000000f0: 8700 6601 6401 6402 8408 7404 7405 8800  ..f.d.d...t.t...
 00000100: 8301 8301 4400 8301 8301 5300 2903 4e63  ....D.....S.).Nc
 00000110: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00000120: 0300 0000 3300 0000 7318 0000 0081 007c  ....3...s......|
 00000130: 005d 077d 0188 007c 0119 0056 0001 0071  .].}...|...V...q
 00000140: 0264 0053 0029 014e a900 2902 da02 2e30  .d.S.).N..)....0
-00000150: da02 6969 a901 5a10 7363 616e 636f 6465  ..ii..Z.scancode
-00000160: 5f77 7261 7070 6572 7205 0000 00fa 372f  _wrapperr.....7/
-00000170: 686f 6d65 2f62 696e 6e65 762f 636f 6465  home/binnev/code
-00000180: 2f72 6f62 696e 6761 6d65 2f72 6f62 696e  /robingame/robin
-00000190: 6761 6d65 2f69 6e70 7574 2f6b 6579 626f  game/input/keybo
-000001a0: 6172 642e 7079 da09 3c67 656e 6578 7072  ard.py..<genexpr
-000001b0: 3e09 0000 0073 0400 0000 0280 1600 7a34  >....s........z4
-000001c0: 4b65 7962 6f61 7264 496e 7075 7451 7565  KeyboardInputQue
-000001d0: 7565 2e67 6574 5f6e 6577 5f76 616c 7565  ue.get_new_value
-000001e0: 732e 3c6c 6f63 616c 733e 2e3c 6765 6e65  s.<locals>.<gene
-000001f0: 7870 723e 2906 da06 7079 6761 6d65 da03  xpr>)...pygame..
-00000200: 6b65 79da 0b67 6574 5f70 7265 7373 6564  key..get_pressed
-00000210: da05 7475 706c 65da 0572 616e 6765 da03  ..tuple..range..
-00000220: 6c65 6e29 01da 0473 656c 6672 0500 0000  len)...selfr....
-00000230: 7208 0000 0072 0900 0000 da0e 6765 745f  r....r......get_
-00000240: 6e65 775f 7661 6c75 6573 0700 0000 7304  new_values....s.
-00000250: 0000 000a 011e 017a 214b 6579 626f 6172  .......z!Keyboar
-00000260: 6449 6e70 7574 5175 6575 652e 6765 745f  dInputQueue.get_
-00000270: 6e65 775f 7661 6c75 6573 4e29 06da 085f  new_valuesN)..._
-00000280: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000290: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000002a0: 5f72 0e00 0000 da03 696e 7472 1200 0000  _r......intr....
-000002b0: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-000002c0: 0900 0000 7203 0000 0006 0000 0073 0400  ....r........s..
-000002d0: 0000 0800 1601 7203 0000 0029 0472 0b00  ......r....).r..
-000002e0: 0000 da15 726f 6269 6e67 616d 652e 696e  ....robingame.in
-000002f0: 7075 742e 7175 6575 6572 0200 0000 7203  put.queuer....r.
-00000300: 0000 0072 0500 0000 7205 0000 0072 0500  ...r....r....r..
-00000310: 0000 7209 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000320: 3e01 0000 0073 0600 0000 0800 0c02 1403  >....s..........
+00000150: da02 6969 a901 da10 7363 616e 636f 6465  ..ii....scancode
+00000160: 5f77 7261 7070 6572 7205 0000 00fa 362f  _wrapperr.....6/
+00000170: 686f 6d65 2f72 6f62 696e 2f63 6f64 652f  home/robin/code/
+00000180: 726f 6269 6e67 616d 652f 726f 6269 6e67  robingame/robing
+00000190: 616d 652f 696e 7075 742f 6b65 7962 6f61  ame/input/keyboa
+000001a0: 7264 2e70 79da 093c 6765 6e65 7870 723e  rd.py..<genexpr>
+000001b0: 0900 0000 7304 0000 0002 8016 007a 344b  ....s........z4K
+000001c0: 6579 626f 6172 6449 6e70 7574 5175 6575  eyboardInputQueu
+000001d0: 652e 6765 745f 6e65 775f 7661 6c75 6573  e.get_new_values
+000001e0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+000001f0: 7072 3e29 06da 0670 7967 616d 65da 036b  pr>)...pygame..k
+00000200: 6579 da0b 6765 745f 7072 6573 7365 64da  ey..get_pressed.
+00000210: 0574 7570 6c65 da05 7261 6e67 65da 036c  .tuple..range..l
+00000220: 656e 2901 da04 7365 6c66 7205 0000 0072  en)...selfr....r
+00000230: 0800 0000 720a 0000 00da 0e67 6574 5f6e  ....r......get_n
+00000240: 6577 5f76 616c 7565 7307 0000 0073 0400  ew_values....s..
+00000250: 0000 0a01 1e01 7a21 4b65 7962 6f61 7264  ......z!Keyboard
+00000260: 496e 7075 7451 7565 7565 2e67 6574 5f6e  InputQueue.get_n
+00000270: 6577 5f76 616c 7565 734e 2906 da08 5f5f  ew_valuesN)...__
+00000280: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000290: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000002a0: 720f 0000 00da 0369 6e74 7213 0000 0072  r......intr....r
+000002b0: 0500 0000 7205 0000 0072 0500 0000 720a  ....r....r....r.
+000002c0: 0000 0072 0300 0000 0600 0000 7304 0000  ...r........s...
+000002d0: 0008 0016 0172 0300 0000 2904 720c 0000  .....r....).r...
+000002e0: 00da 1572 6f62 696e 6761 6d65 2e69 6e70  ...robingame.inp
+000002f0: 7574 2e71 7565 7565 7202 0000 0072 0300  ut.queuer....r..
+00000300: 0000 7205 0000 0072 0500 0000 7205 0000  ..r....r....r...
+00000310: 0072 0a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000320: 0100 0000 7306 0000 0008 000c 0214 03    ....s..........
```

### Comparing `robingame-0.0.9/robingame/input/__pycache__/queue.cpython-310.pyc` & `robingame-0.1.0/robingame/input/__pycache__/queue.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Oct 23 16:14:19 2022 UTC, .py size: 3194 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5b68 5563 7a0c 0000  o.......[hUcz...
+00000000: 6f0d 0d0a 0000 0000 88a3 6064 7a0c 0000  o.........`dz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 8303 5a05 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
 00000060: 6501 8303 5a06 6407 5300 2908 e900 0000  e...Z.d.S.).....
 00000070: 0029 01da 0564 6571 7565 2901 da0b 636f  .)...deque)...co
@@ -20,248 +20,248 @@
 00000130: 7479 2070 7967 616d 652e 6b65 792e 6765  ty pygame.key.ge
 00000140: 745f 7072 6573 7365 6428 2920 7475 706c  t_pressed() tupl
 00000150: 652e da06 7265 7475 726e 6301 0000 0000  e...returnc.....
 00000160: 0000 0000 0000 0003 0000 0001 0000 004f  ...............O
 00000170: 0000 0073 0400 0000 6401 5300 2902 4e72  ...s....d.S.).Nr
 00000180: 0100 0000 a900 2903 da04 7365 6c66 da04  ......)...self..
 00000190: 6172 6773 da06 6b77 6172 6773 7206 0000  args..kwargsr...
-000001a0: 0072 0600 0000 fa34 2f68 6f6d 652f 6269  .r.....4/home/bi
-000001b0: 6e6e 6576 2f63 6f64 652f 726f 6269 6e67  nnev/code/robing
-000001c0: 616d 652f 726f 6269 6e67 616d 652f 696e  ame/robingame/in
-000001d0: 7075 742f 7175 6575 652e 7079 da0b 5f5f  put/queue.py..__
-000001e0: 6765 7469 7465 6d5f 5f0a 0000 0073 0200  getitem__....s..
-000001f0: 0000 0401 7a11 456d 7074 792e 5f5f 6765  ....z.Empty.__ge
-00000200: 7469 7465 6d5f 5f4e 2906 da08 5f5f 6e61  titem__N)...__na
-00000210: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000220: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000230: 5f5f 646f 635f 5fda 0369 6e74 720b 0000  __doc__..intr...
-00000240: 0072 0600 0000 7206 0000 0072 0600 0000  .r....r....r....
-00000250: 720a 0000 0072 0400 0000 0600 0000 7306  r....r........s.
-00000260: 0000 0008 0004 0112 0372 0400 0000 6300  .........r....c.
-00000270: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000280: 0000 0000 0000 0073 b400 0000 6500 5a01  .......s....e.Z.
-00000290: 6400 5a02 6401 5a03 641c 8700 6601 6403  d.Z.d.Z.d...f.d.
-000002a0: 6404 8409 5a04 6405 6505 6506 1900 6602  d...Z.d.e.e...f.
-000002b0: 6406 6407 8404 5a07 6408 6409 8400 5a08  d.d...Z.d.d...Z.
-000002c0: 6405 6505 6506 1900 6602 640a 640b 8404  d.e.e...f.d.d...
-000002d0: 5a09 6405 6505 6506 1900 6602 640c 640d  Z.d.e.e...f.d.d.
-000002e0: 8404 5a0a 6405 6505 6506 1900 6602 640e  ..Z.d.e.e...f.d.
-000002f0: 640f 8404 5a0b 6405 6506 6602 6410 6411  d...Z.d.e.f.d.d.
-00000300: 8404 5a0c 6405 6506 6602 6412 6413 8404  ..Z.d.e.f.d.d...
-00000310: 5a0d 6405 6506 6602 6414 6415 8404 5a0e  Z.d.e.f.d.d...Z.
-00000320: 6416 6417 8400 5a0f 6418 6419 8400 5a10  d.d...Z.d.d...Z.
-00000330: 641a 641b 8400 5a11 8700 0400 5a12 5300  d.d...Z.....Z.S.
-00000340: 291d da0a 496e 7075 7451 7565 7565 7ac1  )...InputQueuez.
-00000350: 0a20 2020 2050 726f 7669 6465 7320 6164  .    Provides ad
-00000360: 6469 7469 6f6e 616c 2066 756e 6374 696f  ditional functio
-00000370: 6e61 6c69 7479 2062 6579 6f6e 6420 7079  nality beyond py
-00000380: 6761 6d65 2e6b 6579 2e67 6574 5f70 7265  game.key.get_pre
-00000390: 7373 6564 2829 2e0a 2020 2020 2d20 4d61  ssed()..    - Ma
-000003a0: 696e 7461 696e 7320 6120 6275 6666 6572  intains a buffer
-000003b0: 206f 6620 7468 6520 6c61 7374 2066 6577   of the last few
-000003c0: 2069 6e70 7574 730a 2020 2020 2d20 4361   inputs.    - Ca
-000003d0: 6c63 756c 6174 6573 2077 6869 6368 206b  lculates which k
-000003e0: 6579 7320 6861 7665 2062 6565 6e20 7072  eys have been pr
-000003f0: 6573 7365 6420 616e 6420 7265 6c65 6173  essed and releas
-00000400: 6564 2074 6869 7320 7469 636b 0a20 2020  ed this tick.   
-00000410: 20e9 0500 0000 6302 0000 0000 0000 0000   .....c.........
-00000420: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-00000430: 1200 0000 7400 8300 6a01 7c01 6401 8d01  ....t...j.|.d...
-00000440: 0100 6400 5300 2902 4e29 01da 066d 6178  ..d.S.).N)...max
-00000450: 6c65 6e29 02da 0573 7570 6572 da08 5f5f  len)...super..__
-00000460: 696e 6974 5f5f 2902 7207 0000 00da 0c71  init__).r......q
-00000470: 7565 7565 5f6c 656e 6774 68a9 01da 095f  ueue_length...._
-00000480: 5f63 6c61 7373 5f5f 7206 0000 0072 0a00  _class__r....r..
-00000490: 0000 7215 0000 0015 0000 00f3 0200 0000  ..r.............
-000004a0: 1201 7a13 496e 7075 7451 7565 7565 2e5f  ..z.InputQueue._
-000004b0: 5f69 6e69 745f 5f72 0500 0000 6301 0000  _init__r....c...
-000004c0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000004d0: 0043 0000 0073 0400 0000 7400 8201 2901  .C...s....t...).
-000004e0: 7a5e 5375 6263 6c61 7373 6573 2073 686f  z^Subclasses sho
-000004f0: 756c 6420 696d 706c 656d 656e 7420 7468  uld implement th
-00000500: 6973 2e20 4974 2073 686f 756c 6420 6265  is. It should be
-00000510: 2073 6f6d 6574 6869 6e67 206c 696b 650a   something like.
-00000520: 2020 2020 2020 2020 7079 6761 6d65 2e6b          pygame.k
-00000530: 6579 2e67 6574 5f70 7265 7373 6564 2829  ey.get_pressed()
-00000540: 2901 da13 4e6f 7449 6d70 6c65 6d65 6e74  )...NotImplement
-00000550: 6564 4572 726f 72a9 0172 0700 0000 7206  edError..r....r.
-00000560: 0000 0072 0600 0000 720a 0000 00da 0e67  ...r....r......g
-00000570: 6574 5f6e 6577 5f76 616c 7565 7318 0000  et_new_values...
-00000580: 0073 0200 0000 0403 7a19 496e 7075 7451  .s......z.InputQ
-00000590: 7565 7565 2e67 6574 5f6e 6577 5f76 616c  ueue.get_new_val
-000005a0: 7565 7363 0100 0000 0000 0000 0000 0000  uesc............
-000005b0: 0100 0000 0400 0000 4300 0000 7312 0000  ........C...s...
-000005c0: 007c 00a0 007c 00a0 01a1 00a1 0101 0064  .|...|.........d
-000005d0: 0053 00a9 014e 2902 da06 6170 7065 6e64  .S...N)...append
-000005e0: 721c 0000 0072 1b00 0000 7206 0000 0072  r....r....r....r
-000005f0: 0600 0000 720a 0000 00da 0f72 6561 645f  ....r......read_
-00000600: 6e65 775f 696e 7075 7473 1d00 0000 7219  new_inputs....r.
-00000610: 0000 007a 1a49 6e70 7574 5175 6575 652e  ...z.InputQueue.
-00000620: 7265 6164 5f6e 6577 5f69 6e70 7574 7363  read_new_inputsc
-00000630: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000640: 0200 0000 4300 0000 731a 0000 0074 007c  ....C...s....t.|
-00000650: 0083 0164 016b 0472 0a7c 0064 0219 0053  ...d.k.r.|.d...S
-00000660: 0074 0183 0053 0029 037a 2d52 6574 7572  .t...S.).z-Retur
-00000670: 6e20 7468 6520 6b65 7973 2077 6869 6368  n the keys which
-00000680: 2061 7265 2063 7572 7265 6e74 6c79 2068   are currently h
-00000690: 656c 6420 646f 776e 7201 0000 00e9 ffff  eld downr.......
-000006a0: ffff 2902 da03 6c65 6e72 0400 0000 721b  ..)...lenr....r.
-000006b0: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
-000006c0: 0000 da08 6765 745f 646f 776e 2000 0000  ....get_down ...
-000006d0: 7302 0000 001a 027a 1349 6e70 7574 5175  s......z.InputQu
-000006e0: 6575 652e 6765 745f 646f 776e 6301 0000  eue.get_downc...
-000006f0: 0000 0000 0000 0000 0001 0000 0008 0000  ................
-00000700: 0003 0000 00f3 4e00 0000 7a1a 7c00 6401  ......N...z.|.d.
-00000710: 1900 8900 7c00 6402 1900 8901 7400 8700  ....|.d.....t...
-00000720: 8701 6602 6403 6404 8408 7401 7402 8800  ..f.d.d...t.t...
-00000730: 8301 8801 8302 4400 8301 8301 5700 5300  ......D.....W.S.
-00000740: 0400 7403 7926 0100 0100 0100 7404 8300  ..t.y&......t...
-00000750: 0600 5900 5300 7700 2905 7a72 5265 7475  ..Y.S.w.).zrRetu
-00000760: 726e 2074 6865 206b 6579 7320 7468 6174  rn the keys that
-00000770: 2068 6176 6520 6a75 7374 2062 6565 6e20   have just been 
-00000780: 7072 6573 7365 642d 2d2d 692e 652e 2074  pressed---i.e. t
-00000790: 686f 7365 2074 6861 7420 6172 6520 646f  hose that are do
-000007a0: 776e 2074 6869 7320 7469 636b 2062 7574  wn this tick but
-000007b0: 0a20 2020 2020 2020 206e 6f74 2074 6865  .        not the
-000007c0: 2070 7265 7669 6f75 7320 7469 636b 7220   previous tickr 
-000007d0: 0000 00e9 feff ffff 6301 0000 0000 0000  ........c.......
-000007e0: 0000 0000 0004 0000 0004 0000 0033 0000  .............3..
-000007f0: 0073 2e00 0000 8100 7c00 5d12 5c02 5c02  .s......|.].\.\.
-00000800: 7d01 7d02 7d03 7400 8800 7c01 1900 6f11  }.}.}.t...|...o.
-00000810: 8801 7c01 1900 0c00 8301 5600 0100 7102  ..|.......V...q.
-00000820: 6400 5300 721d 0000 00a9 0172 1000 0000  d.S.r......r....
-00000830: a904 da02 2e30 da01 69da 0163 da01 70a9  .....0..i..c..p.
-00000840: 02da 0763 7572 7265 6e74 da08 7072 6576  ...current..prev
-00000850: 696f 7573 7206 0000 0072 0a00 0000 da09  iousr....r......
-00000860: 3c67 656e 6578 7072 3e2d 0000 00f3 0a00  <genexpr>-......
-00000870: 0000 0280 0400 0a02 14ff 0aff 7a29 496e  ............z)In
-00000880: 7075 7451 7565 7565 2e67 6574 5f70 7265  putQueue.get_pre
-00000890: 7373 6564 2e3c 6c6f 6361 6c73 3e2e 3c67  ssed.<locals>.<g
-000008a0: 656e 6578 7072 3ea9 05da 0574 7570 6c65  enexpr>....tuple
-000008b0: da03 7a69 70da 0965 6e75 6d65 7261 7465  ..zip..enumerate
-000008c0: da0a 496e 6465 7845 7272 6f72 7204 0000  ..IndexErrorr...
-000008d0: 0072 1b00 0000 7206 0000 0072 2b00 0000  .r....r....r+...
-000008e0: 720a 0000 00da 0b67 6574 5f70 7265 7373  r......get_press
-000008f0: 6564 2400 0000 7312 0000 0002 0308 0108  ed$...s.........
-00000900: 010e 040c 020a fe0c 040a 0102 ff7a 1649  .............z.I
-00000910: 6e70 7574 5175 6575 652e 6765 745f 7072  nputQueue.get_pr
-00000920: 6573 7365 6463 0100 0000 0000 0000 0000  essedc..........
-00000930: 0000 0100 0000 0800 0000 0300 0000 7223  ..............r#
-00000940: 0000 0029 057a 7e52 6574 7572 6e20 7468  ...).z~Return th
-00000950: 6520 6b65 7973 2074 6861 7420 6861 7665  e keys that have
-00000960: 206a 7573 7420 6265 656e 2072 656c 6561   just been relea
-00000970: 7365 642d 2d2d 692e 652e 2074 686f 7365  sed---i.e. those
-00000980: 2074 6861 7420 6172 6520 6e6f 7420 646f   that are not do
-00000990: 776e 2074 6869 730a 2020 2020 2020 2020  wn this.        
-000009a0: 7469 636b 2c20 6275 7420 7765 7265 2064  tick, but were d
-000009b0: 6f77 6e20 7468 6520 7072 6576 696f 7573  own the previous
-000009c0: 2074 6963 6b72 2000 0000 7224 0000 0063   tickr ...r$...c
-000009d0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000009e0: 0400 0000 3300 0000 732e 0000 0081 007c  ....3...s......|
-000009f0: 005d 125c 025c 027d 017d 027d 0374 0088  .].\.\.}.}.}.t..
-00000a00: 017c 0119 006f 1188 007c 0119 000c 0083  .|...o...|......
-00000a10: 0156 0001 0071 0264 0053 0072 1d00 0000  .V...q.d.S.r....
-00000a20: 7225 0000 0072 2600 0000 722b 0000 0072  r%...r&...r+...r
-00000a30: 0600 0000 720a 0000 0072 2e00 0000 3a00  ....r....r....:.
-00000a40: 0000 722f 0000 007a 2a49 6e70 7574 5175  ..r/...z*InputQu
-00000a50: 6575 652e 6765 745f 7265 6c65 6173 6564  eue.get_released
-00000a60: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00000a70: 7072 3e72 3000 0000 721b 0000 0072 0600  pr>r0...r....r..
-00000a80: 0000 722b 0000 0072 0a00 0000 da0c 6765  ..r+...r......ge
-00000a90: 745f 7265 6c65 6173 6564 3400 0000 7312  t_released4...s.
-00000aa0: 0000 0002 0308 0108 010e 010c 020a fe0c  ................
-00000ab0: 040a 0102 ff7a 1749 6e70 7574 5175 6575  .....z.InputQueu
-00000ac0: 652e 6765 745f 7265 6c65 6173 6564 6302  e.get_releasedc.
-00000ad0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00000ae0: 0000 0043 0000 00f3 1000 0000 7c00 a000  ...C........|...
-00000af0: a100 7d02 7c02 7c01 1900 5300 2901 7a29  ..}.|.|...S.).z)
-00000b00: 4368 6563 6b20 6966 2061 206b 6579 2068  Check if a key h
-00000b10: 6173 2062 6565 6e20 7072 6573 7365 6420  as been pressed 
-00000b20: 7468 6973 2074 6963 6b29 0172 3500 0000  this tick).r5...
-00000b30: a903 7207 0000 00da 036b 6579 da04 6b65  ..r......key..ke
-00000b40: 7973 7206 0000 0072 0600 0000 720a 0000  ysr....r....r...
-00000b50: 00da 0a69 735f 7072 6573 7365 6441 0000  ...is_pressedA..
-00000b60: 00f3 0400 0000 0802 0801 7a15 496e 7075  ..........z.Inpu
-00000b70: 7451 7565 7565 2e69 735f 7072 6573 7365  tQueue.is_presse
-00000b80: 6463 0200 0000 0000 0000 0000 0000 0300  dc..............
-00000b90: 0000 0200 0000 4300 0000 7237 0000 0029  ......C...r7...)
-00000ba0: 017a 2543 6865 636b 2069 6620 6120 6b65  .z%Check if a ke
-00000bb0: 7920 6973 2063 7572 7265 6e74 6c79 2068  y is currently h
-00000bc0: 656c 6420 646f 776e 2901 7222 0000 0072  eld down).r"...r
-00000bd0: 3800 0000 7206 0000 0072 0600 0000 720a  8...r....r....r.
-00000be0: 0000 00da 0769 735f 646f 776e 4600 0000  .....is_downF...
-00000bf0: 723c 0000 007a 1249 6e70 7574 5175 6575  r<...z.InputQueu
-00000c00: 652e 6973 5f64 6f77 6e63 0200 0000 0000  e.is_downc......
-00000c10: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
-00000c20: 0000 7237 0000 0029 017a 2a43 6865 636b  ..r7...).z*Check
-00000c30: 2069 6620 6120 6b65 7920 6861 7320 6265   if a key has be
-00000c40: 656e 2072 656c 6561 7365 6420 7468 6973  en released this
-00000c50: 2074 6963 6b29 0172 3600 0000 7238 0000   tick).r6...r8..
-00000c60: 0072 0600 0000 7206 0000 0072 0a00 0000  .r....r....r....
-00000c70: da0b 6973 5f72 656c 6561 7365 644b 0000  ..is_releasedK..
-00000c80: 0072 3c00 0000 7a16 496e 7075 7451 7565  .r<...z.InputQue
-00000c90: 7565 2e69 735f 7265 6c65 6173 6564 6303  ue.is_releasedc.
-00000ca0: 0000 0000 0000 0000 0000 0005 0000 0003  ................
-00000cb0: 0000 0003 0000 0073 2c00 0000 7400 7c00  .......s,...t.|.
-00000cc0: 8301 7c02 0b00 6401 8502 1900 7d03 8700  ..|...d.....}...
-00000cd0: 6601 6402 6403 8408 7c03 4400 8301 7d04  f.d.d...|.D...}.
-00000ce0: 7401 7c04 8301 5300 2904 7a46 436f 756e  t.|...S.).zFCoun
-00000cf0: 7420 7468 6520 7269 7369 6e67 2061 6e64  t the rising and
-00000d00: 2066 616c 6c69 6e67 2065 6467 6573 2e20   falling edges. 
-00000d10: 4361 6e20 6265 2075 7365 6420 746f 2064  Can be used to d
-00000d20: 6574 6563 7420 7061 7374 2069 6e70 7574  etect past input
-00000d30: 732e 4e63 0100 0000 0000 0000 0000 0000  s.Nc............
-00000d40: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
-00000d50: 0067 007c 005d 067d 017c 0188 0019 0091  .g.|.].}.|......
-00000d60: 0271 0253 0072 0600 0000 7206 0000 0029  .q.S.r....r....)
-00000d70: 0272 2700 0000 da05 6c61 7965 72a9 0172  .r'.....layer..r
-00000d80: 3900 0000 7206 0000 0072 0a00 0000 da0a  9...r....r......
-00000d90: 3c6c 6973 7463 6f6d 703e 5300 0000 7302  <listcomp>S...s.
-00000da0: 0000 0014 007a 2e49 6e70 7574 5175 6575  .....z.InputQueu
-00000db0: 652e 6275 6666 6572 6564 5f69 6e70 7574  e.buffered_input
-00000dc0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-00000dd0: 636f 6d70 3e29 02da 046c 6973 7472 0300  comp>)...listr..
-00000de0: 0000 2905 7207 0000 0072 3900 0000 da0d  ..).r....r9.....
-00000df0: 6275 6666 6572 5f6c 656e 6774 68da 0662  buffer_length..b
-00000e00: 7566 6665 72da 0676 616c 7565 7372 0600  uffer..valuesr..
-00000e10: 0000 7240 0000 0072 0a00 0000 da0f 6275  ..r@...r......bu
-00000e20: 6666 6572 6564 5f69 6e70 7574 7350 0000  ffered_inputsP..
-00000e30: 0073 0600 0000 1202 1201 0801 7a1a 496e  .s..........z.In
-00000e40: 7075 7451 7565 7565 2e62 7566 6665 7265  putQueue.buffere
-00000e50: 645f 696e 7075 7473 6303 0000 0000 0000  d_inputsc.......
-00000e60: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00000e70: 0073 1400 0000 7c00 a000 7c01 7c02 a102  .s....|...|.|...
-00000e80: 5c02 7d03 7d04 7c03 5300 721d 0000 00a9  \.}.}.|.S.r.....
-00000e90: 0172 4600 0000 a905 7207 0000 0072 3900  .rF.....r....r9.
-00000ea0: 0000 7243 0000 005a 0672 6973 696e 675a  ..rC...Z.risingZ
-00000eb0: 0766 616c 6c69 6e67 7206 0000 0072 0600  .fallingr....r..
-00000ec0: 0000 720a 0000 00da 1062 7566 6665 7265  ..r......buffere
-00000ed0: 645f 7072 6573 7365 7356 0000 00f3 0400  d_pressesV......
-00000ee0: 0000 1001 0401 7a1b 496e 7075 7451 7565  ......z.InputQue
-00000ef0: 7565 2e62 7566 6665 7265 645f 7072 6573  ue.buffered_pres
-00000f00: 7365 7363 0300 0000 0000 0000 0000 0000  sesc............
-00000f10: 0500 0000 0400 0000 4300 0000 7314 0000  ........C...s...
-00000f20: 007c 00a0 007c 017c 02a1 025c 027d 037d  .|...|.|...\.}.}
-00000f30: 047c 0453 0072 1d00 0000 7247 0000 0072  .|.S.r....rG...r
-00000f40: 4800 0000 7206 0000 0072 0600 0000 720a  H...r....r....r.
-00000f50: 0000 00da 1162 7566 6665 7265 645f 7265  .....buffered_re
-00000f60: 6c65 6173 6573 5a00 0000 724a 0000 007a  leasesZ...rJ...z
-00000f70: 1c49 6e70 7574 5175 6575 652e 6275 6666  .InputQueue.buff
-00000f80: 6572 6564 5f72 656c 6561 7365 7329 0172  ered_releases).r
-00000f90: 1200 0000 2913 720c 0000 0072 0d00 0000  ....).r....r....
-00000fa0: 720e 0000 0072 0f00 0000 7215 0000 0072  r....r....r....r
-00000fb0: 3100 0000 7210 0000 0072 1c00 0000 721f  1...r....r....r.
-00000fc0: 0000 0072 2200 0000 7235 0000 0072 3600  ...r"...r5...r6.
-00000fd0: 0000 723b 0000 0072 3d00 0000 723e 0000  ..r;...r=...r>..
-00000fe0: 0072 4600 0000 7249 0000 0072 4b00 0000  .rF...rI...rK...
-00000ff0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00001000: 0600 0000 7206 0000 0072 1700 0000 720a  ....r....r....r.
-00001010: 0000 0072 1100 0000 0e00 0000 731c 0000  ...r........s...
-00001020: 0008 0004 010e 0612 0308 0512 0312 0412  ................
-00001030: 100e 0d0e 050e 0508 0508 0610 0472 1100  .............r..
-00001040: 0000 4e29 07da 0b63 6f6c 6c65 6374 696f  ..N)...collectio
-00001050: 6e73 7202 0000 005a 0f72 6f62 696e 6761  nsr....Z.robinga
-00001060: 6d65 2e75 7469 6c73 7203 0000 0072 3100  me.utilsr....r1.
-00001070: 0000 7204 0000 0072 1100 0000 7206 0000  ..r....r....r...
-00001080: 0072 0600 0000 7206 0000 0072 0a00 0000  .r....r....r....
-00001090: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-000010a0: 0000 000c 000c 0210 0314 08              ...........
+000001a0: 0072 0600 0000 fa33 2f68 6f6d 652f 726f  .r.....3/home/ro
+000001b0: 6269 6e2f 636f 6465 2f72 6f62 696e 6761  bin/code/robinga
+000001c0: 6d65 2f72 6f62 696e 6761 6d65 2f69 6e70  me/robingame/inp
+000001d0: 7574 2f71 7565 7565 2e70 79da 0b5f 5f67  ut/queue.py..__g
+000001e0: 6574 6974 656d 5f5f 0a00 0000 7302 0000  etitem__....s...
+000001f0: 0004 017a 1145 6d70 7479 2e5f 5f67 6574  ...z.Empty.__get
+00000200: 6974 656d 5f5f 4e29 06da 085f 5f6e 616d  item__N)...__nam
+00000210: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000220: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000230: 5f64 6f63 5f5f da03 696e 7472 0b00 0000  _doc__..intr....
+00000240: 7206 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00000250: 0a00 0000 7204 0000 0006 0000 0073 0600  ....r........s..
+00000260: 0000 0800 0401 1203 7204 0000 0063 0000  ........r....c..
+00000270: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000280: 0000 0000 0000 73b4 0000 0065 005a 0164  ......s....e.Z.d
+00000290: 005a 0264 015a 0364 1c87 0066 0164 0364  .Z.d.Z.d...f.d.d
+000002a0: 0484 095a 0464 0565 0565 0619 0066 0264  ...Z.d.e.e...f.d
+000002b0: 0664 0784 045a 0764 0864 0984 005a 0864  .d...Z.d.d...Z.d
+000002c0: 0565 0565 0619 0066 0264 0a64 0b84 045a  .e.e...f.d.d...Z
+000002d0: 0964 0565 0565 0619 0066 0264 0c64 0d84  .d.e.e...f.d.d..
+000002e0: 045a 0a64 0565 0565 0619 0066 0264 0e64  .Z.d.e.e...f.d.d
+000002f0: 0f84 045a 0b64 0565 0666 0264 1064 1184  ...Z.d.e.f.d.d..
+00000300: 045a 0c64 0565 0666 0264 1264 1384 045a  .Z.d.e.f.d.d...Z
+00000310: 0d64 0565 0666 0264 1464 1584 045a 0e64  .d.e.f.d.d...Z.d
+00000320: 1664 1784 005a 0f64 1864 1984 005a 1064  .d...Z.d.d...Z.d
+00000330: 1a64 1b84 005a 1187 0004 005a 1253 0029  .d...Z.....Z.S.)
+00000340: 1dda 0a49 6e70 7574 5175 6575 657a c10a  ...InputQueuez..
+00000350: 2020 2020 5072 6f76 6964 6573 2061 6464      Provides add
+00000360: 6974 696f 6e61 6c20 6675 6e63 7469 6f6e  itional function
+00000370: 616c 6974 7920 6265 796f 6e64 2070 7967  ality beyond pyg
+00000380: 616d 652e 6b65 792e 6765 745f 7072 6573  ame.key.get_pres
+00000390: 7365 6428 292e 0a20 2020 202d 204d 6169  sed()..    - Mai
+000003a0: 6e74 6169 6e73 2061 2062 7566 6665 7220  ntains a buffer 
+000003b0: 6f66 2074 6865 206c 6173 7420 6665 7720  of the last few 
+000003c0: 696e 7075 7473 0a20 2020 202d 2043 616c  inputs.    - Cal
+000003d0: 6375 6c61 7465 7320 7768 6963 6820 6b65  culates which ke
+000003e0: 7973 2068 6176 6520 6265 656e 2070 7265  ys have been pre
+000003f0: 7373 6564 2061 6e64 2072 656c 6561 7365  ssed and release
+00000400: 6420 7468 6973 2074 6963 6b0a 2020 2020  d this tick.    
+00000410: e905 0000 0063 0200 0000 0000 0000 0000  .....c..........
+00000420: 0000 0200 0000 0300 0000 0300 0000 7312  ..............s.
+00000430: 0000 0074 0083 006a 017c 0164 018d 0101  ...t...j.|.d....
+00000440: 0064 0053 0029 024e 2901 da06 6d61 786c  .d.S.).N)...maxl
+00000450: 656e 2902 da05 7375 7065 72da 085f 5f69  en)...super..__i
+00000460: 6e69 745f 5f29 0272 0700 0000 da0c 7175  nit__).r......qu
+00000470: 6575 655f 6c65 6e67 7468 a901 da09 5f5f  eue_length....__
+00000480: 636c 6173 735f 5f72 0600 0000 720a 0000  class__r....r...
+00000490: 0072 1500 0000 1500 0000 f302 0000 0012  .r..............
+000004a0: 017a 1349 6e70 7574 5175 6575 652e 5f5f  .z.InputQueue.__
+000004b0: 696e 6974 5f5f 7205 0000 0063 0100 0000  init__r....c....
+000004c0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000004d0: 4300 0000 7304 0000 0074 0082 0129 017a  C...s....t...).z
+000004e0: 5e53 7562 636c 6173 7365 7320 7368 6f75  ^Subclasses shou
+000004f0: 6c64 2069 6d70 6c65 6d65 6e74 2074 6869  ld implement thi
+00000500: 732e 2049 7420 7368 6f75 6c64 2062 6520  s. It should be 
+00000510: 736f 6d65 7468 696e 6720 6c69 6b65 0a20  something like. 
+00000520: 2020 2020 2020 2070 7967 616d 652e 6b65         pygame.ke
+00000530: 792e 6765 745f 7072 6573 7365 6428 2929  y.get_pressed())
+00000540: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
+00000550: 6445 7272 6f72 a901 7207 0000 0072 0600  dError..r....r..
+00000560: 0000 7206 0000 0072 0a00 0000 da0e 6765  ..r....r......ge
+00000570: 745f 6e65 775f 7661 6c75 6573 1800 0000  t_new_values....
+00000580: 7302 0000 0004 037a 1949 6e70 7574 5175  s......z.InputQu
+00000590: 6575 652e 6765 745f 6e65 775f 7661 6c75  eue.get_new_valu
+000005a0: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
+000005b0: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
+000005c0: 7c00 a000 7c00 a001 a100 a101 0100 6400  |...|.........d.
+000005d0: 5300 a901 4e29 02da 0661 7070 656e 6472  S...N)...appendr
+000005e0: 1c00 0000 721b 0000 0072 0600 0000 7206  ....r....r....r.
+000005f0: 0000 0072 0a00 0000 da0f 7265 6164 5f6e  ...r......read_n
+00000600: 6577 5f69 6e70 7574 731d 0000 0072 1900  ew_inputs....r..
+00000610: 0000 7a1a 496e 7075 7451 7565 7565 2e72  ..z.InputQueue.r
+00000620: 6561 645f 6e65 775f 696e 7075 7473 6301  ead_new_inputsc.
+00000630: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000640: 0000 0043 0000 0073 1a00 0000 7400 7c00  ...C...s....t.|.
+00000650: 8301 6401 6b04 720a 7c00 6402 1900 5300  ..d.k.r.|.d...S.
+00000660: 7401 8300 5300 2903 7a2d 5265 7475 726e  t...S.).z-Return
+00000670: 2074 6865 206b 6579 7320 7768 6963 6820   the keys which 
+00000680: 6172 6520 6375 7272 656e 746c 7920 6865  are currently he
+00000690: 6c64 2064 6f77 6e72 0100 0000 e9ff ffff  ld downr........
+000006a0: ff29 02da 036c 656e 7204 0000 0072 1b00  .)...lenr....r..
+000006b0: 0000 7206 0000 0072 0600 0000 720a 0000  ..r....r....r...
+000006c0: 00da 0867 6574 5f64 6f77 6e20 0000 0073  ...get_down ...s
+000006d0: 0200 0000 1a02 7a13 496e 7075 7451 7565  ......z.InputQue
+000006e0: 7565 2e67 6574 5f64 6f77 6e63 0100 0000  ue.get_downc....
+000006f0: 0000 0000 0000 0000 0100 0000 0800 0000  ................
+00000700: 0300 0000 f34e 0000 007a 1a7c 0064 0119  .....N...z.|.d..
+00000710: 0089 007c 0064 0219 0089 0174 0087 0087  ...|.d.....t....
+00000720: 0166 0264 0364 0484 0874 0174 0288 0083  .f.d.d...t.t....
+00000730: 0188 0183 0244 0083 0183 0157 0053 0004  .....D.....W.S..
+00000740: 0074 0379 2601 0001 0001 0074 0483 0006  .t.y&......t....
+00000750: 0059 0053 0077 0029 057a 7252 6574 7572  .Y.S.w.).zrRetur
+00000760: 6e20 7468 6520 6b65 7973 2074 6861 7420  n the keys that 
+00000770: 6861 7665 206a 7573 7420 6265 656e 2070  have just been p
+00000780: 7265 7373 6564 2d2d 2d69 2e65 2e20 7468  ressed---i.e. th
+00000790: 6f73 6520 7468 6174 2061 7265 2064 6f77  ose that are dow
+000007a0: 6e20 7468 6973 2074 6963 6b20 6275 740a  n this tick but.
+000007b0: 2020 2020 2020 2020 6e6f 7420 7468 6520          not the 
+000007c0: 7072 6576 696f 7573 2074 6963 6b72 2000  previous tickr .
+000007d0: 0000 e9fe ffff ff63 0100 0000 0000 0000  .......c........
+000007e0: 0000 0000 0400 0000 0400 0000 3300 0000  ............3...
+000007f0: 732e 0000 0081 007c 005d 125c 025c 027d  s......|.].\.\.}
+00000800: 017d 027d 0374 0088 007c 0119 006f 1188  .}.}.t...|...o..
+00000810: 017c 0119 000c 0083 0156 0001 0071 0264  .|.......V...q.d
+00000820: 0053 0072 1d00 0000 a901 7210 0000 00a9  .S.r......r.....
+00000830: 04da 022e 30da 0169 da01 63da 0170 a902  ....0..i..c..p..
+00000840: da07 6375 7272 656e 74da 0870 7265 7669  ..current..previ
+00000850: 6f75 7372 0600 0000 720a 0000 00da 093c  ousr....r......<
+00000860: 6765 6e65 7870 723e 2d00 0000 f30a 0000  genexpr>-.......
+00000870: 0002 8004 000a 0214 ff0a ff7a 2949 6e70  ...........z)Inp
+00000880: 7574 5175 6575 652e 6765 745f 7072 6573  utQueue.get_pres
+00000890: 7365 642e 3c6c 6f63 616c 733e 2e3c 6765  sed.<locals>.<ge
+000008a0: 6e65 7870 723e a905 da05 7475 706c 65da  nexpr>....tuple.
+000008b0: 037a 6970 da09 656e 756d 6572 6174 65da  .zip..enumerate.
+000008c0: 0a49 6e64 6578 4572 726f 7272 0400 0000  .IndexErrorr....
+000008d0: 721b 0000 0072 0600 0000 722b 0000 0072  r....r....r+...r
+000008e0: 0a00 0000 da0b 6765 745f 7072 6573 7365  ......get_presse
+000008f0: 6424 0000 0073 1200 0000 0203 0801 0801  d$...s..........
+00000900: 0e04 0c02 0afe 0c04 0a01 02ff 7a16 496e  ............z.In
+00000910: 7075 7451 7565 7565 2e67 6574 5f70 7265  putQueue.get_pre
+00000920: 7373 6564 6301 0000 0000 0000 0000 0000  ssedc...........
+00000930: 0001 0000 0008 0000 0003 0000 0072 2300  .............r#.
+00000940: 0000 2905 7a7e 5265 7475 726e 2074 6865  ..).z~Return the
+00000950: 206b 6579 7320 7468 6174 2068 6176 6520   keys that have 
+00000960: 6a75 7374 2062 6565 6e20 7265 6c65 6173  just been releas
+00000970: 6564 2d2d 2d69 2e65 2e20 7468 6f73 6520  ed---i.e. those 
+00000980: 7468 6174 2061 7265 206e 6f74 2064 6f77  that are not dow
+00000990: 6e20 7468 6973 0a20 2020 2020 2020 2074  n this.        t
+000009a0: 6963 6b2c 2062 7574 2077 6572 6520 646f  ick, but were do
+000009b0: 776e 2074 6865 2070 7265 7669 6f75 7320  wn the previous 
+000009c0: 7469 636b 7220 0000 0072 2400 0000 6301  tickr ...r$...c.
+000009d0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+000009e0: 0000 0033 0000 0073 2e00 0000 8100 7c00  ...3...s......|.
+000009f0: 5d12 5c02 5c02 7d01 7d02 7d03 7400 8801  ].\.\.}.}.}.t...
+00000a00: 7c01 1900 6f11 8800 7c01 1900 0c00 8301  |...o...|.......
+00000a10: 5600 0100 7102 6400 5300 721d 0000 0072  V...q.d.S.r....r
+00000a20: 2500 0000 7226 0000 0072 2b00 0000 7206  %...r&...r+...r.
+00000a30: 0000 0072 0a00 0000 722e 0000 003a 0000  ...r....r....:..
+00000a40: 0072 2f00 0000 7a2a 496e 7075 7451 7565  .r/...z*InputQue
+00000a50: 7565 2e67 6574 5f72 656c 6561 7365 642e  ue.get_released.
+00000a60: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000a70: 723e 7230 0000 0072 1b00 0000 7206 0000  r>r0...r....r...
+00000a80: 0072 2b00 0000 720a 0000 00da 0c67 6574  .r+...r......get
+00000a90: 5f72 656c 6561 7365 6434 0000 0073 1200  _released4...s..
+00000aa0: 0000 0203 0801 0801 0e01 0c02 0afe 0c04  ................
+00000ab0: 0a01 02ff 7a17 496e 7075 7451 7565 7565  ....z.InputQueue
+00000ac0: 2e67 6574 5f72 656c 6561 7365 6463 0200  .get_releasedc..
+00000ad0: 0000 0000 0000 0000 0000 0300 0000 0200  ................
+00000ae0: 0000 4300 0000 f310 0000 007c 00a0 00a1  ..C........|....
+00000af0: 007d 027c 027c 0119 0053 0029 017a 2943  .}.|.|...S.).z)C
+00000b00: 6865 636b 2069 6620 6120 6b65 7920 6861  heck if a key ha
+00000b10: 7320 6265 656e 2070 7265 7373 6564 2074  s been pressed t
+00000b20: 6869 7320 7469 636b 2901 7235 0000 00a9  his tick).r5....
+00000b30: 0372 0700 0000 da03 6b65 79da 046b 6579  .r......key..key
+00000b40: 7372 0600 0000 7206 0000 0072 0a00 0000  sr....r....r....
+00000b50: da0a 6973 5f70 7265 7373 6564 4100 0000  ..is_pressedA...
+00000b60: f304 0000 0008 0208 017a 1549 6e70 7574  .........z.Input
+00000b70: 5175 6575 652e 6973 5f70 7265 7373 6564  Queue.is_pressed
+00000b80: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000b90: 0002 0000 0043 0000 0072 3700 0000 2901  .....C...r7...).
+00000ba0: 7a25 4368 6563 6b20 6966 2061 206b 6579  z%Check if a key
+00000bb0: 2069 7320 6375 7272 656e 746c 7920 6865   is currently he
+00000bc0: 6c64 2064 6f77 6e29 0172 2200 0000 7238  ld down).r"...r8
+00000bd0: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
+00000be0: 0000 da07 6973 5f64 6f77 6e46 0000 0072  ....is_downF...r
+00000bf0: 3c00 0000 7a12 496e 7075 7451 7565 7565  <...z.InputQueue
+00000c00: 2e69 735f 646f 776e 6302 0000 0000 0000  .is_downc.......
+00000c10: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+00000c20: 0072 3700 0000 2901 7a2a 4368 6563 6b20  .r7...).z*Check 
+00000c30: 6966 2061 206b 6579 2068 6173 2062 6565  if a key has bee
+00000c40: 6e20 7265 6c65 6173 6564 2074 6869 7320  n released this 
+00000c50: 7469 636b 2901 7236 0000 0072 3800 0000  tick).r6...r8...
+00000c60: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
+00000c70: 0b69 735f 7265 6c65 6173 6564 4b00 0000  .is_releasedK...
+00000c80: 723c 0000 007a 1649 6e70 7574 5175 6575  r<...z.InputQueu
+00000c90: 652e 6973 5f72 656c 6561 7365 6463 0300  e.is_releasedc..
+00000ca0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00000cb0: 0000 0300 0000 732c 0000 0074 007c 0083  ......s,...t.|..
+00000cc0: 017c 020b 0064 0185 0219 007d 0387 0066  .|...d.....}...f
+00000cd0: 0164 0264 0384 087c 0344 0083 017d 0474  .d.d...|.D...}.t
+00000ce0: 017c 0483 0153 0029 047a 4643 6f75 6e74  .|...S.).zFCount
+00000cf0: 2074 6865 2072 6973 696e 6720 616e 6420   the rising and 
+00000d00: 6661 6c6c 696e 6720 6564 6765 732e 2043  falling edges. C
+00000d10: 616e 2062 6520 7573 6564 2074 6f20 6465  an be used to de
+00000d20: 7465 6374 2070 6173 7420 696e 7075 7473  tect past inputs
+00000d30: 2e4e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000d40: 0000 0004 0000 0013 0000 0073 1400 0000  ...........s....
+00000d50: 6700 7c00 5d06 7d01 7c01 8800 1900 9102  g.|.].}.|.......
+00000d60: 7102 5300 7206 0000 0072 0600 0000 2902  q.S.r....r....).
+00000d70: 7227 0000 00da 056c 6179 6572 a901 7239  r'.....layer..r9
+00000d80: 0000 0072 0600 0000 720a 0000 00da 0a3c  ...r....r......<
+00000d90: 6c69 7374 636f 6d70 3e53 0000 0073 0200  listcomp>S...s..
+00000da0: 0000 1400 7a2e 496e 7075 7451 7565 7565  ....z.InputQueue
+00000db0: 2e62 7566 6665 7265 645f 696e 7075 7473  .buffered_inputs
+00000dc0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000dd0: 6f6d 703e 2902 da04 6c69 7374 7203 0000  omp>)...listr...
+00000de0: 0029 0572 0700 0000 7239 0000 00da 0d62  .).r....r9.....b
+00000df0: 7566 6665 725f 6c65 6e67 7468 da06 6275  uffer_length..bu
+00000e00: 6666 6572 da06 7661 6c75 6573 7206 0000  ffer..valuesr...
+00000e10: 0072 4000 0000 720a 0000 00da 0f62 7566  .r@...r......buf
+00000e20: 6665 7265 645f 696e 7075 7473 5000 0000  fered_inputsP...
+00000e30: 7306 0000 0012 0212 0108 017a 1a49 6e70  s..........z.Inp
+00000e40: 7574 5175 6575 652e 6275 6666 6572 6564  utQueue.buffered
+00000e50: 5f69 6e70 7574 7363 0300 0000 0000 0000  _inputsc........
+00000e60: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00000e70: 7314 0000 007c 00a0 007c 017c 02a1 025c  s....|...|.|...\
+00000e80: 027d 037d 047c 0353 0072 1d00 0000 a901  .}.}.|.S.r......
+00000e90: 7246 0000 00a9 0572 0700 0000 7239 0000  rF.....r....r9..
+00000ea0: 0072 4300 0000 da06 7269 7369 6e67 da07  .rC.....rising..
+00000eb0: 6661 6c6c 696e 6772 0600 0000 7206 0000  fallingr....r...
+00000ec0: 0072 0a00 0000 da10 6275 6666 6572 6564  .r......buffered
+00000ed0: 5f70 7265 7373 6573 5600 0000 f304 0000  _pressesV.......
+00000ee0: 0010 0104 017a 1b49 6e70 7574 5175 6575  .....z.InputQueu
+00000ef0: 652e 6275 6666 6572 6564 5f70 7265 7373  e.buffered_press
+00000f00: 6573 6303 0000 0000 0000 0000 0000 0005  esc.............
+00000f10: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
+00000f20: 7c00 a000 7c01 7c02 a102 5c02 7d03 7d04  |...|.|...\.}.}.
+00000f30: 7c04 5300 721d 0000 0072 4700 0000 7248  |.S.r....rG...rH
+00000f40: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
+00000f50: 0000 da11 6275 6666 6572 6564 5f72 656c  ....buffered_rel
+00000f60: 6561 7365 735a 0000 0072 4c00 0000 7a1c  easesZ...rL...z.
+00000f70: 496e 7075 7451 7565 7565 2e62 7566 6665  InputQueue.buffe
+00000f80: 7265 645f 7265 6c65 6173 6573 2901 7212  red_releases).r.
+00000f90: 0000 0029 1372 0c00 0000 720d 0000 0072  ...).r....r....r
+00000fa0: 0e00 0000 720f 0000 0072 1500 0000 7231  ....r....r....r1
+00000fb0: 0000 0072 1000 0000 721c 0000 0072 1f00  ...r....r....r..
+00000fc0: 0000 7222 0000 0072 3500 0000 7236 0000  ..r"...r5...r6..
+00000fd0: 0072 3b00 0000 723d 0000 0072 3e00 0000  .r;...r=...r>...
+00000fe0: 7246 0000 0072 4b00 0000 724d 0000 00da  rF...rK...rM....
+00000ff0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7206  .__classcell__r.
+00001000: 0000 0072 0600 0000 7217 0000 0072 0a00  ...r....r....r..
+00001010: 0000 7211 0000 000e 0000 0073 1c00 0000  ..r........s....
+00001020: 0800 0401 0e06 1203 0805 1203 1204 1210  ................
+00001030: 0e0d 0e05 0e05 0805 0806 1004 7211 0000  ............r...
+00001040: 004e 2907 da0b 636f 6c6c 6563 7469 6f6e  .N)...collection
+00001050: 7372 0200 0000 da0f 726f 6269 6e67 616d  sr......robingam
+00001060: 652e 7574 696c 7372 0300 0000 7231 0000  e.utilsr....r1..
+00001070: 0072 0400 0000 7211 0000 0072 0600 0000  .r....r....r....
+00001080: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
+00001090: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
+000010a0: 0000 0c00 0c02 1003 1408                 ..........
```

### Comparing `robingame-0.0.9/robingame/input/event.py` & `robingame-0.1.0/robingame/input/event.py`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/input/gamecube.py` & `robingame-0.1.0/robingame/input/gamecube.py`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/input/queue.py` & `robingame-0.1.0/robingame/input/queue.py`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/input/visualization.py` & `robingame-0.1.0/robingame/input/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable
 
 from pygame.color import Color
 from pygame.surface import Surface
 
 from robingame.image import brighten_color
 from robingame.input import GamecubeController
-from robingame.objects import Entity, Group, Particle
+from robingame.objects import Entity, Group, Particle, Game
 
 
 class SmashParticle(Particle):
     radius = 20
     decay = 2
     color = Color("red")
     gravity = 0
@@ -154,17 +154,15 @@
     class GCVizGame(Game):
         screen_color = Color("darkgray")
 
         def __init__(self):
             super().__init__()
             self.input = GamecubeController(controller_id=0)
             self.objects = Group()
-            self.child_groups = [
-                self.objects,
-            ]
+            self.child_groups = [self.objects]
             self.visualizer = GamecubeControllerVisualizer(
                 x=0,
                 y=0,
                 input=self.input,
                 groups=[self.objects],
             )
```

### Comparing `robingame-0.0.9/robingame/objects/__pycache__/game.cpython-310.pyc` & `robingame-0.1.0/robingame/objects/__pycache__/game.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 2711 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,205 +1,187 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 970a 0000  o.......u.5c....
+00000000: 6f0d 0d0a 0000 0000 8874 a564 de09 0000  o........t.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
 00000080: 6407 6408 8400 6408 6509 8303 5a0d 6401  d.d...d.e...Z.d.
 00000090: 5300 2909 e900 0000 004e 2901 da05 436f  S.)......N)...Co
 000000a0: 6c6f 7229 01da 0753 7572 6661 6365 2901  lor)...Surface).
 000000b0: da0a 4576 656e 7451 7565 7565 2902 da06  ..EventQueue)...
 000000c0: 456e 7469 7479 da05 4772 6f75 7029 01da  Entity..Group)..
 000000d0: 0a46 7073 5472 6163 6b65 7263 0000 0000  .FpsTrackerc....
 000000e0: 0000 0000 0000 0000 0000 0000 0500 0000  ................
-000000f0: 0000 0000 73b6 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+000000f0: 0000 0000 73a2 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
 00000100: 0255 0064 015a 0364 025a 0465 0565 0664  .U.d.Z.d.Z.e.e.d
 00000110: 033c 0064 045a 0765 0565 0664 053c 0064  .<.d.Z.e.e.d.<.d
-00000120: 045a 0865 0565 0664 063c 0064 075a 0965  .Z.e.e.d.<.d.Z.e
-00000130: 0a65 0664 083c 0064 095a 0b65 0a65 0664  .e.d.<.d.Z.e.e.d
-00000140: 0a3c 0064 0b5a 0c65 0565 0664 0c3c 0064  .<.d.Z.e.e.d.<.d
-00000150: 0d5a 0d65 0e64 0e83 015a 0f64 0f5a 1087  .Z.e.d...Z.d.Z..
-00000160: 0066 0164 1064 1184 085a 1164 1264 1384  .f.d.d...Z.d.d..
-00000170: 005a 1264 1464 1584 005a 1364 1664 1784  .Z.d.d...Z.d.d..
-00000180: 005a 1464 1864 1984 005a 1564 1a64 1b84  .Z.d.d...Z.d.d..
-00000190: 005a 1664 2064 1c65 1764 1d65 1866 0464  .Z.d d.e.d.e.f.d
-000001a0: 1e64 1f84 055a 1987 0004 005a 1a53 0029  .d...Z.....Z.S.)
-000001b0: 21da 0447 616d 657a 4153 7065 6369 616c  !..GamezASpecial
-000001c0: 2063 6173 6520 6f66 2045 6e74 6974 793b   case of Entity;
-000001d0: 2069 7420 6973 2061 7420 7468 6520 7665   it is at the ve
-000001e0: 7279 2074 6f70 206f 6620 7468 6520 6f62  ry top of the ob
-000001f0: 6a65 6374 2074 7265 652e e93c 0000 00da  ject tree..<....
-00000200: 0366 7073 69f4 0100 00da 0c77 696e 646f  .fpsi......windo
-00000210: 775f 7769 6474 68da 0d77 696e 646f 775f  w_width..window_
-00000220: 6865 6967 6874 da00 da0e 7769 6e64 6f77  height....window
-00000230: 5f63 6170 7469 6f6e 5a0f 7562 756e 7475  _captionZ.ubuntu
-00000240: 636f 6e64 656e 7365 64da 0966 6f6e 745f  condensed..font_
-00000250: 6e61 6d65 e91e 0000 00da 0966 6f6e 745f  name.......font_
-00000260: 7369 7a65 da04 6761 6d65 da05 626c 6163  size..game..blac
-00000270: 6b46 6301 0000 0000 0000 0000 0000 0001  kFc.............
-00000280: 0000 0005 0000 0003 0000 0073 8600 0000  ...........s....
-00000290: 7400 8300 a001 a100 0100 7402 a003 a100  t.........t.....
-000002a0: 0100 7404 8300 7c00 5f05 7406 8300 7c00  ..t...|._.t...|.
-000002b0: 5f07 7c00 6a05 6701 7c00 5f08 7402 6a09  _.|.j.g.|._.t.j.
-000002c0: a003 a100 0100 7402 6a09 a00a 7402 6a09  ......t.j...t.j.
-000002d0: a00b 7c00 6a0c a101 7c00 6a0d a102 7c00  ..|.j...|.j...|.
-000002e0: 5f09 7402 6a0e a00f 7c00 6a10 7c00 6a11  _.t.j...|.j.|.j.
-000002f0: 6602 a101 7c00 5f12 7402 6a0e a013 7c00  f...|._.t.j...|.
-00000300: 6a14 a101 0100 7402 6a15 a016 a100 7c00  j.....t.j.....|.
-00000310: 5f17 6400 5300 a901 4e29 18da 0573 7570  _.d.S...N)...sup
-00000320: 6572 da08 5f5f 696e 6974 5f5f da06 7079  er..__init__..py
-00000330: 6761 6d65 da04 696e 6974 7206 0000 00da  game..initr.....
-00000340: 0673 6365 6e65 7372 0700 0000 da0b 6670  .scenesr......fp
-00000350: 735f 7472 6163 6b65 72da 0c63 6869 6c64  s_tracker..child
-00000360: 5f67 726f 7570 73da 0466 6f6e 74da 0446  _groups..font..F
-00000370: 6f6e 74da 0a6d 6174 6368 5f66 6f6e 7472  ont..match_fontr
-00000380: 0f00 0000 7211 0000 00da 0764 6973 706c  ....r......displ
-00000390: 6179 da08 7365 745f 6d6f 6465 720b 0000  ay..set_moder...
-000003a0: 0072 0c00 0000 da06 7769 6e64 6f77 da0b  .r......window..
-000003b0: 7365 745f 6361 7074 696f 6e72 0e00 0000  set_captionr....
-000003c0: da04 7469 6d65 da05 436c 6f63 6bda 0563  ..time..Clock..c
-000003d0: 6c6f 636b a901 da04 7365 6c66 a901 da09  lock....self....
-000003e0: 5f5f 636c 6173 735f 5fa9 00fa 352f 686f  __class__...5/ho
-000003f0: 6d65 2f62 696e 6e65 762f 636f 6465 2f72  me/binnev/code/r
-00000400: 6f62 696e 6761 6d65 2f72 6f62 696e 6761  obingame/robinga
-00000410: 6d65 2f6f 626a 6563 7473 2f67 616d 652e  me/objects/game.
-00000420: 7079 7216 0000 0019 0000 0073 1400 0000  pyr........s....
-00000430: 0a01 0801 0802 0801 0a01 0a02 1c01 1601  ................
-00000440: 0e01 1001 7a0d 4761 6d65 2e5f 5f69 6e69  ....z.Game.__ini
-00000450: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000460: 0100 0000 0400 0000 4300 0000 7340 0000  ........C...s@..
-00000470: 0064 017c 005f 007c 006a 0072 167c 00a0  .d.|._.|.j.r.|..
-00000480: 01a1 0001 007c 006a 027c 006a 037c 006a  .....|.j.|.j.|.j
-00000490: 0464 028d 0201 007c 006a 0073 0674 05a0  .d.....|.j.s.t..
-000004a0: 06a1 0001 0074 07a0 08a1 0001 0064 0353  .....t.......d.S
-000004b0: 0029 047a 9c54 6869 7320 6973 2074 6865  .).z.This is the
-000004c0: 206f 7574 6572 6d6f 7374 2067 616d 6520   outermost game 
-000004d0: 6675 6e63 7469 6f6e 2077 6869 6368 2072  function which r
-000004e0: 756e 7320 6f6e 6365 2e20 4974 2063 6f6e  uns once. It con
-000004f0: 7461 696e 7320 7468 6520 6f75 7465 726d  tains the outerm
-00000500: 6f73 7420 6761 6d65 0a20 2020 2020 2020  ost game.       
-00000510: 206c 6f6f 702e 2048 6572 6527 7320 7768   loop. Here's wh
-00000520: 6572 6520 796f 7520 7368 6f75 6c64 2070  ere you should p
-00000530: 7574 2079 6f75 7220 6d61 696e 2065 7665  ut your main eve
-00000540: 6e74 2073 7461 7465 206d 6163 6869 6e65  nt state machine
-00000550: 2e54 2901 da05 6465 6275 674e 2909 5a07  .T)...debugN).Z.
-00000560: 7275 6e6e 696e 67da 075f 7570 6461 7465  running.._update
-00000570: da05 5f64 7261 7772 2100 0000 722c 0000  .._drawr!...r,..
-00000580: 0072 1700 0000 da04 7175 6974 da03 7379  .r......quit..sy
-00000590: 73da 0465 7869 7472 2600 0000 722a 0000  s..exitr&...r*..
-000005a0: 0072 2a00 0000 722b 0000 00da 046d 6169  .r*...r+.....mai
-000005b0: 6e27 0000 0073 0e00 0000 0603 0601 0801  n'...s..........
-000005c0: 1201 06fe 0803 0c01 7a09 4761 6d65 2e6d  ........z.Game.m
-000005d0: 6169 6e63 0100 0000 0000 0000 0000 0000  ainc............
-000005e0: 0200 0000 0400 0000 4700 0000 7316 0000  ........G...s...
-000005f0: 007c 006a 007c 0164 017c 006a 0169 018e  .|.j.|.d.|.j.i..
-00000600: 0101 0064 0053 0029 024e da05 6772 6f75  ...d.S.).N..grou
-00000610: 7029 02da 0c61 6464 5f74 6f5f 6772 6f75  p)...add_to_grou
-00000620: 7072 1900 0000 2902 7227 0000 00da 076f  pr....).r'.....o
-00000630: 626a 6563 7473 722a 0000 0072 2a00 0000  bjectsr*...r*...
-00000640: 722b 0000 00da 0961 6464 5f73 6365 6e65  r+.....add_scene
-00000650: 3100 0000 7302 0000 0016 017a 0e47 616d  1...s......z.Gam
-00000660: 652e 6164 645f 7363 656e 6563 0100 0000  e.add_scenec....
-00000670: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000680: 4300 0000 7356 0000 0074 00a0 01a1 0001  C...sV...t......
-00000690: 0074 006a 0244 005d 217d 017c 016a 0374  .t.j.D.]!}.|.j.t
-000006a0: 046a 056b 0272 1774 04a0 06a1 0001 0074  .j.k.r.t.......t
-000006b0: 07a0 08a1 0001 007c 016a 0374 046a 096b  .......|.j.t.j.k
-000006c0: 0272 287c 016a 0a74 046a 0b6b 0272 287c  .r(|.j.t.j.k.r(|
-000006d0: 006a 0c0c 007c 005f 0c71 0764 0153 0029  .j...|._.q.d.S.)
-000006e0: 0261 0901 0000 4927 7665 2070 7574 2074  .a....I've put t
-000006f0: 6869 7320 696e 2061 2073 6570 6172 6174  his in a separat
-00000700: 6520 6d65 7468 6f64 2062 6563 6175 7365  e method because
-00000710: 2049 2064 6f6e 2774 206c 696b 6520 7468   I don't like th
-00000720: 6520 6964 6561 206f 6620 7075 7474 696e  e idea of puttin
-00000730: 6720 7468 6520 696e 7075 7473 0a20 2020  g the inputs.   
-00000740: 2020 2020 2069 6e20 7468 6520 7361 6d65       in the same
-00000750: 206c 6973 7420 6173 206f 7468 6572 2063   list as other c
-00000760: 6869 6c64 2067 726f 7570 732e 2054 6865  hild groups. The
-00000770: 206f 7264 6572 206d 6967 6874 2067 6574   order might get
-00000780: 2072 7569 6e65 642c 206f 7220 6120 7375   ruined, or a su
-00000790: 6263 6c61 7373 206d 6967 6874 0a20 2020  bclass might.   
-000007a0: 2020 2020 206f 7665 7277 7269 7465 2074       overwrite t
-000007b0: 6865 206c 6973 742e 2049 7427 7320 6372  he list. It's cr
-000007c0: 7563 6961 6c20 7468 6174 2074 6865 2069  ucial that the i
-000007d0: 6e70 7574 7320 6172 6520 7265 6164 2062  nputs are read b
-000007e0: 6566 6f72 6520 7570 6461 7469 6e67 2e4e  efore updating.N
-000007f0: 290d 7204 0000 00da 0675 7064 6174 65da  ).r......update.
-00000800: 0665 7665 6e74 73da 0474 7970 6572 1700  .events..typer..
-00000810: 0000 da04 5155 4954 722f 0000 0072 3000  ....QUITr/...r0.
-00000820: 0000 7231 0000 00da 074b 4559 444f 574e  ..r1.....KEYDOWN
-00000830: da03 6b65 79da 044b 5f46 3172 2c00 0000  ..key..K_F1r,...
-00000840: 2902 7227 0000 00da 0565 7665 6e74 722a  ).r'.....eventr*
-00000850: 0000 0072 2a00 0000 722b 0000 00da 0b72  ...r*...r+.....r
-00000860: 6561 645f 696e 7075 7473 3400 0000 7312  ead_inputs4...s.
-00000870: 0000 0008 040a 010c 0108 0108 0118 010a  ................
-00000880: 0102 8004 fb7a 1047 616d 652e 7265 6164  .....z.Game.read
-00000890: 5f69 6e70 7574 7363 0100 0000 0000 0000  _inputsc........
-000008a0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000008b0: 7304 0000 0064 0053 0072 1400 0000 722a  s....d.S.r....r*
-000008c0: 0000 0072 2600 0000 722a 0000 0072 2a00  ...r&...r*...r*.
-000008d0: 0000 722b 0000 00da 1070 7269 6e74 5f64  ..r+.....print_d
-000008e0: 6562 7567 5f69 6e66 6f40 0000 0073 0200  ebug_info@...s..
-000008f0: 0000 0401 7a15 4761 6d65 2e70 7269 6e74  ....z.Game.print
-00000900: 5f64 6562 7567 5f69 6e66 6f63 0100 0000  _debug_infoc....
-00000910: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000920: 4300 0000 7344 0000 007c 00a0 00a1 0001  C...sD...|......
-00000930: 007c 006a 0172 0b7c 00a0 02a1 0001 007c  .|.j.r.|.......|
-00000940: 00a0 03a1 0001 007c 006a 04a0 03a1 0001  .......|.j......
-00000950: 007c 006a 0572 207c 006a 06a0 077c 006a  .|.j.r |.j...|.j
-00000960: 05a1 0101 0064 0153 0064 0153 0029 027a  .....d.S.d.S.).z
-00000970: 320a 2020 2020 2020 2020 312e 2072 6561  2.        1. rea
-00000980: 6420 696e 7075 7473 0a20 2020 2020 2020  d inputs.       
-00000990: 2032 2e20 7570 6461 7465 0a20 2020 2020   2. update.     
-000009a0: 2020 204e 2908 723f 0000 0072 2c00 0000     N).r?...r,...
-000009b0: 7240 0000 0072 3700 0000 721a 0000 0072  r@...r7...r....r
-000009c0: 0a00 0000 7225 0000 00da 0474 6963 6b72  ....r%.....tickr
-000009d0: 2600 0000 722a 0000 0072 2a00 0000 722b  &...r*...r*...r+
-000009e0: 0000 0072 2d00 0000 4300 0000 7310 0000  ...r-...C...s...
-000009f0: 0008 0506 0108 0108 010a 0106 0112 0104  ................
-00000a00: ff7a 0c47 616d 652e 5f75 7064 6174 65da  .z.Game._update.
-00000a10: 0773 7572 6661 6365 722c 0000 0063 0300  .surfacer,...c..
-00000a20: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000a30: 0000 4300 0000 7334 0000 007c 01a0 007c  ..C...s4...|...|
-00000a40: 006a 01a1 0101 007c 00a0 027c 017c 02a1  .j.....|...|.|..
-00000a50: 0201 007c 006a 03a0 027c 017c 02a1 0201  ...|.j...|.|....
-00000a60: 0074 046a 05a0 06a1 0001 0064 0053 0072  .t.j.......d.S.r
-00000a70: 1400 0000 2907 da04 6669 6c6c da0c 7363  ....)...fill..sc
-00000a80: 7265 656e 5f63 6f6c 6f72 da04 6472 6177  reen_color..draw
-00000a90: 721a 0000 0072 1700 0000 721f 0000 0072  r....r....r....r
-00000aa0: 3700 0000 2903 7227 0000 0072 4200 0000  7...).r'...rB...
-00000ab0: 722c 0000 0072 2a00 0000 722a 0000 0072  r,...r*...r*...r
-00000ac0: 2b00 0000 722e 0000 0050 0000 0073 0800  +...r....P...s..
-00000ad0: 0000 0c01 0c01 0e01 0e01 7a0a 4761 6d65  ..........z.Game
-00000ae0: 2e5f 6472 6177 2901 4629 1bda 085f 5f6e  ._draw).F)...__n
-00000af0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000b00: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000b10: 075f 5f64 6f63 5f5f 720a 0000 00da 0369  .__doc__r......i
-00000b20: 6e74 da0f 5f5f 616e 6e6f 7461 7469 6f6e  nt..__annotation
-00000b30: 735f 5f72 0b00 0000 720c 0000 0072 0e00  s__r....r....r..
-00000b40: 0000 da03 7374 7272 0f00 0000 7211 0000  ....strr....r...
-00000b50: 00da 0d70 6172 656e 7461 6c5f 6e61 6d65  ...parental_name
-00000b60: 7202 0000 0072 4400 0000 722c 0000 0072  r....rD...r,...r
-00000b70: 1600 0000 7232 0000 0072 3600 0000 723f  ....r2...r6...r?
-00000b80: 0000 0072 4000 0000 722d 0000 0072 0300  ...r@...r-...r..
-00000b90: 0000 da04 626f 6f6c 722e 0000 00da 0d5f  ....boolr......_
-00000ba0: 5f63 6c61 7373 6365 6c6c 5f5f 722a 0000  _classcell__r*..
-00000bb0: 0072 2a00 0000 7228 0000 0072 2b00 0000  .r*...r(...r+...
-00000bc0: 7208 0000 000c 0000 0073 2400 0000 0a00  r........s$.....
-00000bd0: 0401 0c02 0c01 0c01 0c01 0c01 0c01 0401  ................
-00000be0: 0801 0401 0c02 080e 080a 0803 080c 0803  ................
-00000bf0: 1c0d 7208 0000 0029 0e72 3000 0000 7217  ..r....).r0...r.
-00000c00: 0000 00da 0c70 7967 616d 652e 636f 6c6f  .....pygame.colo
-00000c10: 7272 0200 0000 5a0e 7079 6761 6d65 2e73  rr....Z.pygame.s
-00000c20: 7572 6661 6365 7203 0000 005a 0f72 6f62  urfacer....Z.rob
-00000c30: 696e 6761 6d65 2e69 6e70 7574 7204 0000  ingame.inputr...
-00000c40: 005a 1872 6f62 696e 6761 6d65 2e6f 626a  .Z.robingame.obj
-00000c50: 6563 7473 2e65 6e74 6974 7972 0500 0000  ects.entityr....
-00000c60: 7206 0000 005a 1972 6f62 696e 6761 6d65  r....Z.robingame
-00000c70: 2e6f 626a 6563 7473 2e68 656c 7065 7273  .objects.helpers
-00000c80: 7207 0000 0072 0800 0000 722a 0000 0072  r....r....r*...r
-00000c90: 2a00 0000 722a 0000 0072 2b00 0000 da08  *...r*...r+.....
-00000ca0: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
-00000cb0: 0008 0008 020c 010c 010c 0210 010c 0114  ................
-00000cc0: 03                                       .
+00000120: 045a 0865 0565 0664 063c 0064 005a 0965  .Z.e.e.d.<.d.Z.e
+00000130: 0a65 0664 073c 0065 0b64 0883 015a 0c64  .e.d.<.e.d...Z.d
+00000140: 095a 0d65 0e65 0664 0a3c 0065 0e65 0664  .Z.e.e.d.<.e.e.d
+00000150: 0b3c 0087 0066 0164 0c64 0d84 085a 0f64  .<...f.d.d...Z.d
+00000160: 0e64 0f84 005a 1064 1064 1184 005a 1164  .d...Z.d.d...Z.d
+00000170: 1264 1384 005a 1264 1464 1584 005a 1364  .d...Z.d.d...Z.d
+00000180: 1964 1665 1464 0a65 0e66 0464 1764 1884  .d.e.d.e.f.d.d..
+00000190: 055a 1587 0004 005a 1653 0029 1ada 0447  .Z.....Z.S.)...G
+000001a0: 616d 657a 820a 2020 2020 5370 6563 6961  amez..    Specia
+000001b0: 6c20 6361 7365 206f 6620 456e 7469 7479  l case of Entity
+000001c0: 3b20 6974 2069 7320 6174 2074 6865 2076  ; it is at the v
+000001d0: 6572 7920 746f 7020 6f66 2074 6865 206f  ery top of the o
+000001e0: 626a 6563 7420 7472 6565 2e0a 2020 2020  bject tree..    
+000001f0: 4861 6e64 6c65 7320 7365 7474 696e 6720  Handles setting 
+00000200: 7570 2061 6e64 2072 756e 6e69 6e67 2074  up and running t
+00000210: 6865 206d 6169 6e20 6761 6d65 206c 6f6f  he main game loo
+00000220: 702e 0a20 2020 20e9 3c00 0000 da03 6670  p..    .<.....fp
+00000230: 7369 f401 0000 da0c 7769 6e64 6f77 5f77  si......window_w
+00000240: 6964 7468 da0d 7769 6e64 6f77 5f68 6569  idth..window_hei
+00000250: 6768 74da 0e77 696e 646f 775f 6361 7074  ght..window_capt
+00000260: 696f 6eda 0562 6c61 636b 46da 0564 6562  ion..blackF..deb
+00000270: 7567 da07 7275 6e6e 696e 6763 0100 0000  ug..runningc....
+00000280: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000290: 0300 0000 734e 0000 0074 0083 00a0 01a1  ....sN...t......
+000002a0: 0001 0074 02a0 03a1 0001 0074 0483 007c  ...t.......t...|
+000002b0: 005f 0574 026a 06a0 077c 006a 087c 006a  ._.t.j...|.j.|.j
+000002c0: 0966 02a1 017c 005f 0a74 026a 06a0 0b7c  .f...|._.t.j...|
+000002d0: 006a 0ca1 0101 0074 026a 0da0 0ea1 007c  .j.....t.j.....|
+000002e0: 005f 0f64 0053 00a9 014e 2910 da05 7375  ._.d.S...N)...su
+000002f0: 7065 72da 085f 5f69 6e69 745f 5fda 0670  per..__init__..p
+00000300: 7967 616d 65da 0469 6e69 7472 0700 0000  ygame..initr....
+00000310: da0b 6670 735f 7472 6163 6b65 72da 0764  ..fps_tracker..d
+00000320: 6973 706c 6179 da08 7365 745f 6d6f 6465  isplay..set_mode
+00000330: 720b 0000 0072 0c00 0000 da06 7769 6e64  r....r......wind
+00000340: 6f77 da0b 7365 745f 6361 7074 696f 6e72  ow..set_captionr
+00000350: 0d00 0000 da04 7469 6d65 da05 436c 6f63  ......time..Cloc
+00000360: 6bda 0563 6c6f 636b a901 da04 7365 6c66  k..clock....self
+00000370: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
+00000380: 342f 686f 6d65 2f72 6f62 696e 2f63 6f64  4/home/robin/cod
+00000390: 652f 726f 6269 6e67 616d 652f 726f 6269  e/robingame/robi
+000003a0: 6e67 616d 652f 6f62 6a65 6374 732f 6761  ngame/objects/ga
+000003b0: 6d65 2e70 7972 1300 0000 1a00 0000 730c  me.pyr........s.
+000003c0: 0000 000a 0108 0108 0116 010e 0110 017a  ...............z
+000003d0: 0d47 616d 652e 5f5f 696e 6974 5f5f 6301  .Game.__init__c.
+000003e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000003f0: 0000 0043 0000 0073 4000 0000 6401 7c00  ...C...s@...d.|.
+00000400: 5f00 7c00 6a00 7216 7c00 a001 a100 0100  _.|.j.r.|.......
+00000410: 7c00 6a02 7c00 6a03 7c00 6a04 6402 8d02  |.j.|.j.|.j.d...
+00000420: 0100 7c00 6a00 7306 7405 a006 a100 0100  ..|.j.s.t.......
+00000430: 7407 a008 a100 0100 6403 5300 2904 7aae  t.......d.S.).z.
+00000440: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+00000450: 2074 6865 206f 7574 6572 6d6f 7374 2067   the outermost g
+00000460: 616d 6520 6675 6e63 7469 6f6e 2077 6869  ame function whi
+00000470: 6368 2072 756e 7320 6f6e 6365 2e20 4974  ch runs once. It
+00000480: 2063 6f6e 7461 696e 7320 7468 6520 6f75   contains the ou
+00000490: 7465 726d 6f73 7420 6761 6d65 206c 6f6f  termost game loo
+000004a0: 702e 0a20 2020 2020 2020 2048 6572 6527  p..        Here'
+000004b0: 7320 7768 6572 6520 796f 7520 7368 6f75  s where you shou
+000004c0: 6c64 2070 7574 2079 6f75 7220 6d61 696e  ld put your main
+000004d0: 2065 7665 6e74 2073 7461 7465 206d 6163   event state mac
+000004e0: 6869 6e65 2e0a 2020 2020 2020 2020 5429  hine..        T)
+000004f0: 0172 0f00 0000 4e29 0972 1000 0000 da07  .r....N).r......
+00000500: 5f75 7064 6174 65da 055f 6472 6177 7219  _update.._drawr.
+00000510: 0000 0072 0f00 0000 7214 0000 00da 0471  ...r....r......q
+00000520: 7569 74da 0373 7973 da04 6578 6974 721e  uit..sys..exitr.
+00000530: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00000540: 0000 da04 6d61 696e 2200 0000 730e 0000  ....main"...s...
+00000550: 0006 0506 0108 0112 0106 fe08 030c 017a  ...............z
+00000560: 0947 616d 652e 6d61 696e 6301 0000 0000  .Game.mainc.....
+00000570: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000580: 0000 0073 5600 0000 7400 a001 a100 0100  ...sV...t.......
+00000590: 7400 6a02 4400 5d21 7d01 7c01 6a03 7404  t.j.D.]!}.|.j.t.
+000005a0: 6a05 6b02 7217 7404 a006 a100 0100 7407  j.k.r.t.......t.
+000005b0: a008 a100 0100 7c01 6a03 7404 6a09 6b02  ......|.j.t.j.k.
+000005c0: 7228 7c01 6a0a 7404 6a0b 6b02 7228 7c00  r(|.j.t.j.k.r(|.
+000005d0: 6a0c 0c00 7c00 5f0c 7107 6401 5300 2902  j...|._.q.d.S.).
+000005e0: 611b 0100 000a 2020 2020 2020 2020 4927  a.....        I'
+000005f0: 7665 2070 7574 2074 6869 7320 696e 2061  ve put this in a
+00000600: 2073 6570 6172 6174 6520 6d65 7468 6f64   separate method
+00000610: 2062 6563 6175 7365 2049 2064 6f6e 2774   because I don't
+00000620: 206c 696b 6520 7468 6520 6964 6561 206f   like the idea o
+00000630: 6620 7075 7474 696e 6720 7468 6520 696e  f putting the in
+00000640: 7075 7473 2069 6e0a 2020 2020 2020 2020  puts in.        
+00000650: 7468 6520 7361 6d65 206c 6973 7420 6173  the same list as
+00000660: 206f 7468 6572 2063 6869 6c64 2067 726f   other child gro
+00000670: 7570 732e 2054 6865 206f 7264 6572 206d  ups. The order m
+00000680: 6967 6874 2067 6574 2072 7569 6e65 642c  ight get ruined,
+00000690: 206f 7220 6120 7375 6263 6c61 7373 206d   or a subclass m
+000006a0: 6967 6874 0a20 2020 2020 2020 206f 7665  ight.        ove
+000006b0: 7277 7269 7465 2074 6865 206c 6973 742e  rwrite the list.
+000006c0: 2049 7427 7320 6372 7563 6961 6c20 7468   It's crucial th
+000006d0: 6174 2074 6865 2069 6e70 7574 7320 6172  at the inputs ar
+000006e0: 6520 7265 6164 2062 6566 6f72 6520 7570  e read before up
+000006f0: 6461 7469 6e67 2e0a 2020 2020 2020 2020  dating..        
+00000700: 4e29 0d72 0400 0000 da06 7570 6461 7465  N).r......update
+00000710: da06 6576 656e 7473 da04 7479 7065 7214  ..events..typer.
+00000720: 0000 00da 0451 5549 5472 2600 0000 7227  .....QUITr&...r'
+00000730: 0000 0072 2800 0000 da07 4b45 5944 4f57  ...r(.....KEYDOW
+00000740: 4eda 036b 6579 da04 4b5f 4631 720f 0000  N..key..K_F1r...
+00000750: 0029 0272 1f00 0000 da05 6576 656e 7472  .).r......eventr
+00000760: 2200 0000 7222 0000 0072 2300 0000 da0b  "...r"...r#.....
+00000770: 7265 6164 5f69 6e70 7574 732e 0000 0073  read_inputs....s
+00000780: 1200 0000 0806 0a01 0c01 0801 0801 1801  ................
+00000790: 0a01 0280 04fb 7a10 4761 6d65 2e72 6561  ......z.Game.rea
+000007a0: 645f 696e 7075 7473 6301 0000 0000 0000  d_inputsc.......
+000007b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+000007c0: 0073 0400 0000 6400 5300 7211 0000 0072  .s....d.S.r....r
+000007d0: 2200 0000 721e 0000 0072 2200 0000 7222  "...r....r"...r"
+000007e0: 0000 0072 2300 0000 da10 7072 696e 745f  ...r#.....print_
+000007f0: 6465 6275 675f 696e 666f 3c00 0000 7302  debug_info<...s.
+00000800: 0000 0004 017a 1547 616d 652e 7072 696e  .....z.Game.prin
+00000810: 745f 6465 6275 675f 696e 666f 6301 0000  t_debug_infoc...
+00000820: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000830: 0043 0000 0073 4400 0000 7c00 a000 a100  .C...sD...|.....
+00000840: 0100 7c00 6a01 720b 7c00 a002 a100 0100  ..|.j.r.|.......
+00000850: 7c00 a003 a100 0100 7c00 6a04 a003 a100  |.......|.j.....
+00000860: 0100 7c00 6a05 7220 7c00 6a06 a007 7c00  ..|.j.r |.j...|.
+00000870: 6a05 a101 0100 6401 5300 6401 5300 2902  j.....d.S.d.S.).
+00000880: 7a32 0a20 2020 2020 2020 2031 2e20 7265  z2.        1. re
+00000890: 6164 2069 6e70 7574 730a 2020 2020 2020  ad inputs.      
+000008a0: 2020 322e 2075 7064 6174 650a 2020 2020    2. update.    
+000008b0: 2020 2020 4e29 0872 3200 0000 720f 0000      N).r2...r...
+000008c0: 0072 3300 0000 722a 0000 0072 1600 0000  .r3...r*...r....
+000008d0: 720a 0000 0072 1d00 0000 da04 7469 636b  r....r......tick
+000008e0: 721e 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
+000008f0: 2300 0000 7224 0000 003f 0000 0073 1000  #...r$...?...s..
+00000900: 0000 0805 0601 0801 0801 0a01 0601 1201  ................
+00000910: 04ff 7a0c 4761 6d65 2e5f 7570 6461 7465  ..z.Game._update
+00000920: da07 7375 7266 6163 6563 0300 0000 0000  ..surfacec......
+00000930: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000940: 0000 7334 0000 007c 01a0 007c 006a 01a1  ..s4...|...|.j..
+00000950: 0101 007c 00a0 027c 017c 02a1 0201 007c  ...|...|.|.....|
+00000960: 006a 03a0 027c 017c 02a1 0201 0074 046a  .j...|.|.....t.j
+00000970: 05a0 06a1 0001 0064 0053 0072 1100 0000  .......d.S.r....
+00000980: 2907 da04 6669 6c6c da0c 7363 7265 656e  )...fill..screen
+00000990: 5f63 6f6c 6f72 da04 6472 6177 7216 0000  _color..drawr...
+000009a0: 0072 1400 0000 7217 0000 0072 2a00 0000  .r....r....r*...
+000009b0: 2903 721f 0000 0072 3500 0000 720f 0000  ).r....r5...r...
+000009c0: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+000009d0: 7225 0000 004c 0000 0073 0800 0000 0c01  r%...L...s......
+000009e0: 0c01 0e01 0e01 7a0a 4761 6d65 2e5f 6472  ......z.Game._dr
+000009f0: 6177 2901 4629 17da 085f 5f6e 616d 655f  aw).F)...__name_
+00000a00: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000a10: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00000a20: 6f63 5f5f 720a 0000 00da 0369 6e74 da0f  oc__r......int..
+00000a30: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00000a40: 0b00 0000 720c 0000 0072 0d00 0000 da03  ....r....r......
+00000a50: 7374 7272 0200 0000 7237 0000 0072 0f00  strr....r7...r..
+00000a60: 0000 da04 626f 6f6c 7213 0000 0072 2900  ....boolr....r).
+00000a70: 0000 7232 0000 0072 3300 0000 7224 0000  ..r2...r3...r$..
+00000a80: 0072 0300 0000 7225 0000 00da 0d5f 5f63  .r....r%.....__c
+00000a90: 6c61 7373 6365 6c6c 5f5f 7222 0000 0072  lasscell__r"...r
+00000aa0: 2200 0000 7220 0000 0072 2300 0000 7208  "...r ...r#...r.
+00000ab0: 0000 000c 0000 0073 1e00 0000 0a00 0401  .......s........
+00000ac0: 0c05 0c01 0c01 0c01 0801 0c01 0801 0c02  ................
+00000ad0: 0808 080c 080e 0803 1c0d 7208 0000 0029  ..........r....)
+00000ae0: 0e72 2700 0000 7214 0000 00da 0c70 7967  .r'...r......pyg
+00000af0: 616d 652e 636f 6c6f 7272 0200 0000 da0e  ame.colorr......
+00000b00: 7079 6761 6d65 2e73 7572 6661 6365 7203  pygame.surfacer.
+00000b10: 0000 00da 0f72 6f62 696e 6761 6d65 2e69  .....robingame.i
+00000b20: 6e70 7574 7204 0000 00da 1872 6f62 696e  nputr......robin
+00000b30: 6761 6d65 2e6f 626a 6563 7473 2e65 6e74  game.objects.ent
+00000b40: 6974 7972 0500 0000 7206 0000 00da 1972  ityr....r......r
+00000b50: 6f62 696e 6761 6d65 2e6f 626a 6563 7473  obingame.objects
+00000b60: 2e68 656c 7065 7273 7207 0000 0072 0800  .helpersr....r..
+00000b70: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
+00000b80: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
+00000b90: 0100 0000 7310 0000 0008 0008 020c 010c  ....s...........
+00000ba0: 010c 0210 010c 0114 03                   .........
```

### Comparing `robingame-0.0.9/robingame/objects/__pycache__/helpers.cpython-310.pyc` & `robingame-0.1.0/robingame/objects/__pycache__/helpers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 1189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 a504 0000  o.......u.5c....
+00000000: 6f0d 0d0a 0000 0000 8874 a564 a404 0000  o........t.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0a 6d0b 5a0b 0100 4700 6407 6408  d.l.m.Z...G.d.d.
-00000080: 8400 6408 6509 8303 5a0c 6401 5300 2909  ..d.e...Z.d.S.).
-00000090: e900 0000 004e 2901 da05 6465 7175 6529  .....N)...deque)
-000000a0: 01da 0543 6f6c 6f72 2901 da07 5375 7266  ...Color)...Surf
-000000b0: 6163 6529 01da 0645 6e74 6974 7929 01da  ace)...Entity)..
-000000c0: 0566 6f6e 7473 6300 0000 0000 0000 0000  .fontsc.........
-000000d0: 0000 0000 0000 0005 0000 0000 0000 0073  ...............s
-000000e0: 4800 0000 6500 5a01 6400 5a02 6401 5a03  H...e.Z.d.Z.d.Z.
-000000f0: 6402 5a04 6505 6a06 5a07 640e 8700 6601  d.Z.e.j.Z.d...f.
-00000100: 6405 6406 840c 5a08 6407 6408 8400 5a09  d.d...Z.d.d...Z.
-00000110: 640f 640a 650a 640b 650b 6604 640c 640d  d.d.e.d.e.f.d.d.
-00000120: 8405 5a0c 8700 0400 5a0d 5300 2910 da0a  ..Z.....Z.S.)...
-00000130: 4670 7354 7261 636b 6572 7a45 4469 7370  FpsTrackerzEDisp
-00000140: 6c61 7973 2061 206c 6974 746c 6520 6e75  lays a little nu
-00000150: 6d62 6572 2069 6e20 7468 6520 746f 7020  mber in the top 
-00000160: 7269 6768 7420 6f66 2074 6865 2077 696e  right of the win
-00000170: 646f 7720 6966 2064 6562 7567 3d54 7275  dow if debug=Tru
-00000180: 65e9 3c00 0000 da06 7265 7475 726e 4e63  e.<.....returnNc
-00000190: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000001a0: 0300 0000 0700 0000 731e 0000 0074 0083  ........s....t..
-000001b0: 006a 017c 018e 0001 0074 027c 006a 0364  .j.|.....t.|.j.d
-000001c0: 018d 017c 005f 0464 0053 0029 024e 2901  ...|._.d.S.).N).
-000001d0: da06 6d61 786c 656e 2905 da05 7375 7065  ..maxlen)...supe
-000001e0: 72da 085f 5f69 6e69 745f 5f72 0200 0000  r..__init__r....
-000001f0: da0d 6275 6666 6572 5f6c 656e 6774 68da  ..buffer_length.
-00000200: 0571 7565 7565 2902 da04 7365 6c66 da06  .queue)...self..
-00000210: 6772 6f75 7073 a901 da09 5f5f 636c 6173  groups....__clas
-00000220: 735f 5fa9 00fa 382f 686f 6d65 2f62 696e  s__...8/home/bin
-00000230: 6e65 762f 636f 6465 2f72 6f62 696e 6761  nev/code/robinga
-00000240: 6d65 2f72 6f62 696e 6761 6d65 2f6f 626a  me/robingame/obj
-00000250: 6563 7473 2f68 656c 7065 7273 2e70 7972  ects/helpers.pyr
-00000260: 0c00 0000 1200 0000 7304 0000 000c 0112  ........s.......
-00000270: 017a 1346 7073 5472 6163 6b65 722e 5f5f  .z.FpsTracker.__
-00000280: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000290: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-000002a0: 4a00 0000 7400 a001 a100 7d01 7c00 6a02  J...t.....}.|.j.
-000002b0: a003 7c01 a101 0100 7c00 6a02 6401 1900  ..|.....|.j.d...
-000002c0: 7c00 6a02 6402 1900 1800 7d02 7c02 7220  |.j.d.....}.|.r 
-000002d0: 7404 7c00 6a05 7c02 1b00 8301 7c00 5f06  t.|.j.|.....|._.
-000002e0: 6400 5300 6402 7c00 5f06 6400 5300 2903  d.S.d.|._.d.S.).
-000002f0: 4ee9 ffff ffff 7201 0000 0029 07da 0474  N.....r....)...t
-00000300: 696d 65da 0c70 6572 665f 636f 756e 7465  ime..perf_counte
-00000310: 7272 0e00 0000 da06 6170 7065 6e64 da03  rr......append..
-00000320: 696e 7472 0d00 0000 da03 6670 7329 0372  intr......fps).r
-00000330: 0f00 0000 da01 74da 0773 6563 6f6e 6473  ......t..seconds
-00000340: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000350: 0675 7064 6174 6516 0000 0073 0800 0000  .update....s....
-00000360: 0801 0c01 1401 2201 7a11 4670 7354 7261  ......".z.FpsTra
-00000370: 636b 6572 2e75 7064 6174 6546 da07 7375  cker.updateF..su
-00000380: 7266 6163 65da 0564 6562 7567 6303 0000  rface..debugc...
-00000390: 0000 0000 0000 0000 0007 0000 0007 0000  ................
-000003a0: 0043 0000 0073 8800 0000 7c02 7242 6401  .C...s....|.rBd.
-000003b0: 7d03 6402 7c03 1400 7d04 7400 7c04 7c04  }.d.|...}.t.|.|.
-000003c0: 6403 1a00 6602 8301 7d05 7c05 a001 7402  d...f...}.|...t.
-000003d0: 6404 8301 a101 0100 7c00 6a03 6a04 7c05  d.......|.j.j.|.
-000003e0: 6405 7c00 6a05 9b00 9d02 7c04 6406 7c03  d.|.j.....|.d.|.
-000003f0: 6407 8d05 0100 7c05 a006 a100 7d06 7c01  d.....|.....}.|.
-00000400: a006 a100 6a07 6408 1800 7c06 5f07 7c01  ....j.d...|._.|.
-00000410: a006 a100 6a08 6408 1700 7c06 5f08 7c01  ....j.d...|._.|.
-00000420: a009 7c05 7c06 a102 0100 6400 5300 6400  ..|.|.....d.S.d.
-00000430: 5300 2909 4ee9 0200 0000 e932 0000 00e9  S.).N......2....
-00000440: 0400 0000 da05 7768 6974 657a 0546 5053  ......whitez.FPS
-00000450: 3a20 7201 0000 0029 03da 0477 7261 70da  : r....)...wrap.
-00000460: 0561 6c69 676e da05 7363 616c 65e9 0a00  .align..scale...
-00000470: 0000 290a 7204 0000 00da 0466 696c 6c72  ..).r......fillr
-00000480: 0300 0000 da04 666f 6e74 da06 7265 6e64  ......font..rend
-00000490: 6572 721a 0000 00da 0867 6574 5f72 6563  err......get_rec
-000004a0: 74da 0572 6967 6874 da03 746f 70da 0462  t..right..top..b
-000004b0: 6c69 7429 0772 0f00 0000 721e 0000 0072  lit).r....r....r
-000004c0: 1f00 0000 7226 0000 00da 0577 6964 7468  ....r&.....width
-000004d0: da04 7375 7266 da04 7265 6374 7213 0000  ..surf..rectr...
-000004e0: 0072 1300 0000 7214 0000 00da 0464 7261  .r....r......dra
-000004f0: 771c 0000 0073 1600 0000 0401 0401 0801  w....s..........
-00000500: 1001 0e01 1e01 0801 1001 1001 1001 04f7  ................
-00000510: 7a0f 4670 7354 7261 636b 6572 2e64 7261  z.FpsTracker.dra
-00000520: 7729 0272 0900 0000 4e29 0146 290e da08  w).r....N).F)...
-00000530: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000540: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000550: 5f5f da07 5f5f 646f 635f 5f72 0d00 0000  __..__doc__r....
-00000560: 7206 0000 005a 0f63 656c 6c70 686f 6e65  r....Z.cellphone
-00000570: 5f62 6c61 636b 7229 0000 0072 0c00 0000  _blackr)...r....
-00000580: 721d 0000 0072 0400 0000 da04 626f 6f6c  r....r......bool
-00000590: 7232 0000 00da 0d5f 5f63 6c61 7373 6365  r2.....__classce
-000005a0: 6c6c 5f5f 7213 0000 0072 1300 0000 7211  ll__r....r....r.
-000005b0: 0000 0072 1400 0000 7207 0000 000c 0000  ...r....r.......
-000005c0: 0073 0e00 0000 0800 0401 0402 0601 0e02  .s..............
-000005d0: 0804 1c06 7207 0000 0029 0d72 1600 0000  ....r....).r....
-000005e0: da0b 636f 6c6c 6563 7469 6f6e 7372 0200  ..collectionsr..
-000005f0: 0000 da06 7079 6761 6d65 da0c 7079 6761  ....pygame..pyga
-00000600: 6d65 2e63 6f6c 6f72 7203 0000 00da 0e70  me.colorr......p
-00000610: 7967 616d 652e 7375 7266 6163 6572 0400  ygame.surfacer..
-00000620: 0000 da18 726f 6269 6e67 616d 652e 6f62  ....robingame.ob
-00000630: 6a65 6374 732e 656e 7469 7479 7205 0000  jects.entityr...
-00000640: 005a 1372 6f62 696e 6761 6d65 2e74 6578  .Z.robingame.tex
-00000650: 742e 666f 6e74 7206 0000 0072 0700 0000  t.fontr....r....
-00000660: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00000670: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000680: 0000 7310 0000 0008 000c 0108 020c 010c  ..s.............
-00000690: 010c 020c 0114 03                        .......
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 4700 6407 6408 8400 6408 6508 8303  ..G.d.d...d.e...
+00000080: 5a0b 6401 5300 2909 e900 0000 004e 2901  Z.d.S.)......N).
+00000090: da05 6465 7175 6529 01da 0543 6f6c 6f72  ..deque)...Color
+000000a0: 2901 da07 5375 7266 6163 6529 01da 0645  )...Surface)...E
+000000b0: 6e74 6974 7929 01da 0566 6f6e 7473 6300  ntity)...fontsc.
+000000c0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000000d0: 0000 0000 0000 0073 5200 0000 6500 5a01  .......sR...e.Z.
+000000e0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
+000000f0: 6a06 5a07 6508 6509 6403 3c00 640f 8700  j.Z.e.e.d.<.d...
+00000100: 6601 6406 6407 840c 5a0a 6408 6409 8400  f.d.d...Z.d.d...
+00000110: 5a0b 6410 640b 650c 640c 650d 6604 640d  Z.d.d.e.d.e.f.d.
+00000120: 640e 8405 5a0e 8700 0400 5a0f 5300 2911  d...Z.....Z.S.).
+00000130: da0a 4670 7354 7261 636b 6572 7a45 4469  ..FpsTrackerzEDi
+00000140: 7370 6c61 7973 2061 206c 6974 746c 6520  splays a little 
+00000150: 6e75 6d62 6572 2069 6e20 7468 6520 746f  number in the to
+00000160: 7020 7269 6768 7420 6f66 2074 6865 2077  p right of the w
+00000170: 696e 646f 7720 6966 2064 6562 7567 3d54  indow if debug=T
+00000180: 7275 65e9 3c00 0000 da03 6670 73da 0672  rue.<.....fps..r
+00000190: 6574 7572 6e4e 6301 0000 0000 0000 0000  eturnNc.........
+000001a0: 0000 0002 0000 0003 0000 0007 0000 0073  ...............s
+000001b0: 1e00 0000 7400 8300 6a01 7c01 8e00 0100  ....t...j.|.....
+000001c0: 7402 7c00 6a03 6401 8d01 7c00 5f04 6400  t.|.j.d...|._.d.
+000001d0: 5300 2902 4e29 01da 066d 6178 6c65 6e29  S.).N)...maxlen)
+000001e0: 05da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
+000001f0: 5f5f 7202 0000 00da 0d62 7566 6665 725f  __r......buffer_
+00000200: 6c65 6e67 7468 da05 7175 6575 6529 02da  length..queue)..
+00000210: 0473 656c 66da 0667 726f 7570 73a9 01da  .self..groups...
+00000220: 095f 5f63 6c61 7373 5f5f a900 fa37 2f68  .__class__...7/h
+00000230: 6f6d 652f 726f 6269 6e2f 636f 6465 2f72  ome/robin/code/r
+00000240: 6f62 696e 6761 6d65 2f72 6f62 696e 6761  obingame/robinga
+00000250: 6d65 2f6f 626a 6563 7473 2f68 656c 7065  me/objects/helpe
+00000260: 7273 2e70 7972 0d00 0000 1200 0000 7304  rs.pyr........s.
+00000270: 0000 000c 0112 017a 1346 7073 5472 6163  .......z.FpsTrac
+00000280: 6b65 722e 5f5f 696e 6974 5f5f 6301 0000  ker.__init__c...
+00000290: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000002a0: 0043 0000 0073 4a00 0000 7400 a001 a100  .C...sJ...t.....
+000002b0: 7d01 7c00 6a02 a003 7c01 a101 0100 7c00  }.|.j...|.....|.
+000002c0: 6a02 6401 1900 7c00 6a02 6402 1900 1800  j.d...|.j.d.....
+000002d0: 7d02 7c02 7220 7404 7c00 6a05 7c02 1b00  }.|.r t.|.j.|...
+000002e0: 8301 7c00 5f06 6400 5300 6402 7c00 5f06  ..|._.d.S.d.|._.
+000002f0: 6400 5300 2903 4ee9 ffff ffff 7201 0000  d.S.).N.....r...
+00000300: 0029 07da 0474 696d 65da 0c70 6572 665f  .)...time..perf_
+00000310: 636f 756e 7465 7272 0f00 0000 da06 6170  counterr......ap
+00000320: 7065 6e64 da03 696e 7472 0e00 0000 7209  pend..intr....r.
+00000330: 0000 0029 0372 1000 0000 da01 74da 0773  ...).r......t..s
+00000340: 6563 6f6e 6473 7214 0000 0072 1400 0000  econdsr....r....
+00000350: 7215 0000 00da 0675 7064 6174 6516 0000  r......update...
+00000360: 0073 0800 0000 0801 0c01 1401 2201 7a11  .s..........".z.
+00000370: 4670 7354 7261 636b 6572 2e75 7064 6174  FpsTracker.updat
+00000380: 6546 da07 7375 7266 6163 65da 0564 6562  eF..surface..deb
+00000390: 7567 6303 0000 0000 0000 0000 0000 0007  ugc.............
+000003a0: 0000 0007 0000 0043 0000 0073 8800 0000  .......C...s....
+000003b0: 7c02 7242 6401 7d03 6402 7c03 1400 7d04  |.rBd.}.d.|...}.
+000003c0: 7400 7c04 7c04 6403 1a00 6602 8301 7d05  t.|.|.d...f...}.
+000003d0: 7c05 a001 7402 6404 8301 a101 0100 7c00  |...t.d.......|.
+000003e0: 6a03 6a04 7c05 6405 7c00 6a05 9b00 9d02  j.j.|.d.|.j.....
+000003f0: 7c04 6406 7c03 6407 8d05 0100 7c05 a006  |.d.|.d.....|...
+00000400: a100 7d06 7c01 a006 a100 6a07 6408 1800  ..}.|.....j.d...
+00000410: 7c06 5f07 7c01 a006 a100 6a08 6408 1700  |._.|.....j.d...
+00000420: 7c06 5f08 7c01 a009 7c05 7c06 a102 0100  |._.|...|.|.....
+00000430: 6400 5300 6400 5300 2909 4ee9 0200 0000  d.S.d.S.).N.....
+00000440: e932 0000 00e9 0400 0000 da05 7768 6974  .2..........whit
+00000450: 657a 0546 5053 3a20 7201 0000 0029 03da  ez.FPS: r....)..
+00000460: 0477 7261 70da 0561 6c69 676e da05 7363  .wrap..align..sc
+00000470: 616c 65e9 0a00 0000 290a 7204 0000 00da  ale.....).r.....
+00000480: 0466 696c 6c72 0300 0000 da04 666f 6e74  .fillr......font
+00000490: da06 7265 6e64 6572 7209 0000 00da 0867  ..renderr......g
+000004a0: 6574 5f72 6563 74da 0572 6967 6874 da03  et_rect..right..
+000004b0: 746f 70da 0462 6c69 7429 0772 1000 0000  top..blit).r....
+000004c0: 721e 0000 0072 1f00 0000 7226 0000 00da  r....r....r&....
+000004d0: 0577 6964 7468 da04 7375 7266 da04 7265  .width..surf..re
+000004e0: 6374 7214 0000 0072 1400 0000 7215 0000  ctr....r....r...
+000004f0: 00da 0464 7261 771c 0000 0073 1600 0000  ...draw....s....
+00000500: 0401 0401 0801 1001 0e01 1e01 0801 1001  ................
+00000510: 1001 1001 04f7 7a0f 4670 7354 7261 636b  ......z.FpsTrack
+00000520: 6572 2e64 7261 7729 0272 0a00 0000 4e29  er.draw).r....N)
+00000530: 0146 2910 da08 5f5f 6e61 6d65 5f5f da0a  .F)...__name__..
+00000540: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000550: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000560: 5f72 0e00 0000 7206 0000 00da 0f63 656c  _r....r......cel
+00000570: 6c70 686f 6e65 5f62 6c61 636b 7229 0000  lphone_blackr)..
+00000580: 0072 1a00 0000 da0f 5f5f 616e 6e6f 7461  .r......__annota
+00000590: 7469 6f6e 735f 5f72 0d00 0000 721d 0000  tions__r....r...
+000005a0: 0072 0400 0000 da04 626f 6f6c 7232 0000  .r......boolr2..
+000005b0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+000005c0: 7214 0000 0072 1400 0000 7212 0000 0072  r....r....r....r
+000005d0: 1500 0000 7207 0000 000b 0000 0073 1000  ....r........s..
+000005e0: 0000 0a00 0401 0402 0601 0801 0e02 0804  ................
+000005f0: 1c06 7207 0000 0029 0c72 1700 0000 da0b  ..r....).r......
+00000600: 636f 6c6c 6563 7469 6f6e 7372 0200 0000  collectionsr....
+00000610: da0c 7079 6761 6d65 2e63 6f6c 6f72 7203  ..pygame.colorr.
+00000620: 0000 00da 0e70 7967 616d 652e 7375 7266  .....pygame.surf
+00000630: 6163 6572 0400 0000 da18 726f 6269 6e67  acer......robing
+00000640: 616d 652e 6f62 6a65 6374 732e 656e 7469  ame.objects.enti
+00000650: 7479 7205 0000 00da 1372 6f62 696e 6761  tyr......robinga
+00000660: 6d65 2e74 6578 742e 666f 6e74 7206 0000  me.text.fontr...
+00000670: 0072 0700 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000680: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+00000690: 756c 653e 0100 0000 730e 0000 0008 000c  ule>....s.......
+000006a0: 010c 020c 010c 020c 0114 03              ...........
```

### Comparing `robingame-0.0.9/robingame/objects/__pycache__/particles.cpython-310.pyc` & `robingame-0.1.0/robingame/objects/__pycache__/particles.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 1680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,121 +1,132 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 9006 0000  o.......u.5c....
+00000000: 6f0d 0d0a 0000 0000 8874 a564 fd07 0000  o........t.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
-00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
-00000060: 6d07 5a07 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
-00000070: 6505 8303 5a08 6401 5300 2908 e900 0000  e...Z.d.S.).....
-00000080: 004e 2901 da04 5265 6374 2901 da05 436f  .N)...Rect)...Co
-00000090: 6c6f 7229 01da 0e50 6879 7369 6361 6c45  lor)...PhysicalE
-000000a0: 6e74 6974 7929 01da 0b63 6972 636c 655f  ntity)...circle_
-000000b0: 7375 7266 6300 0000 0000 0000 0000 0000  surfc...........
-000000c0: 0000 0000 0004 0000 0000 0000 0073 7c00  .............s|.
-000000d0: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
-000000e0: 5a05 6506 6507 6401 3c00 6506 6507 6402  Z.e.e.d.<.e.e.d.
-000000f0: 3c00 6506 6507 6403 3c00 6508 6507 6404  <.e.e.d.<.e.e.d.
-00000100: 3c00 6506 6507 6405 3c00 0906 0906 0907  <.e.e.d.<.......
-00000110: 0907 0907 0907 0907 0907 6411 8700 6601  ..........d...f.
-00000120: 6408 6409 8409 5a09 640a 640b 8400 5a0a  d.d...Z.d.d...Z.
-00000130: 6412 640d 640e 8401 5a0b 650c 640f 6410  d.d.d...Z.e.d.d.
-00000140: 8400 8301 5a0d 8700 0400 5a0e 5300 2913  ....Z.....Z.S.).
-00000150: da08 5061 7274 6963 6c65 da07 6772 6176  ..Particle..grav
-00000160: 6974 79da 0866 7269 6374 696f 6eda 0564  ity..friction..d
-00000170: 6563 6179 da05 636f 6c6f 72da 0672 6164  ecay..color..rad
-00000180: 6975 7372 0100 0000 4e63 0b00 0000 0000  iusr....Nc......
-00000190: 0000 0000 0000 0b00 0000 0500 0000 0300  ................
-000001a0: 0000 73ae 0000 0074 0083 00a0 01a1 0001  ..s....t........
-000001b0: 007c 0664 0075 0072 0c7c 006a 026e 017c  .|.d.u.r.|.j.n.|
-000001c0: 067c 005f 027c 0764 0075 0072 167c 006a  .|._.|.d.u.r.|.j
-000001d0: 036e 017c 077c 005f 037c 0864 0075 0072  .n.|.|._.|.d.u.r
-000001e0: 207c 006a 046e 017c 087c 005f 047c 0964   |.j.n.|.|._.|.d
-000001f0: 0075 0072 2a7c 006a 056e 017c 097c 005f  .u.r*|.j.n.|.|._
-00000200: 057c 0a64 0075 0072 347c 006a 066e 017c  .|.d.u.r4|.j.n.|
-00000210: 0a7c 005f 067c 0564 0075 0072 3e7c 006a  .|._.|.d.u.r>|.j
-00000220: 076e 017c 057c 005f 0774 0864 0164 0164  .n.|.|._.t.d.d.d
-00000230: 0164 0183 047c 005f 097c 017c 005f 0a7c  .d...|._.|.|._.|
-00000240: 027c 005f 0b7c 037c 005f 0c7c 047c 005f  .|._.|.|._.|.|._
-00000250: 0d64 0053 00a9 024e 7201 0000 0029 0eda  .d.S...Nr....)..
-00000260: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
-00000270: 720a 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000280: 0900 0000 da09 626c 6974 5f66 6c61 6772  ......blit_flagr
-00000290: 0b00 0000 7202 0000 00da 0472 6563 74da  ....r......rect.
-000002a0: 0178 da01 79da 0175 da01 7629 0bda 0473  .x..y..u..v)...s
-000002b0: 656c 6672 1100 0000 7212 0000 0072 1300  elfr....r....r..
-000002c0: 0000 7214 0000 0072 0b00 0000 720a 0000  ..r....r....r...
-000002d0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-000002e0: 720f 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
-000002f0: 5f5f a900 fa3a 2f68 6f6d 652f 6269 6e6e  __...:/home/binn
-00000300: 6576 2f63 6f64 652f 726f 6269 6e67 616d  ev/code/robingam
-00000310: 652f 726f 6269 6e67 616d 652f 6f62 6a65  e/robingame/obje
-00000320: 6374 732f 7061 7274 6963 6c65 732e 7079  cts/particles.py
-00000330: 720e 0000 0011 0000 0073 1800 0000 0a0d  r........s......
-00000340: 1401 1401 1401 1401 1401 1401 1001 0601  ................
-00000350: 0601 0601 0a01 7a11 5061 7274 6963 6c65  ......z.Particle
-00000360: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000370: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000380: 0000 737e 0000 007c 0004 006a 007c 006a  ..s~...|...j.|.j
-00000390: 0137 0002 005f 007c 0004 006a 027c 006a  .7..._.|...j.|.j
-000003a0: 0337 0002 005f 027c 0004 006a 037c 006a  .7..._.|...j.|.j
-000003b0: 0437 0002 005f 037c 0004 006a 0164 017c  .7..._.|...j.d.|
-000003c0: 006a 0518 0039 0002 005f 017c 0004 006a  .j...9..._.|...j
-000003d0: 0364 017c 006a 0518 0039 0002 005f 037c  .d.|.j...9..._.|
-000003e0: 0004 006a 067c 006a 0738 0002 005f 067c  ...j.|.j.8..._.|
-000003f0: 006a 0872 3d7c 00a0 09a1 0001 0064 0053  .j.r=|.......d.S
-00000400: 0064 0053 0029 024e e901 0000 0029 0a72  .d.S.).N.....).r
-00000410: 1100 0000 7213 0000 0072 1200 0000 7214  ....r....r....r.
-00000420: 0000 0072 0700 0000 7208 0000 0072 0b00  ...r....r....r..
-00000430: 0000 7209 0000 00da 0f64 6561 7468 5f63  ..r......death_c
-00000440: 6f6e 6469 7469 6f6e da04 6b69 6c6c a901  ondition..kill..
-00000450: 7215 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000460: 1900 0000 da06 7570 6461 7465 2b00 0000  ......update+...
-00000470: 7312 0000 0010 0110 0110 0114 0114 0110  s...............
-00000480: 0106 010c 0104 ff7a 0f50 6172 7469 636c  .......z.Particl
-00000490: 652e 7570 6461 7465 4663 0300 0000 0000  e.updateFc......
-000004a0: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-000004b0: 0000 733a 0000 0074 0074 017c 006a 0283  ..s:...t.t.|.j..
-000004c0: 017c 006a 0383 027d 037c 03a0 04a1 007d  .|.j...}.|.....}
-000004d0: 047c 006a 056a 067c 045f 067c 016a 077c  .|.j.j.|._.|.j.|
-000004e0: 037c 047c 006a 0864 018d 0301 0064 0053  .|.|.j.d.....d.S
-000004f0: 0029 024e 2901 5a0d 7370 6563 6961 6c5f  .).N).Z.special_
-00000500: 666c 6167 7329 0972 0500 0000 da05 726f  flags).r......ro
-00000510: 756e 6472 0b00 0000 720a 0000 00da 0867  undr....r......g
-00000520: 6574 5f72 6563 7472 1000 0000 da06 6365  et_rectr......ce
-00000530: 6e74 6572 da04 626c 6974 720f 0000 0029  nter..blitr....)
-00000540: 0572 1500 0000 da07 7375 7266 6163 65da  .r......surface.
-00000550: 0564 6562 7567 da04 7375 7266 da0a 696d  .debug..surf..im
-00000560: 6167 655f 7265 6374 7218 0000 0072 1800  age_rectr....r..
-00000570: 0000 7219 0000 00da 0464 7261 7735 0000  ..r......draw5..
-00000580: 0073 0800 0000 1201 0801 0a01 1601 7a0d  .s............z.
-00000590: 5061 7274 6963 6c65 2e64 7261 7763 0100  Particle.drawc..
-000005a0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000005b0: 0000 4300 0000 730a 0000 007c 006a 0064  ..C...s....|.j.d
-000005c0: 016b 0153 0072 0c00 0000 2901 720b 0000  .k.S.r....).r...
-000005d0: 0072 1d00 0000 7218 0000 0072 1800 0000  .r....r....r....
-000005e0: 7219 0000 0072 1b00 0000 3b00 0000 7302  r....r....;...s.
-000005f0: 0000 000a 027a 1850 6172 7469 636c 652e  .....z.Particle.
-00000600: 6465 6174 685f 636f 6e64 6974 696f 6e29  death_condition)
-00000610: 0872 0100 0000 7201 0000 004e 4e4e 4e4e  .r....r....NNNNN
-00000620: 4e29 0146 290f da08 5f5f 6e61 6d65 5f5f  N).F)...__name__
-00000630: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000640: 7175 616c 6e61 6d65 5f5f da06 7079 6761  qualname__..pyga
-00000650: 6d65 da0d 424c 454e 445f 5247 425f 4144  me..BLEND_RGB_AD
-00000660: 4472 0f00 0000 da05 666c 6f61 74da 0f5f  Dr......float.._
-00000670: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 7203  _annotations__r.
-00000680: 0000 0072 0e00 0000 721e 0000 0072 2700  ...r....r....r'.
-00000690: 0000 da08 7072 6f70 6572 7479 721b 0000  ....propertyr...
-000006a0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-000006b0: 7218 0000 0072 1800 0000 7216 0000 0072  r....r....r....r
-000006c0: 1900 0000 7206 0000 0009 0000 0073 2800  ....r........s(.
-000006d0: 0000 0a00 0601 0801 0801 0801 0801 0801  ................
-000006e0: 0206 0201 0201 0201 0201 0201 0201 0201  ................
-000006f0: 0ef5 081a 0a0a 0206 1201 7206 0000 0029  ..........r....)
-00000700: 0972 2b00 0000 7202 0000 00da 0c70 7967  .r+...r......pyg
-00000710: 616d 652e 636f 6c6f 7272 0300 0000 5a18  ame.colorr....Z.
-00000720: 726f 6269 6e67 616d 652e 6f62 6a65 6374  robingame.object
-00000730: 732e 656e 7469 7479 7204 0000 00da 0f72  s.entityr......r
-00000740: 6f62 696e 6761 6d65 2e75 7469 6c73 7205  obingame.utilsr.
-00000750: 0000 0072 0600 0000 7218 0000 0072 1800  ...r....r....r..
-00000760: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
-00000770: 6f64 756c 653e 0100 0000 730c 0000 0008  odule>....s.....
-00000780: 000c 010c 010c 020c 0114 03              ...........
+00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
+00000060: 8400 6406 6504 8303 5a07 6401 5300 2907  ..d.e...Z.d.S.).
+00000070: e900 0000 004e 2901 da05 436f 6c6f 7229  .....N)...Color)
+00000080: 01da 0645 6e74 6974 7929 01da 0b63 6972  ...Entity)...cir
+00000090: 636c 655f 7375 7266 6300 0000 0000 0000  cle_surfc.......
+000000a0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+000000b0: 0073 9400 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+000000c0: 6503 6a04 5a05 6401 5a06 6507 6508 6402  e.j.Z.d.Z.e.e.d.
+000000d0: 3c00 6401 5a09 6507 6508 6403 3c00 6401  <.d.Z.e.e.d.<.d.
+000000e0: 5a0a 6507 6508 6404 3c00 6405 5a0b 6507  Z.e.e.d.<.d.Z.e.
+000000f0: 6508 6406 3c00 650c 6508 6407 3c00 650c  e.d.<.e.e.d.<.e.
+00000100: 6408 8301 5a0d 0909 0909 090a 090a 090a  d...Z...........
+00000110: 090a 090a 090a 6414 8700 6601 640b 640c  ......d...f.d.d.
+00000120: 8409 5a0e 640d 640e 8400 5a0f 6415 6410  ..Z.d.d...Z.d.d.
+00000130: 6411 8401 5a10 6511 6412 6413 8400 8301  d...Z.e.d.d.....
+00000140: 5a12 8700 0400 5a13 5300 2916 da08 5061  Z.....Z.S.)...Pa
+00000150: 7274 6963 6c65 6700 0000 0000 0000 00da  rticleg.........
+00000160: 0767 7261 7669 7479 da08 6672 6963 7469  .gravity..fricti
+00000170: 6f6e da05 6465 6361 79e9 0100 0000 da06  on..decay.......
+00000180: 7261 6469 7573 da05 636f 6c6f 72da 0372  radius..color..r
+00000190: 6564 7201 0000 004e 630b 0000 0000 0000  edr....Nc.......
+000001a0: 0000 0000 000b 0000 0002 0000 0003 0000  ................
+000001b0: 0073 9e00 0000 7400 8300 a001 a100 0100  .s....t.........
+000001c0: 7c06 6400 7500 720c 7c00 6a02 6e01 7c06  |.d.u.r.|.j.n.|.
+000001d0: 7c00 5f02 7c07 6400 7500 7216 7c00 6a03  |._.|.d.u.r.|.j.
+000001e0: 6e01 7c07 7c00 5f03 7c08 6400 7500 7220  n.|.|._.|.d.u.r 
+000001f0: 7c00 6a04 6e01 7c08 7c00 5f04 7c09 6400  |.j.n.|.|._.|.d.
+00000200: 7500 722a 7c00 6a05 6e01 7c09 7c00 5f05  u.r*|.j.n.|.|._.
+00000210: 7c0a 6400 7500 7234 7c00 6a06 6e01 7c0a  |.d.u.r4|.j.n.|.
+00000220: 7c00 5f06 7c05 6400 7500 723e 7c00 6a07  |._.|.d.u.r>|.j.
+00000230: 6e01 7c05 7c00 5f07 7c01 7c00 5f08 7c02  n.|.|._.|.|._.|.
+00000240: 7c00 5f09 7c03 7c00 5f0a 7c04 7c00 5f0b  |._.|.|._.|.|._.
+00000250: 6400 5300 2901 4e29 0cda 0573 7570 6572  d.S.).N)...super
+00000260: da08 5f5f 696e 6974 5f5f 720b 0000 0072  ..__init__r....r
+00000270: 0600 0000 7207 0000 0072 0800 0000 da09  ....r....r......
+00000280: 626c 6974 5f66 6c61 6772 0a00 0000 da01  blit_flagr......
+00000290: 78da 0179 da01 75da 0176 290b da04 7365  x..y..u..v)...se
+000002a0: 6c66 7210 0000 0072 1100 0000 7212 0000  lfr....r....r...
+000002b0: 0072 1300 0000 720a 0000 0072 0b00 0000  .r....r....r....
+000002c0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+000002d0: 0f00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+000002e0: 5fa9 00fa 392f 686f 6d65 2f72 6f62 696e  _...9/home/robin
+000002f0: 2f63 6f64 652f 726f 6269 6e67 616d 652f  /code/robingame/
+00000300: 726f 6269 6e67 616d 652f 6f62 6a65 6374  robingame/object
+00000310: 732f 7061 7274 6963 6c65 732e 7079 720e  s/particles.pyr.
+00000320: 0000 0011 0000 0073 1600 0000 0a0d 1401  .......s........
+00000330: 1401 1401 1401 1401 1401 0601 0601 0601  ................
+00000340: 0a01 7a11 5061 7274 6963 6c65 2e5f 5f69  ..z.Particle.__i
+00000350: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000360: 0000 0100 0000 0400 0000 4300 0000 737e  ..........C...s~
+00000370: 0000 007c 0004 006a 007c 006a 0137 0002  ...|...j.|.j.7..
+00000380: 005f 007c 0004 006a 027c 006a 0337 0002  ._.|...j.|.j.7..
+00000390: 005f 027c 0004 006a 037c 006a 0437 0002  ._.|...j.|.j.7..
+000003a0: 005f 037c 0004 006a 0164 017c 006a 0518  ._.|...j.d.|.j..
+000003b0: 0039 0002 005f 017c 0004 006a 0364 017c  .9..._.|...j.d.|
+000003c0: 006a 0518 0039 0002 005f 037c 0004 006a  .j...9..._.|...j
+000003d0: 067c 006a 0738 0002 005f 067c 006a 0872  .|.j.8..._.|.j.r
+000003e0: 3d7c 00a0 09a1 0001 0064 0053 0064 0053  =|.......d.S.d.S
+000003f0: 0029 024e 7209 0000 0029 0a72 1000 0000  .).Nr....).r....
+00000400: 7212 0000 0072 1100 0000 7213 0000 0072  r....r....r....r
+00000410: 0600 0000 7207 0000 0072 0a00 0000 7208  ....r....r....r.
+00000420: 0000 00da 0f64 6561 7468 5f63 6f6e 6469  .....death_condi
+00000430: 7469 6f6e da04 6b69 6c6c a901 7214 0000  tion..kill..r...
+00000440: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000450: da06 7570 6461 7465 2a00 0000 7312 0000  ..update*...s...
+00000460: 0010 0110 0110 0114 0114 0110 0106 010c  ................
+00000470: 0104 ff7a 0f50 6172 7469 636c 652e 7570  ...z.Particle.up
+00000480: 6461 7465 4663 0300 0000 0000 0000 0000  dateFc..........
+00000490: 0000 0500 0000 0600 0000 4300 0000 7380  ..........C...s.
+000004a0: 0000 0074 0074 017c 006a 0283 017c 006a  ...t.t.|.j...|.j
+000004b0: 0383 027d 037c 03a0 04a1 007d 047c 006a  ...}.|.....}.|.j
+000004c0: 057c 006a 0666 027c 045f 077c 016a 087c  .|.j.f.|._.|.j.|
+000004d0: 037c 047c 006a 0964 018d 0301 007c 0272  .|.|.j.d.....|.r
+000004e0: 3e74 0a6a 0b6a 0c7c 017c 006a 0d7c 0464  >t.j.j.|.|.j.|.d
+000004f0: 0264 038d 0401 0074 0a6a 0b6a 0c7c 017c  .d.....t.j.j.|.|
+00000500: 006a 0d67 007c 046a 07a2 0164 0491 0164  .j.g.|.j...d...d
+00000510: 0491 0152 0064 058d 0301 0064 0053 0064  ...R.d.....d.S.d
+00000520: 0053 0029 064e 2901 da0d 7370 6563 6961  .S.).N)...specia
+00000530: 6c5f 666c 6167 7372 0900 0000 2903 720b  l_flagsr....).r.
+00000540: 0000 00da 0472 6563 74da 0577 6964 7468  .....rect..width
+00000550: e902 0000 0029 0272 0b00 0000 721e 0000  .....).r....r...
+00000560: 0029 0e72 0400 0000 da05 726f 756e 6472  .).r......roundr
+00000570: 0a00 0000 720b 0000 00da 0867 6574 5f72  ....r......get_r
+00000580: 6563 7472 1000 0000 7211 0000 00da 0663  ectr....r......c
+00000590: 656e 7465 72da 0462 6c69 7472 0f00 0000  enter..blitr....
+000005a0: da06 7079 6761 6d65 da04 6472 6177 721e  ..pygame..drawr.
+000005b0: 0000 00da 0b64 6562 7567 5f63 6f6c 6f72  .....debug_color
+000005c0: 2905 7214 0000 00da 0773 7572 6661 6365  ).r......surface
+000005d0: da05 6465 6275 67da 0473 7572 66da 0a69  ..debug..surf..i
+000005e0: 6d61 6765 5f72 6563 7472 1700 0000 7217  mage_rectr....r.
+000005f0: 0000 0072 1800 0000 7226 0000 0034 0000  ...r....r&...4..
+00000600: 0073 2200 0000 1201 0801 0e01 1201 0401  .s".............
+00000610: 0602 0201 0401 0201 0201 06fc 0607 0201  ................
+00000620: 0401 1201 0afd 04f7 7a0d 5061 7274 6963  ........z.Partic
+00000630: 6c65 2e64 7261 7763 0100 0000 0000 0000  le.drawc........
+00000640: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000650: 730a 0000 007c 006a 0064 016b 0153 0029  s....|.j.d.k.S.)
+00000660: 024e 7201 0000 0029 0172 0a00 0000 721b  .Nr....).r....r.
+00000670: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000680: 0000 7219 0000 0048 0000 0073 0200 0000  ..r....H...s....
+00000690: 0a02 7a18 5061 7274 6963 6c65 2e64 6561  ..z.Particle.dea
+000006a0: 7468 5f63 6f6e 6469 7469 6f6e 2908 7201  th_condition).r.
+000006b0: 0000 0072 0100 0000 4e4e 4e4e 4e4e 2901  ...r....NNNNNN).
+000006c0: 4629 14da 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
+000006d0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000006e0: 6c6e 616d 655f 5f72 2500 0000 da0d 424c  lname__r%.....BL
+000006f0: 454e 445f 5247 425f 4144 4472 0f00 0000  END_RGB_ADDr....
+00000700: 7206 0000 00da 0566 6c6f 6174 da0f 5f5f  r......float..__
+00000710: 616e 6e6f 7461 7469 6f6e 735f 5f72 0700  annotations__r..
+00000720: 0000 7208 0000 0072 0a00 0000 7202 0000  ..r....r....r...
+00000730: 0072 2700 0000 720e 0000 0072 1c00 0000  .r'...r....r....
+00000740: 7226 0000 00da 0870 726f 7065 7274 7972  r&.....propertyr
+00000750: 1900 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00000760: 6c5f 5f72 1700 0000 7217 0000 0072 1500  l__r....r....r..
+00000770: 0000 7218 0000 0072 0500 0000 0800 0000  ..r....r........
+00000780: 732a 0000 000a 0006 010c 010c 010c 010c  s*..............
+00000790: 0108 0108 0102 0602 0102 0102 0102 0102  ................
+000007a0: 0102 0102 010e f508 190a 0a02 1412 0172  ...............r
+000007b0: 0500 0000 2908 7225 0000 00da 0c70 7967  ....).r%.....pyg
+000007c0: 616d 652e 636f 6c6f 7272 0200 0000 da18  ame.colorr......
+000007d0: 726f 6269 6e67 616d 652e 6f62 6a65 6374  robingame.object
+000007e0: 732e 656e 7469 7479 7203 0000 00da 0f72  s.entityr......r
+000007f0: 6f62 696e 6761 6d65 2e75 7469 6c73 7204  obingame.utilsr.
+00000800: 0000 0072 0500 0000 7217 0000 0072 1700  ...r....r....r..
+00000810: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
+00000820: 6f64 756c 653e 0100 0000 730a 0000 0008  odule>....s.....
+00000830: 000c 010c 020c 0114 03                   .........
```

### Comparing `robingame-0.0.9/robingame/objects/game.py` & `robingame-0.1.0/robingame/objects/game.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,57 +6,53 @@
 
 from robingame.input import EventQueue
 from robingame.objects.entity import Entity, Group
 from robingame.objects.helpers import FpsTracker
 
 
 class Game(Entity):
-    """Special case of Entity; it is at the very top of the object tree."""
+    """
+    Special case of Entity; it is at the very top of the object tree.
+    Handles setting up and running the main game loop.
+    """
 
     fps: int = 60
     window_width: int = 500
     window_height: int = 500
-    window_caption: str = ""
-    font_name: str = "ubuntucondensed"
-    font_size: int = 30
-    parental_name = "game"
+    window_caption: str = "Game"
     screen_color = Color("black")
-    debug = False
+    debug: bool = False  # draw / print debug info?
+    running: bool  # is the main game loop running
 
     def __init__(self):
         super().__init__()
         pygame.init()
-
-        self.scenes = Group()
         self.fps_tracker = FpsTracker()
-        self.child_groups = [self.scenes]
-
-        pygame.font.init()
-        self.font = pygame.font.Font(pygame.font.match_font(self.font_name), self.font_size)
         self.window = pygame.display.set_mode((self.window_width, self.window_height))
         pygame.display.set_caption(self.window_caption)
         self.clock = pygame.time.Clock()
 
     def main(self):
-        """This is the outermost game function which runs once. It contains the outermost game
-        loop. Here's where you should put your main event state machine."""
+        """
+        This is the outermost game function which runs once. It contains the outermost game loop.
+        Here's where you should put your main event state machine.
+        """
         self.running = True
         while self.running:
             self._update()
             self._draw(self.window, debug=self.debug)
         pygame.quit()
         sys.exit()
 
-    def add_scene(self, *objects):
-        self.add_to_group(*objects, group=self.scenes)
-
     def read_inputs(self):
-        """I've put this in a separate method because I don't like the idea of putting the inputs
-        in the same list as other child groups. The order might get ruined, or a subclass might
-        overwrite the list. It's crucial that the inputs are read before updating."""
+        """
+        I've put this in a separate method because I don't like the idea of putting the inputs in
+        the same list as other child groups. The order might get ruined, or a subclass might
+        overwrite the list. It's crucial that the inputs are read before updating.
+        """
         EventQueue.update()
         for event in EventQueue.events:
             if event.type == pygame.QUIT:
                 pygame.quit()
                 sys.exit()
             if event.type == pygame.KEYDOWN and event.key == pygame.K_F1:
                 self.debug = not self.debug
```

### Comparing `robingame-0.0.9/robingame/objects/helpers.py` & `robingame-0.1.0/robingame/objects/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import time
 from collections import deque
 
-import pygame
 from pygame.color import Color
 from pygame.surface import Surface
 
 from robingame.objects.entity import Entity
 from robingame.text.font import fonts
 
 
 class FpsTracker(Entity):
     """Displays a little number in the top right of the window if debug=True"""
 
     buffer_length = 60
     font = fonts.cellphone_black
+    fps: int
 
     def __init__(self, *groups) -> None:
         super().__init__(*groups)
         self.queue = deque(maxlen=self.buffer_length)
 
     def update(self):
         t = time.perf_counter()
```

### Comparing `robingame-0.0.9/robingame/objects/particles.py` & `robingame-0.1.0/robingame/objects/particles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pygame
-from pygame import Rect
 from pygame.color import Color
 
-from robingame.objects.entity import PhysicalEntity
+from robingame.objects.entity import Entity
 from robingame.utils import circle_surf
 
 
-class Particle(PhysicalEntity):
+class Particle(Entity):
     blit_flag = pygame.BLEND_RGB_ADD
-    gravity: float
-    friction: float
-    decay: float
+    gravity: float = 0.0
+    friction: float = 0.0
+    decay: float = 0.0
+    radius: float = 1
     color: Color
-    radius: float
+    debug_color = Color("red")
 
     def __init__(
         self,
         x,
         y,
         u=0,
         v=0,
@@ -30,15 +30,14 @@
         super().__init__()
         self.color = self.color if color is None else color
         self.gravity = self.gravity if gravity is None else gravity
         self.friction = self.friction if friction is None else friction
         self.decay = self.decay if decay is None else decay
         self.blit_flag = self.blit_flag if blit_flag is None else blit_flag
         self.radius = self.radius if radius is None else radius
-        self.rect = Rect(0, 0, 0, 0)
         self.x = x
         self.y = y
         self.u = u
         self.v = v
 
     def update(self):
         self.x += self.u
@@ -49,13 +48,27 @@
         self.radius -= self.decay
         if self.death_condition:
             self.kill()
 
     def draw(self, surface, debug=False):
         surf = circle_surf(round(self.radius), self.color)
         image_rect = surf.get_rect()
-        image_rect.center = self.rect.center
+        image_rect.center = self.x, self.y
         surface.blit(surf, image_rect, special_flags=self.blit_flag)
+        if debug:
+            # bounding box
+            pygame.draw.rect(
+                surface,
+                color=self.debug_color,
+                rect=image_rect,
+                width=1,
+            )
+            # center
+            pygame.draw.rect(
+                surface,
+                color=self.debug_color,
+                rect=(*image_rect.center, 2, 2),
+            )
 
     @property
     def death_condition(self):
         return self.radius <= 0
```

### Comparing `robingame-0.0.9/robingame/recording.py` & `robingame-0.1.0/robingame/recording.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 
 
 def save_image_async(filename, img_string: bytes, size: tuple[int, int], output_dir: Path):
     image = pygame.image.fromstring(img_string, size, "RGBA")
     pygame.image.save(image, str(output_dir / f"{filename}.png"))
 
 
-def save_images_async(images: list[Surface], output_dir: Path):
+def save_images_async(images: list[Surface], output_dir: Path, processes: int):
     stringified = (
         (
             pygame.image.tostring(image, "RGBA"),
             image.get_size(),
         )
         for image in images
     )
-    with multiprocessing.Pool(processes=8) as pool:
+    with multiprocessing.Pool(processes=processes) as pool:
         result = pool.starmap(
             func=save_image_async,
             iterable=(
                 (ii, string, size, output_dir) for ii, (string, size) in enumerate(stringified)
             ),
         )
     return result
@@ -103,27 +103,27 @@
         screenshot = Surface(surface.get_size()).convert_alpha()
         func(self, screenshot, debug)
         screenshots.append(screenshot)
 
     return wrapped
 
 
-def decorate_main(func, screenshots: deque, output_dir: Path, filename: str):
+def decorate_main(func, screenshots: deque, output_dir: Path, filename: str, processes: int):
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         """Run the game as normal, but intercept the quit signal and save all the screenshots to
         file."""
         try:
             func(*args, **kwargs)
         except SystemExit:
             print("Deleting old images/videos...")
             clean_empty_recordings_dir(output_dir)
             print(f"Saving {len(screenshots)} images...")
             t1 = time.perf_counter()
-            save_images_async(screenshots, output_dir)
+            save_images_async(screenshots, output_dir, processes=processes)
             t2 = time.perf_counter()
             print(f"Images saved in {t2-t1}s")
             print("Creating videos...")
             create_videos(output_dir, filename)
         pygame.quit()
         sys.exit()
 
@@ -132,14 +132,15 @@
 
 def record(
     cls: Game = None,
     *,
     n_frames: int,
     output_dir: Path,
     filename="out",
+    processes=4,
 ):
     """
     Patch the Game's ._draw() and .main() methods so that we keep a screenshot of every frame,
     which we later stitch into videos.
     """
     output_dir = output_dir or Path(__file__).parent / "recordings"
     screenshots = deque(maxlen=n_frames)
@@ -147,11 +148,12 @@
     def decorate(cls):
         cls._draw = decorate_draw(cls._draw, screenshots=screenshots)
         cls.main = decorate_main(
             cls.main,
             screenshots=screenshots,
             output_dir=output_dir,
             filename=filename,
+            processes=processes,
         )
         return cls
 
     return decorate(cls) if cls else decorate
```

### Comparing `robingame-0.0.9/robingame/sound.py` & `robingame-0.1.0/robingame/sound.py`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/assets/cellphone-black.png` & `robingame-0.1.0/robingame/text/assets/cellphone-black.png`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/assets/cellphone-white.png` & `robingame-0.1.0/robingame/text/assets/cellphone-white.png`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/assets/test_font.aseprite` & `robingame-0.1.0/robingame/text/assets/test_font.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/assets/test_font.png` & `robingame-0.1.0/robingame/text/assets/test_font.png`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/font/__pycache__/classes.cpython-310.pyc` & `robingame-0.1.0/robingame/text/font/__pycache__/classes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:02:45 2022 UTC, .py size: 4112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7597 3563 1010 0000  o.......u.5c....
+00000000: 6f0d 0d0a 0000 0000 88a3 6064 1010 0000  o.........`d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 8302 5a0c  ..G.d.d...d...Z.
@@ -53,201 +53,201 @@
 00000340: 6565 742c 2069 6e20 7468 6520 7361 6d65  eet, in the same
 00000350: 206f 7264 6572 2efa 0120 da03 7265 6472   order... ..redr
 00000360: 0b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
 00000370: 0003 0000 0004 0000 0053 0000 0073 1600  .........S...s..
 00000380: 0000 6900 7c00 5d07 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
 00000390: 7c02 9302 7102 5300 a900 7211 0000 0029  |...q.S...r....)
 000003a0: 03da 022e 30da 066c 6574 7465 72da 0569  ....0..letter..i
-000003b0: 6d61 6765 7211 0000 0072 1100 0000 fa3a  mager....r.....:
-000003c0: 2f68 6f6d 652f 6269 6e6e 6576 2f63 6f64  /home/binnev/cod
-000003d0: 652f 726f 6269 6e67 616d 652f 726f 6269  e/robingame/robi
-000003e0: 6e67 616d 652f 7465 7874 2f66 6f6e 742f  ngame/text/font/
-000003f0: 636c 6173 7365 732e 7079 da0a 3c64 6963  classes.py..<dic
-00000400: 7463 6f6d 703e 2600 0000 7302 0000 0016  tcomp>&...s.....
-00000410: 007a 2146 6f6e 742e 5f5f 696e 6974 5f5f  .z!Font.__init__
-00000420: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000430: 6f6d 703e 4e29 0e72 0b00 0000 720c 0000  omp>N).r....r...
-00000440: 0072 0d00 0000 da04 6469 6374 720a 0000  .r......dictr...
-00000450: 0072 0700 0000 7204 0000 00da 096e 6f74  .r....r......not
-00000460: 5f66 6f75 6e64 da04 6669 6c6c 7203 0000  _found..fillr...
-00000470: 0072 0500 0000 da0b 7472 696d 5f69 6d61  .r......trim_ima
-00000480: 6765 73da 0675 7064 6174 65da 037a 6970  ges..update..zip
-00000490: 290c da04 7365 6c66 720e 0000 0072 0b00  )...selfr....r..
-000004a0: 0000 720a 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-000004b0: 00da 0474 7269 6d5a 0b73 7061 6365 5f77  ...trimZ.space_w
-000004c0: 6964 7468 da06 6b77 6172 6773 da05 7769  idth..kwargs..wi
-000004d0: 6474 68da 0668 6569 6768 74da 0669 6d61  dth..height..ima
-000004e0: 6765 7372 1100 0000 7211 0000 0072 1500  gesr....r....r..
-000004f0: 0000 da08 5f5f 696e 6974 5f5f 1000 0000  ....__init__....
-00000500: 7316 0000 000e 0c06 0106 0108 0116 010a  s...............
-00000510: 0110 0114 0104 010a 0120 017a 0d46 6f6e  ......... .z.Fon
-00000520: 742e 5f5f 696e 6974 5f5f e901 0000 00da  t.__init__......
-00000530: 0473 7572 66da 0474 6578 74da 0178 da01  .surf..text..x..
-00000540: 79da 0573 6361 6c65 da04 7772 6170 da05  y..scale..wrap..
-00000550: 616c 6967 6eda 0672 6574 7572 6e63 0800  align..returnc..
-00000560: 0000 0000 0000 0000 0000 1000 0000 0900  ................
-00000570: 0000 4300 0000 73b0 0000 007c 006a 005c  ..C...s....|.j.\
-00000580: 027d 087d 097c 037d 0a7c 02a0 01a1 0044  .}.}.|.}.|.....D
-00000590: 005d 4a7d 0b7c 0672 177c 00a0 027c 0b7c  .]J}.|.r.|...|.|
-000005a0: 067c 037c 05a1 046e 027c 0b67 017d 0c7c  .|.|...n.|.g.}.|
-000005b0: 0c44 005d 387d 0b7c 00a0 037c 0b7c 037c  .D.]8}.|...|.|.|
-000005c0: 077c 057c 06a1 057d 0a7c 0b44 005d 217d  .|.|...}.|.D.]!}
-000005d0: 0d7c 00a0 047c 0da1 017d 0e74 057c 0e7c  .|...|...}.t.|.|
-000005e0: 0583 027d 0e7c 01a0 067c 0e7c 0a7c 0466  ...}.|...|.|.|.f
-000005f0: 02a1 0201 007c 0ea0 07a1 007d 0f7c 0a7c  .....|.....}.|.|
-00000600: 0f7c 006a 087c 0514 0017 0037 007d 0a71  .|.j.|.....7.}.q
-00000610: 297c 047c 097c 006a 0917 007c 0514 0037  )|.|.|.j...|...7
-00000620: 007d 0471 1c71 0b7c 0a53 0029 017a 5f0a  .}.q.q.|.S.).z_.
-00000630: 2020 2020 2020 2020 616c 6967 6e3a 202d          align: -
-00000640: 313d 6c65 6674 2c20 303d 6365 6e74 6572  1=left, 0=center
-00000650: 2c20 313d 7269 6768 740a 2020 2020 2020  , 1=right.      
-00000660: 2020 7772 6170 3a20 7820 7769 6474 6820    wrap: x width 
-00000670: 6174 2077 6869 6368 2074 6f20 7772 6170  at which to wrap
-00000680: 2074 6578 740a 2020 2020 2020 2020 290a   text.        ).
-00000690: 720b 0000 00da 0a73 706c 6974 6c69 6e65  r......splitline
-000006a0: 73da 0a77 7261 705f 776f 7264 73da 0c61  s..wrap_words..a
-000006b0: 6c69 676e 5f63 7572 736f 72da 0367 6574  lign_cursor..get
-000006c0: 7206 0000 00da 0462 6c69 74da 0967 6574  r......blit..get
-000006d0: 5f77 6964 7468 720c 0000 0072 0d00 0000  _widthr....r....
-000006e0: 2910 721d 0000 0072 2500 0000 7226 0000  ).r....r%...r&..
-000006f0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
-00000700: 722a 0000 0072 2b00 0000 da01 5fda 0579  r*...r+....._..y
-00000710: 7369 7a65 da06 6375 7273 6f72 da04 6c69  size..cursor..li
-00000720: 6e65 5a0d 7772 6170 7065 645f 6c69 6e65  neZ.wrapped_line
-00000730: 7372 1300 0000 7214 0000 00da 0177 7211  sr....r......wr.
-00000740: 0000 0072 1100 0000 7215 0000 00da 0672  ...r....r......r
-00000750: 656e 6465 7228 0000 0073 1e00 0000 0a0e  ender(...s......
-00000760: 0401 0c01 1a01 0801 1201 0801 0a01 0a01  ................
-00000770: 1001 0801 1401 1401 02f8 0409 7a0b 466f  ............z.Fo
-00000780: 6e74 2e72 656e 6465 7272 3600 0000 6306  nt.renderr6...c.
-00000790: 0000 0000 0000 0000 0000 0009 0000 0004  ................
-000007a0: 0000 0043 0000 0073 9400 0000 7c03 0400  ...C...s....|...
-000007b0: 0400 6401 6b02 7207 6e07 0400 6402 7500  ..d.k.r.n...d.u.
-000007c0: 720c 6e02 0100 6e06 0100 0100 7c02 7d06  r.n...n.....|.}.
-000007d0: 7c06 5300 0400 6403 6b02 7231 0100 7c05  |.S...d.k.r1..|.
-000007e0: 731f 7400 6404 8301 8201 7c00 a001 7c01  s.t.d.....|...|.
-000007f0: 7c04 a102 7d07 7c05 7c07 1800 7d08 7c02  |...}.|.|...}.|.
-00000800: 7c08 6405 1a00 1700 7d06 7c06 5300 6406  |.d.....}.|.S.d.
-00000810: 6b02 7242 7c00 a001 7c01 7c04 a102 7d07  k.rB|...|.|...}.
-00000820: 7c02 7c05 1700 7c07 1800 7d06 7c06 5300  |.|...|...}.|.S.
-00000830: 0900 7400 6407 7c03 9b00 9d02 8301 8201  ..t.d.|.........
-00000840: 2908 7a2c 5573 6564 2066 6f72 206c 6566  ).z,Used for lef
-00000850: 742f 7269 6768 742f 6365 6e74 6572 6564  t/right/centered
-00000860: 2074 6578 7420 616c 6967 6e6d 6e65 6e74   text alignmnent
-00000870: e9ff ffff ff4e 7201 0000 007a 3243 616e  .....Nr....z2Can
-00000880: 2774 2063 656e 7465 7220 7465 7874 2077  't center text w
-00000890: 6974 686f 7574 2073 7065 6369 6679 696e  ithout specifyin
-000008a0: 6720 6120 7772 6170 2077 6964 7468 2ee9  g a wrap width..
-000008b0: 0200 0000 7224 0000 007a 1542 6164 2061  ....r$...z.Bad a
-000008c0: 6c69 676e 6d65 6e74 2076 616c 7565 3a20  lignment value: 
-000008d0: 2902 7208 0000 00da 0d70 7269 6e74 6564  ).r......printed
-000008e0: 5f77 6964 7468 2909 721d 0000 0072 3600  _width).r....r6.
-000008f0: 0000 7227 0000 0072 2b00 0000 7229 0000  ..r'...r+...r)..
-00000900: 0072 2a00 0000 7235 0000 00da 0a6c 696e  .r*...r5.....lin
-00000910: 655f 7769 6474 685a 0573 6c61 636b 7211  e_widthZ.slackr.
-00000920: 0000 0072 1100 0000 7215 0000 0072 2f00  ...r....r....r/.
-00000930: 0000 4500 0000 7322 0000 0002 021e 0104  ..E...s"........
-00000940: 0104 0c0a f504 0108 010c 0108 010c 0104  ................
-00000950: 0606 fb0c 010c 0104 0302 fe0e 017a 1146  .............z.F
-00000960: 6f6e 742e 616c 6967 6e5f 6375 7273 6f72  ont.align_cursor
-00000970: 6305 0000 0000 0000 0000 0000 0009 0000  c...............
-00000980: 0005 0000 0043 0000 0073 6000 0000 6700  .....C...s`...g.
-00000990: 7d05 6401 7d06 7c01 a000 6402 a101 4400  }.d.}.|...d...D.
-000009a0: 5d1f 7d07 7c06 7214 7c06 9b00 6402 7c07  ].}.|.r.|...d.|.
-000009b0: 9b00 9d03 6e01 7c07 7d08 7c00 a001 7c08  ....n.|.}.|...|.
-000009c0: 7c04 a102 7c02 6b01 7221 7c08 7d06 7109  |...|.k.r!|.}.q.
-000009d0: 7c05 a002 7c06 a101 0100 7c07 7d06 7109  |...|.....|.}.q.
-000009e0: 7c05 a002 7c06 a101 0100 7c05 5300 2903  |...|.....|.S.).
-000009f0: 7a40 4272 6561 6b20 6f6e 6520 6c6f 6e67  z@Break one long
-00000a00: 206c 696e 6520 696e 746f 206d 756c 7469   line into multi
-00000a10: 706c 6520 6c69 6e65 7320 6261 7365 6420  ple lines based 
-00000a20: 6f6e 2074 6865 2077 7261 7020 7769 6474  on the wrap widt
-00000a30: 682e da00 720f 0000 0029 03da 0573 706c  h...r....)...spl
-00000a40: 6974 723b 0000 00da 0661 7070 656e 6429  itr;.....append)
-00000a50: 0972 1d00 0000 7226 0000 0072 2a00 0000  .r....r&...r*...
-00000a60: 7227 0000 0072 2900 0000 da05 6c69 6e65  r'...r).....line
-00000a70: 7372 3600 0000 da04 776f 7264 5a08 6e65  sr6.....wordZ.ne
-00000a80: 775f 6c69 6e65 7211 0000 0072 1100 0000  w_liner....r....
-00000a90: 7215 0000 0072 2e00 0000 5700 0000 7314  r....r....W...s.
-00000aa0: 0000 0004 0204 010e 0116 0110 0106 010a  ................
-00000ab0: 0206 010a 0104 017a 0f46 6f6e 742e 7772  .......z.Font.wr
-00000ac0: 6170 5f77 6f72 6473 6303 0000 0000 0000  ap_wordsc.......
-00000ad0: 0000 0000 0003 0000 0004 0000 0003 0000  ................
-00000ae0: 0073 1800 0000 7400 8700 8701 6602 6401  .s....t.....f.d.
-00000af0: 6402 8408 7c01 4400 8301 8301 5300 2903  d...|.D.....S.).
-00000b00: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00000b10: 0000 0400 0000 3300 0000 7328 0000 0081  ......3...s(....
-00000b20: 007c 005d 0f7d 0188 01a0 007c 01a1 01a0  .|.].}.....|....
-00000b30: 01a1 0088 016a 0217 0088 0014 0056 0001  .....j.......V..
-00000b40: 0071 0264 0053 00a9 014e 2903 7230 0000  .q.d.S...N).r0..
-00000b50: 0072 3200 0000 720c 0000 0029 0272 1200  .r2...r....).r..
-00000b60: 0000 7213 0000 00a9 0272 2900 0000 721d  ..r......r)...r.
-00000b70: 0000 0072 1100 0000 7215 0000 00da 093c  ...r....r......<
-00000b80: 6765 6e65 7870 723e 6600 0000 7304 0000  genexpr>f...s...
-00000b90: 0002 8026 007a 2546 6f6e 742e 7072 696e  ...&.z%Font.prin
-00000ba0: 7465 645f 7769 6474 682e 3c6c 6f63 616c  ted_width.<local
-00000bb0: 733e 2e3c 6765 6e65 7870 723e 2901 da03  s>.<genexpr>)...
-00000bc0: 7375 6d29 0372 1d00 0000 7226 0000 0072  sum).r....r&...r
-00000bd0: 2900 0000 7211 0000 0072 4300 0000 7215  )...r....rC...r.
-00000be0: 0000 0072 3b00 0000 6500 0000 7302 0000  ...r;...e...s...
-00000bf0: 0018 017a 1246 6f6e 742e 7072 696e 7465  ...z.Font.printe
-00000c00: 645f 7769 6474 6872 2200 0000 6302 0000  d_widthr"...c...
-00000c10: 0000 0000 0000 0000 000a 0000 0007 0000  ................
-00000c20: 0043 0000 0073 4e00 0000 6700 7d02 7c01  .C...sN...g.}.|.
-00000c30: 4400 5d20 7d03 7c03 a000 a100 5c04 7d04  D.] }.|.....\.}.
-00000c40: 7d05 7d06 7d05 7c03 a001 a100 5c04 7d05  }.}.}.|.....\.}.
-00000c50: 7d07 7d05 7d08 7c03 a002 7c04 7c07 7c06  }.}.}.|...|.|.|.
-00000c60: 7c08 6604 a101 7d09 7c02 a003 7c09 a101  |.f...}.|...|...
-00000c70: 0100 7104 7c02 5300 2901 7a25 4d61 6b65  ..q.|.S.).z%Make
-00000c80: 2061 206d 6f6e 6f73 7061 6365 6420 666f   a monospaced fo
-00000c90: 6e74 206e 6f6e 2d6d 6f6e 6f73 7061 6365  nt non-monospace
-00000ca0: 6429 04da 1167 6574 5f62 6f75 6e64 696e  d)...get_boundin
-00000cb0: 675f 7265 6374 da08 6765 745f 7265 6374  g_rect..get_rect
-00000cc0: da0a 7375 6273 7572 6661 6365 723f 0000  ..subsurfacer?..
-00000cd0: 0029 0a72 1d00 0000 7222 0000 005a 0774  .).r....r"...Z.t
-00000ce0: 7269 6d6d 6564 7214 0000 0072 2700 0000  rimmedr....r'...
-00000cf0: 7233 0000 0072 3700 0000 7228 0000 00da  r3...r7...r(....
-00000d00: 0168 da03 6e65 7772 1100 0000 7211 0000  .h..newr....r...
-00000d10: 0072 1500 0000 721a 0000 0068 0000 0073  .r....r....h...s
-00000d20: 0e00 0000 0402 0801 1001 1001 1201 0c01  ................
-00000d30: 0401 7a10 466f 6e74 2e74 7269 6d5f 696d  ..z.Font.trim_im
-00000d40: 6167 6573 7213 0000 0063 0200 0000 0000  agesr....c......
-00000d50: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00000d60: 0000 7326 0000 007a 067c 006a 007c 0119  ..s&...z.|.j.|..
-00000d70: 0057 0053 0004 0074 0179 1201 0001 0001  .W.S...t.y......
-00000d80: 007c 006a 0206 0059 0053 0077 0072 4200  .|.j...Y.S.w.rB.
-00000d90: 0000 2903 720a 0000 00da 084b 6579 4572  ..).r......KeyEr
-00000da0: 726f 7272 1800 0000 2902 721d 0000 0072  rorr....).r....r
-00000db0: 1300 0000 7211 0000 0072 1100 0000 7215  ....r....r....r.
-00000dc0: 0000 0072 3000 0000 7200 0000 730a 0000  ...r0...r...s...
-00000dd0: 0002 010c 010c 010a 0102 ff7a 0846 6f6e  ...........z.Fon
-00000de0: 742e 6765 7429 0472 0100 0000 7201 0000  t.get).r....r...
-00000df0: 0046 4e29 0572 0100 0000 7201 0000 0072  .FN).r....r....r
-00000e00: 2400 0000 7201 0000 004e 2902 7201 0000  $...r....N).r...
-00000e10: 0072 2400 0000 2912 da08 5f5f 6e61 6d65  .r$...)...__name
-00000e20: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000e30: 5f5f 7175 616c 6e61 6d65 5f5f 7217 0000  __qualname__r...
-00000e40: 00da 0373 7472 7204 0000 00da 0f5f 5f61  ...strr......__a
-00000e50: 6e6e 6f74 6174 696f 6e73 5f5f da05 7475  nnotations__..tu
-00000e60: 706c 65da 0369 6e74 7202 0000 0072 2300  ple..intr....r#.
-00000e70: 0000 7238 0000 0072 2f00 0000 da04 6c69  ..r8...r/.....li
-00000e80: 7374 722e 0000 0072 3b00 0000 721a 0000  str....r;...r...
-00000e90: 0072 3000 0000 7211 0000 0072 1100 0000  .r0...r....r....
-00000ea0: 7211 0000 0072 1500 0000 7209 0000 000a  r....r....r.....
-00000eb0: 0000 0073 5600 0000 0a00 1001 1001 0801  ...sV...........
-00000ec0: 0801 0207 0201 0201 0201 04f8 0602 02fe  ................
-00000ed0: 0a03 02fd 0204 0afc 021c 0201 0201 0201  ................
-00000ee0: 0201 04f8 0202 02fe 0203 02fd 0204 02fc  ................
-00000ef0: 0205 02fb 0206 02fa 0207 02f9 0208 02f8  ................
-00000f00: 0209 0af7 221d 2412 160e 1a03 160a 7209  ....".$.......r.
-00000f10: 0000 004e 290d da07 7061 7468 6c69 6272  ...N)...pathlibr
-00000f20: 0200 0000 da0c 7079 6761 6d65 2e63 6f6c  ......pygame.col
-00000f30: 6f72 7203 0000 00da 0e70 7967 616d 652e  orr......pygame.
-00000f40: 7375 7266 6163 6572 0400 0000 da0f 726f  surfacer......ro
-00000f50: 6269 6e67 616d 652e 696d 6167 6572 0500  bingame.imager..
-00000f60: 0000 7206 0000 0072 0700 0000 5a19 726f  ..r....r....Z.ro
-00000f70: 6269 6e67 616d 652e 7465 7874 2e65 7863  bingame.text.exc
-00000f80: 6570 7469 6f6e 7372 0800 0000 7209 0000  eptionsr....r...
-00000f90: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
-00000fa0: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000fb0: 0000 0073 0c00 0000 0c00 0c02 0c01 1402  ...s............
-00000fc0: 0c01 1203                                ....
+000003b0: 6d61 6765 7211 0000 0072 1100 0000 fa39  mager....r.....9
+000003c0: 2f68 6f6d 652f 726f 6269 6e2f 636f 6465  /home/robin/code
+000003d0: 2f72 6f62 696e 6761 6d65 2f72 6f62 696e  /robingame/robin
+000003e0: 6761 6d65 2f74 6578 742f 666f 6e74 2f63  game/text/font/c
+000003f0: 6c61 7373 6573 2e70 79da 0a3c 6469 6374  lasses.py..<dict
+00000400: 636f 6d70 3e26 0000 0073 0200 0000 1600  comp>&...s......
+00000410: 7a21 466f 6e74 2e5f 5f69 6e69 745f 5f2e  z!Font.__init__.
+00000420: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00000430: 6d70 3e4e 290e 720b 0000 0072 0c00 0000  mp>N).r....r....
+00000440: 720d 0000 00da 0464 6963 7472 0a00 0000  r......dictr....
+00000450: 7207 0000 0072 0400 0000 da09 6e6f 745f  r....r......not_
+00000460: 666f 756e 64da 0466 696c 6c72 0300 0000  found..fillr....
+00000470: 7205 0000 00da 0b74 7269 6d5f 696d 6167  r......trim_imag
+00000480: 6573 da06 7570 6461 7465 da03 7a69 7029  es..update..zip)
+00000490: 0cda 0473 656c 6672 0e00 0000 720b 0000  ...selfr....r...
+000004a0: 0072 0a00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000004b0: da04 7472 696d da0b 7370 6163 655f 7769  ..trim..space_wi
+000004c0: 6474 68da 066b 7761 7267 73da 0577 6964  dth..kwargs..wid
+000004d0: 7468 da06 6865 6967 6874 da06 696d 6167  th..height..imag
+000004e0: 6573 7211 0000 0072 1100 0000 7215 0000  esr....r....r...
+000004f0: 00da 085f 5f69 6e69 745f 5f10 0000 0073  ...__init__....s
+00000500: 1600 0000 0e0c 0601 0601 0801 1601 0a01  ................
+00000510: 1001 1401 0401 0a01 2001 7a0d 466f 6e74  ........ .z.Font
+00000520: 2e5f 5f69 6e69 745f 5fe9 0100 0000 da04  .__init__.......
+00000530: 7375 7266 da04 7465 7874 da01 78da 0179  surf..text..x..y
+00000540: da05 7363 616c 65da 0477 7261 70da 0561  ..scale..wrap..a
+00000550: 6c69 676e da06 7265 7475 726e 6308 0000  lign..returnc...
+00000560: 0000 0000 0000 0000 0010 0000 0009 0000  ................
+00000570: 0043 0000 0073 b000 0000 7c00 6a00 5c02  .C...s....|.j.\.
+00000580: 7d08 7d09 7c03 7d0a 7c02 a001 a100 4400  }.}.|.}.|.....D.
+00000590: 5d4a 7d0b 7c06 7217 7c00 a002 7c0b 7c06  ]J}.|.r.|...|.|.
+000005a0: 7c03 7c05 a104 6e02 7c0b 6701 7d0c 7c0c  |.|...n.|.g.}.|.
+000005b0: 4400 5d38 7d0b 7c00 a003 7c0b 7c03 7c07  D.]8}.|...|.|.|.
+000005c0: 7c05 7c06 a105 7d0a 7c0b 4400 5d21 7d0d  |.|...}.|.D.]!}.
+000005d0: 7c00 a004 7c0d a101 7d0e 7405 7c0e 7c05  |...|...}.t.|.|.
+000005e0: 8302 7d0e 7c01 a006 7c0e 7c0a 7c04 6602  ..}.|...|.|.|.f.
+000005f0: a102 0100 7c0e a007 a100 7d0f 7c0a 7c0f  ....|.....}.|.|.
+00000600: 7c00 6a08 7c05 1400 1700 3700 7d0a 7129  |.j.|.....7.}.q)
+00000610: 7c04 7c09 7c00 6a09 1700 7c05 1400 3700  |.|.|.j...|...7.
+00000620: 7d04 711c 710b 7c0a 5300 2901 7a5f 0a20  }.q.q.|.S.).z_. 
+00000630: 2020 2020 2020 2061 6c69 676e 3a20 2d31         align: -1
+00000640: 3d6c 6566 742c 2030 3d63 656e 7465 722c  =left, 0=center,
+00000650: 2031 3d72 6967 6874 0a20 2020 2020 2020   1=right.       
+00000660: 2077 7261 703a 2078 2077 6964 7468 2061   wrap: x width a
+00000670: 7420 7768 6963 6820 746f 2077 7261 7020  t which to wrap 
+00000680: 7465 7874 0a20 2020 2020 2020 2029 0a72  text.        ).r
+00000690: 0b00 0000 da0a 7370 6c69 746c 696e 6573  ......splitlines
+000006a0: da0a 7772 6170 5f77 6f72 6473 da0c 616c  ..wrap_words..al
+000006b0: 6967 6e5f 6375 7273 6f72 da03 6765 7472  ign_cursor..getr
+000006c0: 0600 0000 da04 626c 6974 da09 6765 745f  ......blit..get_
+000006d0: 7769 6474 6872 0c00 0000 720d 0000 0029  widthr....r....)
+000006e0: 1072 1d00 0000 7226 0000 0072 2700 0000  .r....r&...r'...
+000006f0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+00000700: 2b00 0000 722c 0000 00da 015f da05 7973  +...r,....._..ys
+00000710: 697a 65da 0663 7572 736f 72da 046c 696e  ize..cursor..lin
+00000720: 65da 0d77 7261 7070 6564 5f6c 696e 6573  e..wrapped_lines
+00000730: 7213 0000 0072 1400 0000 da01 7772 1100  r....r......wr..
+00000740: 0000 7211 0000 0072 1500 0000 da06 7265  ..r....r......re
+00000750: 6e64 6572 2800 0000 731e 0000 000a 0e04  nder(...s.......
+00000760: 010c 011a 0108 0112 0108 010a 010a 0110  ................
+00000770: 0108 0114 0114 0102 f804 097a 0b46 6f6e  ...........z.Fon
+00000780: 742e 7265 6e64 6572 7237 0000 0063 0600  t.renderr7...c..
+00000790: 0000 0000 0000 0000 0000 0900 0000 0400  ................
+000007a0: 0000 4300 0000 7394 0000 007c 0304 0004  ..C...s....|....
+000007b0: 0064 016b 0272 076e 0704 0064 0275 0072  .d.k.r.n...d.u.r
+000007c0: 0c6e 0201 006e 0601 0001 007c 027d 067c  .n...n.....|.}.|
+000007d0: 0653 0004 0064 036b 0272 3101 007c 0573  .S...d.k.r1..|.s
+000007e0: 1f74 0064 0483 0182 017c 00a0 017c 017c  .t.d.....|...|.|
+000007f0: 04a1 027d 077c 057c 0718 007d 087c 027c  ...}.|.|...}.|.|
+00000800: 0864 051a 0017 007d 067c 0653 0064 066b  .d.....}.|.S.d.k
+00000810: 0272 427c 00a0 017c 017c 04a1 027d 077c  .rB|...|.|...}.|
+00000820: 027c 0517 007c 0718 007d 067c 0653 0009  .|...|...}.|.S..
+00000830: 0074 0064 077c 039b 009d 0283 0182 0129  .t.d.|.........)
+00000840: 087a 2c55 7365 6420 666f 7220 6c65 6674  .z,Used for left
+00000850: 2f72 6967 6874 2f63 656e 7465 7265 6420  /right/centered 
+00000860: 7465 7874 2061 6c69 676e 6d6e 656e 74e9  text alignmnent.
+00000870: ffff ffff 4e72 0100 0000 7a32 4361 6e27  ....Nr....z2Can'
+00000880: 7420 6365 6e74 6572 2074 6578 7420 7769  t center text wi
+00000890: 7468 6f75 7420 7370 6563 6966 7969 6e67  thout specifying
+000008a0: 2061 2077 7261 7020 7769 6474 682e e902   a wrap width...
+000008b0: 0000 0072 2500 0000 7a15 4261 6420 616c  ...r%...z.Bad al
+000008c0: 6967 6e6d 656e 7420 7661 6c75 653a 2029  ignment value: )
+000008d0: 0272 0800 0000 da0d 7072 696e 7465 645f  .r......printed_
+000008e0: 7769 6474 6829 0972 1d00 0000 7237 0000  width).r....r7..
+000008f0: 0072 2800 0000 722c 0000 0072 2a00 0000  .r(...r,...r*...
+00000900: 722b 0000 0072 3600 0000 da0a 6c69 6e65  r+...r6.....line
+00000910: 5f77 6964 7468 da05 736c 6163 6b72 1100  _width..slackr..
+00000920: 0000 7211 0000 0072 1500 0000 7230 0000  ..r....r....r0..
+00000930: 0045 0000 0073 2200 0000 0202 1e01 0401  .E...s".........
+00000940: 040c 0af5 0401 0801 0c01 0801 0c01 0406  ................
+00000950: 06fb 0c01 0c01 0403 02fe 0e01 7a11 466f  ............z.Fo
+00000960: 6e74 2e61 6c69 676e 5f63 7572 736f 7263  nt.align_cursorc
+00000970: 0500 0000 0000 0000 0000 0000 0900 0000  ................
+00000980: 0500 0000 4300 0000 7360 0000 0067 007d  ....C...s`...g.}
+00000990: 0564 017d 067c 01a0 0064 02a1 0144 005d  .d.}.|...d...D.]
+000009a0: 1f7d 077c 0672 147c 069b 0064 027c 079b  .}.|.r.|...d.|..
+000009b0: 009d 036e 017c 077d 087c 00a0 017c 087c  ...n.|.}.|...|.|
+000009c0: 04a1 027c 026b 0172 217c 087d 0671 097c  ...|.k.r!|.}.q.|
+000009d0: 05a0 027c 06a1 0101 007c 077d 0671 097c  ...|.....|.}.q.|
+000009e0: 05a0 027c 06a1 0101 007c 0553 0029 037a  ...|.....|.S.).z
+000009f0: 4042 7265 616b 206f 6e65 206c 6f6e 6720  @Break one long 
+00000a00: 6c69 6e65 2069 6e74 6f20 6d75 6c74 6970  line into multip
+00000a10: 6c65 206c 696e 6573 2062 6173 6564 206f  le lines based o
+00000a20: 6e20 7468 6520 7772 6170 2077 6964 7468  n the wrap width
+00000a30: 2eda 0072 0f00 0000 2903 da05 7370 6c69  ...r....)...spli
+00000a40: 7472 3d00 0000 da06 6170 7065 6e64 2909  tr=.....append).
+00000a50: 721d 0000 0072 2700 0000 722b 0000 0072  r....r'...r+...r
+00000a60: 2800 0000 722a 0000 00da 056c 696e 6573  (...r*.....lines
+00000a70: 7237 0000 00da 0477 6f72 64da 086e 6577  r7.....word..new
+00000a80: 5f6c 696e 6572 1100 0000 7211 0000 0072  _liner....r....r
+00000a90: 1500 0000 722f 0000 0057 0000 0073 1400  ....r/...W...s..
+00000aa0: 0000 0402 0401 0e01 1601 1001 0601 0a02  ................
+00000ab0: 0601 0a01 0401 7a0f 466f 6e74 2e77 7261  ......z.Font.wra
+00000ac0: 705f 776f 7264 7363 0300 0000 0000 0000  p_wordsc........
+00000ad0: 0000 0000 0300 0000 0400 0000 0300 0000  ................
+00000ae0: 7318 0000 0074 0087 0087 0166 0264 0164  s....t.....f.d.d
+00000af0: 0284 087c 0144 0083 0183 0153 0029 034e  ...|.D.....S.).N
+00000b00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000b10: 0004 0000 0033 0000 0073 2800 0000 8100  .....3...s(.....
+00000b20: 7c00 5d0f 7d01 8801 a000 7c01 a101 a001  |.].}.....|.....
+00000b30: a100 8801 6a02 1700 8800 1400 5600 0100  ....j.......V...
+00000b40: 7102 6400 5300 a901 4e29 0372 3100 0000  q.d.S...N).r1...
+00000b50: 7233 0000 0072 0c00 0000 2902 7212 0000  r3...r....).r...
+00000b60: 0072 1300 0000 a902 722a 0000 0072 1d00  .r......r*...r..
+00000b70: 0000 7211 0000 0072 1500 0000 da09 3c67  ..r....r......<g
+00000b80: 656e 6578 7072 3e66 0000 0073 0400 0000  enexpr>f...s....
+00000b90: 0280 2600 7a25 466f 6e74 2e70 7269 6e74  ..&.z%Font.print
+00000ba0: 6564 5f77 6964 7468 2e3c 6c6f 6361 6c73  ed_width.<locals
+00000bb0: 3e2e 3c67 656e 6578 7072 3e29 01da 0373  >.<genexpr>)...s
+00000bc0: 756d 2903 721d 0000 0072 2700 0000 722a  um).r....r'...r*
+00000bd0: 0000 0072 1100 0000 7247 0000 0072 1500  ...r....rG...r..
+00000be0: 0000 723d 0000 0065 0000 0073 0200 0000  ..r=...e...s....
+00000bf0: 1801 7a12 466f 6e74 2e70 7269 6e74 6564  ..z.Font.printed
+00000c00: 5f77 6964 7468 7223 0000 0063 0200 0000  _widthr#...c....
+00000c10: 0000 0000 0000 0000 0a00 0000 0700 0000  ................
+00000c20: 4300 0000 734e 0000 0067 007d 027c 0144  C...sN...g.}.|.D
+00000c30: 005d 207d 037c 03a0 00a1 005c 047d 047d  .] }.|.....\.}.}
+00000c40: 057d 067d 057c 03a0 01a1 005c 047d 057d  .}.}.|.....\.}.}
+00000c50: 077d 057d 087c 03a0 027c 047c 077c 067c  .}.}.|...|.|.|.|
+00000c60: 0866 04a1 017d 097c 02a0 037c 09a1 0101  .f...}.|...|....
+00000c70: 0071 047c 0253 0029 017a 254d 616b 6520  .q.|.S.).z%Make 
+00000c80: 6120 6d6f 6e6f 7370 6163 6564 2066 6f6e  a monospaced fon
+00000c90: 7420 6e6f 6e2d 6d6f 6e6f 7370 6163 6564  t non-monospaced
+00000ca0: 2904 da11 6765 745f 626f 756e 6469 6e67  )...get_bounding
+00000cb0: 5f72 6563 74da 0867 6574 5f72 6563 74da  _rect..get_rect.
+00000cc0: 0a73 7562 7375 7266 6163 6572 4200 0000  .subsurfacerB...
+00000cd0: 290a 721d 0000 0072 2300 0000 da07 7472  ).r....r#.....tr
+00000ce0: 696d 6d65 6472 1400 0000 7228 0000 0072  immedr....r(...r
+00000cf0: 3400 0000 7239 0000 0072 2900 0000 da01  4...r9...r).....
+00000d00: 68da 036e 6577 7211 0000 0072 1100 0000  h..newr....r....
+00000d10: 7215 0000 0072 1a00 0000 6800 0000 730e  r....r....h...s.
+00000d20: 0000 0004 0208 0110 0110 0112 010c 0104  ................
+00000d30: 017a 1046 6f6e 742e 7472 696d 5f69 6d61  .z.Font.trim_ima
+00000d40: 6765 7372 1300 0000 6302 0000 0000 0000  gesr....c.......
+00000d50: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
+00000d60: 0073 2600 0000 7a06 7c00 6a00 7c01 1900  .s&...z.|.j.|...
+00000d70: 5700 5300 0400 7401 7912 0100 0100 0100  W.S...t.y.......
+00000d80: 7c00 6a02 0600 5900 5300 7700 7246 0000  |.j...Y.S.w.rF..
+00000d90: 0029 0372 0a00 0000 da08 4b65 7945 7272  .).r......KeyErr
+00000da0: 6f72 7218 0000 0029 0272 1d00 0000 7213  orr....).r....r.
+00000db0: 0000 0072 1100 0000 7211 0000 0072 1500  ...r....r....r..
+00000dc0: 0000 7231 0000 0072 0000 0073 0a00 0000  ..r1...r...s....
+00000dd0: 0201 0c01 0c01 0a01 02ff 7a08 466f 6e74  ..........z.Font
+00000de0: 2e67 6574 2904 7201 0000 0072 0100 0000  .get).r....r....
+00000df0: 464e 2905 7201 0000 0072 0100 0000 7225  FN).r....r....r%
+00000e00: 0000 0072 0100 0000 4e29 0272 0100 0000  ...r....N).r....
+00000e10: 7225 0000 0029 12da 085f 5f6e 616d 655f  r%...)...__name_
+00000e20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000e30: 5f71 7561 6c6e 616d 655f 5f72 1700 0000  _qualname__r....
+00000e40: da03 7374 7272 0400 0000 da0f 5f5f 616e  ..strr......__an
+00000e50: 6e6f 7461 7469 6f6e 735f 5fda 0574 7570  notations__..tup
+00000e60: 6c65 da03 696e 7472 0200 0000 7224 0000  le..intr....r$..
+00000e70: 0072 3a00 0000 7230 0000 00da 046c 6973  .r:...r0.....lis
+00000e80: 7472 2f00 0000 723d 0000 0072 1a00 0000  tr/...r=...r....
+00000e90: 7231 0000 0072 1100 0000 7211 0000 0072  r1...r....r....r
+00000ea0: 1100 0000 7215 0000 0072 0900 0000 0a00  ....r....r......
+00000eb0: 0000 7356 0000 000a 0010 0110 0108 0108  ..sV............
+00000ec0: 0102 0702 0102 0102 0104 f806 0202 fe0a  ................
+00000ed0: 0302 fd02 040a fc02 1c02 0102 0102 0102  ................
+00000ee0: 0104 f802 0202 fe02 0302 fd02 0402 fc02  ................
+00000ef0: 0502 fb02 0602 fa02 0702 f902 0802 f802  ................
+00000f00: 090a f722 1d24 1216 0e1a 0316 0a72 0900  ...".$.......r..
+00000f10: 0000 4e29 0dda 0770 6174 686c 6962 7202  ..N)...pathlibr.
+00000f20: 0000 00da 0c70 7967 616d 652e 636f 6c6f  .....pygame.colo
+00000f30: 7272 0300 0000 da0e 7079 6761 6d65 2e73  rr......pygame.s
+00000f40: 7572 6661 6365 7204 0000 00da 0f72 6f62  urfacer......rob
+00000f50: 696e 6761 6d65 2e69 6d61 6765 7205 0000  ingame.imager...
+00000f60: 0072 0600 0000 7207 0000 00da 1972 6f62  .r....r......rob
+00000f70: 696e 6761 6d65 2e74 6578 742e 6578 6365  ingame.text.exce
+00000f80: 7074 696f 6e73 7208 0000 0072 0900 0000  ptionsr....r....
+00000f90: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000fa0: 1500 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000fb0: 0000 730c 0000 000c 000c 020c 0114 020c  ..s.............
+00000fc0: 0112 03                                  ...
```

### Comparing `robingame-0.0.9/robingame/text/font/__pycache__/fonts.cpython-310.pyc` & `robingame-0.1.0/robingame/text/font/__pycache__/fonts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 13:48:23 2022 UTC, .py size: 1406 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 27a2 3563 7e05 0000  o.......'.5c~...
+00000000: 6f0d 0d0a 0000 0000 7d99 9d64 8705 0000  o.......}..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6504 8300 5a07  d.l.m.Z...e...Z.
 00000060: 6502 6508 8301 6a09 6a09 6405 1b00 5a0a  e.e...j.j.d...Z.
 00000070: 6506 650a 6406 1b00 6407 6500 6a0b 6500  e.e.d...d.e.j.e.
@@ -16,47 +16,47 @@
 000000f0: 6506 650a 6415 1b00 640e 640f 6500 6a0b  e.e.d...d.d.e.j.
 00000100: 1700 6410 1700 6500 6a0c 1700 6411 1700  ..d...e.j...d...
 00000110: 6412 6416 8d04 5a10 6401 5300 2917 e900  d.d...Z.d.S.)...
 00000120: 0000 004e 2901 da04 5061 7468 2901 da0c  ...N)...Path)...
 00000130: 696e 6974 5f64 6973 706c 6179 2901 da04  init_display)...
 00000140: 466f 6e74 da06 6173 7365 7473 7a0d 7465  Font..assetsz.te
 00000150: 7374 5f66 6f6e 742e 706e 6729 02e9 1000  st_font.png)....
-00000160: 0000 7206 0000 007a 2a31 3233 3435 3637  ..r....z*1234567
+00000160: 0000 7206 0000 007a 2b31 3233 3435 3637  ..r....z+1234567
 00000170: 3839 302d 3d21 4023 2425 5e26 2a28 295f  890-=!@#$%^&*()_
-00000180: 2b5b 5d5c 3b27 2c2e 2f7b 7d7c 3a22 3c3e  +[]\;',./{}|:"<>
-00000190: 3f7e 6054 e901 0000 00e9 0800 0000 2906  ?~`T..........).
-000001a0: da08 6669 6c65 6e61 6d65 da0a 696d 6167  ..filename..imag
-000001b0: 655f 7369 7a65 da07 6c65 7474 6572 73da  e_size..letters.
-000001c0: 0474 7269 6dda 0478 7061 64da 0b73 7061  .trim..xpad..spa
-000001d0: 6365 5f77 6964 7468 7a13 6365 6c6c 7068  ce_widthz.cellph
-000001e0: 6f6e 652d 626c 6163 6b2e 706e 6729 02e9  one-black.png)..
-000001f0: 0700 0000 e909 0000 007a 2021 2223 2425  .........z !"#$%
-00000200: 2627 2829 2a2b 2c2d 2e2f 3031 3233 3435  &'()*+,-./012345
-00000210: 3637 3839 3a27 3c3d 3e3f 407a 065b 5c5d  6789:'<=>?@z.[\]
-00000220: 5e5f 607a 047b 7c7d 7ee9 ffff ffff e904  ^_`z.{|}~.......
-00000230: 0000 0029 0772 0900 0000 720a 0000 0072  ...).r....r....r
-00000240: 0b00 0000 720d 0000 00da 0863 6f6c 6f72  ....r......color
-00000250: 6b65 7972 0c00 0000 720e 0000 007a 1363  keyr....r....z.c
-00000260: 656c 6c70 686f 6e65 2d77 6869 7465 2e70  ellphone-white.p
-00000270: 6e67 2904 7209 0000 0072 0a00 0000 720b  ng).r....r....r.
-00000280: 0000 0072 1300 0000 2911 da06 7374 7269  ...r....)...stri
-00000290: 6e67 da07 7061 7468 6c69 6272 0200 0000  ng..pathlibr....
-000002a0: da0f 726f 6269 6e67 616d 652e 696d 6167  ..robingame.imag
-000002b0: 6572 0300 0000 da13 726f 6269 6e67 616d  er......robingam
-000002c0: 652e 7465 7874 2e66 6f6e 7472 0400 0000  e.text.fontr....
-000002d0: da06 7769 6e64 6f77 da08 5f5f 6669 6c65  ..window..__file
-000002e0: 5f5f da06 7061 7265 6e74 7205 0000 00da  __..parentr.....
-000002f0: 0f61 7363 6969 5f75 7070 6572 6361 7365  .ascii_uppercase
-00000300: da0f 6173 6369 695f 6c6f 7765 7263 6173  ..ascii_lowercas
-00000310: 655a 0974 6573 745f 666f 6e74 da0f 6365  eZ.test_font..ce
-00000320: 6c6c 7068 6f6e 655f 626c 6163 6b5a 0f63  llphone_blackZ.c
-00000330: 656c 6c70 686f 6e65 5f77 6869 7465 5a14  ellphone_whiteZ.
-00000340: 6365 6c6c 7068 6f6e 655f 7768 6974 655f  cellphone_white_
-00000350: 6d6f 6e6f a900 721e 0000 0072 1e00 0000  mono..r....r....
-00000360: fa38 2f68 6f6d 652f 6269 6e6e 6576 2f63  .8/home/binnev/c
+00000180: 2b5b 5d5c 3b27 2c2e 2f7b 7d7c 3a5c 223c  +[]\;',./{}|:\"<
+00000190: 3e3f 7e60 54e9 0100 0000 e908 0000 0029  >?~`T..........)
+000001a0: 06da 0866 696c 656e 616d 65da 0a69 6d61  ...filename..ima
+000001b0: 6765 5f73 697a 65da 076c 6574 7465 7273  ge_size..letters
+000001c0: da04 7472 696d da04 7870 6164 da0b 7370  ..trim..xpad..sp
+000001d0: 6163 655f 7769 6474 687a 1363 656c 6c70  ace_widthz.cellp
+000001e0: 686f 6e65 2d62 6c61 636b 2e70 6e67 2902  hone-black.png).
+000001f0: e907 0000 00e9 0900 0000 7a20 2122 2324  ..........z !"#$
+00000200: 2526 2728 292a 2b2c 2d2e 2f30 3132 3334  %&'()*+,-./01234
+00000210: 3536 3738 393a 3b3c 3d3e 3f40 7a06 5b5c  56789:;<=>?@z.[\
+00000220: 5d5e 5f60 7a04 7b7c 7d7e e9ff ffff ffe9  ]^_`z.{|}~......
+00000230: 0400 0000 2907 7209 0000 0072 0a00 0000  ....).r....r....
+00000240: 720b 0000 0072 0d00 0000 da08 636f 6c6f  r....r......colo
+00000250: 726b 6579 720c 0000 0072 0e00 0000 7a13  rkeyr....r....z.
+00000260: 6365 6c6c 7068 6f6e 652d 7768 6974 652e  cellphone-white.
+00000270: 706e 6729 0472 0900 0000 720a 0000 0072  png).r....r....r
+00000280: 0b00 0000 7213 0000 0029 11da 0673 7472  ....r....)...str
+00000290: 696e 67da 0770 6174 686c 6962 7202 0000  ing..pathlibr...
+000002a0: 00da 0f72 6f62 696e 6761 6d65 2e69 6d61  ...robingame.ima
+000002b0: 6765 7203 0000 00da 1372 6f62 696e 6761  ger......robinga
+000002c0: 6d65 2e74 6578 742e 666f 6e74 7204 0000  me.text.fontr...
+000002d0: 00da 0677 696e 646f 77da 085f 5f66 696c  ...window..__fil
+000002e0: 655f 5fda 0670 6172 656e 7472 0500 0000  e__..parentr....
+000002f0: da0f 6173 6369 695f 7570 7065 7263 6173  ..ascii_uppercas
+00000300: 65da 0f61 7363 6969 5f6c 6f77 6572 6361  e..ascii_lowerca
+00000310: 7365 da09 7465 7374 5f66 6f6e 74da 0f63  se..test_font..c
+00000320: 656c 6c70 686f 6e65 5f62 6c61 636b da0f  ellphone_black..
+00000330: 6365 6c6c 7068 6f6e 655f 7768 6974 65da  cellphone_white.
+00000340: 1463 656c 6c70 686f 6e65 5f77 6869 7465  .cellphone_white
+00000350: 5f6d 6f6e 6fa9 0072 2100 0000 7221 0000  _mono..r!...r!..
+00000360: 00fa 372f 686f 6d65 2f72 6f62 696e 2f63  ..7/home/robin/c
 00000370: 6f64 652f 726f 6269 6e67 616d 652f 726f  ode/robingame/ro
 00000380: 6269 6e67 616d 652f 7465 7874 2f66 6f6e  bingame/text/fon
 00000390: 742f 666f 6e74 732e 7079 da08 3c6d 6f64  t/fonts.py..<mod
 000003a0: 756c 653e 0100 0000 7384 0000 0008 000c  ule>....s.......
 000003b0: 010c 020c 0106 0210 0202 0206 0102 0104  ................
 000003c0: 0204 0102 ff02 0202 fe02 0402 0102 0106  ................
 000003d0: f602 0d06 0102 0102 0204 0102 ff02 0202  ................
```

### Comparing `robingame-0.0.9/robingame/text/font/classes.py` & `robingame-0.1.0/robingame/text/font/classes.py`

 * *Files identical despite different names*

### Comparing `robingame-0.0.9/robingame/text/font/font_sandbox.py` & `robingame-0.1.0/robingame/text/font/font_sandbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Ook    in 
 de     spelling 
 van    sommige andere talen wordt de umlaut gebruikt, bijvoorbeeld in verwante 
 talen als het IJslands en het Zweeds, om een soortgelijk 
 
 klankverschijnsel
 weer
-te
+te;;;'''
 
 geven, of in niet-verwante talen als het Fins, het Hongaars of het Turks, om dezelfde e-, eu- en u-klank weer te geven, die echter niet het resultaat van hetzelfde klankverschijnsel zijn.
 """
 
 
 class FontTest(Game):
     window_width = 1500
```

### Comparing `robingame-0.0.9/robingame/text/font/fonts.py` & `robingame-0.1.0/robingame/text/font/fonts.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,56 +10,56 @@
 
 test_font = Font(
     filename=assets / "test_font.png",
     image_size=(16, 16),
     letters=(
         string.ascii_uppercase
         + string.ascii_lowercase
-        + "1234567890-=!@#$%^&*()_+[]\;',./{}|:\"<>?~`"
+        + r"1234567890-=!@#$%^&*()_+[]\;',./{}|:\"<>?~`"
     ),
     trim=True,
     xpad=1,
     space_width=8,
 )
 
 cellphone_black = Font(
     filename=assets / "cellphone-black.png",
     image_size=(7, 9),
     letters=(
-        """!"#$%&'()*+,-./0123456789:'<=>?@"""
+        """!"#$%&'()*+,-./0123456789:;<=>?@"""
         + string.ascii_uppercase
-        + "[\]^_`"
+        + r"[\]^_`"
         + string.ascii_lowercase
-        + "{|}~"
+        + r"{|}~"
     ),
     xpad=1,
     colorkey=-1,
     trim=True,
     space_width=4,
 )
 cellphone_white = Font(
     filename=assets / "cellphone-white.png",
     image_size=(7, 9),
     letters=(
-        """!"#$%&'()*+,-./0123456789:'<=>?@"""
+        r"""!"#$%&'()*+,-./0123456789:;<=>?@"""
         + string.ascii_uppercase
-        + "[\]^_`"
+        + r"[\]^_`"
         + string.ascii_lowercase
-        + "{|}~"
+        + r"{|}~"
     ),
     xpad=1,
     colorkey=-1,
     trim=True,
     space_width=4,
 )
 cellphone_white_mono = Font(
     filename=assets / "cellphone-white.png",
     image_size=(7, 9),
     letters=(
-        """!"#$%&'()*+,-./0123456789:'<=>?@"""
+        r"""!"#$%&'()*+,-./0123456789:;<=>?@"""
         + string.ascii_uppercase
-        + "[\]^_`"
+        + r"[\]^_`"
         + string.ascii_lowercase
-        + "{|}~"
+        + r"{|}~"
     ),
     colorkey=-1,
 )
```

### Comparing `robingame-0.0.9/robingame/utils.py` & `robingame-0.1.0/robingame/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,18 +87,14 @@
 
 
 def outline_image(surface: Surface):
     mask = maskFromSurface(surface)
     return mask.outline()
 
 
-def ticks_to_frames(tick, ticks_per_frame):
-    return tick // ticks_per_frame
-
-
 def draw_arrow(surface, origin, angle_deg, color=None, length=50):
     """angle needs to be in degrees"""
     arrow_xy = arrow_coords(length, length // 10, length // 4)
     r = rotation_matrix(angle_deg)
     arrow_xy = arrow_xy.dot(r)
     arrow_xy += numpy.array(origin)
     pygame.draw.polygon(surface, color, arrow_xy, 2)
@@ -162,30 +158,14 @@
 
 
 def mouse_hovering_over(element):
     mouse_x, mouse_y = pygame.mouse.get_pos()
     return element.rect.collidepoint(mouse_x, mouse_y)
 
 
-class MyEnumMeta(enum.EnumMeta):
-    """
-    Incredibly, enum.Enum does not have a __contains__ method, so we can't do stuff like:
-    class Colours(Enum):
-        ...
-    assert "red" in Colours
-    """
-
-    def __contains__(cls, member):
-        return any(x.value == member for x in cls)
-
-
-class Enum(enum.Enum, metaclass=MyEnumMeta):
-    pass
-
-
 def circle_surf(radius, color):
     radius = int(radius)
     surf = Surface((radius * 2, radius * 2))
     pygame.draw.circle(surf, color, (radius, radius), radius)
     surf.set_colorkey((0, 0, 0))
     return surf
 
@@ -261,36 +241,11 @@
     def height(self) -> int:
         _, height = self.size
         return height
 
     def copy(self) -> "SparseMatrix":
         return SparseMatrix(super().copy())
 
-    def scale_to_screen(self, screen_size: (int, int)) -> (float, int, int):
-        """
-        Calculate the scaling factor and x/y offset required to blit a group of pixels
-        representing self onto a screen
-        """
-        screen_width, screen_height = screen_size
-        self_width, self_height = self.size
-        xlim, ylim = self.limits
-        x_scaling = screen_width // self_width
-        y_scaling = screen_height // self_height
-        scaling = max(1, min(x_scaling, y_scaling))
-
-        x_offset = screen_width // 2 - (xlim[0] + self_width // 2) * scaling
-        y_offset = screen_height // 2 - (ylim[0] + self_height // 2) * scaling
-        return scaling, x_offset, y_offset
-
-    def screen_coords(self, xy, scaling, x_offset, y_offset) -> tuple[int, int]:
-        """
-        Convert col/row number (xy) into screen coordinates (in pixels)
-        """
-        x, y = xy
-        screen_x = x_offset + x * scaling
-        screen_y = y_offset + y * scaling
-        return screen_x, screen_y
-
 
 def draw_text(s: str, surface: Surface, position, font, color, antialias=False):
     text_bitmap = font.render(s, antialias, color)
     surface.blit(text_bitmap, position)
```

### Comparing `robingame-0.0.9/robingame.egg-info/SOURCES.txt` & `robingame-0.1.0/robingame.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,34 @@
 robingame.egg-info/dependency_links.txt
 robingame.egg-info/requires.txt
 robingame.egg-info/top_level.txt
 robingame/__pycache__/__init__.cpython-310.pyc
 robingame/__pycache__/animation.cpython-310.pyc
 robingame/__pycache__/utils.cpython-310.pyc
 robingame/examples/__init__.py
+robingame/examples/particle_example.py
 robingame/examples/__pycache__/__init__.cpython-310.pyc
 robingame/examples/gui_examples/__init__.py
 robingame/examples/gui_examples/coloured_button_effects.py
 robingame/examples/gui_examples/complicated_on_press_hook.py
 robingame/examples/gui_examples/on_press_event.py
 robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
+robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc
 robingame/examples/gui_examples/assets/__init__.py
 robingame/examples/gui_examples/assets/button-up.aseprite
 robingame/examples/gui_examples/assets/button-up.png
 robingame/examples/gui_examples/assets/flashybutton.aseprite
 robingame/examples/gui_examples/assets/flashybutton.png
 robingame/examples/gui_examples/assets/__pycache__/__init__.cpython-310.pyc
 robingame/gui/__init__.py
 robingame/gui/button.py
 robingame/gui/menu.py
 robingame/gui/__pycache__/__init__.cpython-310.pyc
 robingame/gui/__pycache__/button.cpython-310.pyc
+robingame/gui/__pycache__/menu.cpython-310.pyc
 robingame/image/__init__.py
 robingame/image/classes.py
 robingame/image/utils.py
 robingame/image/__pycache__/__init__.cpython-310.pyc
 robingame/image/__pycache__/classes.cpython-310.pyc
 robingame/image/__pycache__/utils.cpython-310.pyc
 robingame/input/__init__.py
@@ -74,8 +77,14 @@
 robingame/text/assets/test_font.png
 robingame/text/font/__init__.py
 robingame/text/font/classes.py
 robingame/text/font/font_sandbox.py
 robingame/text/font/fonts.py
 robingame/text/font/__pycache__/__init__.cpython-310.pyc
 robingame/text/font/__pycache__/classes.cpython-310.pyc
-robingame/text/font/__pycache__/fonts.cpython-310.pyc
+robingame/text/font/__pycache__/fonts.cpython-310.pyc
+tests/test_animation.py
+tests/test_event.py
+tests/test_image.py
+tests/test_inputs.py
+tests/test_text.py
+tests/test_utils.py
```

### Comparing `robingame-0.0.9/setup.cfg` & `robingame-0.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = robingame
-version = 0.0.9
+version = 0.1.0
 author = Robin Neville
 author_email = robin.m.neville@gmail.com
 description = Object-oriented tools for Pygame projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/binnev/robingame
 project_urls = 
@@ -17,14 +17,15 @@
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	pygame >=2.0
 	typing >=3.7
 	packaging >=3.0
+	numpy
 include_package_data = True
 
 [options.packages.find]
 include = 
 	robingame*
 
 [egg_info]
```

