# Comparing `tmp/antcal-0.0.6.tar.gz` & `tmp/antcal-0.0.8.tar.gz`

## Comparing `antcal-0.0.6.tar` & `antcal-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/design.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/utils.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/application/__init__.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/application/hfss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/model/__init__.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/model/dra.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/plot/__init__.py
--rw-r--r--   0        0        0   124523 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/plot/plot.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/test/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 antcal-0.0.6/test/hfss.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 antcal-0.0.6/.gitignore
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 antcal-0.0.6/LICENSE
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 antcal-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 antcal-0.0.6/../README.md
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 antcal-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/design.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/fitness.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/report.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/application/__init__.py
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/application/hfss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/model/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/model/dipole.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/model/dra.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/sim/__init__.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 antcal-0.0.8/src/antcal/sim/hfss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 antcal-0.0.8/test/hfss.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 antcal-0.0.8/.gitignore
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 antcal-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 antcal-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 antcal-0.0.8/../README.md
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 antcal-0.0.8/PKG-INFO
```

### Comparing `antcal-0.0.6/src/antcal/utils.py` & `antcal-0.0.8/src/antcal/utils.py`

 * *Files identical despite different names*

### Comparing `antcal-0.0.6/src/antcal/application/hfss.py` & `antcal-0.0.8/src/antcal/application/hfss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """A wrapper around {py:class}`pyaedt.hfss.Hfss`
 to manage the lifecycle of the AEDT application
 in a custom way.
 """
 
 # %% Import
 from __future__ import annotations
+
+from io import StringIO
+from contextlib import redirect_stdout
 from enum import Enum
-from os import getcwd, mkdir, path
+from pathlib import Path
 from typing import cast
-from loguru import logger
+
 import pyaedt
+from loguru import logger
 from pyaedt.application.Variables import VariableManager
 from pyaedt.desktop import Desktop
 from pyaedt.generic.general_methods import remove_project_lock
 from pyaedt.hfss import Hfss
 from pyaedt.modeler.modeler3d import Modeler3D
 from pyaedt.modules.AdvancedPostProcessing import PostProcessor
 from pyaedt.modules.MaterialLib import Materials
@@ -48,43 +52,49 @@
         non_graphical: bool = True,
         new_desktop_session: bool = True,
         close_on_exit: bool = True,
         student_version: bool = False,
     ) -> None:
         """Create a new AEDT desktop.
 
-        :param str | None specified_version: defaults to None
-        :param bool non_graphical: defaults to True
-        :param bool new_desktop_session: defaults to True
-        :param bool close_on_exit: defaults to True
-        :param bool student_version: defaults to False
+        :param str | None specified_version: _description_, defaults to None
+        :param bool non_graphical: _description_, defaults to True
+        :param bool new_desktop_session: _description_, defaults to True
+        :param bool close_on_exit: _description_, defaults to True
+        :param bool student_version: _description_, defaults to False
         """
-
         logger.info("Initializing AEDT...")
-        self._desktop = Desktop(
-            specified_version=specified_version,
-            non_graphical=non_graphical,
-            new_desktop_session=new_desktop_session,
-            close_on_exit=close_on_exit,
-            student_version=student_version,
-        )
+        with redirect_stdout(StringIO()) as f:
+            self._desktop = Desktop(
+                specified_version=specified_version,
+                non_graphical=non_graphical,
+                new_desktop_session=new_desktop_session,
+                close_on_exit=close_on_exit,
+                student_version=student_version,
+            )
+            self.desktop.enable_autosave()
+            self.desktop.change_license_type("Pack")
+        logger.info(f.getvalue())
         logger.info(f"AEDT initialized. ")
 
     def __enter__(self) -> AEDTDesktop:
         """
         :return AEDTDesktop: The object itself.
         """
         return self
-    
+
     def __exit__(self) -> None:
         """Release AEDT."""
+        logger.info("Releasing AEDT...")
         res = self.desktop.release_desktop()
         if res:
-            logger.info("[antcal.application.]")
-    
+            logger.info("AEDT released.")
+        else:
+            logger.error("Failed to release AEDT.")
+
     def __del__(self) -> None:
         """Destructor."""
         self.__exit__()
 
     @property
     def desktop(self) -> Desktop:
         """
@@ -102,69 +112,60 @@
 
 
 class HFSS:
     """Represents the Pyaedt HFSS application."""
 
     def __init__(
         self,
-        non_graphical: bool,
         design_name: str,
         solution_type: SOLUTIONS.Hfss,
         project_name: str = "project.aedt",
         project_dir: str = "projectfiles",
     ) -> None:
         """Initialize HFSS.
 
         :param bool non_graphical: Start without GUI or not.
         :param str design_name: Default design name.
         :param SOLUTIONS.Hfss solution_type: Solution type.
         :param str project_name: Project file name, defaults to "project.aedt"
         :param str project_dir: Project file path, defaults to "projectfiles"
         """
-        self._project_dir = path.join(getcwd(), project_dir)
-        if not path.exists(self._project_dir):
-            mkdir(self._project_dir)
-        self._project_path = path.join(self._project_dir, project_name)
-        remove_project_lock(self._project_path)
-        self._hfss = Hfss(
-            self._project_path,
-            design_name,
-            solution_type,
-            non_graphical=non_graphical,
-            close_on_exit=True,
-        )
-        self.hfss.autosave_enable()
-        self.hfss.change_material_override()
-        print("[antcal.design.HFSS] HFSS initialized.")
+        logger.info("Initializing HFSS...")
+        self._project_dir = Path.cwd() / project_dir
+        Path.mkdir(self._project_dir, exist_ok=True)
+        self._project_path = self._project_dir / project_name
+        remove_project_lock(str(self._project_path))
+        with redirect_stdout(StringIO()) as f:
+            self._hfss = Hfss(
+                str(self._project_path),
+                design_name,
+                solution_type,
+                new_desktop_session=False,
+                close_on_exit=True,
+            )
+            self.hfss.autosave_enable()
+            self.hfss.change_material_override()
+        logger.info(f.getvalue())
+        logger.info("HFSS initialized.")
 
     def __enter__(self) -> HFSS:
         """Return self in the context manager.
 
         :return HFSS: The object itself.
         """
         return self
 
     def __exit__(self) -> None:
         """Release HFSS when leaving the context manager."""
-        print("[antcal.design.HFSS] Releasing HFSS...")
-        res = self.release()
-        if res:
-            print("[antcal.design.HFSS] HFSS released successfully.")
-        else:
-            print("[antcal.design.HFSS] Failed releasing HFSS")
-        return None
+        ...
 
     def __del__(self) -> None:
         """Release HFSS when there's no more reference."""
         self.__exit__()
 
-    def release(self) -> bool:
-        """`release_desktop()` in PyAEDT."""
-        return self.hfss.release_desktop()
-
     @property
     def hfss(self) -> Hfss:
         """Return the HFSS application."""
         return self._hfss
 
     @property
     def name(self) -> str:
@@ -217,11 +218,13 @@
         if not variable_manager:
             raise AttributeError(variable_manager)
         return variable_manager
 
     def solve(self, setup_name: str) -> None:
         """Solve the current setup.
 
-        :param str setup_name: The name of the setup to solve."""
+        :param str setup_name: The name of the setup to solve.
+        :raise AssertionError: Validation failed.
+        """
         self.hfss.save_project()
         assert self.hfss.validate_simple()
         self.hfss.analyze_setup(setup_name)
```

### Comparing `antcal-0.0.6/LICENSE` & `antcal-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antcal-0.0.6/pyproject.toml` & `antcal-0.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,24 @@
     "Typing :: Typed",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
     "pyaedt",
-    "plotly",
     "pandas",
     "numpy",
     "loguru",
     "rich",
     "colorama",
     "orjson",
 ]
 
 [project.optional-dependencies]
-dev = ["hatch", "black", "ipython", "ipykernel"]
+dev = ["hatch", "conda-lock", "black", "ipython", "ipykernel"]
 docs = [
     "sphinx",
     "myst-parser",
     "sphinx-rtd-theme",
     "sphinx-autodoc2",
     "sphinx-copybutton",
     "sphinx-autobuild",
```

### Comparing `antcal-0.0.6/../README.md` & `antcal-0.0.8/../README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 ## Build
 
 ### Python package
 
 - Restore `conda` environment
   ```shell
-  conda-lock install --mamba -e dev -e vis -e docs -p ./python/venv -f ./python/conda-lock.yml
+  conda-lock install --mamba -E dev -E vis -E docs -p ./python/venv ./python/conda-lock.yml
   ```
 - Create lockfile
   ```shell
-  conda-lock --mamba -E dev -E vis -E docs -f ./python/pyproject.toml --lockfile ./python/conda-lock.yml
+  conda-lock --mamba -e dev -e vis -e docs -f ./python/pyproject.toml --lockfile ./python/conda-lock.yml
   ```
 - Build
   ```shell
   cd python
   hatch build
   ``` 
 - Publish
```

### Comparing `antcal-0.0.6/PKG-INFO` & `antcal-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antcal
-Version: 0.0.6
+Version: 0.0.8
 Summary: Antenna calculator
 Project-URL: Homepage, https://github.com/atlanswer/AntCal
 Project-URL: Repository, https://github.com/atlanswer/AntCal.git
 Project-URL: Documentation, https://github.com/atlanswer/AntCal#readme
 Project-URL: Issues, https://github.com/atlanswer/AntCal/issue
 Author-email: Atlanswer <atlanswer@gmail.com>
 License: MIT License
@@ -44,19 +44,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: colorama
 Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: pandas
-Requires-Dist: plotly
 Requires-Dist: pyaedt
 Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
+Requires-Dist: conda-lock; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
@@ -92,19 +92,19 @@
 
 ## Build
 
 ### Python package
 
 - Restore `conda` environment
   ```shell
-  conda-lock install --mamba -e dev -e vis -e docs -p ./python/venv -f ./python/conda-lock.yml
+  conda-lock install --mamba -E dev -E vis -E docs -p ./python/venv ./python/conda-lock.yml
   ```
 - Create lockfile
   ```shell
-  conda-lock --mamba -E dev -E vis -E docs -f ./python/pyproject.toml --lockfile ./python/conda-lock.yml
+  conda-lock --mamba -e dev -e vis -e docs -f ./python/pyproject.toml --lockfile ./python/conda-lock.yml
   ```
 - Build
   ```shell
   cd python
   hatch build
   ``` 
 - Publish
```

