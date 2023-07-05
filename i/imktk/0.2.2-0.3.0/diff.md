# Comparing `tmp/imktk-0.2.2.tar.gz` & `tmp/imktk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imktk-0.2.2.tar", max compression
+gzip compressed data, was "imktk-0.3.0.tar", max compression
```

## Comparing `imktk-0.2.2.tar` & `imktk-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2022-12-19 13:01:41.687700 imktk-0.2.2/LICENSE
--rw-r--r--   0        0        0     4235 2022-12-19 13:01:41.687700 imktk-0.2.2/README.md
--rw-r--r--   0        0        0     3269 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/README.md
--rw-r--r--   0        0        0     1061 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/__init__.py
--rw-r--r--   0        0        0       97 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/constants/__init__.py
--rw-r--r--   0        0        0      943 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/constants/_constants.py
--rw-r--r--   0        0        0      428 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/constants/_custom_defined.py
--rw-r--r--   0        0        0        0 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/.gitinclude
--rw-r--r--   0        0        0     1256 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/_template.py
--rw-r--r--   0        0        0      749 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/ad_temp.py
--rw-r--r--   0        0        0      608 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/anomalies.py
--rw-r--r--   0        0        0      343 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/climatology.py
--rw-r--r--   0        0        0     2165 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/flight_track.py
--rw-r--r--   0        0        0     1289 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/num_den.py
--rw-r--r--   0        0        0      789 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/vapour_pres_ice.py
--rw-r--r--   0        0        0      961 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataarray_methods/vapour_pres_liq.py
--rw-r--r--   0        0        0        0 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataset_methods/.gitinclude
--rw-r--r--   0        0        0     1241 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/dataset_methods/_template.py
--rw-r--r--   0        0        0     3486 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/toolkit.py
--rw-r--r--   0        0        0     2563 2022-12-19 13:01:41.687700 imktk-0.2.2/imktk/tutorial.py
--rw-r--r--   0        0        0     1258 2022-12-19 13:01:41.687700 imktk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5225 2022-12-19 13:01:54.100772 imktk-0.2.2/setup.py
--rw-r--r--   0        0        0     5324 2022-12-19 13:01:54.101178 imktk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-05 10:54:33.095626 imktk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4235 2023-07-05 10:54:33.095626 imktk-0.3.0/README.md
+-rw-r--r--   0        0        0     3269 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/README.md
+-rw-r--r--   0        0        0     1061 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/constants/__init__.py
+-rw-r--r--   0        0        0      943 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/constants/_constants.py
+-rw-r--r--   0        0        0      428 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/constants/_custom_defined.py
+-rw-r--r--   0        0        0        0 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/.gitinclude
+-rw-r--r--   0        0        0     1256 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/_template.py
+-rw-r--r--   0        0        0      749 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/ad_temp.py
+-rw-r--r--   0        0        0      608 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/anomalies.py
+-rw-r--r--   0        0        0      343 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/climatology.py
+-rw-r--r--   0        0        0     2165 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/flight_track.py
+-rw-r--r--   0        0        0     1289 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/num_den.py
+-rw-r--r--   0        0        0      789 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/vapour_pres_ice.py
+-rw-r--r--   0        0        0      961 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataarray_methods/vapour_pres_liq.py
+-rw-r--r--   0        0        0        0 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataset_methods/.gitinclude
+-rw-r--r--   0        0        0     1241 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/dataset_methods/_template.py
+-rw-r--r--   0        0        0     3486 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/toolkit.py
+-rw-r--r--   0        0        0     2563 2023-07-05 10:54:33.095626 imktk-0.3.0/imktk/tutorial.py
+-rw-r--r--   0        0        0     1318 2023-07-05 10:54:33.095626 imktk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 imktk-0.3.0/setup.py
+-rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 imktk-0.3.0/PKG-INFO
```

### Comparing `imktk-0.2.2/LICENSE` & `imktk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/README.md` & `imktk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/README.md` & `imktk-0.3.0/imktk/README.md`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/__init__.py` & `imktk-0.3.0/imktk/__init__.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/constants/_constants.py` & `imktk-0.3.0/imktk/constants/_constants.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/_template.py` & `imktk-0.3.0/imktk/dataarray_methods/_template.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/ad_temp.py` & `imktk-0.3.0/imktk/dataarray_methods/ad_temp.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/anomalies.py` & `imktk-0.3.0/imktk/dataarray_methods/anomalies.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/flight_track.py` & `imktk-0.3.0/imktk/dataarray_methods/flight_track.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/num_den.py` & `imktk-0.3.0/imktk/dataarray_methods/num_den.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/vapour_pres_ice.py` & `imktk-0.3.0/imktk/dataarray_methods/vapour_pres_ice.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataarray_methods/vapour_pres_liq.py` & `imktk-0.3.0/imktk/dataarray_methods/vapour_pres_liq.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/dataset_methods/_template.py` & `imktk-0.3.0/imktk/dataset_methods/_template.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/toolkit.py` & `imktk-0.3.0/imktk/toolkit.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/imktk/tutorial.py` & `imktk-0.3.0/imktk/tutorial.py`

 * *Files identical despite different names*

### Comparing `imktk-0.2.2/pyproject.toml` & `imktk-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imktk"
-version = "0.2.2"
+version = "0.3.0"
 description = "Toolkit provided by IMK at KIT"
 license = "MIT"
 authors = [
     "Uğur Çayoğlu <Ugur.Cayoglu@kit.edu>",
 ]
 readme = "README.md"
 homepage = "https://github.com/imk-toolkit/imk-toolkit"
@@ -18,26 +18,28 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8, <3.11"
+python = "^3.8"
 xarray = "^0.20.1"
 netCDF4 = "^1.5.8"
 scipy = "^1.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^3.4"
 black = "^22.6.0"
 flake8 = "^4.0.1"
+requests = "<2.30.0"
 
 [tool.poetry.scripts]
 imktk = "imktk:main"
 
 [tool.black]
 line-length = 140
 target-version = ['py38']
```

### Comparing `imktk-0.2.2/setup.py` & `imktk-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['netCDF4>=1.5.8,<2.0.0', 'scipy>=1.9.0,<2.0.0', 'xarray>=0.20.1,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['imktk = imktk:main']}
 
 setup_kwargs = {
     'name': 'imktk',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'Toolkit provided by IMK at KIT',
     'long_description': '# IMK Toolkit\n\nThis toolkit provides [post-processing scripts](/imktk) developed by members of the\n[Institute of Meteorology and Climate Research (IMK)](https://dev.to/epassaro/keep-your-research-reproducible-with-conda-pack-and-github-actions-339n)\nat the Karlsruhe Institute of Technology (KIT). The goal of this module is to\ngather together python post-processing scripts for the analysis of netCDF data\nand distribute them easily.\n\n## Usage\nSimply import the library using `import imktk`. From then on all scripts are\navailable using the `imktk` attribute:\n\n```python\nimport imktk\n\nds = imktk.tutorial.open_dataset("toy_weather")  # Load example dataset\nanomaly_free_tmin = ds.tmin.imktk.anomalies()  # Select dataarray `xr.tmin` and execute anomalies script\n```\n\nThe following is a list of available scripts:\n\n\n| Description | Example usage | Link to Script\n|--------|--------|-------------|\n|Calculate temperature for adiabatic process in air|`ds.tmin.imktk.ad_temp(temp_at_0, press_at_0)`| [here](./imktk/dataarray_methods/ad_temp.py)|\n|Calculate monthly anomalies|`ds.tmin.imktk.anomalies()`| [here](./imktk/dataarray_methods/anomalies.py)|\n|Calculate monthly climatology|`ds.tmin.imktk.climatology()`| [here](./imktk/dataarray_methods/climatology.py)|\n|Interpolation routine for flight track (incl. aircraft and satellites)| `ds.tmin.imktk.flight_track(**dims)` | [here](./imktk/dataarray_methods/flight_track.py) |\n|Calculate number density from mixing ratio, temperature and pressure| `ds.tmin.imktk.num_den(temp, press)` | [here](./imktk/dataarray_methods/num_den.py)|\n|Calculate saturation vapour pressure over ice for temperatures > 110 K| `ds.tmin.imktk.vapour_pres_ice()` | [here](./imktk/dataarray_methods/vapour_pres_ice.py)|\n|Calculate saturation vapour pressure over liquid water for temperatures 123 K < T < 332 K|`ds.tmin.imktk.vapour_pres_liq()` | [here](./imktk/dataarray_methods/vapour_pres_liq.py)|\n\n## Getting Started\n\nThe easiest method to test the module is to use an interactive session with docker.\nIn this environment you will have a Python 3 environment with all necessary dependencies already installed.\n\n```bash\ndocker run -it imktk/imktk:latest bash\n```\n\n> For the brave: You can test the latest release candidate by changing `latest` to `testing`\n\n## Install\n\nChoose one of the following methods to install the package:\n\n1. Install using `pip`\n2. Install using `conda`\n3. Install using `git clone`\n\n> This package supports only Python 3 with version `>=3.7`. If you are using\n> an earlier version of Python please consider updating.\n\n### `pip`\n\nReleases are automatically uploaded to PyPI. Please execute following command\nto install the package.\n\n```bash\npython3 -m pip install imktk\n```\n\n### `conda`\n\nCurrently the package does no support native installation using `conda`\nrespectively `conda-forge`. This feature is on the roadmap and you can follow\nits process using issue [#34](https://github.com/imk-toolkit/imk-toolkit/issues/34).\nThe current workaround for `conda` installation is to use the following steps\nfor any given environment `<env>`.\n\n1. Activate the environment\n\n    ```bash\n    conda activate <env>\n    ```\n\n2. Install using `pip`\n\n    ```bash\n    python3 -m pip install imktk\n    ```\n\n### `git clone`\n\nIt is also possible to install the package natively by cloning the repository.\nIf you are interested in using this method of installation please follow\nthese steps\n\n1. Install build dependencies\n\n    ```bash\n    python3 -m pip install build\n    ```\n\n2. Clone repository\n\n    ```bash\n    git clone https://github.com/imk-toolkit/imk-toolkit.git\n    ```\n\n3. Generate the Python packages\n\n    ```bash\n    python3 -m build  # or `make build`\n    ```\n\n4. Install packages\n\n    ```bash\n    pip3 install dist/imktk-<current.version>-py3-none-any.whl  # or `make install`\n    ```\n\n> Please be aware that this package uses `HDF5` and `netCDF` c-libraries in the\n> backend. If you are installing using `git clone` the `HDF5_DIR` environment\n> variable with the location of the HDF5 header files needs to be set.\n\n## Further reading\n\nIf you are interested in the inner workings of the package and details of the\nimplementation please refer to the embedded [README.md](/imktk/README.md).\n',
     'author': 'Uğur Çayoğlu',
     'author_email': 'Ugur.Cayoglu@kit.edu',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/imk-toolkit/imk-toolkit',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `imktk-0.2.2/PKG-INFO` & `imktk-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: imktk
-Version: 0.2.2
+Version: 0.3.0
 Summary: Toolkit provided by IMK at KIT
 Home-page: https://github.com/imk-toolkit/imk-toolkit
 License: MIT
 Author: Uğur Çayoğlu
 Author-email: Ugur.Cayoglu@kit.edu
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Dist: netCDF4 (>=1.5.8,<2.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: xarray (>=0.20.1,<0.21.0)
```

