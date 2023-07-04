# Comparing `tmp/home_assistant_streamdeck_yaml-2023.7.1.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.1.tar", last modified: Mon Jul  3 23:06:01 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.2.tar", last modified: Tue Jul  4 23:34:55 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.7.1.tar` & `home_assistant_streamdeck_yaml-2023.7.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.438255 home_assistant_streamdeck_yaml-2023.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.438255 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 23:06:01.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    59997 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:06:01.442255 home_assistant_streamdeck_yaml-2023.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-03 23:05:43.000000 home_assistant_streamdeck_yaml-2023.7.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.086859 home_assistant_streamdeck_yaml-2023.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.086859 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.086859 home_assistant_streamdeck_yaml-2023.7.2/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 23:34:55.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60076 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:34:55.090859 home_assistant_streamdeck_yaml-2023.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-04 23:34:37.000000 home_assistant_streamdeck_yaml-2023.7.2/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.github/release.py` & `home_assistant_streamdeck_yaml-2023.7.2/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.7.2/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.gitignore` & `home_assistant_streamdeck_yaml-2023.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.7.2/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: "https://github.com/ambv/black"
     rev: 23.3.0
     hooks:
       - id: black-jupyter
         language_version: python3
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.276"
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.3.0"
+    rev: "v1.4.1"
     hooks:
       - id: mypy
         additional_dependencies: ["types-PyYAML", "types-requests", "types-setuptools"]
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/Dockerfile` & `home_assistant_streamdeck_yaml-2023.7.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/LICENSE` & `home_assistant_streamdeck_yaml-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
@@ -299,15 +299,15 @@
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 | Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
 |:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
 | `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
 | `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
 | `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
 | `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
 | `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/README.md` & `home_assistant_streamdeck_yaml-2023.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 | Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
 |:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
 | `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
 | `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
 | `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
 | `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
 | `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.7.2/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.7.2/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/configuration.yaml` & `home_assistant_streamdeck_yaml-2023.7.2/configuration.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/docker-compose.yaml` & `home_assistant_streamdeck_yaml-2023.7.2/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
@@ -299,15 +299,15 @@
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 | Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
 |:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
 | `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
 | `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
 | `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
 | `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
 | `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
 | `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.7.2/home_assistant_streamdeck_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 class Button(BaseModel, extra="forbid"):  # type: ignore[call-arg]
     """Button configuration."""
 
     entity_id: str | None = Field(
         default=None,
         allow_template=True,
         description="The `entity_id` that this button controls."
-        " This entitity will be passed to the `service` when the button is pressed.",
+        " This entitity will be passed to the `service` when the button is pressed."
+        " The button is re-rendered whenever the state of this entity changes.",
     )
     service: str | None = Field(
         default=None,
         allow_template=True,
         description="The `service` that will be called when the button is pressed.",
     )
     service_data: dict[str, Any] | None = Field(
@@ -917,15 +918,15 @@
                 await websocket.send(json.dumps(auth_payload))
 
                 # Wait for the authentication response
                 auth_response = await websocket.recv()
                 console.log(auth_response)
                 console.log("Connected to Home Assistant")
                 yield websocket
-        except ConnectionResetError:
+        except ConnectionResetError:  # noqa: PERF203
             # Connection was reset, retrying in 3 seconds
             console.print_exception(show_locals=True)
             console.log("Connection was reset, retrying in 3 seconds")
             await asyncio.sleep(5)
 
 
 async def subscribe_state_changes(
@@ -1692,16 +1693,15 @@
         return Image.open(filename)
     image_content = _download(url)
     image = Image.open(io.BytesIO(image_content))
     if image.mode != "RGB":
         image = image.convert("RGB")
     if filename is not None:
         image.save(filename)
-    image = image.resize(size)
-    return image
+    return image.resize(size)
 
 
 def update_all_key_images(
     deck: StreamDeck,
     config: Config,
     complete_state: StateDict,
 ) -> None:
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "D402",    # First line should not be the function's signature
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
     "SLF001",  # Private member accessed
     "PLR0913", # Too many arguments to function call (N > 5)
     "TD002",   # Missing author in TODO; try: `# TODO(<author_name>): ...`
     "TD003",   # Missing issue link on the line following this TODO
+    "FIX002",  # Line contains TODO
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["SLF001"]
 "tests/test_examples.py" = ["E501"]
 ".github/*" = ["INP001"]
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.7.2/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/tests/state.json` & `home_assistant_streamdeck_yaml-2023.7.2/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.7.2/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,17 +249,17 @@
 
 
 def test_buttons(buttons: list[Button], state: dict[str, dict[str, Any]]) -> None:
     """Test buttons."""
     page = Page(name="Home", buttons=buttons)
     config = Config(pages=[page])
     first_page = config.to_page(0)
-    rendered_buttons = []
-    for button in first_page.buttons:
-        rendered_buttons.append(button.rendered_template_button(state))
+    rendered_buttons = [
+        button.rendered_template_button(state) for button in first_page.buttons
+    ]
 
     b = rendered_buttons[0]  # LIGHT
     assert b.domain == "light"
     icon = b.render_icon(state)
     assert isinstance(icon, Image.Image)
 
     b = rendered_buttons[1]  # VOLUME_DOWN
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.1/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.7.2/tests/test_examples.py`

 * *Files identical despite different names*

