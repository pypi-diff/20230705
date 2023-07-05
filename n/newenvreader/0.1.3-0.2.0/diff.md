# Comparing `tmp/newenvreader-0.1.3.tar.gz` & `tmp/newenvreader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newenvreader-0.1.3.tar", max compression
+gzip compressed data, was "newenvreader-0.2.0.tar", max compression
```

## Comparing `newenvreader-0.1.3.tar` & `newenvreader-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-02 07:19:49.243406 newenvreader-0.1.3/LICENSE
--rw-r--r--   0        0        0      268 2023-07-03 13:13:58.225661 newenvreader-0.1.3/README.md
--rw-r--r--   0        0        0     3687 2023-07-04 07:52:23.395860 newenvreader-0.1.3/newenvreader.py
--rw-r--r--   0        0        0      278 2023-07-04 08:01:20.489058 newenvreader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 newenvreader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-05 11:20:04.659986 newenvreader-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3518 2023-07-05 11:20:04.659986 newenvreader-0.2.0/README.md
+-rw-r--r--   0        0        0     4842 2023-07-05 11:20:04.659986 newenvreader-0.2.0/newenvreader.py
+-rw-r--r--   0        0        0      278 2023-07-05 11:20:04.659986 newenvreader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 newenvreader-0.2.0/PKG-INFO
```

### Comparing `newenvreader-0.1.3/LICENSE` & `newenvreader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newenvreader-0.1.3/newenvreader.py` & `newenvreader-0.2.0/newenvreader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 """
 This module provides utility functions for reading environment variables.
 """
 
 import os
+from configparser import ConfigParser, MissingSectionHeaderError
 from typing import TypeVar, Optional
 
 T = TypeVar("T")
 
 
+def clean_env_var(value: str) -> str:
+    """Clean an environment variable value.
+
+    :param value: The value to clean.
+    :type value: str
+    :return: The cleaned value.
+    :rtype: str
+    """
+    if value.startswith(("'")) and value.endswith(("'")) and len(value) > 2:
+        return value[1:-1]
+    elif value.startswith(('"')) and value.endswith(('"')) and len(value) > 2:
+        return value[1:-1]
+    return value
+
+
 def parse_env_file(path: str) -> dict[str, str]:
     """Parse a .env file.
 
     :param path: Path to the .env file.
     :type path: str
     :return: A dictionary of environment variables.
     :rtype: dict
@@ -21,21 +37,38 @@
         for line in file:
             line = line.strip()
             if not line:
                 continue
 
             key, value = line.split("=", maxsplit=1)
             key = key.strip()
-            value = value.strip()
-            if value.startswith(("'")) and value.endswith(("'")) and len(value) > 2:
-                value = value[1:-1]
-            elif value.startswith(('"')) and value.endswith(('"')) and len(value) > 2:
-                value = value[1:-1]
-            env_file_val[key] = value
+            env_file_val[key] = clean_env_var(value.strip())
+
+    return env_file_val
 
+
+def parse_ini_file(path: str) -> dict[str, str]:
+    """Parse a .ini file.
+
+    :param path: Path to the .ini file.
+    :type path: str
+    :return: A dictionary of environment variables.
+    :rtype: dict
+    """
+    parser = ConfigParser()
+    parser.optionxform = lambda option: option
+    with open(path, "r", encoding="utf-8") as file:
+        try:
+            parser.read_file(file)
+        except MissingSectionHeaderError as err:
+            raise ValueError(
+                "Invalid .ini file: File contains no settings section"
+            ) from err
+        # get alls key values from section settings
+        env_file_val = dict(parser.items("settings"))
     return env_file_val
 
 
 def search_env_file(start_path: str) -> str:
     """Search for a .env file in the current directory and its parent directories.
 
     :param start_path: Start directory to search for the .env file.
@@ -45,15 +78,16 @@
     :rtype: str
 
     """
     current_dir = os.path.abspath(start_path)
 
     for root, _, files in os.walk(current_dir):
         for file in files:
-            if file.endswith(".env"):
+            # Check if it's file ending with .env or is settings.ini
+            if file.endswith(".env") or file == "settings.ini":
                 return os.path.join(root, file)
 
     parent_dir = os.path.dirname(current_dir)
     if parent_dir == current_dir:
         # Reached the root directory, file not found
         raise FileNotFoundError("No .env file found")
 
@@ -67,17 +101,17 @@
     :type value: str
     :return: The boolean value.
     :rtype: bool
     """
     if not isinstance(value, str):
         return bool(value)
 
-    if value.lower() in ("yes", "true", "t", "1", "on"):
+    if value.lower() in ("yes", "true", "t", "1", "on", "y"):
         return True
-    if value.lower() in ("no", "false", "f", "0", "off"):
+    if value.lower() in ("no", "false", "f", "0", "off", "n", ""):
         return False
 
     raise ValueError("Invalid boolean value")
 
 
 def load_env() -> dict[str, str]:
     """Load environment variables from the .env file or the system environment.
@@ -88,18 +122,20 @@
     """
     env = {}
     for key, value in os.environ.items():
         env[key] = value
 
     try:
         found_env_path = search_env_file(os.getcwd())
-        env.update(parse_env_file(found_env_path))
+        if found_env_path.endswith(".ini"):
+            env.update(parse_ini_file(found_env_path))
+        else:
+            env.update(parse_env_file(found_env_path))
     except FileNotFoundError:
         pass
-
     return env
 
 
 loaded_env = load_env()
 
 
 def get_env(key: str, cast: type[T] = str, default: Optional[T] = None) -> T:
```

