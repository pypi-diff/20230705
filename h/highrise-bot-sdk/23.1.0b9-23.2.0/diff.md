# Comparing `tmp/highrise_bot_sdk-23.1.0b9.tar.gz` & `tmp/highrise_bot_sdk-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.1.0b9.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.2.0.tar", max compression
```

## Comparing `highrise_bot_sdk-23.1.0b9.tar` & `highrise_bot_sdk-23.2.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     2898 2023-05-11 12:57:50.234072 highrise_bot_sdk-23.1.0b9/README.md
--rw-r--r--   0        0        0      992 2023-04-28 08:59:38.259801 highrise_bot_sdk-23.1.0b9/pyproject.toml
--rw-r--r--   0        0        0     8766 2023-05-11 11:53:57.781777 highrise_bot_sdk-23.1.0b9/src/highrise/__init__.py
--rw-r--r--   0        0        0     8652 2023-05-11 11:54:03.830476 highrise_bot_sdk-23.1.0b9/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b9/src/highrise/_unions.py
--rw-r--r--   0        0        0     8965 2023-05-11 11:54:03.830659 highrise_bot_sdk-23.1.0b9/src/highrise/models.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b9/src/highrise/py.typed
--rw-r--r--   0        0        0     3886 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b9/setup.py
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b9/PKG-INFO
+-rw-r--r--   0        0        0     8050 2023-07-05 14:35:02.697133 highrise_bot_sdk-23.2.0/README.md
+-rw-r--r--   0        0        0     1037 2023-07-05 13:51:49.568149 highrise_bot_sdk-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14031 2023-07-05 13:51:49.569748 highrise_bot_sdk-23.2.0/src/highrise/__init__.py
+-rw-r--r--   0        0        0    15583 2023-06-30 08:26:21.404700 highrise_bot_sdk-23.2.0/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.2.0/src/highrise/_unions.py
+-rw-r--r--   0        0        0    16035 2023-07-05 13:51:49.569715 highrise_bot_sdk-23.2.0/src/highrise/models.py
+-rw-r--r--   0        0        0      621 2023-06-30 16:42:03.849460 highrise_bot_sdk-23.2.0/src/highrise/models_control.py
+-rw-r--r--   0        0        0     3171 2023-07-04 12:50:01.833389 highrise_bot_sdk-23.2.0/src/highrise/models_webapi.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.2.0/src/highrise/py.typed
+-rw-r--r--   0        0        0     5431 2023-06-30 08:26:21.404899 highrise_bot_sdk-23.2.0/src/highrise/webapi.py
+-rw-r--r--   0        0        0     9149 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.2.0/setup.py
+-rw-r--r--   0        0        0     8755 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.2.0/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.1.0b9/pyproject.toml` & `highrise_bot_sdk-23.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.1.0.b9"
+version = "23.2.0"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">= 3.8.4"
 click = ">= 8.1.3"
-cattrs = "^22.2.0"
+cattrs = "22.2.0"
 quattro = "^22.1.0"
+pendulum = "^2.1.2"
+typing_extensions = "<4.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
-mypy = "^1.1.1"
+mypy = "<1.3.1"
 flake8 = "^6.0.0"
 types-setuptools = "^67.6.0.7"
 
 
 [tool.poetry.scripts]
 highrise = "highrise.__main__:run"
```

### Comparing `highrise_bot_sdk-23.1.0b9/src/highrise/_unions.py` & `highrise_bot_sdk-23.2.0/src/highrise/_unions.py`

 * *Files identical despite different names*

