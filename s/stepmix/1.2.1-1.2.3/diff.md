# Comparing `tmp/stepmix-1.2.1.tar.gz` & `tmp/stepmix-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.2.1.tar", last modified: Mon Jun 26 18:13:50 2023, max compression
+gzip compressed data, was "stepmix-1.2.3.tar", last modified: Wed Jul  5 17:44:45 2023, max compression
```

## Comparing `stepmix-1.2.1.tar` & `stepmix-1.2.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.2.1/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.2.1/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.2.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.2.1/README-dev.md
--rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.2.1/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.2.1/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.2.1/docs/make.bat
--rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.2.1/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-06-26 18:09:07.154854 stepmix-1.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.2.1/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.2.1/docs/source/installation.rst
--rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.2.1/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1884 2023-06-26 18:09:07.154854 stepmix-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/README.md
--rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-06-26 18:09:07.154854 stepmix-1.2.1/stepmix/__init__.py
--rw-r--r--   0        0        0    10523 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.2.1/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     8129 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.2.1/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6162 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.2.1/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.2.1/stepmix/emission/nested.py
--rw-r--r--   0        0        0    57922 2023-06-26 18:00:08.954995 stepmix-1.2.1/stepmix/stepmix.py
--rw-r--r--   0        0        0    19721 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.2.1/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.2.1/test/test_benchmarks.py
--rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.2.1/test/test_bootstrap.py
--rw-r--r--   0        0        0      735 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_buffers.py
--rw-r--r--   0        0        0    10743 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.2.1/test/test_fiml.py
--rw-r--r--   0        0        0     1944 2023-06-26 18:00:08.954995 stepmix-1.2.1/test/test_inputs.py
--rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.2.1/test/test_progress_bar.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.2.1/test/test_random_state.py
--rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.2.1/test/test_sample_weight.py
--rw-r--r--   0        0        0      792 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.2.1/test/test_steps.py
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.2.3/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.2.3/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.2.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.2.3/README-dev.md
+-rw-r--r--   0        0        0     4627 2023-07-05 16:04:05.023728 stepmix-1.2.3/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.2.3/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.2.3/docs/make.bat
+-rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.2.3/docs/source/api.rst
+-rw-r--r--   0        0        0     1075 2023-07-05 17:41:21.892644 stepmix-1.2.3/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.2.3/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.2.3/docs/source/installation.rst
+-rw-r--r--   0        0        0     2468 2023-07-05 17:20:09.532154 stepmix-1.2.3/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1884 2023-07-05 17:41:21.888644 stepmix-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.2.3/scripts/README.md
+-rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.2.3/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.2.3/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-07-05 17:41:21.888644 stepmix-1.2.3/stepmix/__init__.py
+-rw-r--r--   0        0        0    10523 2023-06-19 18:10:28.893235 stepmix-1.2.3/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.2.3/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.2.3/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.2.3/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.2.3/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     8129 2023-06-19 18:10:28.893235 stepmix-1.2.3/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.2.3/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6162 2023-06-19 18:10:28.893235 stepmix-1.2.3/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15625 2023-07-05 15:43:03.863066 stepmix-1.2.3/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.2.3/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    58231 2023-07-05 15:43:03.863066 stepmix-1.2.3/stepmix/stepmix.py
+-rw-r--r--   0        0        0    19721 2023-06-19 18:10:28.893235 stepmix-1.2.3/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.2.3/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.2.3/test/test_benchmarks.py
+-rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.2.3/test/test_bootstrap.py
+-rw-r--r--   0        0        0      735 2023-06-19 18:10:28.893235 stepmix-1.2.3/test/test_buffers.py
+-rw-r--r--   0        0        0     9370 2023-07-05 15:43:03.867066 stepmix-1.2.3/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.2.3/test/test_fiml.py
+-rw-r--r--   0        0        0     1944 2023-06-26 18:00:08.954995 stepmix-1.2.3/test/test_inputs.py
+-rw-r--r--   0        0        0     3943 2023-07-05 15:43:03.867066 stepmix-1.2.3/test/test_n_parameters.py
+-rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.2.3/test/test_progress_bar.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.2.3/test/test_random_state.py
+-rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.2.3/test/test_sample_weight.py
+-rw-r--r--   0        0        0      792 2023-06-19 18:10:28.893235 stepmix-1.2.3/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.2.3/test/test_steps.py
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 stepmix-1.2.3/PKG-INFO
```

### Comparing `stepmix-1.2.1/.github/workflows/pytest.yaml` & `stepmix-1.2.3/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/LICENSE` & `stepmix-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/README-dev.md` & `stepmix-1.2.3/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/README.md` & `stepmix-1.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,55 +29,33 @@
 
 # Install
 You can install StepMix with pip, preferably in a virtual environment: 
 ```
 pip install stepmix
 ``` 
 # Quickstart
-A simple StepMix mixture using the continuous variables of the Iris Dataset:
+A StepMix mixture using categorical variables on a preloaded data matrix. StepMix accepts either `numpy.array`or 
+`pandas.DataFrame`. Categories should be integer-encoded and 0-indexed.
 
 ```python
-import pandas as pd
-from sklearn.datasets import load_iris
-from sklearn.metrics import rand_score
-
 from stepmix.stepmix import StepMix
 
-# Load dataset in a Dataframe
-data_continuous, target = load_iris(return_X_y=True, as_frame=True)
-
-# Continuous StepMix Model with 3 latent classes
-model = StepMix(n_components=3, measurement="continuous", verbose=0, random_state=123)
-
-# Fit model and predict clusters
-model.fit(data_continuous)
-pred_continuous = model.predict(data_continuous)
+# Categorical StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="categorical")
+model.fit(data)
 
-# A Rand score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_continuous, target))
+# Allow missing values
+model_nan = StepMix(n_components=3, measurement="categorical_nan")
+model_nan.fit(data_nan)
 ```
-StepMix also provides support for categorical mixtures:
+For binary data you can also use `measurement="binary"` or `measurement="binary_nan"`. For continuous data, you can fit a Gaussian Mixture with diagonal covariances using `measurement="continuous"` or `measurement="continuous_nan"`.
 
-```python
-# Create categorical data based on the Iris Dataset quantiles
-data_categorical = data_continuous.copy()
-for col in data_categorical:
-   data_categorical[col] = pd.qcut(data_continuous[col], q=3).cat.codes
+Set `verbose=1` for a detailed output.
 
-# Categorical StepMix Model with 3 latent classes
-model = StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
-
-# Fit model and predict clusters
-model.fit(data_categorical)
-pred_categorical = model.predict(data_categorical)
-
-# A Rand score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_categorical, target))
-```
-Please refer to the StepMix tutorials to learn how to handle missing values and combine continuous and categorical data in the same model.
+Please refer to the StepMix tutorials to learn how to combine continuous and categorical data in the same model.
 # Tutorials
 Detailed tutorials are available in notebooks: 
 1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): 
 an in-depth look at how latent class models can be defined with StepMix. The tutorial uses the Iris Dataset as an example
 and covers:
    1. Continuous LCA models (latent profile analysis/gaussian mixture model);
    2. Binary LCA models;
```

#### html2text {}

```diff
@@ -19,36 +19,28 @@
 please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
 ``` @article{morin2023stepmix, title={StepMix: A Python Package for Pseudo-
 Likelihood Estimation of Generalized Mixture Models with External Variables},
 author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re,
 Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
 journal={arXiv preprint arXiv:2304.03853}, year={2023} } ``` # Install You can
 install StepMix with pip, preferably in a virtual environment: ``` pip install
-stepmix ``` # Quickstart A simple StepMix mixture using the continuous
-variables of the Iris Dataset: ```python import pandas as pd from
-sklearn.datasets import load_iris from sklearn.metrics import rand_score from
-stepmix.stepmix import StepMix # Load dataset in a Dataframe data_continuous,
-target = load_iris(return_X_y=True, as_frame=True) # Continuous StepMix Model
-with 3 latent classes model = StepMix(n_components=3, measurement="continuous",
-verbose=0, random_state=123) # Fit model and predict clusters model.fit
-(data_continuous) pred_continuous = model.predict(data_continuous) # A Rand
-score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_continuous, target)) ``` StepMix also provides support
-for categorical mixtures: ```python # Create categorical data based on the Iris
-Dataset quantiles data_categorical = data_continuous.copy() for col in
-data_categorical: data_categorical[col] = pd.qcut(data_continuous[col],
-q=3).cat.codes # Categorical StepMix Model with 3 latent classes model =
-StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
-# Fit model and predict clusters model.fit(data_categorical) pred_categorical =
-model.predict(data_categorical) # A Rand score close to 1 indicates good
-alignment between clusters and flower types print(rand_score(pred_categorical,
-target)) ``` Please refer to the StepMix tutorials to learn how to handle
-missing values and combine continuous and categorical data in the same model. #
-Tutorials Detailed tutorials are available in notebooks: 1. [Generalized
-Mixture Models with StepMix](https://colab.research.google.com/drive/
+stepmix ``` # Quickstart A StepMix mixture using categorical variables on a
+preloaded data matrix. StepMix accepts either `numpy.array`or
+`pandas.DataFrame`. Categories should be integer-encoded and 0-indexed.
+```python from stepmix.stepmix import StepMix # Categorical StepMix Model with
+3 latent classes model = StepMix(n_components=3, measurement="categorical")
+model.fit(data) # Allow missing values model_nan = StepMix(n_components=3,
+measurement="categorical_nan") model_nan.fit(data_nan) ``` For binary data you
+can also use `measurement="binary"` or `measurement="binary_nan"`. For
+continuous data, you can fit a Gaussian Mixture with diagonal covariances using
+`measurement="continuous"` or `measurement="continuous_nan"`. Set `verbose=1`
+for a detailed output. Please refer to the StepMix tutorials to learn how to
+combine continuous and categorical data in the same model. # Tutorials Detailed
+tutorials are available in notebooks: 1. [Generalized Mixture Models with
+StepMix](https://colab.research.google.com/drive/
 1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): an in-depth look at how latent
 class models can be defined with StepMix. The tutorial uses the Iris Dataset as
 an example and covers: 1. Continuous LCA models (latent profile analysis/
 gaussian mixture model); 2. Binary LCA models; 3. Categorical LCA models; 3.
 Mixed variables mixture models (continuous and categorical data); 5. Missing
 Values through Full-Information Maximum Likelihood. 2. [Stepwise Estimation
 with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-
```

### Comparing `stepmix-1.2.1/docs/Makefile` & `stepmix-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/docs/make.bat` & `stepmix-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/docs/source/api.rst` & `stepmix-1.2.3/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/docs/source/index.rst` & `stepmix-1.2.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/docs/source/tutorials.rst` & `stepmix-1.2.3/docs/source/tutorials.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,28 @@
 Tutorials
 =========
 Quickstart
 ----------
-The following shows a simple StepMix mixture using the continuous variables of the Iris Dataset. ``n_components`` controls
-the number of latent classes.::
-
-    import pandas as pd
-    from sklearn.datasets import load_iris
-    from sklearn.metrics import rand_score
+A StepMix mixture using categorical variables on a preloaded data matrix. StepMix accepts either ``numpy.array`` or ``pandas.DataFrame``. Categories should be integer-encoded and 0-indexed. ::
 
     from stepmix.stepmix import StepMix
 
-    # Load dataset in a Dataframe
-    data_continuous, target = load_iris(return_X_y=True, as_frame=True)
-
-    # Continuous StepMix Model with 3 latent classes
-    model = StepMix(n_components=3, measurement="continuous", verbose=1, random_state=123)
-
-    # Fit model and predict clusters
-    model.fit(data_continuous)
-    pred_continuous = model.predict(data_continuous)
-
-    # A Rand score close to 1 indicates good alignment between clusters and flower types
-    print(rand_score(pred_continuous, target))
-
-The API allows to easily predict class memberships or probabilities::
-
-    class_ids = model.predict(X, Y)
-    class_probs = model.predict_proba(X, Y)
-
-StepMix also provides support for categorical mixtures::
-
-    # Create categorical data based on the Iris Dataset quantiles
-    data_categorical = data_continuous.copy()
-    for col in data_categorical:
-       data_categorical[col] = pd.qcut(data_continuous[col], q=3).cat.codes
-
     # Categorical StepMix Model with 3 latent classes
-    model = StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
+    model = StepMix(n_components=3, measurement="categorical")
+    model.fit(data)
 
-    # Fit model and predict clusters
-    model.fit(data_categorical)
-    pred_categorical = model.predict(data_categorical)
+    # Allow missing values
+    model_nan = StepMix(n_components=3, measurement="categorical_nan")
+    model_nan.fit(data_nan)
 
-    # A Rand score close to 1 indicates good alignment between clusters and flower types
-    print(rand_score(pred_categorical, target))
+For binary data you can also use ``measurement="binary"`` or ``measurement="binary_nan"``. For continuous data, you can fit a Gaussian Mixture with diagonal covariances using ``measurement="continuous"`` or ``measurement="continuous_nan"``.
 
-Input Data
-----------
-StepMix accepts the ``numpy.array`` and ``pandas.DataFrame`` data types. Additionally, emission models suffixed with
-``_nan`` support missing values denoted by ``np.NaN``.
+Set ``verbose=1`` for a detailed output.
+
+Please refer to the StepMix tutorials to learn how to combine continuous and categorical data in the same model.
 
 Advanced Usage
 --------------
 For all available options, please refer to the :doc:`api` documentation.
 Detailed tutorials are available in notebooks :
 
 #. `Latent Class Analysis with StepMix <https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing>`_ : an in-depth look at how latent class models can be defined with StepMix. The tutorial uses the Iris Dataset as an example and covers
```

### Comparing `stepmix-1.2.1/pyproject.toml` & `stepmix-1.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.2.1/scripts/README.md` & `stepmix-1.2.3/scripts/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/scripts/run_bakk_simulation.py` & `stepmix-1.2.3/scripts/run_bakk_simulation.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/scripts/run_bakk_simulation_complete.py` & `stepmix-1.2.3/scripts/run_bakk_simulation_complete.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/bootstrap.py` & `stepmix-1.2.3/stepmix/bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/corrections.py` & `stepmix-1.2.3/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/datasets.py` & `stepmix-1.2.3/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/emission/build_emission.py` & `stepmix-1.2.3/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/emission/categorical.py` & `stepmix-1.2.3/stepmix/emission/categorical.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/emission/covariate.py` & `stepmix-1.2.3/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/emission/emission.py` & `stepmix-1.2.3/stepmix/emission/emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/emission/gaussian.py` & `stepmix-1.2.3/stepmix/emission/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,19 @@
             covariances=self.covariances_,
             tied=self.covariance_type == "tied",
         )
 
     @property
     def n_parameters(self):
         n = GaussianMixture._n_parameters(self)
+
+        # Remove class weights from the count
+        # We add them back in the main StepMix class
+        n -= self.n_components - 1
+
         return n
 
     def permute_classes(self, perm, axis=0):
         # Latent classes are on first axis
         self.means_ = self.means_[perm]
 
         # Tied has a single covariance (and precisions) shared among all classes
```

### Comparing `stepmix-1.2.1/stepmix/emission/nested.py` & `stepmix-1.2.3/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/stepmix/stepmix.py` & `stepmix-1.2.3/stepmix/stepmix.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,23 @@
         if init_emission:
             self._sm.initialize(Y, np.exp(self.log_resp_), random_state)
 
     @property
     def n_parameters(self):
         """Get number of free parameters."""
         check_is_fitted(self)
-        n = self.n_components - 1 + self._mm.n_parameters
+
+        # Only include class weights dof if they are used for likelihood computations
+        # Class weights are not used in the conditional perspective (e.g., covariate models)
+        n = (self.n_components - 1) if self._class_weight_likelihood else 0
+
+        # Measurement parameters
+        n += self._mm.n_parameters
+
+        # Optional structural parameters
         if hasattr(self, "_sm"):
             n += self._sm.n_parameters
         return n
 
     def _check_x_y(self, X=None, Y=None, reset=False):
         """Input validation function.
```

### Comparing `stepmix-1.2.1/stepmix/utils.py` & `stepmix-1.2.3/stepmix/utils.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/conftest.py` & `stepmix-1.2.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_benchmarks.py` & `stepmix-1.2.3/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_bootstrap.py` & `stepmix-1.2.3/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_buffers.py` & `stepmix-1.2.3/test/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_emission.py` & `stepmix-1.2.3/test/test_emission.py`

 * *Files 8% similar despite different names*

```diff
@@ -314,56 +314,7 @@
     model = StepMix(
         n_components=3, measurement="categorical", verbose=1, random_state=123
     )
 
     model.fit(train)
 
     preds = model.predict(test)
-
-
-@pytest.mark.filterwarnings(
-    "ignore::sklearn.exceptions.ConvergenceWarning"
-)  # Ignore convergence warnings
-def test_categorical_n_parameters():
-    """Test number of parameters of a simple categorical mixture."""
-    rng = np.random.default_rng(42)
-    data = rng.choice(a=[0, 1, 2], size=200).reshape(-1, 1)
-
-    model = StepMix(
-        n_components=3,
-        measurement="categorical",
-        random_state=42,
-        verbose=0,
-        max_iter=5000,
-        n_init=1,
-    )
-
-    model.fit(data)
-
-    assert model.n_parameters == 8
-
-
-@pytest.mark.filterwarnings(
-    "ignore::sklearn.exceptions.ConvergenceWarning"
-)  # Ignore convergence warnings
-def test_categorical_n_parameters_max():
-    """Test number of parameters of a categorical mixture where some categorical features have fewer outcomes."""
-    rng = np.random.default_rng(42)
-    data_1 = rng.choice(a=[0, 1, 2, 3], size=300).reshape(-1, 1)
-    data_2 = rng.choice(a=[0, 1, 2], size=300).reshape(-1, 1)
-    data_3 = rng.choice(a=[0, 1], size=300).reshape(-1, 1)
-    data = np.hstack((data_1, data_2, data_3))
-
-    model = StepMix(
-        n_components=4,
-        measurement="categorical",
-        random_state=42,
-        verbose=0,
-        max_iter=5000,
-        n_init=1,
-    )
-
-    model.fit(data)
-
-    n_parameters = (4 - 1) + 4 * (1 + 2 + 3)
-
-    assert model.n_parameters == n_parameters
```

### Comparing `stepmix-1.2.1/test/test_fiml.py` & `stepmix-1.2.3/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_inputs.py` & `stepmix-1.2.3/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_random_state.py` & `stepmix-1.2.3/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_sample_weight.py` & `stepmix-1.2.3/test/test_sample_weight.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_sklearn.py` & `stepmix-1.2.3/test/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/test/test_steps.py` & `stepmix-1.2.3/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.1/PKG-INFO` & `stepmix-1.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -55,55 +55,33 @@
 
 # Install
 You can install StepMix with pip, preferably in a virtual environment: 
 ```
 pip install stepmix
 ``` 
 # Quickstart
-A simple StepMix mixture using the continuous variables of the Iris Dataset:
+A StepMix mixture using categorical variables on a preloaded data matrix. StepMix accepts either `numpy.array`or 
+`pandas.DataFrame`. Categories should be integer-encoded and 0-indexed.
 
 ```python
-import pandas as pd
-from sklearn.datasets import load_iris
-from sklearn.metrics import rand_score
-
 from stepmix.stepmix import StepMix
 
-# Load dataset in a Dataframe
-data_continuous, target = load_iris(return_X_y=True, as_frame=True)
-
-# Continuous StepMix Model with 3 latent classes
-model = StepMix(n_components=3, measurement="continuous", verbose=0, random_state=123)
-
-# Fit model and predict clusters
-model.fit(data_continuous)
-pred_continuous = model.predict(data_continuous)
+# Categorical StepMix Model with 3 latent classes
+model = StepMix(n_components=3, measurement="categorical")
+model.fit(data)
 
-# A Rand score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_continuous, target))
+# Allow missing values
+model_nan = StepMix(n_components=3, measurement="categorical_nan")
+model_nan.fit(data_nan)
 ```
-StepMix also provides support for categorical mixtures:
+For binary data you can also use `measurement="binary"` or `measurement="binary_nan"`. For continuous data, you can fit a Gaussian Mixture with diagonal covariances using `measurement="continuous"` or `measurement="continuous_nan"`.
 
-```python
-# Create categorical data based on the Iris Dataset quantiles
-data_categorical = data_continuous.copy()
-for col in data_categorical:
-   data_categorical[col] = pd.qcut(data_continuous[col], q=3).cat.codes
+Set `verbose=1` for a detailed output.
 
-# Categorical StepMix Model with 3 latent classes
-model = StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
-
-# Fit model and predict clusters
-model.fit(data_categorical)
-pred_categorical = model.predict(data_categorical)
-
-# A Rand score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_categorical, target))
-```
-Please refer to the StepMix tutorials to learn how to handle missing values and combine continuous and categorical data in the same model.
+Please refer to the StepMix tutorials to learn how to combine continuous and categorical data in the same model.
 # Tutorials
 Detailed tutorials are available in notebooks: 
 1. [Generalized Mixture Models with StepMix](https://colab.research.google.com/drive/1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): 
 an in-depth look at how latent class models can be defined with StepMix. The tutorial uses the Iris Dataset as an example
 and covers:
    1. Continuous LCA models (latent profile analysis/gaussian mixture model);
    2. Binary LCA models;
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.2.1 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.2.3 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
@@ -37,36 +37,28 @@
 please consider citing our [arXiv preprint](https://arxiv.org/abs/2304.03853):
 ``` @article{morin2023stepmix, title={StepMix: A Python Package for Pseudo-
 Likelihood Estimation of Generalized Mixture Models with External Variables},
 author={Morin, Sacha and Legault, Robin and Bakk, Zsuzsa and Gigu{\`e}re,
 Charles-{\'E}douard and de la Sablonni{\`e}re, Roxane and Lacourse, {\'E}ric},
 journal={arXiv preprint arXiv:2304.03853}, year={2023} } ``` # Install You can
 install StepMix with pip, preferably in a virtual environment: ``` pip install
-stepmix ``` # Quickstart A simple StepMix mixture using the continuous
-variables of the Iris Dataset: ```python import pandas as pd from
-sklearn.datasets import load_iris from sklearn.metrics import rand_score from
-stepmix.stepmix import StepMix # Load dataset in a Dataframe data_continuous,
-target = load_iris(return_X_y=True, as_frame=True) # Continuous StepMix Model
-with 3 latent classes model = StepMix(n_components=3, measurement="continuous",
-verbose=0, random_state=123) # Fit model and predict clusters model.fit
-(data_continuous) pred_continuous = model.predict(data_continuous) # A Rand
-score close to 1 indicates good alignment between clusters and flower types
-print(rand_score(pred_continuous, target)) ``` StepMix also provides support
-for categorical mixtures: ```python # Create categorical data based on the Iris
-Dataset quantiles data_categorical = data_continuous.copy() for col in
-data_categorical: data_categorical[col] = pd.qcut(data_continuous[col],
-q=3).cat.codes # Categorical StepMix Model with 3 latent classes model =
-StepMix(n_components=3, measurement="categorical", verbose=0, random_state=123)
-# Fit model and predict clusters model.fit(data_categorical) pred_categorical =
-model.predict(data_categorical) # A Rand score close to 1 indicates good
-alignment between clusters and flower types print(rand_score(pred_categorical,
-target)) ``` Please refer to the StepMix tutorials to learn how to handle
-missing values and combine continuous and categorical data in the same model. #
-Tutorials Detailed tutorials are available in notebooks: 1. [Generalized
-Mixture Models with StepMix](https://colab.research.google.com/drive/
+stepmix ``` # Quickstart A StepMix mixture using categorical variables on a
+preloaded data matrix. StepMix accepts either `numpy.array`or
+`pandas.DataFrame`. Categories should be integer-encoded and 0-indexed.
+```python from stepmix.stepmix import StepMix # Categorical StepMix Model with
+3 latent classes model = StepMix(n_components=3, measurement="categorical")
+model.fit(data) # Allow missing values model_nan = StepMix(n_components=3,
+measurement="categorical_nan") model_nan.fit(data_nan) ``` For binary data you
+can also use `measurement="binary"` or `measurement="binary_nan"`. For
+continuous data, you can fit a Gaussian Mixture with diagonal covariances using
+`measurement="continuous"` or `measurement="continuous_nan"`. Set `verbose=1`
+for a detailed output. Please refer to the StepMix tutorials to learn how to
+combine continuous and categorical data in the same model. # Tutorials Detailed
+tutorials are available in notebooks: 1. [Generalized Mixture Models with
+StepMix](https://colab.research.google.com/drive/
 1KAxcvxjL_vB2lAG9e47we7hrf_2fR1eK?usp=sharing): an in-depth look at how latent
 class models can be defined with StepMix. The tutorial uses the Iris Dataset as
 an example and covers: 1. Continuous LCA models (latent profile analysis/
 gaussian mixture model); 2. Binary LCA models; 3. Categorical LCA models; 3.
 Mixed variables mixture models (continuous and categorical data); 5. Missing
 Values through Full-Information Maximum Likelihood. 2. [Stepwise Estimation
 with StepMix](https://colab.research.google.com/drive/1T_UObkN5Y-
```

