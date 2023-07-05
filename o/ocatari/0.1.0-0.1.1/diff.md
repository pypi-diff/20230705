# Comparing `tmp/ocatari-0.1.0.tar.gz` & `tmp/ocatari-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-0.1.0.tar", last modified: Tue Jul  4 07:56:55 2023, max compression
+gzip compressed data, was "ocatari-0.1.1.tar", last modified: Wed Jul  5 09:43:42 2023, max compression
```

## Comparing `ocatari-0.1.0.tar` & `ocatari-0.1.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.720723 ocatari-0.1.0/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1171 2023-06-28 09:13:01.000000 ocatari-0.1.0/LICENSE
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-04 07:56:55.720723 ocatari-0.1.0/PKG-INFO
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5810 2023-07-04 07:44:43.000000 ocatari-0.1.0/README.md
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.704714 ocatari-0.1.0/ocatari/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       48 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12715 2023-06-28 14:12:36.000000 ocatari-0.1.0/ocatari/core.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2895 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/environments.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.712719 ocatari-0.1.0/ocatari/ram/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      232 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3214 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3910 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/alien.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    14100 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/assault.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8663 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/asterix.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12123 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/asterix_new.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6852 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/asteroids.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13513 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/atlantis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3833 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/beamrider.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9499 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/berzerk.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5576 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/bowling.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5162 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/boxing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6780 2023-06-28 14:13:46.000000 ocatari-0.1.0/ocatari/ram/breakout.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10878 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/carnival.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10550 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/centipede.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    28535 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/choppercommand.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5686 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/demonattack.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13324 2023-06-28 13:49:33.000000 ocatari-0.1.0/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2032 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4329 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/fishingderby.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3000 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/freeway.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11674 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/frostbite.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3967 2023-06-29 14:37:11.000000 ocatari-0.1.0/ocatari/ram/game_objects.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5970 2023-07-03 16:34:05.000000 ocatari-0.1.0/ocatari/ram/hero.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10155 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/kangaroo.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    47493 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6102 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/mspacman.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13675 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/pitfall.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5523 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/pong.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    17006 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/qbert.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10118 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/riverraid.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13070 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/roadrunner.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11341 2023-06-28 14:01:20.000000 ocatari-0.1.0/ocatari/ram/seaquest.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8679 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/skiing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11961 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8543 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/tennis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3124 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5020 2023-06-28 10:08:50.000000 ocatari-0.1.0/ocatari/utils.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.716721 ocatari-0.1.0/ocatari/vision/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      182 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2615 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/alien.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6175 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/assault.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8795 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/asterix.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2588 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/asteroids.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7361 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/atlantis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6024 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/beamrider.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2817 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/berzerk.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2486 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/bowling.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1788 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/boxing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2992 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/breakout.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5182 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/carnival.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4292 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/centipede.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5801 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/choppercommand.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2382 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/demonAttack.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4982 2023-06-28 13:51:23.000000 ocatari-0.1.0/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      580 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3509 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/fishingderby.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1579 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/freeway.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5612 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/frostbite.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2994 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/game_objects.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9157 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/hero.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5685 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/kangaroo.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6525 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2631 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/mspacman.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7227 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/pitfall.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2065 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/pong.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3978 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/qbert.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3867 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/riverraid.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8142 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/roadrunner.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4510 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/seaquest.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2143 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/skiing.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2909 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2499 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/tennis.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    20937 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/utils.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3766 2023-06-28 09:13:01.000000 ocatari-0.1.0/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.708716 ocatari-0.1.0/ocatari.egg-info/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-04 07:56:55.000000 ocatari-0.1.0/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2404 2023-07-04 07:56:55.000000 ocatari-0.1.0/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        1 2023-07-04 07:56:55.000000 ocatari-0.1.0/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      156 2023-07-04 07:56:55.000000 ocatari-0.1.0/ocatari.egg-info/requires.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       14 2023-07-04 07:56:55.000000 ocatari-0.1.0/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       38 2023-07-04 07:56:55.720723 ocatari-0.1.0/setup.cfg
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      709 2023-07-04 07:50:49.000000 ocatari-0.1.0/setup.py
-drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-04 07:56:55.720723 ocatari-0.1.0/tests/
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        0 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/__init__.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10202 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/get_metrics.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10382 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/metrics_utils.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1673 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/plot_speed_results.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1859 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/test_explanation.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2383 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/test_game.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4109 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/test_game_both.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1291 2023-06-28 09:13:01.000000 ocatari-0.1.0/tests/test_speed.py
--rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1787 2023-06-29 14:47:14.000000 ocatari-0.1.0/tests/test_velocity.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.397053 ocatari-0.1.1/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1171 2023-06-28 09:13:01.000000 ocatari-0.1.1/LICENSE
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 09:43:42.397053 ocatari-0.1.1/PKG-INFO
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5810 2023-07-04 07:44:43.000000 ocatari-0.1.1/README.md
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.381054 ocatari-0.1.1/ocatari/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       48 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12715 2023-06-28 14:12:36.000000 ocatari-0.1.1/ocatari/core.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2895 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/environments.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.389054 ocatari-0.1.1/ocatari/ram/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      232 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3214 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/_helper_methods.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3910 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/alien.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    14100 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/assault.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8663 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asterix.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    12123 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asterix_new.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6852 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/asteroids.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13513 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/atlantis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3833 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/beamrider.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9499 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/berzerk.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5576 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/bowling.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5162 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/boxing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6780 2023-06-28 14:13:46.000000 ocatari-0.1.1/ocatari/ram/breakout.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10878 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/carnival.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10550 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/centipede.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    28535 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/choppercommand.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5686 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/demonattack.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13378 2023-07-05 09:26:38.000000 ocatari-0.1.1/ocatari/ram/extract_ram_info.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2032 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/extract_ram_info_short.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4329 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/fishingderby.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3000 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/freeway.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11674 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/frostbite.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3991 2023-07-05 09:29:01.000000 ocatari-0.1.1/ocatari/ram/game_objects.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5970 2023-07-03 16:34:05.000000 ocatari-0.1.1/ocatari/ram/hero.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10155 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/kangaroo.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    47493 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/montezumarevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6102 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/mspacman.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13675 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/pitfall.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5523 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/pong.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    17006 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/qbert.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10118 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/riverraid.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    13070 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/roadrunner.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11341 2023-06-28 14:01:20.000000 ocatari-0.1.1/ocatari/ram/seaquest.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8679 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/skiing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    11961 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/spaceinvaders.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8543 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/tennis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3124 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/ram/yarsrevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5020 2023-06-28 10:08:50.000000 ocatari-0.1.1/ocatari/utils.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.393053 ocatari-0.1.1/ocatari/vision/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      182 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2615 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/alien.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6175 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/assault.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8795 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/asterix.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2588 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/asteroids.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7361 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/atlantis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6024 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/beamrider.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2817 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/berzerk.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2486 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/bowling.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1788 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/boxing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2992 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/breakout.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5182 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/carnival.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4292 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/centipede.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5801 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/choppercommand.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2382 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/demonAttack.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4982 2023-06-28 13:51:23.000000 ocatari-0.1.1/ocatari/vision/extract_vision_info.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      580 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/extract_vision_info_short.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3509 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/fishingderby.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1579 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/freeway.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5612 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/frostbite.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2994 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/game_objects.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     9157 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/hero.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     5685 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/kangaroo.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6525 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/montezumarevenge.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2631 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/mspacman.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     7227 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/pitfall.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2065 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/pong.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3978 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/qbert.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3867 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/riverraid.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     8142 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/roadrunner.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4510 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/seaquest.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2143 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/skiing.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2909 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/spaceinvaders.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2499 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/tennis.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    20937 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/utils.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     3766 2023-06-28 09:13:01.000000 ocatari-0.1.1/ocatari/vision/yarsrevenge.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.381054 ocatari-0.1.1/ocatari.egg-info/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     6079 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/PKG-INFO
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2404 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/SOURCES.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        1 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/dependency_links.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      156 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/requires.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       14 2023-07-05 09:43:42.000000 ocatari-0.1.1/ocatari.egg-info/top_level.txt
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)       38 2023-07-05 09:43:42.397053 ocatari-0.1.1/setup.cfg
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)      709 2023-07-05 09:43:37.000000 ocatari-0.1.1/setup.py
+drwxrwxr-x   0 k4ntz     (1000) k4ntz     (1000)        0 2023-07-05 09:43:42.397053 ocatari-0.1.1/tests/
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)        0 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/__init__.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10202 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/get_metrics.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)    10382 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/metrics_utils.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1673 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/plot_speed_results.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1859 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_explanation.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     2383 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_game.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     4109 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_game_both.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1291 2023-06-28 09:13:01.000000 ocatari-0.1.1/tests/test_speed.py
+-rw-rw-r--   0 k4ntz     (1000) k4ntz     (1000)     1790 2023-07-05 09:32:46.000000 ocatari-0.1.1/tests/test_velocity.py
```

### Comparing `ocatari-0.1.0/LICENSE` & `ocatari-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/PKG-INFO` & `ocatari-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 0.1.0
+Version: 0.1.1
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocatari-0.1.0/README.md` & `ocatari-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/core.py` & `ocatari-0.1.1/ocatari/core.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/environments.py` & `ocatari-0.1.1/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/_helper_methods.py` & `ocatari-0.1.1/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/alien.py` & `ocatari-0.1.1/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/assault.py` & `ocatari-0.1.1/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/asterix.py` & `ocatari-0.1.1/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/asterix_new.py` & `ocatari-0.1.1/ocatari/ram/asterix_new.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/asteroids.py` & `ocatari-0.1.1/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/atlantis.py` & `ocatari-0.1.1/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/beamrider.py` & `ocatari-0.1.1/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/berzerk.py` & `ocatari-0.1.1/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/bowling.py` & `ocatari-0.1.1/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/boxing.py` & `ocatari-0.1.1/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/breakout.py` & `ocatari-0.1.1/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/carnival.py` & `ocatari-0.1.1/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/centipede.py` & `ocatari-0.1.1/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/choppercommand.py` & `ocatari-0.1.1/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/demonattack.py` & `ocatari-0.1.1/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/extract_ram_info.py` & `ocatari-0.1.1/ocatari/ram/extract_ram_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         exit(1)
 
 
 def detect_objects_revised(objects, ram_state, game_name, hud):
     """
     Augment the info dictionary with object centric information
     """
-    GameObject._save_prev()
+    for obj in objects: # saving the previsous positions
+        obj._save_prev()
     if game_name.lower() == "boxing":
         _detect_objects_boxing_revised(objects, ram_state, hud)
     elif game_name.lower() == "breakout":
         _detect_objects_breakout_revised(objects, ram_state, hud)
     elif game_name.lower() == "freeway":
         _detect_objects_freeway_revised(objects, ram_state, hud)
     elif game_name.lower() == "pong":
```

### Comparing `ocatari-0.1.0/ocatari/ram/extract_ram_info_short.py` & `ocatari-0.1.1/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/fishingderby.py` & `ocatari-0.1.1/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/freeway.py` & `ocatari-0.1.1/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/frostbite.py` & `ocatari-0.1.1/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/game_objects.py` & `ocatari-0.1.1/ocatari/ram/game_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     :ivar x: The x positional coordinate on the image (on the horizontal axis).
     :type x: int
     :ivar y: The y positional coordinate on the image (on the vertical axis).
     :type y: int
     """
     GET_COLOR = False
     GET_WH = False
-    _xy = None
 
     def __init__(self):
         self.rgb = (0, 0, 0)
         self._xy = (0, 0)
         self.wh = (0, 0)
         self._prev_xy = None
         self._orientation = 0
@@ -58,76 +57,81 @@
         """
         return self.wh[1]
     
     @h.setter
     def h(self, h):
         self.wh = self.w, h
 
+
+    @property
+    def prev_xy(self):
+        if self._prev_xy:
+            return self._prev_xy
+        else:
+            return self._xy
+
+    @prev_xy.setter
+    def prev_xy(self, newval):
+        self._prev_xy = newval
+
     @property
     def xy(self):
         """
         Both (x, y) positional coordinates in a tuple. 
 
         :type: (int, int)
         """
         return self._xy
 
     @xy.setter
     def xy(self, xy):
-        # self._prev_xy = self._xy
         self._xy = xy
 
     # returns 2 lists with current and past coords
     @property
     def h_coords(self):
         """
         History of coordinates, i.e. current (x, y) and previous (x, y) position.
 
         :type: [(int, int), (int, int)]
         """
-        return [self._xy, self._prev_xy]
+        return [self._xy, self.prev_xy]
 
     @property
     def dx(self):
         """
         The pixel movement correponding to: current_x - previous_x.
 
         :type: int
         """
-        if self._prev_xy:
-            return self._xy[0] - self._prev_xy[0]
-        else:
-            return 0
+        return self._xy[0] - self.prev_xy[0]
+
 
     @property
     def dy(self):
         """
         The pixel movement correponding to: current_y - previous_y.
 
         :type: int
         """
-        if self._prev_xy:
-            return self._xy[1] - self._prev_xy[1]
-        else:
-            return 0
+        return self._xy[1] - self.prev_xy[1]
+
 
     @property
     def xywh(self):
         """
         The (x, y, w, h) positional and width coordinates.
 
         :type: (int, int, int, int)
         """
         return self._xy[0], self._xy[1], self.wh[0], self.wh[1]
 
-    @classmethod
     def _save_prev(self):
         self._prev_xy = self._xy
 
-
     # @x.setter
     # def x(self, x):
 
     #     self._xy = x, self.xy[1]
     
     # @y.setter
     # def y(self, y):
```

### Comparing `ocatari-0.1.0/ocatari/ram/hero.py` & `ocatari-0.1.1/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/kangaroo.py` & `ocatari-0.1.1/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/montezumarevenge.py` & `ocatari-0.1.1/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/mspacman.py` & `ocatari-0.1.1/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/pitfall.py` & `ocatari-0.1.1/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/pong.py` & `ocatari-0.1.1/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/qbert.py` & `ocatari-0.1.1/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/riverraid.py` & `ocatari-0.1.1/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/roadrunner.py` & `ocatari-0.1.1/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/seaquest.py` & `ocatari-0.1.1/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/skiing.py` & `ocatari-0.1.1/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/spaceinvaders.py` & `ocatari-0.1.1/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/tennis.py` & `ocatari-0.1.1/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/ram/yarsrevenge.py` & `ocatari-0.1.1/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/utils.py` & `ocatari-0.1.1/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/alien.py` & `ocatari-0.1.1/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/assault.py` & `ocatari-0.1.1/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/asterix.py` & `ocatari-0.1.1/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/asteroids.py` & `ocatari-0.1.1/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/atlantis.py` & `ocatari-0.1.1/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/beamrider.py` & `ocatari-0.1.1/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/berzerk.py` & `ocatari-0.1.1/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/bowling.py` & `ocatari-0.1.1/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/boxing.py` & `ocatari-0.1.1/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/breakout.py` & `ocatari-0.1.1/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/carnival.py` & `ocatari-0.1.1/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/centipede.py` & `ocatari-0.1.1/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/choppercommand.py` & `ocatari-0.1.1/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/demonAttack.py` & `ocatari-0.1.1/ocatari/vision/demonAttack.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/extract_vision_info.py` & `ocatari-0.1.1/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/extract_vision_info_short.py` & `ocatari-0.1.1/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/fishingderby.py` & `ocatari-0.1.1/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/freeway.py` & `ocatari-0.1.1/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/frostbite.py` & `ocatari-0.1.1/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/game_objects.py` & `ocatari-0.1.1/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/hero.py` & `ocatari-0.1.1/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/kangaroo.py` & `ocatari-0.1.1/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/montezumarevenge.py` & `ocatari-0.1.1/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/mspacman.py` & `ocatari-0.1.1/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/pitfall.py` & `ocatari-0.1.1/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/pong.py` & `ocatari-0.1.1/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/qbert.py` & `ocatari-0.1.1/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/riverraid.py` & `ocatari-0.1.1/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/roadrunner.py` & `ocatari-0.1.1/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/seaquest.py` & `ocatari-0.1.1/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/skiing.py` & `ocatari-0.1.1/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/spaceinvaders.py` & `ocatari-0.1.1/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/tennis.py` & `ocatari-0.1.1/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/utils.py` & `ocatari-0.1.1/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari/vision/yarsrevenge.py` & `ocatari-0.1.1/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/ocatari.egg-info/PKG-INFO` & `ocatari-0.1.1/ocatari.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 0.1.0
+Version: 0.1.1
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ocatari-0.1.0/ocatari.egg-info/SOURCES.txt` & `ocatari-0.1.1/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/setup.py` & `ocatari-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 
 setup(
     name='ocatari',
-    version='0.1.0',
+    version='0.1.1',
     author='Quentin Delfosse',
     author_email='quentin.delfosse@cs.tu-darmstadt.de',
     packages=find_packages(),
     # package_data={'': extra_files},
     include_package_data=True,
     # package_dir={'':'src'},
     url='https://github.com/k4ntz/OC_Atari',
```

### Comparing `ocatari-0.1.0/tests/get_metrics.py` & `ocatari-0.1.1/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/metrics_utils.py` & `ocatari-0.1.1/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/plot_speed_results.py` & `ocatari-0.1.1/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/test_explanation.py` & `ocatari-0.1.1/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/test_game.py` & `ocatari-0.1.1/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/test_game_both.py` & `ocatari-0.1.1/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/test_speed.py` & `ocatari-0.1.1/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `ocatari-0.1.0/tests/test_velocity.py` & `ocatari-0.1.1/tests/test_velocity.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 
 # import faulthandler
 
 
 # faulthandler.enable()
 
-env_name = "ALE/Seaquest-v5"
+env_name = "PongNoFrameskip-v4"
 
 env = OCAtari(env_name, mode='revised', hud=False, render_mode="rgb_array", frameskip=1)
 env.reset()
 
 transition = 0
 episode = 0
```

