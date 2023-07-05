# Comparing `tmp/ocatari-0.1.1.tar.gz` & `tmp/ocatari-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-0.1.1.tar", last modified: Wed Jul  5 09:43:42 2023, max compression
+gzip compressed data, was "ocatari-0.1.2.tar", last modified: Wed Jul  5 10:00:34 2023, max compression
```

## Comparing `ocatari-0.1.1.tar` & `ocatari-0.1.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.397053 ocatari-0.1.1/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1171 2023-06-28 09:13:01.000000 ocatari-0.1.1/LICENSE
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 09:43:42.397053 ocatari-0.1.1/PKG-INFO
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5810 2023-07-04 07:44:43.000000 ocatari-0.1.1/README.md
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.381054 ocatari-0.1.1/ocatari/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       48 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12715 2023-06-28 14:12:36.000000 ocatari-0.1.1/ocatari/core.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2895 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/environments.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.389054 ocatari-0.1.1/ocatari/ram/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      232 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3214 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3910 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/alien.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    14100 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/assault.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8663 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asterix.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12123 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asterix_new.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6852 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asteroids.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13513 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/atlantis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3833 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/beamrider.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9499 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/berzerk.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5576 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/bowling.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5162 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/boxing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6780 2023-06-28 14:13:46.000000 ocatari-0.1.1/ocatari/ram/breakout.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10878 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/carnival.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10550 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/centipede.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    28535 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/choppercommand.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5686 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/demonattack.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13378 2023-07-05 09:26:38.000000 ocatari-0.1.1/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2032 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4329 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/fishingderby.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3000 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/freeway.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11674 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/frostbite.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3991 2023-07-05 09:29:01.000000 ocatari-0.1.1/ocatari/ram/game_objects.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5970 2023-07-03 16:34:05.000000 ocatari-0.1.1/ocatari/ram/hero.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10155 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/kangaroo.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    47493 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6102 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/mspacman.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13675 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/pitfall.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5523 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/pong.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    17006 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/qbert.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10118 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/riverraid.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13070 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/roadrunner.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11341 2023-06-28 14:01:20.000000 ocatari-0.1.1/ocatari/ram/seaquest.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8679 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/skiing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11961 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8543 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/tennis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3124 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5020 2023-06-28 10:08:50.000000 ocatari-0.1.1/ocatari/utils.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.393053 ocatari-0.1.1/ocatari/vision/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      182 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2615 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/alien.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6175 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/assault.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8795 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/asterix.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2588 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/asteroids.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7361 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/atlantis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6024 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/beamrider.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2817 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/berzerk.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2486 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/bowling.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1788 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/boxing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2992 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/breakout.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5182 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/carnival.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4292 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/centipede.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5801 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/choppercommand.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2382 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/demonAttack.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4982 2023-06-28 13:51:23.000000 ocatari-0.1.1/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      580 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3509 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/fishingderby.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1579 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/freeway.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5612 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/frostbite.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2994 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/game_objects.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9157 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/hero.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5685 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/kangaroo.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6525 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2631 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/mspacman.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7227 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/pitfall.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2065 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/pong.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3978 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/qbert.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3867 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/riverraid.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8142 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/roadrunner.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4510 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/seaquest.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2143 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/skiing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2909 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2499 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/tennis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    20937 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/utils.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3766 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.381054 ocatari-0.1.1/ocatari.egg-info/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2404 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        1 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      156 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/requires.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       14 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       38 2023-07-05 09:43:42.397053 ocatari-0.1.1/setup.cfg
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      709 2023-07-05 09:43:37.000000 ocatari-0.1.1/setup.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.397053 ocatari-0.1.1/tests/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        0 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10202 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/get_metrics.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10382 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/metrics_utils.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1673 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/plot_speed_results.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1859 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_explanation.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2383 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_game.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4109 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_game_both.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1291 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_speed.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1790 2023-07-05 09:32:46.000000 ocatari-0.1.1/tests/test_velocity.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.831293 ocatari-0.1.2/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1171 2023-06-28 09:13:01.000000 ocatari-0.1.2/LICENSE
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 10:00:34.827293 ocatari-0.1.2/PKG-INFO
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5810 2023-07-04 07:44:43.000000 ocatari-0.1.2/README.md
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.799294 ocatari-0.1.2/ocatari/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       48 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12715 2023-06-28 14:12:36.000000 ocatari-0.1.2/ocatari/core.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2895 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/environments.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.811293 ocatari-0.1.2/ocatari/ram/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      232 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3214 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/_helper_methods.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3910 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/alien.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    14100 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/assault.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8663 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/asterix.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12123 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/asterix_new.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6852 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/asteroids.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13513 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/atlantis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3833 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/beamrider.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9499 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/berzerk.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5576 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/bowling.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5162 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/boxing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6780 2023-06-28 14:13:46.000000 ocatari-0.1.2/ocatari/ram/breakout.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10878 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/carnival.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10550 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/centipede.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    28535 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/choppercommand.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5686 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/demonattack.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13378 2023-07-05 09:26:38.000000 ocatari-0.1.2/ocatari/ram/extract_ram_info.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2032 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/extract_ram_info_short.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4329 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/fishingderby.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3000 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/freeway.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11674 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/frostbite.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3991 2023-07-05 09:29:01.000000 ocatari-0.1.2/ocatari/ram/game_objects.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5970 2023-07-03 16:34:05.000000 ocatari-0.1.2/ocatari/ram/hero.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10155 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/kangaroo.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    47493 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/montezumarevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6102 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/mspacman.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13675 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/pitfall.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5523 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/pong.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    17006 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/qbert.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10118 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/riverraid.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13070 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/roadrunner.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11341 2023-06-28 14:01:20.000000 ocatari-0.1.2/ocatari/ram/seaquest.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8679 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/skiing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11961 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/spaceinvaders.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8543 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/tennis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3124 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/ram/yarsrevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5020 2023-06-28 10:08:50.000000 ocatari-0.1.2/ocatari/utils.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.823294 ocatari-0.1.2/ocatari/vision/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      182 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2615 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/alien.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6175 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/assault.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8795 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/asterix.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2588 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/asteroids.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7361 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/atlantis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6024 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/beamrider.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2817 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/berzerk.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2486 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/bowling.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1788 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/boxing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2992 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/breakout.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5182 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/carnival.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4292 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/centipede.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5801 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/choppercommand.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2382 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/demonAttack.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4982 2023-06-28 13:51:23.000000 ocatari-0.1.2/ocatari/vision/extract_vision_info.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      580 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/extract_vision_info_short.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3509 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/fishingderby.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1579 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/freeway.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5612 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/frostbite.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2994 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/game_objects.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9157 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/hero.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5685 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/kangaroo.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6525 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/montezumarevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2631 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/mspacman.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7227 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/pitfall.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2065 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/pong.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3978 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/qbert.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3867 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/riverraid.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8142 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/roadrunner.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4510 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/seaquest.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2143 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/skiing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2909 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/spaceinvaders.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2499 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/tennis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    20937 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/utils.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3766 2023-06-28 09:13:01.000000 ocatari-0.1.2/ocatari/vision/yarsrevenge.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.799294 ocatari-0.1.2/ocatari.egg-info/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 10:00:34.000000 ocatari-0.1.2/ocatari.egg-info/PKG-INFO
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2404 2023-07-05 10:00:34.000000 ocatari-0.1.2/ocatari.egg-info/SOURCES.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        1 2023-07-05 10:00:34.000000 ocatari-0.1.2/ocatari.egg-info/dependency_links.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      106 2023-07-05 10:00:34.000000 ocatari-0.1.2/ocatari.egg-info/requires.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       14 2023-07-05 10:00:34.000000 ocatari-0.1.2/ocatari.egg-info/top_level.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       38 2023-07-05 10:00:34.831293 ocatari-0.1.2/setup.cfg
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      958 2023-07-05 10:00:30.000000 ocatari-0.1.2/setup.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 10:00:34.827293 ocatari-0.1.2/tests/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        0 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10202 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/get_metrics.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10382 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/metrics_utils.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1673 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/plot_speed_results.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1859 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/test_explanation.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2383 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/test_game.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4109 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/test_game_both.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1291 2023-06-28 09:13:01.000000 ocatari-0.1.2/tests/test_speed.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1790 2023-07-05 09:32:46.000000 ocatari-0.1.2/tests/test_velocity.py
```

### Comparing `ocatari-0.1.1/LICENSE` & `ocatari-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/PKG-INFO` & `ocatari-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 0.1.1
+Version: 0.1.2
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocatari-0.1.1/README.md` & `ocatari-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/core.py` & `ocatari-0.1.2/ocatari/core.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/environments.py` & `ocatari-0.1.2/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/_helper_methods.py` & `ocatari-0.1.2/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/alien.py` & `ocatari-0.1.2/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/assault.py` & `ocatari-0.1.2/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/asterix.py` & `ocatari-0.1.2/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/asterix_new.py` & `ocatari-0.1.2/ocatari/ram/asterix_new.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/asteroids.py` & `ocatari-0.1.2/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/atlantis.py` & `ocatari-0.1.2/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/beamrider.py` & `ocatari-0.1.2/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/berzerk.py` & `ocatari-0.1.2/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/bowling.py` & `ocatari-0.1.2/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/boxing.py` & `ocatari-0.1.2/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/breakout.py` & `ocatari-0.1.2/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/carnival.py` & `ocatari-0.1.2/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/centipede.py` & `ocatari-0.1.2/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/choppercommand.py` & `ocatari-0.1.2/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/demonattack.py` & `ocatari-0.1.2/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/extract_ram_info.py` & `ocatari-0.1.2/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/extract_ram_info_short.py` & `ocatari-0.1.2/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/fishingderby.py` & `ocatari-0.1.2/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/freeway.py` & `ocatari-0.1.2/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/frostbite.py` & `ocatari-0.1.2/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/game_objects.py` & `ocatari-0.1.2/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/hero.py` & `ocatari-0.1.2/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/kangaroo.py` & `ocatari-0.1.2/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/montezumarevenge.py` & `ocatari-0.1.2/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/mspacman.py` & `ocatari-0.1.2/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/pitfall.py` & `ocatari-0.1.2/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/pong.py` & `ocatari-0.1.2/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/qbert.py` & `ocatari-0.1.2/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/riverraid.py` & `ocatari-0.1.2/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/roadrunner.py` & `ocatari-0.1.2/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/seaquest.py` & `ocatari-0.1.2/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/skiing.py` & `ocatari-0.1.2/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/spaceinvaders.py` & `ocatari-0.1.2/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/tennis.py` & `ocatari-0.1.2/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/ram/yarsrevenge.py` & `ocatari-0.1.2/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/utils.py` & `ocatari-0.1.2/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/alien.py` & `ocatari-0.1.2/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/assault.py` & `ocatari-0.1.2/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/asterix.py` & `ocatari-0.1.2/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/asteroids.py` & `ocatari-0.1.2/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/atlantis.py` & `ocatari-0.1.2/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/beamrider.py` & `ocatari-0.1.2/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/berzerk.py` & `ocatari-0.1.2/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/bowling.py` & `ocatari-0.1.2/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/boxing.py` & `ocatari-0.1.2/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/breakout.py` & `ocatari-0.1.2/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/carnival.py` & `ocatari-0.1.2/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/centipede.py` & `ocatari-0.1.2/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/choppercommand.py` & `ocatari-0.1.2/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/demonAttack.py` & `ocatari-0.1.2/ocatari/vision/demonAttack.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/extract_vision_info.py` & `ocatari-0.1.2/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/extract_vision_info_short.py` & `ocatari-0.1.2/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/fishingderby.py` & `ocatari-0.1.2/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/freeway.py` & `ocatari-0.1.2/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/frostbite.py` & `ocatari-0.1.2/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/game_objects.py` & `ocatari-0.1.2/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/hero.py` & `ocatari-0.1.2/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/kangaroo.py` & `ocatari-0.1.2/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/montezumarevenge.py` & `ocatari-0.1.2/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/mspacman.py` & `ocatari-0.1.2/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/pitfall.py` & `ocatari-0.1.2/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/pong.py` & `ocatari-0.1.2/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/qbert.py` & `ocatari-0.1.2/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/riverraid.py` & `ocatari-0.1.2/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/roadrunner.py` & `ocatari-0.1.2/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/seaquest.py` & `ocatari-0.1.2/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/skiing.py` & `ocatari-0.1.2/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/spaceinvaders.py` & `ocatari-0.1.2/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/tennis.py` & `ocatari-0.1.2/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/utils.py` & `ocatari-0.1.2/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari/vision/yarsrevenge.py` & `ocatari-0.1.2/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/ocatari.egg-info/PKG-INFO` & `ocatari-0.1.2/ocatari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 0.1.1
+Version: 0.1.2
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocatari-0.1.1/ocatari.egg-info/SOURCES.txt` & `ocatari-0.1.2/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/get_metrics.py` & `ocatari-0.1.2/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/metrics_utils.py` & `ocatari-0.1.2/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/plot_speed_results.py` & `ocatari-0.1.2/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/test_explanation.py` & `ocatari-0.1.2/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/test_game.py` & `ocatari-0.1.2/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/test_game_both.py` & `ocatari-0.1.2/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/test_speed.py` & `ocatari-0.1.2/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.1/tests/test_velocity.py` & `ocatari-0.1.2/tests/test_velocity.py`

 * *Files identical despite different names*

