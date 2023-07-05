# Comparing `tmp/multimodal_autoencoders-0.2.1.tar.gz` & `tmp/multimodal_autoencoders-0.2.2.tar.gz`

## Comparing `multimodal_autoencoders-0.2.1.tar` & `multimodal_autoencoders-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/__init__.py
--rw-r--r--   0        0        0    44971 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/joint_trainer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/autoencoder.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/base_dataset.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/data_loader/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/data_loader/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/__init__.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/classifiers.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/decoders.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/encoders.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/metric.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/LICENSE
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/README.md
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/hatch.toml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/__init__.py
+-rw-r--r--   0        0        0    44971 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/joint_trainer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/autoencoder.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/base_dataset.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/data_loader/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/data_loader/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/__init__.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/classifiers.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/decoders.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/encoders.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/metric.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/README.md
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/hatch.toml
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 multimodal_autoencoders-0.2.2/PKG-INFO
```

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/joint_trainer.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/joint_trainer.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/autoencoder.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/autoencoder.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/base_dataset.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/base/base_model.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/base/base_model.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/data_loader/datasets.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/data_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/classifiers.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/classifiers.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/decoders.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/decoders.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/encoders.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/encoders.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/multimodal_autoencoders/model/metric.py` & `multimodal_autoencoders-0.2.2/multimodal_autoencoders/model/metric.py`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/.gitignore` & `multimodal_autoencoders-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/LICENSE` & `multimodal_autoencoders-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/README.md` & `multimodal_autoencoders-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ChemBioMultimodalAutoencoders
  
 
 <div>
 
  |||
 | --- | --- |
-| CI/CD | [![tests](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-test.yml/badge.svg?branch=main)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-test.yml) [![builds](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml) |
+| CI/CD | [![tests](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-tests.yml/badge.svg?branch=main)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-tests.yml) [![builds](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/multimodal-autoencoders.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/multimodal-autoencoders/) ![Downloads](https://static.pepy.tech/badge/multimodal-autoencoders)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/multimodal-autoencoders.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/multimodal-autoencoders/) |
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![imports - isort](https://img.shields.io/badge/imports-isort-ef8336.svg)](https://github.com/pycqa/isort) [![LICENSE](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/blob/readme-update/license.txt)
 
  
 
 </div>
```

### Comparing `multimodal_autoencoders-0.2.1/hatch.toml` & `multimodal_autoencoders-0.2.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `multimodal_autoencoders-0.2.1/pyproject.toml` & `multimodal_autoencoders-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,20 @@
     { name = "Thibault, Bechtler", email = "th.bechtler@gmail.com" },
     { name = "Bartosz, Baranowski", email = "bartosz.baranowski@novartis.com" },
 ]
 contributors = [
     { name = "Steffen, Renner", email = "steffen.renner@novartis.com" },
     { name = "Michal, Pikusa", email = "michal.pikusa@novartis.com" },
 ]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+]
 dependencies = [
     "dataclasses",
     "numpy",
     "scikit-learn",
     "torch",
 ]
 
@@ -33,17 +39,17 @@
 ]
 exclude = [
   "/.github",
   "/.git",
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/multimodal_autoencoders#readme"
-Issues = "https://github.com/unknown/multimodal_autoencoders/issues"
-Source = "https://github.com/unknown/multimodal_autoencoders"
+Documentation = "https://github.com/Novartis/ChemBioMultimodalAutoencoders#readme"
+Issues = "https://github.com/Novartis/ChemBioMultimodalAutoencoders/issues"
+Source = "https://github.com/Novartis/ChemBioMultimodalAutoencoders"
 
 [tool.mypy]
 disallow_untyped_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
```

### Comparing `multimodal_autoencoders-0.2.1/PKG-INFO` & `multimodal_autoencoders-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: multimodal_autoencoders
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pytorch reimplementation of https://www.nature.com/articles/s41467-020-20249-2 for streamlined multidomain data integration and translation based on cross-modal autoencoders architectures
-Project-URL: Documentation, https://github.com/unknown/multimodal_autoencoders#readme
-Project-URL: Issues, https://github.com/unknown/multimodal_autoencoders/issues
-Project-URL: Source, https://github.com/unknown/multimodal_autoencoders
+Project-URL: Documentation, https://github.com/Novartis/ChemBioMultimodalAutoencoders#readme
+Project-URL: Issues, https://github.com/Novartis/ChemBioMultimodalAutoencoders/issues
+Project-URL: Source, https://github.com/Novartis/ChemBioMultimodalAutoencoders
 Author-email: "Thibault, Bechtler" <th.bechtler@gmail.com>, "Bartosz, Baranowski" <bartosz.baranowski@novartis.com>
 License-Expression: MIT
 License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dataclasses
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: torch
 Description-Content-Type: text/markdown
 
 # ChemBioMultimodalAutoencoders
  
 
 <div>
 
  |||
 | --- | --- |
-| CI/CD | [![tests](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-test.yml/badge.svg?branch=main)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-test.yml) [![builds](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml) |
+| CI/CD | [![tests](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-tests.yml/badge.svg?branch=main)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/python-package-tests.yml) [![builds](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/actions/workflows/build-and-publish.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/multimodal-autoencoders.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/multimodal-autoencoders/) ![Downloads](https://static.pepy.tech/badge/multimodal-autoencoders)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/multimodal-autoencoders.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/multimodal-autoencoders/) |
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![imports - isort](https://img.shields.io/badge/imports-isort-ef8336.svg)](https://github.com/pycqa/isort) [![LICENSE](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/Novartis/ChemBioMultimodalAutoencoders/blob/readme-update/license.txt)
 
  
 
 </div>
```

