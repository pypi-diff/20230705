# Comparing `tmp/arena-py-0.4.3.tar.gz` & `tmp/arena-py-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena-py-0.4.3.tar", last modified: Wed Jul  5 20:33:55 2023, max compression
+gzip compressed data, was "arena-py-0.4.4.tar", last modified: Wed Jul  5 20:50:30 2023, max compression
```

## Comparing `arena-py-0.4.3.tar` & `arena-py-0.4.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1533 2023-05-26 22:34:51.000000 arena-py-0.4.3/LICENSE
--rw-rw-r--   0 edward    (1000) edward    (1000)     4417 2023-07-05 20:33:55.937358 arena-py-0.4.3/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)     3913 2023-07-05 20:31:34.000000 arena-py-0.4.3/README.md
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.933358 arena-py-0.4.3/arena/
--rw-rw-r--   0 edward    (1000) edward    (1000)      279 2023-07-05 20:29:55.000000 arena-py-0.4.3/arena/__init__.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)     3148 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/__main__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    12667 2023-07-05 20:21:44.000000 arena-py-0.4.3/arena/arena_mqtt.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/attributes/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1022 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1031 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/animation.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      139 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/animation_mixer.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      175 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/attribute.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1135 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/color.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     4974 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/data.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      362 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/goto_url.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      764 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/impulse.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      503 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/jitsi_video.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      811 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/landmark.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      611 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/material.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      237 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/morph.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      357 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/physics.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      496 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/position.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2681 2023-07-05 18:37:42.000000 arena-py-0.4.3/arena/attributes/rotation.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      355 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/scale.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      247 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/sound.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      475 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/text_input.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      152 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/attributes/video_control.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    16461 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/auth.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1127 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/base_object.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2837 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/device.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/event_loop/
--rw-rw-r--   0 edward    (1000) edward    (1000)      267 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      419 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/async_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2395 2023-07-05 20:19:01.000000 arena-py-0.4.3/arena/event_loop/asyncio_mqtt.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1749 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/event_loop.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      651 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/lazy_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      841 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/persistent_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      129 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/single_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1171 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/event_loop/worker.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/events/
--rw-rw-r--   0 edward    (1000) edward    (1000)       25 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/events/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      984 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/events/event.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/objects/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1289 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     6766 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/arena_object.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      516 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/box.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1569 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/camera.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/circle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      228 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/cone.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      243 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/cylinder.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      260 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/dodecahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/entity.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1320 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/gltf.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      256 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/icosahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      249 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/image.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/light.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      332 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/line.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      252 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/octahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      244 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/particle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/plane.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      228 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/ring.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/sphere.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      256 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/tetrahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      264 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/text.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1023 2023-07-05 18:37:42.000000 arena-py-0.4.3/arena/objects/thickline.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/torus.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      248 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/torus_knot.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      244 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/objects/triangle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    16309 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scene.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/scripts/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/__init__.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      122 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/arena_py_permissions.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      557 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/arena_py_pub.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      118 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/arena_py_signout.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      559 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/arena_py_sub.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      229 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/scripts/arena_py_token.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena/utils/
--rw-rw-r--   0 edward    (1000) edward    (1000)       25 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/utils/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      781 2023-05-26 22:34:51.000000 arena-py-0.4.3/arena/utils/utils.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 20:33:55.937358 arena-py-0.4.3/arena_py.egg-info/
--rw-rw-r--   0 edward    (1000) edward    (1000)     4417 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)     2057 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/SOURCES.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/dependency_links.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      308 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/entry_points.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      125 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/requires.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        6 2023-07-05 20:33:55.000000 arena-py-0.4.3/arena_py.egg-info/top_level.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)       38 2023-07-05 20:33:55.937358 arena-py-0.4.3/setup.cfg
--rw-rw-r--   0 edward    (1000) edward    (1000)     1404 2023-07-05 20:28:48.000000 arena-py-0.4.3/setup.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.924195 arena-py-0.4.4/
+-rw-r--r--   0 Edward     (502) staff       (20)     1533 2021-03-04 00:17:57.000000 arena-py-0.4.4/LICENSE
+-rw-r--r--   0 Edward     (502) staff       (20)     4417 2023-07-05 20:50:30.924017 arena-py-0.4.4/PKG-INFO
+-rw-r--r--   0 Edward     (502) staff       (20)     3913 2023-07-05 20:46:40.000000 arena-py-0.4.4/README.md
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.912760 arena-py-0.4.4/arena/
+-rw-r--r--   0 Edward     (502) staff       (20)      279 2023-07-05 20:49:19.000000 arena-py-0.4.4/arena/__init__.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)     3148 2023-05-31 20:38:43.000000 arena-py-0.4.4/arena/__main__.py
+-rw-r--r--   0 Edward     (502) staff       (20)    12667 2023-07-05 20:46:40.000000 arena-py-0.4.4/arena/arena_mqtt.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.915632 arena-py-0.4.4/arena/attributes/
+-rw-r--r--   0 Edward     (502) staff       (20)     1022 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/__init__.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1031 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/attributes/animation.py
+-rw-r--r--   0 Edward     (502) staff       (20)      139 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/attributes/animation_mixer.py
+-rw-r--r--   0 Edward     (502) staff       (20)      175 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/attributes/attribute.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1135 2021-05-21 05:01:05.000000 arena-py-0.4.4/arena/attributes/color.py
+-rw-r--r--   0 Edward     (502) staff       (20)     4974 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/data.py
+-rw-r--r--   0 Edward     (502) staff       (20)      362 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/goto_url.py
+-rw-r--r--   0 Edward     (502) staff       (20)      764 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/impulse.py
+-rw-r--r--   0 Edward     (502) staff       (20)      503 2021-08-20 17:34:16.000000 arena-py-0.4.4/arena/attributes/jitsi_video.py
+-rw-r--r--   0 Edward     (502) staff       (20)      811 2021-04-30 21:26:45.000000 arena-py-0.4.4/arena/attributes/landmark.py
+-rw-r--r--   0 Edward     (502) staff       (20)      611 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/material.py
+-rw-r--r--   0 Edward     (502) staff       (20)      237 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/morph.py
+-rw-r--r--   0 Edward     (502) staff       (20)      357 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/physics.py
+-rw-r--r--   0 Edward     (502) staff       (20)      496 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/attributes/position.py
+-rw-r--r--   0 Edward     (502) staff       (20)     2681 2023-07-05 19:04:15.000000 arena-py-0.4.4/arena/attributes/rotation.py
+-rw-r--r--   0 Edward     (502) staff       (20)      355 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/attributes/scale.py
+-rw-r--r--   0 Edward     (502) staff       (20)      247 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/sound.py
+-rw-r--r--   0 Edward     (502) staff       (20)      475 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/text_input.py
+-rw-r--r--   0 Edward     (502) staff       (20)      152 2023-04-12 15:08:29.000000 arena-py-0.4.4/arena/attributes/video_control.py
+-rw-r--r--   0 Edward     (502) staff       (20)    16461 2023-05-31 20:38:43.000000 arena-py-0.4.4/arena/auth.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1127 2021-09-08 19:31:56.000000 arena-py-0.4.4/arena/base_object.py
+-rw-r--r--   0 Edward     (502) staff       (20)     2837 2023-05-31 20:38:43.000000 arena-py-0.4.4/arena/device.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.916925 arena-py-0.4.4/arena/event_loop/
+-rw-r--r--   0 Edward     (502) staff       (20)      267 2021-03-07 17:22:29.000000 arena-py-0.4.4/arena/event_loop/__init__.py
+-rw-r--r--   0 Edward     (502) staff       (20)      419 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/event_loop/async_worker.py
+-rw-r--r--   0 Edward     (502) staff       (20)     2457 2023-07-05 20:48:09.000000 arena-py-0.4.4/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1749 2021-05-20 04:16:27.000000 arena-py-0.4.4/arena/event_loop/event_loop.py
+-rw-r--r--   0 Edward     (502) staff       (20)      651 2021-05-17 04:11:29.000000 arena-py-0.4.4/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 Edward     (502) staff       (20)      841 2021-05-17 04:11:57.000000 arena-py-0.4.4/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 Edward     (502) staff       (20)      129 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/event_loop/single_worker.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1171 2021-05-17 04:12:52.000000 arena-py-0.4.4/arena/event_loop/worker.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.917270 arena-py-0.4.4/arena/events/
+-rw-r--r--   0 Edward     (502) staff       (20)       25 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/events/__init__.py
+-rw-r--r--   0 Edward     (502) staff       (20)      984 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/events/event.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.921550 arena-py-0.4.4/arena/objects/
+-rw-r--r--   0 Edward     (502) staff       (20)     1289 2023-05-26 03:21:00.000000 arena-py-0.4.4/arena/objects/__init__.py
+-rw-r--r--   0 Edward     (502) staff       (20)     6766 2023-07-05 19:05:48.000000 arena-py-0.4.4/arena/objects/arena_object.py
+-rw-r--r--   0 Edward     (502) staff       (20)      516 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/box.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1569 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/camera.py
+-rw-r--r--   0 Edward     (502) staff       (20)      236 2021-03-07 17:04:44.000000 arena-py-0.4.4/arena/objects/circle.py
+-rw-r--r--   0 Edward     (502) staff       (20)      228 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/cone.py
+-rw-r--r--   0 Edward     (502) staff       (20)      243 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/cylinder.py
+-rw-r--r--   0 Edward     (502) staff       (20)      260 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/dodecahedron.py
+-rw-r--r--   0 Edward     (502) staff       (20)      236 2023-05-26 03:21:00.000000 arena-py-0.4.4/arena/objects/entity.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1320 2021-09-08 19:31:56.000000 arena-py-0.4.4/arena/objects/gltf.py
+-rw-r--r--   0 Edward     (502) staff       (20)      256 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/icosahedron.py
+-rw-r--r--   0 Edward     (502) staff       (20)      249 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/image.py
+-rw-r--r--   0 Edward     (502) staff       (20)      232 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/light.py
+-rw-r--r--   0 Edward     (502) staff       (20)      332 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/line.py
+-rw-r--r--   0 Edward     (502) staff       (20)      252 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/octahedron.py
+-rw-r--r--   0 Edward     (502) staff       (20)      244 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/particle.py
+-rw-r--r--   0 Edward     (502) staff       (20)      232 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/plane.py
+-rw-r--r--   0 Edward     (502) staff       (20)      228 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/ring.py
+-rw-r--r--   0 Edward     (502) staff       (20)      236 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/sphere.py
+-rw-r--r--   0 Edward     (502) staff       (20)      256 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/tetrahedron.py
+-rw-r--r--   0 Edward     (502) staff       (20)      264 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/text.py
+-rw-r--r--   0 Edward     (502) staff       (20)     1023 2023-07-05 19:04:15.000000 arena-py-0.4.4/arena/objects/thickline.py
+-rw-r--r--   0 Edward     (502) staff       (20)      232 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/torus.py
+-rw-r--r--   0 Edward     (502) staff       (20)      248 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/torus_knot.py
+-rw-r--r--   0 Edward     (502) staff       (20)      244 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/objects/triangle.py
+-rw-r--r--   0 Edward     (502) staff       (20)    16309 2023-07-05 19:05:49.000000 arena-py-0.4.4/arena/scene.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.922255 arena-py-0.4.4/arena/scripts/
+-rw-r--r--   0 Edward     (502) staff       (20)        0 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/__init__.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)      122 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)      557 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)      118 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)      559 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 Edward     (502) staff       (20)      229 2021-10-01 18:31:38.000000 arena-py-0.4.4/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.922487 arena-py-0.4.4/arena/utils/
+-rw-r--r--   0 Edward     (502) staff       (20)       25 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/utils/__init__.py
+-rw-r--r--   0 Edward     (502) staff       (20)      781 2021-03-04 00:17:57.000000 arena-py-0.4.4/arena/utils/utils.py
+drwxr-xr-x   0 Edward     (502) staff       (20)        0 2023-07-05 20:50:30.923771 arena-py-0.4.4/arena_py.egg-info/
+-rw-r--r--   0 Edward     (502) staff       (20)     4417 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 Edward     (502) staff       (20)     2057 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 Edward     (502) staff       (20)        1 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 Edward     (502) staff       (20)      308 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 Edward     (502) staff       (20)      125 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/requires.txt
+-rw-r--r--   0 Edward     (502) staff       (20)        6 2023-07-05 20:50:30.000000 arena-py-0.4.4/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 Edward     (502) staff       (20)       38 2023-07-05 20:50:30.924240 arena-py-0.4.4/setup.cfg
+-rw-r--r--   0 Edward     (502) staff       (20)     1404 2023-07-05 20:49:24.000000 arena-py-0.4.4/setup.py
```

### Comparing `arena-py-0.4.3/LICENSE` & `arena-py-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/PKG-INFO` & `arena-py-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.3
+Version: 0.4.4
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.4.3/README.md` & `arena-py-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/__main__.py` & `arena-py-0.4.4/arena/__main__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/arena_mqtt.py` & `arena-py-0.4.4/arena/arena_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/__init__.py` & `arena-py-0.4.4/arena/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/animation.py` & `arena-py-0.4.4/arena/attributes/animation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/color.py` & `arena-py-0.4.4/arena/attributes/color.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/data.py` & `arena-py-0.4.4/arena/attributes/data.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/impulse.py` & `arena-py-0.4.4/arena/attributes/impulse.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/landmark.py` & `arena-py-0.4.4/arena/attributes/landmark.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/material.py` & `arena-py-0.4.4/arena/attributes/material.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/attributes/rotation.py` & `arena-py-0.4.4/arena/attributes/rotation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/auth.py` & `arena-py-0.4.4/arena/auth.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/base_object.py` & `arena-py-0.4.4/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/device.py` & `arena-py-0.4.4/arena/device.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.4.4/arena/event_loop/asyncio_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 
     def on_socket_close(self, client, userdata, sock):
         self.loop.remove_reader(sock)
         self.connected = False
 
     def on_socket_register_write(self, client, userdata, sock):
         def cb():
-            client.loop_write()
+            try:
+                client.loop_write()
+            except:
+                pass
 
         self.loop.add_writer(sock, cb)
 
     def on_socket_unregister_write(self, client, userdata, sock):
         self.loop.remove_writer(sock)
 
     async def misc_loop(self):
```

### Comparing `arena-py-0.4.3/arena/event_loop/event_loop.py` & `arena-py-0.4.4/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/event_loop/lazy_worker.py` & `arena-py-0.4.4/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/event_loop/persistent_worker.py` & `arena-py-0.4.4/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/event_loop/worker.py` & `arena-py-0.4.4/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/events/event.py` & `arena-py-0.4.4/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/__init__.py` & `arena-py-0.4.4/arena/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/arena_object.py` & `arena-py-0.4.4/arena/objects/arena_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/box.py` & `arena-py-0.4.4/arena/objects/box.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/camera.py` & `arena-py-0.4.4/arena/objects/camera.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/gltf.py` & `arena-py-0.4.4/arena/objects/gltf.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/objects/thickline.py` & `arena-py-0.4.4/arena/objects/thickline.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/scene.py` & `arena-py-0.4.4/arena/scene.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/scripts/arena_py_pub.py` & `arena-py-0.4.4/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/scripts/arena_py_sub.py` & `arena-py-0.4.4/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena/utils/utils.py` & `arena-py-0.4.4/arena/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/arena_py.egg-info/PKG-INFO` & `arena-py-0.4.4/arena_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.3
+Version: 0.4.4
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.4.3/arena_py.egg-info/SOURCES.txt` & `arena-py-0.4.4/arena_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.3/setup.py` & `arena-py-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="arena-py",
-    version="0.4.3",
+    version="0.4.4",
     author="Conix Research Center",
     author_email="info@conix.io",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/ARENA-py",
```

