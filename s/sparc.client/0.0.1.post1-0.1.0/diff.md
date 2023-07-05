# Comparing `tmp/sparc.client-0.0.1.post1.tar.gz` & `tmp/sparc.client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparc.client-0.0.1.post1.tar", last modified: Tue Jan 31 16:19:46 2023, max compression
+gzip compressed data, was "sparc.client-0.1.0.tar", last modified: Wed Jul  5 13:32:13 2023, max compression
```

## Comparing `sparc.client-0.0.1.post1.tar` & `sparc.client-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16816 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2574 2023-01-31 16:19:06.000000 sparc.client-0.0.1.post1/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1851 2023-01-31 16:19:06.000000 sparc.client-0.0.1.post1/pyproject.toml
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/setup.cfg
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/sparc.client.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16816 2023-01-31 16:19:46.000000 sparc.client-0.0.1.post1/sparc.client.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      404 2023-01-31 16:19:46.000000 sparc.client-0.0.1.post1/sparc.client.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-01-31 16:19:46.000000 sparc.client-0.0.1.post1/sparc.client.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       66 2023-01-31 16:19:46.000000 sparc.client-0.0.1.post1/sparc.client.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        6 2023-01-31 16:19:46.000000 sparc.client-0.0.1.post1/sparc.client.egg-info/top_level.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/src/sparc/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      169 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/src/sparc/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/src/sparc/client/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      179 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/src/sparc/client/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3944 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/src/sparc/client/client.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-01-31 16:19:46.195881 sparc.client-0.0.1.post1/src/sparc/client/services/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      839 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/src/sparc/client/services/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1579 2023-01-30 22:46:37.000000 sparc.client-0.0.1.post1/src/sparc/client/services/_default.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12298 2023-01-31 16:19:06.000000 sparc.client-0.0.1.post1/src/sparc/client/services/pennsieve.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.906762 sparc.client-0.1.0/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-02-28 19:41:18.000000 sparc.client-0.1.0/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    17862 2023-07-05 13:32:13.906762 sparc.client-0.1.0/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3626 2023-07-05 13:27:55.000000 sparc.client-0.1.0/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1880 2023-03-06 17:50:20.000000 sparc.client-0.1.0/pyproject.toml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-07-05 13:32:13.906762 sparc.client-0.1.0/setup.cfg
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.902763 sparc.client-0.1.0/sparc.client.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    17862 2023-07-05 13:32:13.000000 sparc.client-0.1.0/sparc.client.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      477 2023-07-05 13:32:13.000000 sparc.client-0.1.0/sparc.client.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-07-05 13:32:13.000000 sparc.client-0.1.0/sparc.client.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       84 2023-07-05 13:32:13.000000 sparc.client-0.1.0/sparc.client.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        6 2023-07-05 13:32:13.000000 sparc.client-0.1.0/sparc.client.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.898763 sparc.client-0.1.0/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.902763 sparc.client-0.1.0/src/sparc/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      132 2023-07-05 13:27:51.000000 sparc.client-0.1.0/src/sparc/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.902763 sparc.client-0.1.0/src/sparc/client/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      223 2023-04-20 16:13:15.000000 sparc.client-0.1.0/src/sparc/client/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4523 2023-04-20 16:13:15.000000 sparc.client-0.1.0/src/sparc/client/client.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.902763 sparc.client-0.1.0/src/sparc/client/services/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      839 2023-02-28 19:41:18.000000 sparc.client-0.1.0/src/sparc/client/services/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1703 2023-02-28 19:41:18.000000 sparc.client-0.1.0/src/sparc/client/services/_default.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12873 2023-07-05 13:27:55.000000 sparc.client-0.1.0/src/sparc/client/services/pennsieve.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 13:32:13.902763 sparc.client-0.1.0/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2151 2023-02-28 19:41:18.000000 sparc.client-0.1.0/tests/test_client.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7670 2023-07-05 13:27:55.000000 sparc.client-0.1.0/tests/test_pennsieve.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1658 2023-03-07 20:51:59.000000 sparc.client-0.1.0/tests/test_pennsieve_api.py
```

### Comparing `sparc.client-0.0.1.post1/LICENSE` & `sparc.client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparc.client-0.0.1.post1/PKG-INFO` & `sparc.client-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparc.client
-Version: 0.0.1.post1
+Version: 0.1.0
 Summary: NIH SPARC Python Client
 Author-email: Patryk Orzechowski <patryk@upenn.edu>
 Maintainer-email: Patryk Orzechowski <patryk@upenn.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -276,20 +276,44 @@
 Each python file in services/ folder with defined class name that is derived from BaseService is imported as a module to SparcClient class.
 For example, pennsieve.py file 
 
 ```python
 from sparc.client import SparcClient
 a = SparcClient(connect=False, config_file='config.ini')
 module = a.pennsieve.connect()
-module.user.whoami() #execute internal functions of the module
+module.info() #execute internal functions of the module
 
 # alternatively connect all the services available
 a.connect()  #connect to all services
 
 ```
 
+## Test generation - PyTest
+
+Some good resource for implementing tests could be found at [Medium](https://medium.com/analytics-vidhya/pytest-mocking-cheatsheet-dcebd84876e3).
+
+## Documentation - Sphinx tutorial
+
+A fresh start for creating documentation with Sphinx could be found at [towardsdatascience](https://towardsdatascience.com/documenting-python-code-with-sphinx-554e1d6c4f6d).
+To reproduce steps:
+
+1. Create a docs folder
+2. Run `sphinx-quickstart` in docs folder, fill the required prompts.
+3. Edit `conf.py` and `index.rst` files to adjust them to your needs
+4. Run in docs folder sphinx-apidoc -o . ../src
+5. Disregard `modules.rst` and `sphinx.rst`, attach `sphinx.client` to toctree in `index.rst`
+6. Run `make html` in docs folder.
+
 # Contribution Guide
 
 1. Define configuration variables in config.ini file (e.g  api_key, api_secret etc.)
 2. Create a file in services/
 3. Create a class within this file that extends BaseService
 4. The class needs to define all the functions required + may add its own.
+
+# Developer Setup
+
+Run `pip install -e '.[test]'` to install the dependencies needed for a development environment.
+
+Run `pytest --cov=./src` to run the tests and get a test coverage summary.
+
+Run `pytest --cov-report html --cov=./src` to run the tests and get a full HTML coverage report output to `htmlcov`.
```

### Comparing `sparc.client-0.0.1.post1/pyproject.toml` & `sparc.client-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sparc.client"
-version = "0.0.1.post1"
+version = "0.1.0"
 description = "NIH SPARC Python Client"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["data science", "datasets"]
 authors = [
   {name = "Patryk Orzechowski", email = "patryk@upenn.edu"}
@@ -23,23 +23,26 @@
   "Topic :: Scientific/Engineering :: Bio-Informatics",
   "Topic :: Scientific/Engineering :: Information Analysis",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-  "pennsieve2",
+  "pennsieve2 >= 0.1.2",
 ]
 
 
 [project.optional-dependencies]
 test = [
-  "pennsieve2 >=1.1.0",
-  "pytest < 5.0.0",
-  "pytest-cov[all]"
+  "pytest ~= 7.2",
+  "pytest-cov",
+  "pytest-mock",
+  "flake8",
+  "black",
+  "responses",
 ]
 
 
 [project.urls]
 homepage = "https://sparc.science"
 documentation = "https://github.com/nih-sparc/sparc.client/README.md"
 repository = "https://github.com/nih-sparc/sparc.client"
```

### Comparing `sparc.client-0.0.1.post1/sparc.client.egg-info/PKG-INFO` & `sparc.client-0.1.0/sparc.client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparc.client
-Version: 0.0.1.post1
+Version: 0.1.0
 Summary: NIH SPARC Python Client
 Author-email: Patryk Orzechowski <patryk@upenn.edu>
 Maintainer-email: Patryk Orzechowski <patryk@upenn.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -276,20 +276,44 @@
 Each python file in services/ folder with defined class name that is derived from BaseService is imported as a module to SparcClient class.
 For example, pennsieve.py file 
 
 ```python
 from sparc.client import SparcClient
 a = SparcClient(connect=False, config_file='config.ini')
 module = a.pennsieve.connect()
-module.user.whoami() #execute internal functions of the module
+module.info() #execute internal functions of the module
 
 # alternatively connect all the services available
 a.connect()  #connect to all services
 
 ```
 
+## Test generation - PyTest
+
+Some good resource for implementing tests could be found at [Medium](https://medium.com/analytics-vidhya/pytest-mocking-cheatsheet-dcebd84876e3).
+
+## Documentation - Sphinx tutorial
+
+A fresh start for creating documentation with Sphinx could be found at [towardsdatascience](https://towardsdatascience.com/documenting-python-code-with-sphinx-554e1d6c4f6d).
+To reproduce steps:
+
+1. Create a docs folder
+2. Run `sphinx-quickstart` in docs folder, fill the required prompts.
+3. Edit `conf.py` and `index.rst` files to adjust them to your needs
+4. Run in docs folder sphinx-apidoc -o . ../src
+5. Disregard `modules.rst` and `sphinx.rst`, attach `sphinx.client` to toctree in `index.rst`
+6. Run `make html` in docs folder.
+
 # Contribution Guide
 
 1. Define configuration variables in config.ini file (e.g  api_key, api_secret etc.)
 2. Create a file in services/
 3. Create a class within this file that extends BaseService
 4. The class needs to define all the functions required + may add its own.
+
+# Developer Setup
+
+Run `pip install -e '.[test]'` to install the dependencies needed for a development environment.
+
+Run `pytest --cov=./src` to run the tests and get a test coverage summary.
+
+Run `pytest --cov-report html --cov=./src` to run the tests and get a full HTML coverage report output to `htmlcov`.
```

### Comparing `sparc.client-0.0.1.post1/src/sparc/client/client.py` & `sparc.client-0.1.0/src/sparc/client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,121 @@
 import logging
 import os
-import sys
-from configparser import ConfigParser
+from configparser import ConfigParser, SectionProxy
 from importlib import import_module
 from inspect import isabstract, isclass
 from pathlib import Path
 from pkgutil import iter_modules
+from typing import Optional, Union
 
 from .services import ServiceBase
 
 
 class SparcClient(object):
     """
     The main class of the sparc.client library.
 
     This class is used to connect existing modules located in <projectbase>/services folder
 
 
-    Attributes
-    ----------
+    Parameters:
+    -----------
     config_file : str
         The location of the file in INI format that is used to extract configuration variables.
         The config file needs to define a [global] section with the name of the default profile
         (in square brackets as well) which holds environmental variables used by the modules.
         Refer to configparser for further details.
     connect : bool (True)
         Calls connect() method of each of the modules.
         By default during initialization all modules are initialized and ready to be used,
         unless connect is set to False.
 
 
-    Attributes
-    ----------
+    Attributes:
+    -----------
     module_names : list
         Stores the list of modules that are automatically loaded from the <projectbase>/services directory.
 
-    Methods
-    -------
+    Methods:
+    --------
     add_module(path, config, connect):
         Adds and optionally connects to a module in a given path with configuration variables defined in config.
     connect()
         Connects all the modules by calling their connect() functions.
     """
 
-    module_names = []
-
-    def __init__(self, config_file="config/config.ini", connect=True) -> None:
+    def __init__(self, config_file: str = "config/config.ini", connect: bool = True) -> None:
         # Read config file
         if not config_file:
             raise RuntimeError("Configuration file not given")
 
         config = ConfigParser()
 
         if os.path.isfile(config_file):
             config.read(config_file)
             logging.debug(str(config))
         current_config = config["global"]["default_profile"]
 
         logging.debug("Using the following config:")
         logging.debug(str(config[current_config]))
+        self.module_names = []
 
         # iterate through the modules in the current package
         package_dir = os.path.join(Path(__file__).resolve().parent, "services")
 
         for _, module_name, _ in iter_modules([package_dir]):
             # import the module and iterate through its attributes
             self.add_module(
                 f"{__package__}.services.{module_name}", config[current_config], connect
             )
 
-    def add_module(self, path, config, connect=True):
+    def add_module(
+        self,
+        paths: Union[str, list[str]],
+        config: Optional[Union[dict, SectionProxy]] = None,
+        connect: bool = True,
+    ) -> None:
         """Adds and optionally connects to a module in a given path with configuration variables defined in config.
 
-        Parameters
-        ----------
-        path : str
+        Parameters:
+        -----------
+        paths : str or list[str]
             a path to the module
         config : dict or configparser.SectionProxy
             a dictionary (or Section of the config file parsed by ConfigParser) with the configuration variables
         connect : bool
             determines if the module should auto-connect
         """
-        module_name = path.split(".")[-1]
-        try:
-            module = import_module(path)
-        except ImportError:
-            logging.debug("Skipping module. Failed to import from %s", f"{path=}", exc_info=True)
-        else:
-            for attribute_name in dir(module):
-                attribute = getattr(module, attribute_name)
-                if (
-                    isclass(attribute)
-                    and issubclass(attribute, ServiceBase)
-                    and not isabstract(attribute)
-                ):
-                    # Add the class to this package's variables
-                    self.module_names.append(module_name)
-                    c = attribute(connect=False, config=config)
-                    setattr(self, module_name, c)
-                    if connect:
-                        c.connect()
+        if not isinstance(paths, list):
+            paths = [paths]
+
+        for path in paths:
+            module_name = path.split(".")[-1] if "." in path else path
+            try:
+                module = import_module(path)
+                for attribute_name in dir(module):
+                    attribute = getattr(module, attribute_name)
+                    if (
+                        isclass(attribute)
+                        and issubclass(attribute, ServiceBase)
+                        and not isabstract(attribute)
+                    ):
+                        # Add the class to this package's variables
+                        self.module_names.append(module_name)
+                        c = attribute(connect=connect, config=config)
+                        setattr(self, module_name, c)
+                        if connect:
+                            c.connect()
+
+            except ModuleNotFoundError:
+                logging.debug(
+                    "Skipping module. Failed to import from %s", f"{path=}", exc_info=True
+                )
+                raise
 
-    def connect(self):
+    def connect(self) -> bool:
         """Connects each of the modules loaded into self.module_names"""
         for module_name in self.module_names:
-            getattr(self, module_name).connect()
+            module = getattr(self, module_name)
+            if hasattr(module, "connect"):
+                getattr(self, module_name).connect()
+        return True
```

### Comparing `sparc.client-0.0.1.post1/src/sparc/client/services/__init__.py` & `sparc.client-0.1.0/src/sparc/client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sparc.client-0.0.1.post1/src/sparc/client/services/_default.py` & `sparc.client-0.1.0/src/sparc/client/services/_default.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
 
 class ServiceBase(ABC):
     """An abstract class determining functions of Sparc Client modules
 
-    Attributes
-    ----------
+    Attributes:
+    -----------
     config : dict
         Dictionary of config variables for the module implementic ServiceBase.
     connect : bool
         Determines if module should be automatically connected.
     args : dict
         All other positional arguments.
     kwargs : dict
         All other keyword arguments.
 
-    Methods
-    -------
+    Methods:
+    --------
     connect(*args, **kwargs) -> Optional
         Connects a given module to Sparc Client.
     info(*args, **kwargs) -> str
         Returns information on the module (e.g. its version).
     get_profile(*args, **kwargs) -> str
         Returns the currently used profile.
     set_profile(*args, **kwargs) -> str
         Sets the new profile.
     close(*args, **kwargs) -> None
         Closes connection with the module.
     """
 
     @abstractmethod
     def __init__(self, config, connect: bool, *args, **kwargs) -> None:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def connect(self, *args, **kwargs) -> Optional:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def info(self, *args, **kwargs) -> str:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def get_profile(self, *args, **kwargs) -> str:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def set_profile(self, *args, **kwargs) -> str:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def close(self, *args, **kwargs) -> None:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
```

### Comparing `sparc.client-0.0.1.post1/src/sparc/client/services/pennsieve.py` & `sparc.client-0.1.0/src/sparc/client/services/pennsieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import logging
 import os
-import requests
 
+import requests
 from pennsieve2 import Pennsieve
-
+from configparser import SectionProxy
+from typing import List, Optional, Union
 from ._default import ServiceBase
 
 
 class PennsieveService(ServiceBase):
     """A wrapper for Pennsieve2 library
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     config : dict
         A configuration with defined profile name (pennsieve_profile_name).
     connect : bool
         Determines if Sparc Client should initiate connection with Pennsieve Agent.
 
-    Attributes
-    ----------
+    Attributes:
+    -----------
     default_headers : dict
         A dictionary with headers to make HTTP requests.
     host_api : str
         A default HTTP address of the Pennsieve.
     Pennsieve : object
         A class holding st
 
 
-    Methods
-    -------
+    Methods:
+    --------
     connect()
         Establishes connection with Pennsieve Agent.
     info() -> str
         Returns the version of Pennsieve Agent.
     get_profile() -> str
         Returns the currently used profile.
     set_profile() -> str
@@ -40,43 +41,45 @@
     close() : None
         Closes Pennsieve Agent.
     list_datasets(...) : dict
         Returns a dictionary with datasets matching search criteria.
     list_files(...) : dict
         Returns a dictionary with datasets matching search criteria.
     list_filenames(...) : list
-        Returns a dictionary with filenames matching search criteria.
+        Returns a dictionary with filenames stored at AWS matching search criteria.
     list_records(...) : dict
         Returns a dictionary with records matching search criteria.
 
     """
 
     default_headers = {
         "Content-Type": "application/json",
         "Accept": "application/json; charset=utf-8",
     }
 
     host_api = "https://api.pennsieve.io"
-    Pennsieve = None
+    Pennsieve: Pennsieve = None
+    profile_name: str = None
 
-    def __init__(self, config=None, connect=False) -> None:
+    def __init__(
+        self, config: Optional[Union[dict, SectionProxy]] = None, connect: bool = False
+    ) -> None:
         logging.info("Initializing Pennsieve...")
         logging.debug(str(config))
 
         self.Pennsieve = Pennsieve(connect=False)
         if config is not None:
             self.profile_name = config.get("pennsieve_profile_name")
             logging.info("Profile: " + self.profile_name)
         else:
-            self.profile_name = None
             logging.info("Profile: none")
         if connect:
             self.connect()  # profile_name=self.profile_name)
 
-    def connect(self):
+    def connect(self) -> Pennsieve:
         """Establishes connection with Pennsieve Agent."""
         logging.info("Connecting to Pennsieve...")
 
         if self.profile_name is not None:
             self.Pennsieve.connect(profile_name=self.profile_name)
         else:
             self.Pennsieve.connect()
@@ -85,53 +88,54 @@
     def info(self) -> str:
         """Returns the version of Pennsieve Agent."""
         return self.Pennsieve.agent_version()
 
     def get_profile(self) -> str:
         """Returns currently used profile.
 
-        Returns
-        -------
+        Returns:
+        --------
         A string with username.
         """
-        return self.Pennsieve.user.whoami()
+        return self.Pennsieve.get_user()
 
-    def set_profile(self, profile_name) -> str:
+    def set_profile(self, profile_name: str) -> str:
         """Changes the profile to the specified name.
-        Parameters
-        ----------
+
+        Parameters:
+        -----------
         profile_name : str
             The name of the profile to change into.
 
-        Returns
-        -------
+        Returns:
+        --------
         A string with confirmation of profile switch.
         """
-        return self.Pennsieve.user.switch(profile_name)
+        return self.Pennsieve.switch(profile_name)
 
     def close(self) -> None:
         """Closes the Pennsieve Agent."""
-        return self.Pennsieve.close()
+        return self.Pennsieve.stop()
 
     def list_datasets(
         self,
-        limit=10,
-        offset=0,
-        query=None,
-        organization=None,
-        organization_id=None,
-        tags=None,
-        embargo=None,
-        order_by=None,
-        order_direction=None,
+        limit: int = 10,
+        offset: int = 0,
+        query: str = None,
+        organization: str = None,
+        organization_id: int = None,
+        tags: List[str] = None,
+        embargo: bool = None,
+        order_by: str = None,
+        order_direction: str = None,
     ) -> list:
         """Gets datasets matching specified criteria.
 
-        Parameters
-        ----------
+        Parameters:
+        -----------
         limit : int
             max number of datasets returned
         offset : int
             offset used for pagination of results
         query : str
             fuzzy text search terms (refer to elasticsearch)
         organization : str
@@ -172,25 +176,25 @@
                 "orderBy": order_by,
                 "orderDirection": order_direction,
             },
         )
 
     def list_files(
         self,
-        limit=10,
-        offset=0,
-        file_type=None,
-        query=None,
-        organization=None,
-        organization_id=None,
-        dataset_id=None,
+        limit: int = 10,
+        offset: int = 0,
+        file_type: str = None,
+        query: str = None,
+        organization: str = None,
+        organization_id: int = None,
+        dataset_id: int = None,
     ) -> list:
         """
-        Parameters
-        ----------
+        Parameters:
+        -----------
         limit : int
             max number of datasets returned
         offset : int
             offset used for pagination of results
         file_type : str
             type of file
         query : str
@@ -199,14 +203,18 @@
             only return records of this model
         organization : str
             publishing organization
         organization_id : int
             publishing organization id
         dataset_id : int
             files within this dataset
+
+        Returns:
+        --------
+        List of files stored at AWS with their parameters.
         """
 
         return self.Pennsieve.get(
             self.host_api + "/discover/search/files",
             headers=self.default_headers,
             params={
                 "limit": limit,
@@ -217,21 +225,21 @@
                 "organizationId": organization_id,
                 "datasetId": dataset_id,
             },
         )["files"]
 
     def list_filenames(
         self,
-        limit=10,
-        offset=0,
-        file_type=None,
-        query=None,
-        organization=None,
-        organization_id=None,
-        dataset_id=None,
+        limit: int = 10,
+        offset: int = 0,
+        file_type: str = None,
+        query: str = None,
+        organization: str = None,
+        organization_id: int = None,
+        dataset_id: int = None,
     ) -> list:
         """Calls list_files() and extracts the names of the files.
         See also
         --------
         list_files()
         """
         response = self.list_files(
@@ -243,19 +251,24 @@
             organization_id=organization_id,
             dataset_id=dataset_id,
         )
 
         return list(map(lambda x: "/".join(x["uri"].split("/")[5:]), response))
 
     def list_records(
-        self, limit=10, offset=0, model=None, organization=None, dataset_id=None
+        self,
+        limit: int = 10,
+        offset: int = 0,
+        model: str = None,
+        organization: str = None,
+        dataset_id: int = None,
     ) -> list:
         """
-        Parameters
-        ----------
+        Parameters:
+        -----------
         limit : int
             max number of datasets returned
         offset : int
             offset used for pagination of results
         model : str
             only return records of this model
         organization : str
@@ -272,27 +285,27 @@
                 "offset": offset,
                 "model": model,
                 "organization": organization,
                 "datasetId": dataset_id,
             },
         )
 
-    def download_file(self, file_list, output_name=None):
+    def download_file(self, file_list: dict, output_name: str = None):
         """Downloads files into a local storage.
 
         Parameters:
         -----------
         file_list : dict
             names of the file(s) to download with their parameters.
             The files need to come from a single database.
         output_name : str
             The name of the output file (used if the archive
 
-        Return:
-        -------
+        Returns:
+        --------
         A response from the server.
         """
 
         # make sure we are passing a list
         file_list = [file_list] if type(file_list) is dict else file_list
 
         # create a tuple with datasetId and version of the dataset
@@ -325,83 +338,83 @@
             output_name = (
                 file_list[0]["name"] if len(paths) == 1 else os.path.splitext(file_list[0]) + ".gz"
             )
         with open(output_name, mode="wb+") as f:
             f.write(response.content)
         return response
 
-    def get(self, url, **kwargs):
+    def get(self, url: str, **kwargs):
         """Invokes GET endpoint on a server. Passing server name in url is optional.
 
         Parameters:
         -----------
         url : str
             the address of the server endpoint to be called (e.g. api.pennsieve.io/datasets).
             The name of the server can be ommitted.
         kwargs : dict
             a dictionary storing additional information
 
-        Return:
+        Returns:
         --------
         String in JSON format with response from the server.
 
         Example:
         --------
         p=Pennsieve()
         p.get('https://api.pennsieve.io/discover/datasets', params={'limit':20})
 
         """
         return self.Pennsieve.get(url, **kwargs)
 
-    def post(self, url, json, **kwargs):
+    def post(self, url: str, json: dict, **kwargs):
         """Invokes POST endpoint on a server. Passing server name in url is optional.
 
         Parameters:
         -----------
         url : str
             the address of the server endpoint to be called (e.g. api.pennsieve.io/datasets).
             The name of the server can be omitted.
         json : dict
             a request payload with parameters defined by a given endpoint
         kwargs : dict
             additional information
 
-        Return:
-        -------
+        Returns:
+        --------
         String in JSON format with response from the server.
         """
         return self.Pennsieve.post(url, json=json, **kwargs)
 
-    def put(self, url, json, **kwargs):
+    def put(self, url: str, json: dict, **kwargs):
         """Invokes PUT endpoint on a server. Passing server name in url is optional.
 
         Parameters:
         -----------
         url : str
             the address of the server endpoint to be called (e.g. api.pennsieve.io/datasets).
             The name of the server can be omitted.
         json : dict
             a request payload with parameters defined by a given endpoint
         kwargs : dict
             additional information
 
-        Return:
+        Returns:
         --------
         String in JSON format with response from the server.
         """
         return self.Pennsieve.put(url, json=json, **kwargs)
 
-    def delete(self, url, **kwargs):
+    def delete(self, url: str, **kwargs):
         """Invokes DELETE endpoint on a server. Passing server name in url is optional.
 
         Parameters:
         -----------
         url : str
             the address of the server endpoint to be called. The name of the server can be omitted.
         kwargs : dict
             additional information
 
-        Return:
-        -------
+        Returns:
+        --------
         String in JSON format with response from the server.
         """
         return self.Pennsieve.delete(url, **kwargs)
```

