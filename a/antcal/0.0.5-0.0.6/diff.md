# Comparing `tmp/antcal-0.0.5.tar.gz` & `tmp/antcal-0.0.6.tar.gz`

## Comparing `antcal-0.0.5.tar` & `antcal-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/design.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/model/__init__.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/model/dra.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/plot/__init__.py
--rw-r--r--   0        0        0   124523 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/plot/plot.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/sim/__init__.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 antcal-0.0.5/src/antcal/sim/hfss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.5/test/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 antcal-0.0.5/test/hfss.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 antcal-0.0.5/.gitignore
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 antcal-0.0.5/LICENSE
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 antcal-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 antcal-0.0.5/../README.md
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 antcal-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/design.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/application/__init__.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/application/hfss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/model/__init__.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/model/dra.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/plot/__init__.py
+-rw-r--r--   0        0        0   124523 2020-02-02 00:00:00.000000 antcal-0.0.6/src/antcal/plot/plot.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antcal-0.0.6/test/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 antcal-0.0.6/test/hfss.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 antcal-0.0.6/.gitignore
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 antcal-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 antcal-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 antcal-0.0.6/../README.md
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 antcal-0.0.6/PKG-INFO
```

### Comparing `antcal-0.0.5/src/antcal/utils.py` & `antcal-0.0.6/src/antcal/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Simple utilities.
 
 """
 
+
 from functools import wraps
 
 
 def add_to_class(cls: type):
     """A decorator that add the decorated function
     to a class as its attribute.
```

### Comparing `antcal-0.0.5/src/antcal/model/dra.py` & `antcal-0.0.6/src/antcal/model/dra.py`

 * *Files identical despite different names*

### Comparing `antcal-0.0.5/src/antcal/plot/plot.ipynb` & `antcal-0.0.6/src/antcal/plot/plot.ipynb`

 * *Files identical despite different names*

### Comparing `antcal-0.0.5/src/antcal/sim/hfss.py` & `antcal-0.0.6/src/antcal/application/hfss.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,110 @@
+"""A wrapper around {py:class}`pyaedt.hfss.Hfss`
+to manage the lifecycle of the AEDT application
+in a custom way.
+"""
+
 # %% Import
 from __future__ import annotations
 from enum import Enum
 from os import getcwd, mkdir, path
 from typing import cast
+from loguru import logger
+import pyaedt
 from pyaedt.application.Variables import VariableManager
+from pyaedt.desktop import Desktop
 from pyaedt.generic.general_methods import remove_project_lock
 from pyaedt.hfss import Hfss
 from pyaedt.modeler.modeler3d import Modeler3D
 from pyaedt.modules.AdvancedPostProcessing import PostProcessor
 from pyaedt.modules.MaterialLib import Materials
 
 
 # %% Class
 class SOLUTIONS:
-    """Provides the names of default solution types."""
+    """Provides the names of default solution types
+    as a enum. Created because
+    {py:class}`pyaedt.generic.constants.SOLUTIONS`
+    is not a enum."""
 
     class Hfss(Enum):
         """Provides HFSS solution types.
         Copied from PyAEDT definition.
         """
 
         DrivenModal = "Modal"
         DrivenTerminal = "Terminal"
         EigenMode = "Eigenmode"
         Transient = "Transient Network"
         SBR = "SBR+"
         Characteristic = "Characteristic"
 
 
+class AEDTDesktop:
+    """Represents a AEDT desktop session."""
+
+    def __init__(
+        self,
+        specified_version: str | None = None,
+        non_graphical: bool = True,
+        new_desktop_session: bool = True,
+        close_on_exit: bool = True,
+        student_version: bool = False,
+    ) -> None:
+        """Create a new AEDT desktop.
+
+        :param str | None specified_version: defaults to None
+        :param bool non_graphical: defaults to True
+        :param bool new_desktop_session: defaults to True
+        :param bool close_on_exit: defaults to True
+        :param bool student_version: defaults to False
+        """
+
+        logger.info("Initializing AEDT...")
+        self._desktop = Desktop(
+            specified_version=specified_version,
+            non_graphical=non_graphical,
+            new_desktop_session=new_desktop_session,
+            close_on_exit=close_on_exit,
+            student_version=student_version,
+        )
+        logger.info(f"AEDT initialized. ")
+
+    def __enter__(self) -> AEDTDesktop:
+        """
+        :return AEDTDesktop: The object itself.
+        """
+        return self
+    
+    def __exit__(self) -> None:
+        """Release AEDT."""
+        res = self.desktop.release_desktop()
+        if res:
+            logger.info("[antcal.application.]")
+    
+    def __del__(self) -> None:
+        """Destructor."""
+        self.__exit__()
+
+    @property
+    def desktop(self) -> Desktop:
+        """
+        :return Desktop: The AEDT application
+        """
+        return self._desktop
+
+    @property
+    def process_id(self) -> int:
+        """
+        :return int: AEDT process ID
+        """
+        # pyright: reportOptionalMemberAccess = false
+        return self.desktop.odesktop.GetProcessID()
+
+
 class HFSS:
     """Represents the Pyaedt HFSS application."""
 
     def __init__(
         self,
         non_graphical: bool,
         design_name: str,
@@ -143,12 +216,12 @@
         variable_manager = self.hfss.variable_manager
         if not variable_manager:
             raise AttributeError(variable_manager)
         return variable_manager
 
     def solve(self, setup_name: str) -> None:
         """Solve the current setup.
-        
+
         :param str setup_name: The name of the setup to solve."""
         self.hfss.save_project()
         assert self.hfss.validate_simple()
         self.hfss.analyze_setup(setup_name)
```

### Comparing `antcal-0.0.5/LICENSE` & `antcal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antcal-0.0.5/pyproject.toml` & `antcal-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,24 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Typing :: Typed",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Science/Research",
 ]
-dependencies = ["pyaedt", "plotly", "pandas", "numpy", "orjson"]
+dependencies = [
+    "pyaedt",
+    "plotly",
+    "pandas",
+    "numpy",
+    "loguru",
+    "rich",
+    "colorama",
+    "orjson",
+]
 
 [project.optional-dependencies]
 dev = ["hatch", "black", "ipython", "ipykernel"]
 docs = [
     "sphinx",
     "myst-parser",
     "sphinx-rtd-theme",
```

### Comparing `antcal-0.0.5/../README.md` & `antcal-0.0.6/../README.md`

 * *Files identical despite different names*

### Comparing `antcal-0.0.5/PKG-INFO` & `antcal-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antcal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Antenna calculator
 Project-URL: Homepage, https://github.com/atlanswer/AntCal
 Project-URL: Repository, https://github.com/atlanswer/AntCal.git
 Project-URL: Documentation, https://github.com/atlanswer/AntCal#readme
 Project-URL: Issues, https://github.com/atlanswer/AntCal/issue
 Author-email: Atlanswer <atlanswer@gmail.com>
 License: MIT License
@@ -39,19 +39,22 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
+Requires-Dist: colorama
+Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pyaedt
+Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
```

