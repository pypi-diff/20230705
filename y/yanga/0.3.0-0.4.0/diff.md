# Comparing `tmp/yanga-0.3.0.tar.gz` & `tmp/yanga-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.3.0.tar", max compression
+gzip compressed data, was "yanga-0.4.0.tar", max compression
```

## Comparing `yanga-0.3.0.tar` & `yanga-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1066 2023-07-03 20:04:56.271476 yanga-0.3.0/LICENSE
--rw-r--r--   0        0        0     4695 2023-07-03 20:04:56.271476 yanga-0.3.0/README.md
--rw-r--r--   0        0        0     2384 2023-07-03 20:04:57.119473 yanga-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-03 20:04:57.087473 yanga-0.3.0/src/yanga/__init__.py
--rw-r--r--   0        0        0      347 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/_yrun.py
--rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1803 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/build.py
--rw-r--r--   0        0        0     2494 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/init.py
--rw-r--r--   0        0        0      412 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/cookiecutter.json
--rw-r--r--   0        0        0        7 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
--rw-r--r--   0        0        0     5389 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
--rw-r--r--   0        0        0     3853 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
--rw-r--r--   0        0        0      785 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
--rw-r--r--   0        0        0      157 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
--rw-r--r--   0        0        0       34 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
--rw-r--r--   0        0        0      247 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
--rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0      278 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/exceptions.py
--rw-r--r--   0        0        0     1583 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/logging.py
--rw-r--r--   0        0        0     6113 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/scoop_wrapper.py
--rw-r--r--   0        0        0     1350 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/subprocess.py
--rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/__init__.py
--rw-r--r--   0        0        0      852 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/build_main.py
--rw-r--r--   0        0        0      965 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/config.py
--rw-r--r--   0        0        0      477 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/environment.py
--rw-r--r--   0        0        0     3141 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/pipeline.py
--rw-r--r--   0        0        0      864 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/project.py
--rw-r--r--   0        0        0     1403 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/stages.py
--rw-r--r--   0        0        0      886 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/variant.py
--rw-r--r--   0        0        0      791 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ymain.py
--rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-05 16:20:02.106532 yanga-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-05 16:20:02.106532 yanga-0.4.0/README.md
+-rw-r--r--   0        0        0     2384 2023-07-05 16:20:02.906541 yanga-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-05 16:20:02.874541 yanga-0.4.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2500 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0     1364 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/install.py
+-rw-r--r--   0        0        0      412 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0        7 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5389 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1
+-rw-r--r--   0        0        0     3853 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0      157 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
+-rw-r--r--   0        0        0       34 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/logging.py
+-rw-r--r--   0        0        0     6618 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1343 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     3141 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0     1403 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0     1098 2023-07-05 16:20:02.110532 yanga-0.4.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.4.0/PKG-INFO
```

### Comparing `yanga-0.3.0/LICENSE` & `yanga-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/README.md` & `yanga-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/pyproject.toml` & `yanga-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.3.0"
+version = "0.4.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
```

### Comparing `yanga-0.3.0/src/yanga/commands/build.py` & `yanga-0.4.0/src/yanga/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class BuildCommand(Command):
     def __init__(self) -> None:
         super().__init__("build", "Build a yanga project")
         self.logger = logger.bind()
 
-    @time_it()
+    @time_it("Build")
     def run(self, args: Namespace) -> int:
         self.logger.info(f"Running {self.name} with args {args}")
         config = BuildCommandConfig.from_namespace(args)
         # search variant
         # create project build artifacts locator
         environment = BuildEnvironment(
             config.variant_name,
```

### Comparing `yanga-0.3.0/src/yanga/commands/init.py` & `yanga-0.4.0/src/yanga/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 class InitCommand(Command):
     def __init__(self) -> None:
         super().__init__("init", "Init a yanga project")
         self.logger = logger.bind()
 
-    @time_it()
+    @time_it("Init")
     def run(self, args: Namespace) -> int:
         self.logger.info(f"Running {self.name} with args {args}")
         YangaInit(InitCommandConfig.from_namespace(args)).run()
         return 0
 
     def _register_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
```

### Comparing `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1` & `yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py` & `yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1` & `yanga-0.4.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/core/cmd_line.py` & `yanga-0.4.0/src/yanga/core/cmd_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,24 +60,27 @@
             self.logger.error(f"Command {args[0]} not registered")
             return 1
 
 
 class CommandLineHandlerBuilder:
     """Builds a command line handler."""
 
-    def __init__(self) -> None:
+    def __init__(self, parser: ArgumentParser) -> None:
         self.commands: Dict[str, Command] = {}
-        self.parser = ArgumentParser(
-            prog="yanga", description="Yanga CLI", exit_on_error=False
-        )
+        self.parser = parser
         self.subparsers = self.parser.add_subparsers(title="Commands", dest="command")
 
     def create(self) -> CommandLineHandler:
         return CommandLineHandler(self.commands, self.parser)
 
+    def add_commands(self, commands: List[Command]) -> "CommandLineHandlerBuilder":
+        for command in commands:
+            self.add_command(command)
+        return self
+
     @fulfills("REQ-CMDLINE_REGISTER_COMMANDS-0.0.1", "REQ-CMDLINE_DUPLICATION-0.0.1")
     def add_command(self, command: Command) -> "CommandLineHandlerBuilder":
         """Add a command to the command line handler."""
         if self.commands.get(command.name, None) is not None:
             raise ValueError(f"Command {command.name} already exists")
         self.commands[command.name] = command
         command.register_parser(self.subparsers)
```

### Comparing `yanga-0.3.0/src/yanga/core/docs_utils.py` & `yanga-0.4.0/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/core/logging.py` & `yanga-0.4.0/src/yanga/core/logging.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/core/scoop_wrapper.py` & `yanga-0.4.0/src/yanga/core/scoop_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
+import re
 from dataclasses import dataclass, field
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, List, Optional, Union
 
 from mashumaro import DataClassDictMixin
 from mashumaro.mixins.json import DataClassJSONMixin
 
 from .exceptions import UserNotificationException
 from .logging import logger
-from .subprocess import SubprocessExecutor, get_app_path  # nosec
+from .subprocess import SubprocessExecutor, which  # nosec
 
 
 @dataclass
 class ScoopFileElement(DataClassDictMixin):
     name: str = field(metadata={"alias": "Name"})
     source: str = field(metadata={"alias": "Source"})
 
@@ -54,38 +55,46 @@
     path: Path
     manifest_file: Path
     bin_dirs: List[Path]
 
 
 class ScoopWrapper:
     def __init__(self) -> None:
-        self.scoop_path = self.get_scoop_path()
+        self.scoop_executable = self._find_scoop_executable()
+        self.scoop_root_dir = self._find_scoop_root_dir(self.scoop_executable)
         self.logger = logger.bind()
 
     @property
-    def scoop_executable(self) -> Path:
-        return self.scoop_path.joinpath("scoop")
-
-    @property
     def apps_directory(self) -> Path:
-        return self.scoop_path.joinpath("apps")
+        return self.scoop_root_dir.joinpath("apps")
 
     def install(self, scoop_file: Path) -> List[ScoopFileElement]:
         return self.do_install(
             ScoopInstallConfigFile.from_file(scoop_file), self.get_installed_apps()
         )
 
-    def get_scoop_path(self) -> Path:
-        scoop_path = get_app_path("scoop")
+    def _find_scoop_executable(self) -> Path:
+        scoop_path = which("scoop")
         if not scoop_path:
             raise UserNotificationException(
                 "Scoop not found in PATH. Please run the build script again."
             )
         return scoop_path
 
+    def _find_scoop_root_dir(self, scoop_executable_path: Path) -> Path:
+        pattern = r"^(.*?/scoop/)"
+        match = re.match(pattern, scoop_executable_path.absolute().as_posix())
+
+        if match:
+            return Path(match.group(1))
+        else:
+            raise UserNotificationException(
+                f"Could not determine scoop directory for {scoop_executable_path}."
+            )
+
     def parse_bin_dirs(
         self, bin_data: Union[str, List[Union[str, List[str]]]]
     ) -> List[Path]:
         """Parse the bin directory from the manifest file."""
 
         def get_parent_dir(bin_entry: Union[str, List[str]]) -> Optional[Path]:
             bin_path = (
@@ -101,14 +110,15 @@
                 for parent in [get_parent_dir(bin_entry) for bin_entry in bin_data]
                 if parent
             ]
         return []
 
     def get_installed_apps(self) -> List[InstalledScoopApp]:
         installed_tools: List[InstalledScoopApp] = []
+        self.logger.info(f"Looking for installed apps in {self.apps_directory}")
         for manifest_file in self.apps_directory.glob("**/manifest.json"):
             app_directory: Path = manifest_file.parent
             # There is a directory level for the version of the tool
             tool_name: str = app_directory.parent.name
             with open(manifest_file) as f:
                 manifest_data: Dict[str, Any] = json.load(f)
                 tool_version: str = manifest_data.get("version", None)
@@ -123,39 +133,39 @@
                     )
                 )
         return installed_tools
 
     def do_install(
         self,
         scoop_install_config: ScoopInstallConfigFile,
-        installed_tools: List[InstalledScoopApp],
+        installed_apps: List[InstalledScoopApp],
     ) -> List[ScoopFileElement]:
         """Check which apps are installed and install the missing ones."""
         apps_to_install = self.get_tools_to_be_installed(
-            scoop_install_config, installed_tools
+            scoop_install_config, installed_apps
         )
         if not apps_to_install:
             self.logger.info("All Scoop apps already installed. Skip installation.")
             return []
-        installed_apps = set(scoop_install_config.apps) - set(apps_to_install)
+        already_installed_apps = set(scoop_install_config.apps) - set(apps_to_install)
         self.logger.info(
-            f"Scoop apps already installed: {','.join(str(app) for app in installed_apps)}"
+            f"Scoop apps already installed: {','.join(str(app) for app in already_installed_apps)}"
         )
         self.logger.info(
             f"Scoop apps to install: {','.join(str(app) for app in apps_to_install)}"
         )
 
         # Create a temporary scoopfile with the remaining apps to install and install them
         with TemporaryDirectory() as tmp_dir:
             tmp_scoop_file = Path(tmp_dir).joinpath("scoopfile.json")
             ScoopInstallConfigFile(
                 scoop_install_config.buckets, apps_to_install
             ).to_file(tmp_scoop_file)
             SubprocessExecutor(
-                [self.scoop_executable, "install", tmp_scoop_file]
+                [self.scoop_executable, "import", tmp_scoop_file]
             ).execute()
         return apps_to_install
 
     @staticmethod
     def get_tools_to_be_installed(
         scoop_install_config: ScoopInstallConfigFile,
         installed_tools: List[InstalledScoopApp],
```

### Comparing `yanga-0.3.0/src/yanga/core/subprocess.py` & `yanga-0.4.0/src/yanga/core/subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 from .exceptions import UserNotificationException
 from .logging import logger
 
 
-def get_app_path(app_name: str) -> Optional[Path]:
+def which(app_name: str) -> Optional[Path]:
     """Return the path to the app if it is in the PATH, otherwise return None."""
     app_path = shutil.which(app_name)
     return Path(app_path) if app_path else None
 
 
 class SubprocessExecutor:
     def __init__(self, command: List[str | Path], cwd: Optional[Path] = None):
```

### Comparing `yanga-0.3.0/src/yanga/ybuild/build_main.py` & `yanga-0.4.0/src/yanga/ybuild/build_main.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/ybuild/config.py` & `yanga-0.4.0/src/yanga/ybuild/config.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/ybuild/pipeline.py` & `yanga-0.4.0/src/yanga/ybuild/pipeline.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/ybuild/project.py` & `yanga-0.4.0/src/yanga/ybuild/project.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/ybuild/stages.py` & `yanga-0.4.0/src/yanga/ybuild/stages.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/src/yanga/ybuild/variant.py` & `yanga-0.4.0/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.3.0/PKG-INFO` & `yanga-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.3.0
+Version: 0.4.0
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yanga Version: 0.3.0 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.4.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

