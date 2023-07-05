# Comparing `tmp/sintef-pyshop-1.4.1a0.tar.gz` & `tmp/sintef-pyshop-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.1a0.tar", last modified: Tue Jun  6 15:06:22 2023, max compression
+gzip compressed data, was "sintef-pyshop-1.4.2.tar", last modified: Wed Jul  5 14:12:37 2023, max compression
```

## Comparing `sintef-pyshop-1.4.1a0.tar` & `sintef-pyshop-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.763214 sintef-pyshop-1.4.1a0/pyshop/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.764214 sintef-pyshop-1.4.1a0/pyshop/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.766214 sintef-pyshop-1.4.1a0/pyshop/lp_model/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py
--rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-06 09:55:12.000000 sintef-pyshop-1.4.1a0/pyshop/shop_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.770214 sintef-pyshop-1.4.1a0/pyshop/shopcore/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    14831 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1859 2023-06-06 15:06:11.000000 sintef-pyshop-1.4.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.772214 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.774214 sintef-pyshop-1.4.1a0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_command.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_time.py
--rw-rw-rw-   0 root         (0) root         (0)     7580 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.172171 sintef-pyshop-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-05 14:12:37.171172 sintef-pyshop-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.147171 sintef-pyshop-1.4.2/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.151171 sintef-pyshop-1.4.2/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.155171 sintef-pyshop-1.4.2/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:59:06.000000 sintef-pyshop-1.4.2/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.163171 sintef-pyshop-1.4.2/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15145 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:12:37.172171 sintef-pyshop-1.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:14:22.000000 sintef-pyshop-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.167171 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.170171 sintef-pyshop-1.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.1a0/LICENSE` & `sintef-pyshop-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/PKG-INFO` & `sintef-pyshop-1.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.1a0
+Version: 1.4.2
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
@@ -20,53 +20,74 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+This project is archived and moved to GitLab. For more information go to https://gitlab.sintef.no/energy/shop/pyshop
+
 # pyshop
+
 Status:
 
-[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
-[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
+[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
+[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
+
+We currently offer two ways to use pyshop:
+
+1. Install pyshop through pypi (simple and quick)
+2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
+
+### Install pyshop using pypi
+
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-## 2 Download the desired SHOP binaries for your system 
+### Install pyshop using Gitlab Package Registry
+
+Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
+
+Run the command below with your personal access token:
+`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
+
+## 2 Download the desired SHOP binaries for your system
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
+
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
+
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -76,17 +97,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-    
+
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-    
+
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1a0/README.md` & `sintef-pyshop-1.4.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,67 @@
+This project is archived and moved to GitLab. For more information go to https://gitlab.sintef.no/energy/shop/pyshop
+
 # pyshop
+
 Status:
 
-[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
-[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
+[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
+[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
+
+We currently offer two ways to use pyshop:
+
+1. Install pyshop through pypi (simple and quick)
+2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
+
+### Install pyshop using pypi
+
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-## 2 Download the desired SHOP binaries for your system 
+### Install pyshop using Gitlab Package Registry
+
+Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
+
+Run the command below with your personal access token:
+`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
+
+## 2 Download the desired SHOP binaries for your system
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
+
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
+
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -50,17 +71,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-    
+
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-    
+
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.2/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/helpers/time.py` & `sintef-pyshop-1.4.2/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.2/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.2/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.2/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.2/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.2/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.2/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shop_runner.py` & `sintef-pyshop-1.4.2/pyshop/shop_runner.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.2/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.2/pyshop/shopcore/model_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.2/pyshop/shopcore/script_generator.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.2/pyshop/shopcore/shop_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Union
 import numpy as np
 import pandas as pd
 
 from ..helpers.typing_annotations import ShopApi, ShopDatatypes, XyType
 from ..helpers.time import get_shop_datetime, get_shop_timestring
-from ..helpers.timeseries import create_constant_time_series, get_timestamp_indexed_series, resample_resolution
+from ..helpers.timeseries import get_timestamp_indexed_series
 
 def get_attribute_value(shop_api:ShopApi, object_name:str, object_type:str, attribute_name:str, datatype:str, dataframe:bool=True) -> ShopDatatypes:
     value = None
     if datatype == 'int':
         value = shop_api.GetIntValue(object_type, object_name, attribute_name)
     elif datatype == 'int_array':
         value = list(shop_api.GetIntArray(object_type, object_name, attribute_name))
@@ -250,62 +250,67 @@
         
         #Note that times is a regular python list while n, x, and y are np arrays
         shop_api.SetXyTCurve(object_type, object_name, attribute_name, times, n, x, y)        
 
     elif datatype == 'txy':
         time = get_time_resolution(shop_api)
 
-        # Make sure we continue on with a Series or a DataFrame
+        opt_start_string = get_shop_timestring(time['starttime'])
+
+        # Constant value can be set straight away
         if isinstance(value, float) or isinstance(value, int):
-            df = create_constant_time_series(value, time['starttime'])
-        else:
-            df = value
+            shop_api.SetTxySeries(object_type, object_name, attribute_name, opt_start_string, np.array([0]), np.array([value]))
+            return
 
+        #Time series is given as pandas Series or DataFrame
+        df = value
+
+        #Empty data frame
         if df.shape[0] == 0:
             shop_api.SetTxySeries(
                 object_type, object_name, attribute_name,
                 get_shop_timestring(time['starttime']), [], []
             )
             return
 
-        # Extract data in time interval
-        if df.loc[time['starttime']:time['starttime']].empty:
-            df.loc[time['starttime']] = df.loc[:time['starttime']].iloc[-1]
-            df.sort_index(inplace=True)
-        df = df.loc[time['starttime']:time['endtime']]
-
-        # Get scaling factor
-        freq = 'H'
-        delta = 1/3600
-        if time['timeunit'] == 'minute':
-            freq = 'T'
-            delta = 1/60
-        elif time['timeunit'] == 'second':
-            freq = 'S'
-            delta = 1
         txy_start_time = df.index[0]
+        txy_start_str = get_shop_timestring(txy_start_time)
 
-        # If we have a non-constant time resolution, we need to resample input accordingly
-        if time['timeresolution'].shape[0] > 1:
-            if df.index[-1] != time['endtime']:
-                if isinstance(df, pd.DataFrame):
-                    new_row = pd.DataFrame(df[-1:].values, index=[time['endtime']], columns=df.columns)
-                else:
-                    new_row = pd.Series(df[-1], index=[time['endtime']])
-                df = pd.concat([df, new_row])
-            df = df.asfreq(freq=freq, method='ffill')
-            df = df[:-1]
-            time_resolution = pd.Series(data=shop_api.GetTimeResolutionY(), index=shop_api.GetTimeResolutionT())
-            df = resample_resolution(time, df, delta, time_resolution)
-            t = df.index
-        else:
-            t = (df.index - time['starttime']).total_seconds() * delta
-        y = df.values
-        shop_api.SetTxySeries(object_type, object_name, attribute_name, get_shop_timestring(txy_start_time),
-                              t.astype(int), y)
+        #If the dataframe is of length one, it is equivalent to setting a constant value starting at the txy start time
+        if len(df.index) == 1:
+            shop_api.SetTxySeries(object_type, object_name, attribute_name, txy_start_str, np.array([0]), df.values)
+            return
+
+        #Time vector in seconds
+        t = np.array([(t-txy_start_time).seconds for t in df.index])
+
+        #Convert to the time unit of the optimization
+        if time['timeunit'] == 'minute':
+            t = t * 1.0/60
+        elif time['timeunit'] == 'hour':
+            t = t * 1.0/3600
+
+        #Calculate the diff between all consecutive time steps and check if any are smaller than 1
+        dt = np.ediff1d(t)
+        smallest_dt = np.amin(dt)
+
+        if smallest_dt < 1.0:
+            print(f"""Warning: TXY {attribute_name} on {object_type} {object_name} has higher resolution than the time unit of the optimization. 
+                  Resampling will be done with averaging and front fill, precision may be lost""")
+
+            #Resample time series with the time unit used in the optimization
+            #Take the average when a lot of data is given within a single time step
+            if time['timeunit'] == 'minute':
+                df = df.resample("min").mean().ffill()
+                t = np.array([(t-txy_start_time).seconds/60.0 for t in df.index])
+            elif time['timeunit'] == 'hour':
+                df = df.resample("H").mean().ffill()
+                t = np.array([(t-txy_start_time).seconds/3600.0 for t in df.index])
+ 
+        shop_api.SetTxySeries(object_type, object_name, attribute_name, txy_start_str, t.astype(int), df.values)
 
 
 def get_time_resolution(shop_api:ShopApi) -> Dict[str,Any]:
     tz_name = get_shop_timzone_name(shop_api)
     starttime = get_shop_datetime(shop_api.GetStartTime(), tz_name)
     endtime = get_shop_datetime(shop_api.GetEndTime(), tz_name)
     timeunit = shop_api.GetTimeUnit()
```

### Comparing `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.2/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/setup.py` & `sintef-pyshop-1.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import os
 import pathlib
 from distutils.core import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(name='sintef-pyshop',
-      version='1.4.1-alpha',
+      version=os.getenv('CI_COMMIT_TAG'),
       author='SINTEF Energy Research',
       description='Python interface to SHOP',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['pyshop',
                 'pyshop.helpers',
                 'pyshop.shopcore',
```

### Comparing `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.2/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.1a0
+Version: 1.4.2
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
@@ -20,53 +20,74 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+This project is archived and moved to GitLab. For more information go to https://gitlab.sintef.no/energy/shop/pyshop
+
 # pyshop
+
 Status:
 
-[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
-[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
+[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
+[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
+
+We currently offer two ways to use pyshop:
+
+1. Install pyshop through pypi (simple and quick)
+2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
+
+### Install pyshop using pypi
+
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-## 2 Download the desired SHOP binaries for your system 
+### Install pyshop using Gitlab Package Registry
+
+Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
+
+Run the command below with your personal access token:
+`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
+
+## 2 Download the desired SHOP binaries for your system
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
+
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
+
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -76,17 +97,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-    
+
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-    
+
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.2/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/tests/test_helpers_command.py` & `sintef-pyshop-1.4.2/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/tests/test_helpers_time.py` & `sintef-pyshop-1.4.2/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1a0/tests/test_shop_api.py` & `sintef-pyshop-1.4.2/tests/test_shop_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,17 +164,32 @@
         assert (res[4] == self.shop_api['GetTxySeriesT']).all()
         assert (res[5] == self.shop_api['GetTxySeriesY']).all()
 
     def test_set_constant_txy(self):
         set_attribute(self.shop_api, 'obj_name', 'obj_type', 'attr_name', 'txy', 1.1)
         res = self.shop_api['SetTxySeries']
         assert res[3].startswith(self.shop_api['GetStartTime'])
-        assert (res[4] == self.shop_api['GetTxySeriesT']).all()
+        assert (np.abs(res[4]) < 1e-15).all()
         assert (np.abs(res[5] - 1.1) < 1e-15).all()
 
+    def test_set_hig_res_txy(self):
+
+        starttime = pd.Timestamp(self.shop_api['GetStartTime'])
+        y = [1,2,3,4,5]
+        txy_val = pd.Series(
+            y,
+            index=[starttime + pd.Timedelta(seconds=30*t) for t in range(len(y))]
+        )
+
+        set_attribute(self.shop_api, 'obj_name', 'obj_type', 'attr_name', 'txy', txy_val)
+        res = self.shop_api['SetTxySeries']
+        assert res[3].startswith(self.shop_api['GetStartTime'])
+        assert (np.abs(res[4] - np.array([0, 1, 2])) < 1e-15).all()
+        assert (np.abs(res[5] - np.array([1.5, 3.5, 5])) < 1e-15).all()
+
 
 class TestTime:
     shop_api = ShopApiMock()
 
     def test_get_time_resolution(self):
         timeres = get_time_resolution(self.shop_api)
         assert timeres['starttime'] == pd.Timestamp(self.shop_api['GetStartTime'])
```

