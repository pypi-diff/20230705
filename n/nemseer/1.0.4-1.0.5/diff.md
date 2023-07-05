# Comparing `tmp/nemseer-1.0.4.tar.gz` & `tmp/nemseer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemseer-1.0.4.tar", max compression
+gzip compressed data, was "nemseer-1.0.5.tar", max compression
```

## Comparing `nemseer-1.0.4.tar` & `nemseer-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0     1518 2022-12-05 07:23:04.868798 nemseer-1.0.4/LICENSE
--rw-r--r--   0        0        0     7082 2022-12-05 07:23:04.868798 nemseer-1.0.4/README.md
--rw-r--r--   0        0        0     2877 2022-12-05 07:23:05.508830 nemseer-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      912 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/__init__.py
--rw-r--r--   0        0        0     4706 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/data.py
--rw-r--r--   0        0        0    15759 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/data_compilers.py
--rw-r--r--   0        0        0     9135 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/data_handlers.py
--rw-r--r--   0        0        0    17937 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/downloader.py
--rw-r--r--   0        0        0        0 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/forecast_type/__init__.py
--rw-r--r--   0        0        0     9275 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/forecast_type/run_time_generators.py
--rw-r--r--   0        0        0    13135 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/forecast_type/validators.py
--rw-r--r--   0        0        0     7810 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/nemseer.py
--rw-r--r--   0        0        0        0 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/py.typed
--rw-r--r--   0        0        0    14181 2022-12-05 07:23:05.508830 nemseer-1.0.4/src/nemseer/query.py
--rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 nemseer-1.0.4/setup.py
--rw-r--r--   0        0        0     8071 1970-01-01 00:00:00.000000 nemseer-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0    35150 2023-07-05 04:40:24.529006 nemseer-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7930 2023-07-05 04:40:24.529006 nemseer-1.0.5/README.md
+-rw-r--r--   0        0        0     2886 2023-07-05 04:40:25.133010 nemseer-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      912 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/__init__.py
+-rw-r--r--   0        0        0     4706 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data.py
+-rw-r--r--   0        0        0    15759 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data_compilers.py
+-rw-r--r--   0        0        0     9135 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data_handlers.py
+-rw-r--r--   0        0        0    17937 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/downloader.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/__init__.py
+-rw-r--r--   0        0        0     9275 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/run_time_generators.py
+-rw-r--r--   0        0        0    13135 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/validators.py
+-rw-r--r--   0        0        0     7810 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/nemseer.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/py.typed
+-rw-r--r--   0        0        0    14181 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/query.py
+-rw-r--r--   0        0        0     8994 1970-01-01 00:00:00.000000 nemseer-1.0.5/PKG-INFO
```

### Comparing `nemseer-1.0.4/README.md` & `nemseer-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # nemseer
 
 [![PyPI version](https://badge.fury.io/py/nemseer.svg)](https://badge.fury.io/py/nemseer)
 [![Continuous Integration and Deployment](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml/badge.svg)](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml)
 [![Documentation Status](https://readthedocs.org/projects/nemseer/badge/?version=latest)](https://nemseer.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/UNSW-CEEM/NEMSEER/branch/master/graph/badge.svg?token=BO69YSQIGI)](https://codecov.io/gh/UNSW-CEEM/NEMSEER)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/508154456.svg)](https://zenodo.org/badge/latestdoi/508154456)
 
 A package for downloading and handling historical National Electricity Market (NEM) forecast data produced by the Australian Energy Market Operator (AEMO).
 
 ## Installation
 
 ```bash
 pip install nemseer
@@ -56,22 +57,32 @@
 
 ## Contributing
 
 Interested in contributing? Check out the [contributing guidelines](./CONTRIBUTING.md), which also includes steps to install `nemseer` for development.
 
 Please note that this project is released with a [Code of Conduct](./CONDUCT.md). By contributing to this project, you agree to abide by its terms.
 
-## License
+## Citation
 
-`nemseer` was created by Abhijith Prakash. It is licensed under the terms of the [BSD 3-Clause license](./LICENSE).
+If you use `nemseer`, please cite the package via the [Zenodo DOI](https://doi.org/10.5281/zenodo.7397514).
+
+If you use code or analysis from any of the demand error and/or price convergence examples in the documentation, please also cite `NEMOSIS` via [this conference paper](https://www.researchgate.net/publication/329798805_NEMOSIS_-_NEM_Open_Source_Information_Service_open-source_access_to_Australian_National_Electricity_Market_Data)
+
+## Licenses
+
+`nemseer` was created by Abhijith Prakash. It is licensed under the terms of [GNU GPL-3.0-or-later licences](./LICENSE).
+
+The content within the documentation for this project is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
 
 ## Credits
 
 `nemseer` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
 
+Development of `nemseer` was funded by the [UNSW Digital Grid Futures Institute](https://www.dgfi.unsw.edu.au/).
+
 ### Contributor Acknowledgements
 
 Thanks to:
 
 - Nicholas Gorman for reviewing `nemseer` code
 - Dylan McConnell for assistance in interpreting PASA run types
 - Declan Heim for suggesting improvements to `nemseer` examples
```

### Comparing `nemseer-1.0.4/pyproject.toml` & `nemseer-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nemseer"
-version = "1.0.4"
+version = "1.0.5"
 description = "A package for downloading and handling forecasts for the National Electricity Market (NEM) from the Australian Energy Market Operator (AEMO)."
 authors = ["Abhijith Prakash"]
-license = "BSD 3-Clause"
+license = "GPL-3.0-or-later"
 readme = "README.md"
 
 # Main dependencies for the package via poetry. Package users will need these dependencies.
 [tool.poetry.dependencies]
-python = ">= 3.8, < 3.11"
+python = ">= 3.8,<3.12"
 attrs = "^21.3.0"
 beautifulsoup4 = "^4"
 netCDF4 = "^1.6.0"
 numpy = "^1.23.0"
 packaging = "^21.3"
 pandas = "^1.2"
 psutil = "^5.9.1"
-pyarrow = "^9.0.0"
+pyarrow = "*"
 requests = "^2"
 tqdm = "^4.64.0"
 xarray = "^2022"
 
 # Packages for developers for creating documentation
 [tool.poetry.group.docs]
 optional = true
@@ -33,14 +33,15 @@
 sphinx-copybutton = "^0.5.0"
 # The packages below are required for compiling example notebooks
 jupyter = "^1.0.0"
 notebook = "^6.4.12"
 myst-nb = "^0.16.0"
 matplotlib = "^3.5.3"
 plotly = "^5.10.0"
+kaleido = "0.2.1"
 hvplot = "^0.8.1"
 nemosis = "^3.2.0"
 
 
 # Packages for developers for debugging
 [tool.poetry.group.debug]
 optional = true
@@ -63,15 +64,15 @@
 types-beautifulsoup4 = "^4.11.4"
 types-python-dateutil = "^2.8.19"
 types-psutil = "^5.9.5"
 pandas-stubs = "^1.4.3.220724"
 types-tqdm = "^4.64.4"
 black = "^22.6.0"
 isort = "^5.10.1"
-pre-commit = "^2.20.0"
+pre-commit = "*"
 
 # Packages for developers for testing
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 # pytest and pytest-cov for coverage
```

### Comparing `nemseer-1.0.4/src/nemseer/__init__.py` & `nemseer-1.0.5/src/nemseer/__init__.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/data.py` & `nemseer-1.0.5/src/nemseer/data.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/data_compilers.py` & `nemseer-1.0.5/src/nemseer/data_compilers.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/data_handlers.py` & `nemseer-1.0.5/src/nemseer/data_handlers.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/downloader.py` & `nemseer-1.0.5/src/nemseer/downloader.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/forecast_type/run_time_generators.py` & `nemseer-1.0.5/src/nemseer/forecast_type/run_time_generators.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/forecast_type/validators.py` & `nemseer-1.0.5/src/nemseer/forecast_type/validators.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/nemseer.py` & `nemseer-1.0.5/src/nemseer/nemseer.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/src/nemseer/query.py` & `nemseer-1.0.5/src/nemseer/query.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.4/setup.py` & `nemseer-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nemseer
+Version: 1.0.5
+Summary: A package for downloading and handling forecasts for the National Electricity Market (NEM) from the Australian Energy Market Operator (AEMO).
+License: GPL-3.0-or-later
+Author: Abhijith Prakash
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=21.3.0,<22.0.0)
+Requires-Dist: beautifulsoup4 (>=4,<5)
+Requires-Dist: netCDF4 (>=1.6.0,<2.0.0)
+Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: pandas (>=1.2,<2.0)
+Requires-Dist: psutil (>=5.9.1,<6.0.0)
+Requires-Dist: pyarrow
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: xarray (>=2022,<2023)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# nemseer
 
-packages = \
-['nemseer', 'nemseer.forecast_type']
+[![PyPI version](https://badge.fury.io/py/nemseer.svg)](https://badge.fury.io/py/nemseer)
+[![Continuous Integration and Deployment](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml/badge.svg)](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml)
+[![Documentation Status](https://readthedocs.org/projects/nemseer/badge/?version=latest)](https://nemseer.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/UNSW-CEEM/NEMSEER/branch/master/graph/badge.svg?token=BO69YSQIGI)](https://codecov.io/gh/UNSW-CEEM/NEMSEER)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/508154456.svg)](https://zenodo.org/badge/latestdoi/508154456)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=21.3.0,<22.0.0',
- 'beautifulsoup4>=4,<5',
- 'netCDF4>=1.6.0,<2.0.0',
- 'numpy>=1.23.0,<2.0.0',
- 'packaging>=21.3,<22.0',
- 'pandas>=1.2,<2.0',
- 'psutil>=5.9.1,<6.0.0',
- 'pyarrow>=9.0.0,<10.0.0',
- 'requests>=2,<3',
- 'tqdm>=4.64.0,<5.0.0',
- 'xarray>=2022,<2023']
-
-setup_kwargs = {
-    'name': 'nemseer',
-    'version': '1.0.4',
-    'description': 'A package for downloading and handling forecasts for the National Electricity Market (NEM) from the Australian Energy Market Operator (AEMO).',
-    'long_description': '# nemseer\n\n[![PyPI version](https://badge.fury.io/py/nemseer.svg)](https://badge.fury.io/py/nemseer)\n[![Continuous Integration and Deployment](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml/badge.svg)](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml)\n[![Documentation Status](https://readthedocs.org/projects/nemseer/badge/?version=latest)](https://nemseer.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/UNSW-CEEM/NEMSEER/branch/master/graph/badge.svg?token=BO69YSQIGI)](https://codecov.io/gh/UNSW-CEEM/NEMSEER)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nA package for downloading and handling historical National Electricity Market (NEM) forecast data produced by the Australian Energy Market Operator (AEMO).\n\n## Installation\n\n```bash\npip install nemseer\n```\n\n## Overview\n\n`nemseer` allows you to access historical AEMO [pre-dispatch](https://aemo.com.au/en/energy-systems/electricity/national-electricity-market-nem/data-nem/market-management-system-mms-data/pre-dispatch) and [Projected Assessment of System Adequacy (PASA)](https://wa.aemo.com.au/energy-systems/electricity/national-electricity-market-nem/nem-forecasting-and-planning/forecasting-and-reliability/projected-assessment-of-system-adequacy) forecast[^1] data available through the [MMSDM Historical Data SQLLoader](https://nemseer.readthedocs.io/en/latest/glossary.html#term-MMSDM-Historical-Data-SQLLOader). `nemseer` can then compile this data into [pandas DataFrames](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe) or [xarray Datasets](https://docs.xarray.dev/en/stable/user-guide/data-structures.html#dataset).\n\n![forecast_overview](docs/source/_static/forecast_timeframes.png)\n\n<sub><sup>Source: [Reserve services in the National Electricity Market, AEMC, 2021](https://www.aemc.gov.au/sites/default/files/2020-12/AEMC_Reserve%20services%20in%20the%20NEM%20directions%20paper_05.01.2021.pdf)</sup></sub>\n\nWhereas PASA processes are primarily used to assess resource adequacy based on technical inputs and assumptions for resources in the market (i.e. used to answer questions such as *"can operational demand be met in the forecast horizon with a sufficient safety (reserve) margin?"*), pre-dispatch processes incorporate the latest set of market participant offers and thus produce regional prices forecasts for energy and frequency control ancillary services [(FCAS)](https://aemo.com.au/-/media/files/electricity/nem/security_and_reliability/ancillary_services/guide-to-ancillary-services-in-the-national-electricity-market.pdf). Overviews of the various pre-dispatch and PASA processes can be found in the [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html).\n\n[^1]: We use the term *"forecast"* loosely, especially given that these *"forecasts"* change once participants update offer information (e.g. through rebidding) or submit revised resource availabilities and energy constraints. Both of these are intended outcomes of these *"ahead processes"*, which are run to provide system and market information to participants to inform their decision-making. However, to avoid confusion and to ensure consistency with the language used by AEMO, we use the terms *"forecast"* (or outputs) and *"forecast types"* (or ahead processes) in `nemseer`.\n\n`nemseer` enables you to download and work with data for the following forecast types. Where available, AEMO process and table descriptions are linked:\n\n1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_222.htm#1))\n2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_260.htm#1))\n3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_467.htm#1))\n4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_335.htm#1))\n5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_210.htm#1))\n\nAnother helpful reference for PASA information is AEMO\'s [Reliability Standard Implementation Guidelines](https://www.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/rsig/reliability-standard-implementation-guidelines.pdf?la=en).\n\n### ST PASA Replacement Project\n\nNote that the methodologies for PD PASA and ST PASA are being reviewed by AEMO. In particular, the ST PASA Replacement project will combine PD PASA and ST PASA into ST PASA. For more detail, refer to the [final determination of the rule change](https://www.aemc.gov.au/sites/default/files/2022-05/ERC0332%20-%20Updating%20Short%20Term%20PASA%20-%20Final%20determination.pdf) and the [AEMO ST PASA Replacement Project home page](https://aemo.com.au/en/initiatives/trials-and-initiatives/st-pasa-replacement-project).\n\n## Usage\n\n### Glossary\n\nThe [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html) contains overviews of the PASA and pre-dispatch processes, and descriptions of terminology used in `nemseer`.\n\n### Quick start\n\nCheck out the [Quick start](https://nemseer.readthedocs.io/en/latest/quick_start.html) for guide on to use `nemseer`.\n\n### Examples\n\nSome use case examples have been included in the [Examples](https://nemseer.readthedocs.io/en/latest/examples.html) section of the documentation.\n\n## Contributing\n\nInterested in contributing? Check out the [contributing guidelines](./CONTRIBUTING.md), which also includes steps to install `nemseer` for development.\n\nPlease note that this project is released with a [Code of Conduct](./CONDUCT.md). By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`nemseer` was created by Abhijith Prakash. It is licensed under the terms of the [BSD 3-Clause license](./LICENSE).\n\n## Credits\n\n`nemseer` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n\n### Contributor Acknowledgements\n\nThanks to:\n\n- Nicholas Gorman for reviewing `nemseer` code\n- Dylan McConnell for assistance in interpreting PASA run types\n- Declan Heim for suggesting improvements to `nemseer` examples\n',
-    'author': 'Abhijith Prakash',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+A package for downloading and handling historical National Electricity Market (NEM) forecast data produced by the Australian Energy Market Operator (AEMO).
 
+## Installation
+
+```bash
+pip install nemseer
+```
+
+## Overview
+
+`nemseer` allows you to access historical AEMO [pre-dispatch](https://aemo.com.au/en/energy-systems/electricity/national-electricity-market-nem/data-nem/market-management-system-mms-data/pre-dispatch) and [Projected Assessment of System Adequacy (PASA)](https://wa.aemo.com.au/energy-systems/electricity/national-electricity-market-nem/nem-forecasting-and-planning/forecasting-and-reliability/projected-assessment-of-system-adequacy) forecast[^1] data available through the [MMSDM Historical Data SQLLoader](https://nemseer.readthedocs.io/en/latest/glossary.html#term-MMSDM-Historical-Data-SQLLOader). `nemseer` can then compile this data into [pandas DataFrames](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe) or [xarray Datasets](https://docs.xarray.dev/en/stable/user-guide/data-structures.html#dataset).
+
+![forecast_overview](docs/source/_static/forecast_timeframes.png)
+
+<sub><sup>Source: [Reserve services in the National Electricity Market, AEMC, 2021](https://www.aemc.gov.au/sites/default/files/2020-12/AEMC_Reserve%20services%20in%20the%20NEM%20directions%20paper_05.01.2021.pdf)</sup></sub>
+
+Whereas PASA processes are primarily used to assess resource adequacy based on technical inputs and assumptions for resources in the market (i.e. used to answer questions such as *"can operational demand be met in the forecast horizon with a sufficient safety (reserve) margin?"*), pre-dispatch processes incorporate the latest set of market participant offers and thus produce regional prices forecasts for energy and frequency control ancillary services [(FCAS)](https://aemo.com.au/-/media/files/electricity/nem/security_and_reliability/ancillary_services/guide-to-ancillary-services-in-the-national-electricity-market.pdf). Overviews of the various pre-dispatch and PASA processes can be found in the [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html).
+
+[^1]: We use the term *"forecast"* loosely, especially given that these *"forecasts"* change once participants update offer information (e.g. through rebidding) or submit revised resource availabilities and energy constraints. Both of these are intended outcomes of these *"ahead processes"*, which are run to provide system and market information to participants to inform their decision-making. However, to avoid confusion and to ensure consistency with the language used by AEMO, we use the terms *"forecast"* (or outputs) and *"forecast types"* (or ahead processes) in `nemseer`.
+
+`nemseer` enables you to download and work with data for the following forecast types. Where available, AEMO process and table descriptions are linked:
+
+1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_222.htm#1))
+2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_260.htm#1))
+3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_467.htm#1))
+4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_335.htm#1))
+5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_210.htm#1))
+
+Another helpful reference for PASA information is AEMO's [Reliability Standard Implementation Guidelines](https://www.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/rsig/reliability-standard-implementation-guidelines.pdf?la=en).
+
+### ST PASA Replacement Project
+
+Note that the methodologies for PD PASA and ST PASA are being reviewed by AEMO. In particular, the ST PASA Replacement project will combine PD PASA and ST PASA into ST PASA. For more detail, refer to the [final determination of the rule change](https://www.aemc.gov.au/sites/default/files/2022-05/ERC0332%20-%20Updating%20Short%20Term%20PASA%20-%20Final%20determination.pdf) and the [AEMO ST PASA Replacement Project home page](https://aemo.com.au/en/initiatives/trials-and-initiatives/st-pasa-replacement-project).
+
+## Usage
+
+### Glossary
+
+The [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html) contains overviews of the PASA and pre-dispatch processes, and descriptions of terminology used in `nemseer`.
+
+### Quick start
+
+Check out the [Quick start](https://nemseer.readthedocs.io/en/latest/quick_start.html) for guide on to use `nemseer`.
+
+### Examples
+
+Some use case examples have been included in the [Examples](https://nemseer.readthedocs.io/en/latest/examples.html) section of the documentation.
+
+## Contributing
+
+Interested in contributing? Check out the [contributing guidelines](./CONTRIBUTING.md), which also includes steps to install `nemseer` for development.
+
+Please note that this project is released with a [Code of Conduct](./CONDUCT.md). By contributing to this project, you agree to abide by its terms.
+
+## Citation
+
+If you use `nemseer`, please cite the package via the [Zenodo DOI](https://doi.org/10.5281/zenodo.7397514).
+
+If you use code or analysis from any of the demand error and/or price convergence examples in the documentation, please also cite `NEMOSIS` via [this conference paper](https://www.researchgate.net/publication/329798805_NEMOSIS_-_NEM_Open_Source_Information_Service_open-source_access_to_Australian_National_Electricity_Market_Data)
+
+## Licenses
+
+`nemseer` was created by Abhijith Prakash. It is licensed under the terms of [GNU GPL-3.0-or-later licences](./LICENSE).
+
+The content within the documentation for this project is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
+
+## Credits
+
+`nemseer` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+
+Development of `nemseer` was funded by the [UNSW Digital Grid Futures Institute](https://www.dgfi.unsw.edu.au/).
+
+### Contributor Acknowledgements
+
+Thanks to:
+
+- Nicholas Gorman for reviewing `nemseer` code
+- Dylan McConnell for assistance in interpreting PASA run types
+- Declan Heim for suggesting improvements to `nemseer` examples
 
-setup(**setup_kwargs)
```

