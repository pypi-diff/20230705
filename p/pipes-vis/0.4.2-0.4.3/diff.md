# Comparing `tmp/pipes-vis-0.4.2.tar.gz` & `tmp/pipes-vis-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hinleung/OneDrive - University of St Andrews/Documents/St Andrews stuff/PhD project/pipes_vis/examples_and_testing/pipes", last modified: Tue Sep 20 09:25:29 2022, max compression
+gzip compressed data, was "dist/pipes-vis-0.4.3.tar", last modified: Wed Jul  5 15:22:22 2023, max compression
```

## Comparing `pipes-vis-0.4.2.tar` & `pipes-vis-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2022-09-20 09:25:29.938590 pipes-vis-0.4.2/
--rw-------   0 hinleung   (501) staff       (20)    35149 2021-11-03 19:58:11.000000 pipes-vis-0.4.2/LICENSE
--rw-r--r--   0 hinleung   (501) staff       (20)     2272 2022-09-20 09:25:29.938332 pipes-vis-0.4.2/PKG-INFO
--rw-r--r--   0 hinleung   (501) staff       (20)     1715 2022-09-19 15:05:52.000000 pipes-vis-0.4.2/README.md
--rw-r--r--   0 hinleung   (501) staff       (20)       38 2022-09-20 09:25:29.938669 pipes-vis-0.4.2/setup.cfg
--rw-------   0 hinleung   (501) staff       (20)      984 2022-09-19 18:48:57.000000 pipes-vis-0.4.2/setup.py
-drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2022-09-20 09:25:29.933793 pipes-vis-0.4.2/src/
-drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2022-09-20 09:25:29.936509 pipes-vis-0.4.2/src/pipes_vis/
--rw-------   0 hinleung   (501) staff       (20)      523 2021-11-03 19:58:11.000000 pipes-vis-0.4.2/src/pipes_vis/__init__.py
--rw-------   0 hinleung   (501) staff       (20)     1601 2021-11-03 19:58:11.000000 pipes-vis-0.4.2/src/pipes_vis/override_config.py
--rw-r--r--   0 hinleung   (501) staff       (20)    11389 2022-09-19 18:18:26.000000 pipes-vis-0.4.2/src/pipes_vis/plotting.py
--rw-------   0 hinleung   (501) staff       (20)     7912 2021-11-27 02:14:21.000000 pipes-vis-0.4.2/src/pipes_vis/slider_params.py
--rw-------   0 hinleung   (501) staff       (20)    18049 2021-11-30 16:29:31.000000 pipes-vis-0.4.2/src/pipes_vis/utils.py
--rw-r--r--   0 hinleung   (501) staff       (20)    37843 2022-09-19 18:28:58.000000 pipes-vis-0.4.2/src/pipes_vis/visualizer.py
-drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2022-09-20 09:25:29.937959 pipes-vis-0.4.2/src/pipes_vis.egg-info/
--rw-r--r--   0 hinleung   (501) staff       (20)     2272 2022-09-20 09:25:29.000000 pipes-vis-0.4.2/src/pipes_vis.egg-info/PKG-INFO
--rw-r--r--   0 hinleung   (501) staff       (20)      377 2022-09-20 09:25:29.000000 pipes-vis-0.4.2/src/pipes_vis.egg-info/SOURCES.txt
--rw-r--r--   0 hinleung   (501) staff       (20)        1 2022-09-20 09:25:29.000000 pipes-vis-0.4.2/src/pipes_vis.egg-info/dependency_links.txt
--rw-r--r--   0 hinleung   (501) staff       (20)       62 2022-09-20 09:25:29.000000 pipes-vis-0.4.2/src/pipes_vis.egg-info/requires.txt
--rw-r--r--   0 hinleung   (501) staff       (20)       10 2022-09-20 09:25:29.000000 pipes-vis-0.4.2/src/pipes_vis.egg-info/top_level.txt
+drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2023-07-05 15:22:22.637773 pipes-vis-0.4.3/
+-rw-r--r--   0 hinleung   (501) staff       (20)     2410 2023-07-05 15:22:22.637464 pipes-vis-0.4.3/PKG-INFO
+-rw-------   0 hinleung   (501) staff       (20)     1715 2022-09-19 15:05:52.000000 pipes-vis-0.4.3/README.md
+-rw-r--r--   0 hinleung   (501) staff       (20)       38 2023-07-05 15:22:22.637874 pipes-vis-0.4.3/setup.cfg
+-rw-------   0 hinleung   (501) staff       (20)      984 2023-07-05 15:08:35.000000 pipes-vis-0.4.3/setup.py
+drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2023-07-05 15:22:22.630900 pipes-vis-0.4.3/src/
+drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2023-07-05 15:22:22.634807 pipes-vis-0.4.3/src/pipes_vis/
+-rw-------   0 hinleung   (501) staff       (20)      523 2021-11-03 19:58:11.000000 pipes-vis-0.4.3/src/pipes_vis/__init__.py
+-rw-------   0 hinleung   (501) staff       (20)     1601 2021-11-03 19:58:11.000000 pipes-vis-0.4.3/src/pipes_vis/override_config.py
+-rw-------   0 hinleung   (501) staff       (20)    11389 2022-09-19 18:18:26.000000 pipes-vis-0.4.3/src/pipes_vis/plotting.py
+-rw-------   0 hinleung   (501) staff       (20)     7912 2021-11-27 02:14:21.000000 pipes-vis-0.4.3/src/pipes_vis/slider_params.py
+-rw-------   0 hinleung   (501) staff       (20)    18049 2021-11-30 16:29:31.000000 pipes-vis-0.4.3/src/pipes_vis/utils.py
+-rw-------   0 hinleung   (501) staff       (20)    37992 2023-07-05 15:04:20.000000 pipes-vis-0.4.3/src/pipes_vis/visualizer.py
+drwxr-xr-x   0 hinleung   (501) staff       (20)        0 2023-07-05 15:22:22.636929 pipes-vis-0.4.3/src/pipes_vis.egg-info/
+-rw-r--r--   0 hinleung   (501) staff       (20)     2410 2023-07-05 15:22:22.000000 pipes-vis-0.4.3/src/pipes_vis.egg-info/PKG-INFO
+-rw-r--r--   0 hinleung   (501) staff       (20)      369 2023-07-05 15:22:22.000000 pipes-vis-0.4.3/src/pipes_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 hinleung   (501) staff       (20)        1 2023-07-05 15:22:22.000000 pipes-vis-0.4.3/src/pipes_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 hinleung   (501) staff       (20)       62 2023-07-05 15:22:22.000000 pipes-vis-0.4.3/src/pipes_vis.egg-info/requires.txt
+-rw-r--r--   0 hinleung   (501) staff       (20)       10 2023-07-05 15:22:22.000000 pipes-vis-0.4.3/src/pipes_vis.egg-info/top_level.txt
```

### Comparing `pipes-vis-0.4.2/PKG-INFO` & `pipes-vis-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pipes-vis
-Version: 0.4.2
+Version: 0.4.3
 Summary: Small interactive GUI/visualizer tool for SPS spectra
 Home-page: https://github.com/HinLeung622/pipes_vis
 Author: Ho-Hin Leung
 Author-email: hhl1@st-andrews.ac.uk
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HinLeung622/pipes_vis/issues
+Description: # pipes_vis
+        A small, interactive GUI/visualizer tool for SPS spectra, powered by Adam Carnall's Bayesian Analysis of Galaxies for Physical Inference and Parameter EStimation [(BAGPIPES)](https://bagpipes.readthedocs.io/en/latest/) <br>
+        
+        A ["Mini-paper"](https://iopscience.iop.org/article/10.3847/2515-5172/ac1680) about pipes_vis is published in the Research Notes of the AAS. Please cite this paper if you use pipes_vis in your publications.<br>
+        
+        To install, type `pip install pipes_vis`. This package depends on Bagpipes, which has non-python packages like multinest as dependencies. If you only wish to use pipes_vis, you need not go through the process to get all non-python dependencies of bagpipes as they are only used for SED fitting rather than modelling. Just ignore complains from Bagpipes when importing. However, if you wish to use Bagpipes for SED fitting, follow the tutorial in Bagpipes' docs to get those non-python packages.<br>
+        
+        You can find examples and documentations of the tool in [this jupyter notebook](https://github.com/HinLeung622/pipes_vis/blob/main/pipes_vis_example.ipynb)
+        
+        Dependencies: bagpipes, numpy, matplotlib, astropy, scipy (visualizer still works even if you do not install multinest and pymultinest as instructed by bagpipes' installation) <br>
+        
+        For requests regarding making the visualizer avaliable as a web interactive tool much like [sengi](https://www.christopherlovell.co.uk/sengi/), it will likely require rewriting large portions of the code in javascript or some other web-purposed languages. Please contact me if you are interested in doing this/want this to be done.<br>
+        
+        ![alt text](https://github.com/HinLeung622/pipes_vis/blob/main/readme_image.png?raw=true)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pipes_vis
-A small, interactive GUI/visualizer tool for SPS spectra, powered by Adam Carnall's Bayesian Analysis of Galaxies for Physical Inference and Parameter EStimation [(BAGPIPES)](https://bagpipes.readthedocs.io/en/latest/) <br>
-
-A ["Mini-paper"](https://iopscience.iop.org/article/10.3847/2515-5172/ac1680) about pipes_vis is published in the Research Notes of the AAS. Please cite this paper if you use pipes_vis in your publications.<br>
-
-To install, type `pip install pipes_vis`. This package depends on Bagpipes, which has non-python packages like multinest as dependencies. If you only wish to use pipes_vis, you need not go through the process to get all non-python dependencies of bagpipes as they are only used for SED fitting rather than modelling. Just ignore complains from Bagpipes when importing. However, if you wish to use Bagpipes for SED fitting, follow the tutorial in Bagpipes' docs to get those non-python packages.<br>
-
-You can find examples and documentations of the tool in [this jupyter notebook](https://github.com/HinLeung622/pipes_vis/blob/main/pipes_vis_example.ipynb)
-
-Dependencies: bagpipes, numpy, matplotlib, astropy, scipy (visualizer still works even if you do not install multinest and pymultinest as instructed by bagpipes' installation) <br>
-
-For requests regarding making the visualizer avaliable as a web interactive tool much like [sengi](https://www.christopherlovell.co.uk/sengi/), it will likely require rewriting large portions of the code in javascript or some other web-purposed languages. Please contact me if you are interested in doing this/want this to be done.<br>
-
-![alt text](https://github.com/HinLeung622/pipes_vis/blob/main/readme_image.png?raw=true)
```

### Comparing `pipes-vis-0.4.2/README.md` & `pipes-vis-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/setup.py` & `pipes-vis-0.4.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pipes-vis",
-    version="0.4.2",
+    version="0.4.3",
     author="Ho-Hin Leung",
     author_email="hhl1@st-andrews.ac.uk",
     description="Small interactive GUI/visualizer tool for SPS spectra",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HinLeung622/pipes_vis",
     project_urls={
```

### Comparing `pipes-vis-0.4.2/src/pipes_vis/__init__.py` & `pipes-vis-0.4.3/src/pipes_vis/__init__.py`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/src/pipes_vis/override_config.py` & `pipes-vis-0.4.3/src/pipes_vis/override_config.py`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/src/pipes_vis/plotting.py` & `pipes-vis-0.4.3/src/pipes_vis/plotting.py`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/src/pipes_vis/slider_params.py` & `pipes-vis-0.4.3/src/pipes_vis/slider_params.py`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/src/pipes_vis/utils.py` & `pipes-vis-0.4.3/src/pipes_vis/utils.py`

 * *Files identical despite different names*

### Comparing `pipes-vis-0.4.2/src/pipes_vis/visualizer.py` & `pipes-vis-0.4.3/src/pipes_vis/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider, Button, TextBox, CheckButtons
-from mpl_toolkits.axes_grid.inset_locator import InsetPosition
+# handle different versions of mpl_toolkits
+try:
+    from mpl_toolkits.axes_grid.inset_locator import InsetPosition
+except ModuleNotFoundError:
+    from mpl_toolkits.axes_grid1.inset_locator import InsetPosition
 import copy
 import os
 #from time import perfcounter
 
 import bagpipes as pipes
 from . import override_config
 override_config.override_config(pipes)
```

### Comparing `pipes-vis-0.4.2/src/pipes_vis.egg-info/PKG-INFO` & `pipes-vis-0.4.3/src/pipes_vis.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pipes-vis
-Version: 0.4.2
+Version: 0.4.3
 Summary: Small interactive GUI/visualizer tool for SPS spectra
 Home-page: https://github.com/HinLeung622/pipes_vis
 Author: Ho-Hin Leung
 Author-email: hhl1@st-andrews.ac.uk
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HinLeung622/pipes_vis/issues
+Description: # pipes_vis
+        A small, interactive GUI/visualizer tool for SPS spectra, powered by Adam Carnall's Bayesian Analysis of Galaxies for Physical Inference and Parameter EStimation [(BAGPIPES)](https://bagpipes.readthedocs.io/en/latest/) <br>
+        
+        A ["Mini-paper"](https://iopscience.iop.org/article/10.3847/2515-5172/ac1680) about pipes_vis is published in the Research Notes of the AAS. Please cite this paper if you use pipes_vis in your publications.<br>
+        
+        To install, type `pip install pipes_vis`. This package depends on Bagpipes, which has non-python packages like multinest as dependencies. If you only wish to use pipes_vis, you need not go through the process to get all non-python dependencies of bagpipes as they are only used for SED fitting rather than modelling. Just ignore complains from Bagpipes when importing. However, if you wish to use Bagpipes for SED fitting, follow the tutorial in Bagpipes' docs to get those non-python packages.<br>
+        
+        You can find examples and documentations of the tool in [this jupyter notebook](https://github.com/HinLeung622/pipes_vis/blob/main/pipes_vis_example.ipynb)
+        
+        Dependencies: bagpipes, numpy, matplotlib, astropy, scipy (visualizer still works even if you do not install multinest and pymultinest as instructed by bagpipes' installation) <br>
+        
+        For requests regarding making the visualizer avaliable as a web interactive tool much like [sengi](https://www.christopherlovell.co.uk/sengi/), it will likely require rewriting large portions of the code in javascript or some other web-purposed languages. Please contact me if you are interested in doing this/want this to be done.<br>
+        
+        ![alt text](https://github.com/HinLeung622/pipes_vis/blob/main/readme_image.png?raw=true)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pipes_vis
-A small, interactive GUI/visualizer tool for SPS spectra, powered by Adam Carnall's Bayesian Analysis of Galaxies for Physical Inference and Parameter EStimation [(BAGPIPES)](https://bagpipes.readthedocs.io/en/latest/) <br>
-
-A ["Mini-paper"](https://iopscience.iop.org/article/10.3847/2515-5172/ac1680) about pipes_vis is published in the Research Notes of the AAS. Please cite this paper if you use pipes_vis in your publications.<br>
-
-To install, type `pip install pipes_vis`. This package depends on Bagpipes, which has non-python packages like multinest as dependencies. If you only wish to use pipes_vis, you need not go through the process to get all non-python dependencies of bagpipes as they are only used for SED fitting rather than modelling. Just ignore complains from Bagpipes when importing. However, if you wish to use Bagpipes for SED fitting, follow the tutorial in Bagpipes' docs to get those non-python packages.<br>
-
-You can find examples and documentations of the tool in [this jupyter notebook](https://github.com/HinLeung622/pipes_vis/blob/main/pipes_vis_example.ipynb)
-
-Dependencies: bagpipes, numpy, matplotlib, astropy, scipy (visualizer still works even if you do not install multinest and pymultinest as instructed by bagpipes' installation) <br>
-
-For requests regarding making the visualizer avaliable as a web interactive tool much like [sengi](https://www.christopherlovell.co.uk/sengi/), it will likely require rewriting large portions of the code in javascript or some other web-purposed languages. Please contact me if you are interested in doing this/want this to be done.<br>
-
-![alt text](https://github.com/HinLeung622/pipes_vis/blob/main/readme_image.png?raw=true)
```

