# Comparing `tmp/syncshell-1.0.6.tar.gz` & `tmp/syncshell-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncshell-1.0.6.tar", max compression
+gzip compressed data, was "syncshell-1.0.7.tar", max compression
```

## Comparing `syncshell-1.0.6.tar` & `syncshell-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     3702 2023-04-22 13:57:36.633541 syncshell-1.0.6/README.md
--rw-r--r--   0        0        0      746 2023-06-04 21:42:58.091907 syncshell-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-18 15:23:24.855682 syncshell-1.0.6/syncshell/__init__.py
--rw-r--r--   0        0        0      184 2023-04-20 23:42:21.663528 syncshell-1.0.6/syncshell/__main__.py
--rw-r--r--   0        0        0     7316 2023-06-04 21:32:02.267513 syncshell-1.0.6/syncshell/cli.py
--rw-r--r--   0        0        0     2268 2023-06-04 21:32:02.269075 syncshell-1.0.6/syncshell/config.py
--rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.6/syncshell/utils/__init__.py
--rw-r--r--   0        0        0      964 2022-07-27 08:15:14.248748 syncshell-1.0.6/syncshell/utils/constants.py
--rw-r--r--   0        0        0      567 2022-06-23 08:51:02.382500 syncshell-1.0.6/syncshell/utils/spinner.py
--rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 syncshell-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     3702 2023-04-22 13:57:36.633541 syncshell-1.0.7/README.md
+-rw-r--r--   0        0        0     1406 2023-07-05 20:42:23.497807 syncshell-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 23:49:18.310340 syncshell-1.0.7/syncshell/__init__.py
+-rw-r--r--   0        0        0     6652 2023-07-05 20:42:23.498652 syncshell-1.0.7/syncshell/cli.py
+-rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.7/syncshell/utils/__init__.py
+-rw-r--r--   0        0        0     4097 2023-07-05 20:42:23.499263 syncshell-1.0.7/syncshell/utils/config.py
+-rw-r--r--   0        0        0      967 2023-07-05 20:42:23.500231 syncshell-1.0.7/syncshell/utils/constants.py
+-rw-r--r--   0        0        0      567 2022-06-23 08:51:02.382500 syncshell-1.0.7/syncshell/utils/spinner.py
+-rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 syncshell-1.0.7/PKG-INFO
```

### Comparing `syncshell-1.0.6/LICENSE.txt` & `syncshell-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.6/README.md` & `syncshell-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.6/syncshell/cli.py` & `syncshell-1.0.7/syncshell/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import sys
-import os
 import textwrap
 import time
 from configparser import ConfigParser
 from subprocess import run, PIPE
 from github import Github, InputFileContent, UnknownObjectException
 from syncshell.utils import constants, spinner as Spinner
-from syncshell.config import SyncShellConfig
+from syncshell.utils.config import SyncShellConfig
+from fire import Fire
 
 # Configuration
 config = SyncShellConfig()
-config.read()
+config.read_config()
 
 
-def prepare_payload():
-    """Prepare history and config file for upload"""
-
-    files = {}
-    config_path = constants.CONFIG_PATH
-
-    with open(constants.SHELL_HISTORY_PATH, "r") as history_file:
-        history_file_path = os.path.basename(history_file.name)
-        try:
-            content = history_file.read()
-            files[history_file_path] = InputFileContent(content)
-        except UnicodeDecodeError:
-            with open(
-                constants.SHELL_HISTORY_PATH, "r", encoding="latin-1"
-            ) as history_file_latin_1:
-                content = history_file_latin_1.read()
-                files[history_file_path] = InputFileContent(content)
-
-    with open(config_path, mode="r") as config_file:
-        # Remove token key on uplaod
-        lines = config_file.readlines()
-        lines.pop(1)
-
-        files[os.path.basename(config_file.name)] = InputFileContent(
-            "".join(map(str, lines))
-        )
+class Application:
+    """SyncShell CLI Application"""
 
-    return files
+    def __prepare_payload(self):
+        """Prepare history and config file for upload"""
 
+        files = {}
+        history_file = config.get_shell_history()
+        config_file = config.get_config()
 
-class Application:
-    """SyncShell CLI Application"""
+        files[history_file["path"]] = InputFileContent(history_file["content"])
+        files[config_file["path"]] = InputFileContent(config_file["content"])
 
-    def __init__(self):
-        pass
+        return files
 
     def auth(self):
         """Retrieve & authenticate user token"""
         try:
             # Help message
             getting_started = textwrap.fill(constants.HELP_MESSAGE, width=80)
             print(getting_started)
@@ -91,33 +70,33 @@
             if config.parser["Auth"]["gist_id"]:
                 gist = config.gist.get_gist(config.parser["Auth"]["gist_id"])
 
                 # Set upload date
                 config.parser["Upload"]["last_date"] = str(int(time.time()))
                 config.write()
 
-                files = prepare_payload()
+                files = self.__prepare_payload()
 
                 gist.edit(files=files)
 
                 spinner.succeed(f"Gist ID ({gist.id}) updated.")
             else:
                 description = "SyncShell Gist"
 
                 user = config.gist.get_user()
-                files = prepare_payload()
+                files = self.__prepare_payload()
                 gist = user.create_gist(False, files, description)
 
                 # Set upload date
                 config.parser["Upload"]["last_date"] = str(int(time.time()))
                 config.parser["Auth"]["gist_id"] = gist.id
 
                 config.write()
 
-                files = prepare_payload()
+                files = self.__prepare_payload()
                 gist.edit(files=files)
                 spinner.succeed(f"New Gist ID ({gist.id}) created.")
         except FileNotFoundError:
             spinner.fail("Couldn't find history file.")
             sys.exit(1)
         except KeyError:
             spinner.fail("Request's data is not valid")
@@ -167,55 +146,59 @@
                 sys.exit(1)
 
             # Write configuration
             config.parser["Auth"]["token"] = token
             config.parser["Auth"]["gist_id"] = gist_id
             config.write()
 
-            with open(constants.SHELL_HISTORY_PATH, "r+") as history_file:
-                history = history_file.read()
+            history_file = config.get_shell_history()
+            history_content = history_file["content"]
 
-                new_changes = gist.files[
-                    constants.SUPPORTED_SHELLS[config.parser["Shell"]["name"]]
-                ]
-
-                synced_changes = new_changes.content + history
-
-                awk_proc = run(
-                    [
-                        "awk",
-                        '"/:[0-9]/ { if(s) { print s } s=$0 } !/:[0-9]/ { s=s"\n"$0 } END { print s }"',
-                    ],
-                    stdout=PIPE,
-                    input=bytes(synced_changes, encoding="utf8"),
-                    check=True,
-                )
-
-                # Remove duplicate lines
-                awk_duplicates_proc = run(
-                    [
-                        "awk",
-                        '"!visited[$0]++ { print $0 }"',
-                    ],
-                    stdout=PIPE,
-                    input=bytes(awk_proc.stdout.decode("utf-8"), encoding="utf8"),
-                    check=True,
-                )
+            new_changes = gist.files[
+                constants.SUPPORTED_SHELLS[config.parser["Shell"]["name"]]
+            ]
+
+            synced_changes = new_changes.content + history_content
+
+            awk_proc = run(
+                [
+                    "awk",
+                    '"/:[0-9]/ { if(s) { print s } s=$0 } !/:[0-9]/ { s=s"\n"$0 } END { print s }"',
+                ],
+                stdout=PIPE,
+                input=bytes(synced_changes, encoding="utf8"),
+                check=True,
+            )
+
+            # Remove duplicate lines
+            awk_duplicates_proc = run(
+                [
+                    "awk",
+                    '"!visited[$0]++ { print $0 }"',
+                ],
+                stdout=PIPE,
+                input=bytes(awk_proc.stdout.decode("utf-8"), encoding="utf8"),
+                check=True,
+            )
+
+            sort_proc = run(
+                ["sort", "-u"],
+                stdout=PIPE,
+                input=bytes(
+                    awk_duplicates_proc.stdout.decode("utf-8"), encoding="utf8"
+                ),
+                check=True,
+            )
 
-                sort_proc = run(
-                    ["sort", "-u"],
-                    stdout=PIPE,
-                    input=bytes(
-                        awk_duplicates_proc.stdout.decode("utf-8"), encoding="utf8"
-                    ),
-                    check=True,
-                )
-
-                history_file.write(sort_proc.stdout.decode("utf-8"))
-                spinner.succeed("Gist downloaded and stored.")
+            config.write_shell_history(sort_proc.stdout.decode("utf-8"))
+            spinner.succeed("Gist downloaded and stored.")
         except KeyboardInterrupt:
             sys.exit(0)
         except FileNotFoundError:
             spinner.fail("Couldn't find history file.")
             sys.exit(1)
         except OSError:
             sys.exit(1)
+
+
+def main():
+    Fire(Application)
```

### Comparing `syncshell-1.0.6/syncshell/utils/constants.py` & `syncshell-1.0.7/syncshell/utils/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
-from pathlib import Path
 
 # Metainfo
 APP_NAME = "syncshell"
 
 # Paths
 APP_ROOT_DIR = os.path.abspath(
     os.path.join(os.path.dirname(os.path.abspath(__file__)), os.pardir, os.pardir)
 )
 CONFIG_FILENAME = ".syncshell.ini"
 CONFIG_PATH_TEMPLATE = os.path.join(APP_ROOT_DIR, CONFIG_FILENAME)
 CONFIG_PATH = os.path.join(os.path.expanduser("~"), CONFIG_FILENAME)
+USER_HOME = os.path.expanduser("~")
 
 # String Colors
 DEFAULT = "\033[39m"
 WHITE = "\033[97m"
 
 # String Attr
 NORMAL = "\033[0m"
@@ -25,14 +25,14 @@
 
 # History
 SUPPORTED_SHELLS = {
     "bash": ".bash_history",
     "zsh": ".zsh_history",
 }
 SHELL = os.path.basename(os.environ.get("SHELL", "bash"))
-SHELL_HISTORY_PATH = str(Path.joinpath(Path.home(), SUPPORTED_SHELLS[SHELL]))
+SHELL_HISTORY_PATH = os.path.join(USER_HOME, SUPPORTED_SHELLS[SHELL])
 HELP_MESSAGE = (
     "If you don't have Github token key, "
     "Please, first go to "
     f"{WHITE}{BOLD}https://github.com/settings/tokens{NORMAL} "
     "address create a personal access token with gist scope."
 )
```

### Comparing `syncshell-1.0.6/syncshell/utils/spinner.py` & `syncshell-1.0.7/syncshell/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.6/PKG-INFO` & `syncshell-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: syncshell
-Version: 1.0.6
-Summary: Keep your machine's shell history synchronized.
+Version: 1.0.7
+Summary: Keep your machine's shell history synchronized
 Home-page: https://github.com/msudgh/syncshell
 License: MIT
 Keywords: sync,shell,history,bash,zsh
 Author: Masoud Ghorbani
-Author-email: msud.ghorbani@gmail.com
+Author-email: masoudghorbani@pm.me
 Requires-Python: >=3.8.16,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyGithub (==1.55)
-Requires-Dist: black (==22.3.0)
-Requires-Dist: fire (==0.1.3)
-Requires-Dist: flake8 (==6.0.0)
-Requires-Dist: halo (==0.0.12)
-Requires-Dist: pytest (==7.3.1)
-Requires-Dist: pytest-testdox (>=3.0.1,<4.0.0)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Utilities
+Requires-Dist: PyGithub (==1.59.0)
+Requires-Dist: fire (==0.5.0)
+Requires-Dist: halo (==0.0.31)
 Project-URL: Repository, https://github.com/msudgh/syncshell
 Description-Content-Type: text/markdown
 
 # SyncShell
 <!-- License -->
 <a href="https://mit-license.org/msudgh">
   <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1 Name: syncshell Version: 1.0.6 Summary: Keep your
-machine's shell history synchronized. Home-page: https://github.com/msudgh/
+Metadata-Version: 2.1 Name: syncshell Version: 1.0.7 Summary: Keep your
+machine's shell history synchronized Home-page: https://github.com/msudgh/
 syncshell License: MIT Keywords: sync,shell,history,bash,zsh Author: Masoud
-Ghorbani Author-email: msud.ghorbani@gmail.com Requires-Python: >=3.8.16,<4.0.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: PyGithub (==1.55) Requires-Dist:
-black (==22.3.0) Requires-Dist: fire (==0.1.3) Requires-Dist: flake8 (==6.0.0)
-Requires-Dist: halo (==0.0.12) Requires-Dist: pytest (==7.3.1) Requires-Dist:
-pytest-testdox (>=3.0.1,<4.0.0) Project-URL: Repository, https://github.com/
-msudgh/syncshell Description-Content-Type: text/markdown # SyncShell  [MIT
-License]  [Build_Status]  [PyPi]  [PyPi] SyncShell as a simple and secure tool
-allows to synchronize machine's shell history across devices. It's built on top
-of Github Gist and written in Python (CLI). With SyncShell, you no longer have
-to worry about manually syncing your office and home machine's shell history
-and let continue where the terminal session left. ## Features - Sync your shell
-history across all your devices - Securely store your shell history on Github
-Gist - Support for `zsh` and `bash` shells - Easy to install and use ##
-Installation To install SyncShell, simply run the following command: ```bash $
-pip install syncshell ``` ## Usage To use SyncShell, It first needs to set up a
-Github token key by following these steps: 1. Open [**Github personal access
-tokens**](https://github.com/settings/tokens) page, [**Generate a new token**]
-(https://github.com/settings/tokens/new) with `gist` scope feature. 2. Execute
-the **`syncshell auth`** command, Enter the token key to validate and confirm
-it. Once finished, try to upload shell history by the following command:
-```bash $ syncshell upload ``` After uploading, the download command lets to
-sync and pull changes on the other machines: ```bash $ syncshell download ```
-### Synopsis ```bash $ syncshell Type: Application String form:
+Ghorbani Author-email: masoudghorbani@pm.me Requires-Python: >=3.8.16,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Topic :: Software Development Classifier: Topic :: System :: Shells Classifier:
+Topic :: Utilities Requires-Dist: PyGithub (==1.59.0) Requires-Dist: fire
+(==0.5.0) Requires-Dist: halo (==0.0.31) Project-URL: Repository, https://
+github.com/msudgh/syncshell Description-Content-Type: text/markdown # SyncShell
+[MIT_License]  [Build_Status]  [PyPi]  [PyPi] SyncShell as a simple and secure
+tool allows to synchronize machine's shell history across devices. It's built
+on top of Github Gist and written in Python (CLI). With SyncShell, you no
+longer have to worry about manually syncing your office and home machine's
+shell history and let continue where the terminal session left. ## Features -
+Sync your shell history across all your devices - Securely store your shell
+history on Github Gist - Support for `zsh` and `bash` shells - Easy to install
+and use ## Installation To install SyncShell, simply run the following command:
+```bash $ pip install syncshell ``` ## Usage To use SyncShell, It first needs
+to set up a Github token key by following these steps: 1. Open [**Github
+personal access tokens**](https://github.com/settings/tokens) page, [**Generate
+a new token**](https://github.com/settings/tokens/new) with `gist` scope
+feature. 2. Execute the **`syncshell auth`** command, Enter the token key to
+validate and confirm it. Once finished, try to upload shell history by the
+following command: ```bash $ syncshell upload ``` After uploading, the download
+command lets to sync and pull changes on the other machines: ```bash $
+syncshell download ``` ### Synopsis ```bash $ syncshell Type: Application
+String form:
 cli.Application object at 0x101b1ff10> Docstring: SyncShell CLI Application
 Usage: syncshell syncshell auth syncshell download syncshell upload ``` ## How
 it Works SyncShell is a tool that synchronizes shell history across all devices
 by securely storing the history file on Github Gist. Github Gist provides two
 types of Gists, `public` and `secret`. When the `syncshell upload` command is
 executed, the shell history file is uploaded and stored securely on Github Gist
 as a secret Gist. To download the uploaded shell history on other devices, the
```

