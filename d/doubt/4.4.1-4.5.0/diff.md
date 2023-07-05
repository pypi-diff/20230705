# Comparing `tmp/doubt-4.4.1.tar.gz` & `tmp/doubt-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubt-4.4.1.tar", max compression
+gzip compressed data, was "doubt-4.5.0.tar", max compression
```

## Comparing `doubt-4.4.1.tar` & `doubt-4.5.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.4.1/LICENSE
--rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.4.1/README.md
--rw-r--r--   0        0        0     1310 2023-04-23 18:38:39.796211 doubt-4.4.1/pyproject.toml
--rw-r--r--   0        0        0      369 2023-03-20 19:12:08.029301 doubt-4.4.1/src/doubt/__init__.py
--rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.4.1/src/doubt/datasets/__init__.py
--rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.4.1/src/doubt/datasets/airfoil.py
--rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.4.1/src/doubt/datasets/bike_sharing_daily.py
--rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.4.1/src/doubt/datasets/bike_sharing_hourly.py
--rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.4.1/src/doubt/datasets/blog.py
--rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.4.1/src/doubt/datasets/concrete.py
--rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.4.1/src/doubt/datasets/cpu.py
--rw-r--r--   0        0        0     4225 2023-03-20 18:57:45.250733 doubt-4.4.1/src/doubt/datasets/dataset.py
--rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.4.1/src/doubt/datasets/facebook_comments.py
--rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.4.1/src/doubt/datasets/facebook_metrics.py
--rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.4.1/src/doubt/datasets/fish_bioconcentration.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.4.1/src/doubt/datasets/fish_toxicity.py
--rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.4.1/src/doubt/datasets/forest_fire.py
--rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.4.1/src/doubt/datasets/gas_turbine.py
--rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.4.1/src/doubt/datasets/nanotube.py
--rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.4.1/src/doubt/datasets/new_taipei_housing.py
--rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.4.1/src/doubt/datasets/parkinsons.py
--rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.4.1/src/doubt/datasets/power_plant.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.4.1/src/doubt/datasets/protein.py
--rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.4.1/src/doubt/datasets/servo.py
--rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.4.1/src/doubt/datasets/solar_flare.py
--rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.4.1/src/doubt/datasets/space_shuttle.py
--rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.4.1/src/doubt/datasets/stocks.py
--rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.4.1/src/doubt/datasets/superconductivity.py
--rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.4.1/src/doubt/datasets/tehran_housing.py
--rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.4.1/src/doubt/datasets/yacht.py
--rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.4.1/src/doubt/models/__init__.py
--rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.4.1/src/doubt/models/boot/__init__.py
--rw-r--r--   0        0        0    16837 2023-04-23 18:36:29.040992 doubt-4.4.1/src/doubt/models/boot/boot.py
--rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.4.1/src/doubt/models/glm/__init__.py
--rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.4.1/src/doubt/models/glm/quantile_loss.py
--rw-r--r--   0        0        0     9220 2023-03-20 18:57:45.276816 doubt-4.4.1/src/doubt/models/glm/quantile_regressor.py
--rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.4.1/src/doubt/models/model.py
--rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.4.1/src/doubt/models/tree/__init__.py
--rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.4.1/src/doubt/models/tree/forest.py
--rw-r--r--   0        0        0    10540 2023-03-20 18:33:10.883879 doubt-4.4.1/src/doubt/models/tree/tree.py
--rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.4.1/src/doubt/models/tree/utils.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 doubt-4.4.1/setup.py
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.5.0/LICENSE
+-rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.5.0/README.md
+-rw-r--r--   0        0        0     1318 2023-07-05 13:28:20.606495 doubt-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-03-20 19:12:08.029301 doubt-4.5.0/src/doubt/__init__.py
+-rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.5.0/src/doubt/datasets/__init__.py
+-rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.5.0/src/doubt/datasets/airfoil.py
+-rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.5.0/src/doubt/datasets/bike_sharing_daily.py
+-rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.5.0/src/doubt/datasets/bike_sharing_hourly.py
+-rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.5.0/src/doubt/datasets/blog.py
+-rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.5.0/src/doubt/datasets/concrete.py
+-rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.5.0/src/doubt/datasets/cpu.py
+-rw-r--r--   0        0        0     4225 2023-03-20 18:57:45.250733 doubt-4.5.0/src/doubt/datasets/dataset.py
+-rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.5.0/src/doubt/datasets/facebook_comments.py
+-rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.5.0/src/doubt/datasets/facebook_metrics.py
+-rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.5.0/src/doubt/datasets/fish_bioconcentration.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.5.0/src/doubt/datasets/fish_toxicity.py
+-rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.5.0/src/doubt/datasets/forest_fire.py
+-rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.5.0/src/doubt/datasets/gas_turbine.py
+-rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.5.0/src/doubt/datasets/nanotube.py
+-rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.5.0/src/doubt/datasets/new_taipei_housing.py
+-rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.5.0/src/doubt/datasets/parkinsons.py
+-rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.5.0/src/doubt/datasets/power_plant.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.5.0/src/doubt/datasets/protein.py
+-rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.5.0/src/doubt/datasets/servo.py
+-rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.5.0/src/doubt/datasets/solar_flare.py
+-rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.5.0/src/doubt/datasets/space_shuttle.py
+-rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.5.0/src/doubt/datasets/stocks.py
+-rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.5.0/src/doubt/datasets/superconductivity.py
+-rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.5.0/src/doubt/datasets/tehran_housing.py
+-rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.5.0/src/doubt/datasets/yacht.py
+-rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.5.0/src/doubt/models/__init__.py
+-rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.5.0/src/doubt/models/boot/__init__.py
+-rw-r--r--   0        0        0    18725 2023-07-05 13:17:39.688583 doubt-4.5.0/src/doubt/models/boot/boot.py
+-rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.5.0/src/doubt/models/glm/__init__.py
+-rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.5.0/src/doubt/models/glm/quantile_loss.py
+-rw-r--r--   0        0        0     9220 2023-03-20 18:57:45.276816 doubt-4.5.0/src/doubt/models/glm/quantile_regressor.py
+-rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.5.0/src/doubt/models/model.py
+-rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.5.0/src/doubt/models/tree/__init__.py
+-rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.5.0/src/doubt/models/tree/forest.py
+-rw-r--r--   0        0        0    10540 2023-07-05 13:23:04.537888 doubt-4.5.0/src/doubt/models/tree/tree.py
+-rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.5.0/src/doubt/models/tree/utils.py
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.5.0/PKG-INFO
```

### Comparing `doubt-4.4.1/LICENSE` & `doubt-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/README.md` & `doubt-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/pyproject.toml` & `doubt-4.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "doubt"
-version = "4.4.1"
+version = "4.5.0"
 description = "Bringing back uncertainty to machine learning."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/saattrupdan/doubt"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 tqdm = "^4.62.0"
 numpy = "^1.23.0"
 pandas = "^1.4.0"
 joblib = "^1.2.0"
-scikit-learn = "^1.1.1"
-tables = "^3.7.0"
+scikit-learn = ">=1.1.0,<1.3.0"
 xlrd = "^2.0.1"
 openpyxl = "^3.0.10"
+tables = "~3.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pdoc = "^7.1.1"
 pre-commit = "^2.17.0"
 black = "^23.1.0"
 requests = "^2.28.0"
 lxml = "^4.9.0"
```

### Comparing `doubt-4.4.1/src/doubt/datasets/__init__.py` & `doubt-4.5.0/src/doubt/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/airfoil.py` & `doubt-4.5.0/src/doubt/datasets/airfoil.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/bike_sharing_daily.py` & `doubt-4.5.0/src/doubt/datasets/bike_sharing_daily.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/bike_sharing_hourly.py` & `doubt-4.5.0/src/doubt/datasets/bike_sharing_hourly.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/blog.py` & `doubt-4.5.0/src/doubt/datasets/blog.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/concrete.py` & `doubt-4.5.0/src/doubt/datasets/concrete.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/cpu.py` & `doubt-4.5.0/src/doubt/datasets/cpu.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/dataset.py` & `doubt-4.5.0/src/doubt/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/facebook_comments.py` & `doubt-4.5.0/src/doubt/datasets/facebook_comments.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/facebook_metrics.py` & `doubt-4.5.0/src/doubt/datasets/facebook_metrics.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/fish_bioconcentration.py` & `doubt-4.5.0/src/doubt/datasets/fish_bioconcentration.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/fish_toxicity.py` & `doubt-4.5.0/src/doubt/datasets/fish_toxicity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/forest_fire.py` & `doubt-4.5.0/src/doubt/datasets/forest_fire.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/gas_turbine.py` & `doubt-4.5.0/src/doubt/datasets/gas_turbine.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/nanotube.py` & `doubt-4.5.0/src/doubt/datasets/nanotube.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/new_taipei_housing.py` & `doubt-4.5.0/src/doubt/datasets/new_taipei_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/parkinsons.py` & `doubt-4.5.0/src/doubt/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/power_plant.py` & `doubt-4.5.0/src/doubt/datasets/power_plant.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/protein.py` & `doubt-4.5.0/src/doubt/datasets/protein.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/servo.py` & `doubt-4.5.0/src/doubt/datasets/servo.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/solar_flare.py` & `doubt-4.5.0/src/doubt/datasets/solar_flare.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/space_shuttle.py` & `doubt-4.5.0/src/doubt/datasets/space_shuttle.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/stocks.py` & `doubt-4.5.0/src/doubt/datasets/stocks.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/superconductivity.py` & `doubt-4.5.0/src/doubt/datasets/superconductivity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/tehran_housing.py` & `doubt-4.5.0/src/doubt/datasets/tehran_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/datasets/yacht.py` & `doubt-4.5.0/src/doubt/datasets/yacht.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/models/boot/boot.py` & `doubt-4.5.0/src/doubt/models/boot/boot.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,57 @@
     model = copy.deepcopy(model)
     model.fit(X_train, y_train)
     if callable(model):
         return model(X_test)
     else:
         return model.predict(X_test)
 
+def _model_fit(
+    model, X_train: np.ndarray, y_train: np.ndarray
+):
+    """Fit the underlying model.
+
+    Args:
+        model (object with `fit` method):
+            The model to fit with.
+        X_train (float matrix):
+            Feature matrix for training, of shape
+            (n_train_samples, n_features).
+        y_train (float array):
+            Target array, of shape (n_train_samples,).
+
+    Returns:
+        The fitted model.
+    """
+    model = copy.deepcopy(model)
+    model.fit(X_train, y_train)
+    return model
+
+def _model_predict(
+    model, X: np.ndarray
+) -> np.ndarray:
+    """Perform predictions with the underlying model.
+
+    This requires that the model is either callable or have a `predict` method.
+
+    Args:
+        model (object with a `predict` method):
+            The model to predict with.
+        X (float matrix):
+            Feature matrix for predicting, of shape
+            (n_test_samples, n_features).
+
+    Returns:
+        Numpy array:
+            Predictions, of shape (n_test_samples,)
+    """
+    if callable(model):
+        return model(X)
+    else:
+        return model.predict(X)
 
 def _dataset_repr(self) -> str:
     return f"Boot(dataset_shape={self.data.shape}, " f"random_seed={self.random_seed})"
 
 
 def _model_repr(self) -> str:
     model_name = self._model.__class__.__name__
@@ -225,14 +268,15 @@
 def predict(
     self,
     X: np.ndarray,
     n_boots: Optional[int] = None,
     uncertainty: Optional[float] = None,
     quantiles: Optional[Union[np.ndarray, List[float]]] = None,
     return_all: bool = False,
+    n_jobs: Optional[int] = None
 ) -> Union[Union[float, NDArray], Tuple[Union[float, NDArray], NDArray]]:
     """Compute bootstrapped predictions.
 
     Args:
         X (float array):
             The array containing the data set, either of shape (f,) or (n, f), with n
             being the number of samples and f being the number of features.
@@ -246,14 +290,17 @@
             used. Defaults to None.
         quantiles (sequence of floats or None, optional):
             List of quantiles to output. Will override the value of `uncertainty` if
             specified. Will not be used if `return_all` is True. Defaults to None.
         return_all (bool, optional):
             Whether the raw bootstrapped predictions should be returned. Will override
             the values of both `quantiles` and `uncertainty`. Defaults to False.
+        n_jobs: (int or None, optional):
+            The number of jobs to use for parallelization. If None then it is equal to the
+            number of available cpus minus one. Defaults to None
 
     Returns:
         float array or pair of float arrays:
             The bootstrapped predictions, and the confidence intervals if `uncertainty`
             is not None, the specified quantiles if `quantiles` is not None, or the raw
             bootstrapped values if `return_all` is True.
     """
@@ -292,22 +339,25 @@
     # number of samples in the training dataset
     if n_boots is None:
         n_boots = int(np.sqrt(n_train).astype(int))
 
     # Sample the bootstrap indices
     train_idxs = rng.choice(n_train, size=(n_boots, n_train), replace=True)
 
+    #set the number of jobs to use
+    if n_jobs is None:
+        jobs = mp.cpu_count() - 1
+    else:
+        jobs = n_jobs
     # Run the worker function in parallel
-    with Parallel(n_jobs=mp.cpu_count() - 1) as parallel:
+    with Parallel(n_jobs=jobs) as parallel:
         bootstrap_preds_list = parallel(
-            delayed(_model_fit_predict)(
-                model=self._model,
-                X_train=self.X_train[train_idxs[boot_idx], :],
-                y_train=self.y_train[train_idxs[boot_idx]],
-                X_test=X,
+            delayed(_model_predict)(
+                model=self._models[boot_idx],
+                X=X,
             )
             for boot_idx in range(n_boots)
         )
 
     # Convert the list of predictions to a Numpy array
     bootstrap_preds = np.array(bootstrap_preds_list)
 
@@ -346,26 +396,29 @@
     else:
         intervals = np.expand_dims(preds, axis=1) + quantile_vals
 
     # Return the predictions and the prediction intervals
     return preds, intervals
 
 
-def fit(self, X: np.ndarray, y: np.ndarray, n_boots: Optional[int] = None):
+def fit(self, X: np.ndarray, y: np.ndarray, n_boots: Optional[int] = None, n_jobs: Optional[int] = None):
     """Fits the model to the data.
 
     Args:
         X (float array):
             The array containing the data set, either of shape (f,) or (n, f), with n
             being the number of samples and f being the number of features.
         y (float array):
             The array containing the target values, of shape (n,)
         n_boots (int or None):
             The number of resamples to bootstrap. If None then it is set to the square
             root of the data set. Defaults to None
+        n_jobs: (int or None):
+            The number of jobs to use for parallelization. If None then it is equal to the
+            number of available cpus minus one. Defaults to None
     """
     # Initialise random number generator
     rng = np.random.default_rng(self.random_seed)
 
     # Set the number of data points in the dataset
     n = X.shape[0]
 
@@ -388,22 +441,35 @@
     # Calculate the training residuals and aggregate them into quantiles, to enable
     # comparison with the validation residuals
     train_residuals = np.quantile(y - preds, q=np.arange(0, 1, 0.01))
 
     # Sample the bootstrap indices
     train_idxs = rng.choice(n, size=(n_boots, n), replace=True)
 
+    # Set the number of jobs
+    if n_jobs is None:
+        jobs = mp.cpu_count() - 1
+    else:
+        jobs = n_jobs
     # Run the worker function in parallel
-    with Parallel(n_jobs=mp.cpu_count() - 1) as parallel:
-        bootstrap_preds = parallel(
-            delayed(_model_fit_predict)(
+    with Parallel(n_jobs=jobs) as parallel:
+        self._models = parallel(
+            delayed(_model_fit)(
                 model=self._model,
                 X_train=self.X_train[train_idxs[boot_idx], :],
                 y_train=self.y_train[train_idxs[boot_idx]],
-                X_test=X[[idx for idx in range(n) if idx not in train_idxs[boot_idx]]],
+
+            )
+            for boot_idx in range(n_boots)
+        )
+    with Parallel(n_jobs=jobs) as parallel:
+        bootstrap_preds = parallel(
+            delayed(_model_predict)(
+                model=self._models[boot_idx],
+                X=X[[idx for idx in range(n) if idx not in train_idxs[boot_idx]]]
             )
             for boot_idx in range(n_boots)
         )
 
     # Compute the validation residuals
     val_residuals_list = [
         y[[idx for idx in range(n) if idx not in train_idxs[boot_idx]]]
```

### Comparing `doubt-4.4.1/src/doubt/models/glm/quantile_loss.py` & `doubt-4.5.0/src/doubt/models/glm/quantile_loss.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/models/glm/quantile_regressor.py` & `doubt-4.5.0/src/doubt/models/glm/quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/models/tree/forest.py` & `doubt-4.5.0/src/doubt/models/tree/forest.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/models/tree/tree.py` & `doubt-4.5.0/src/doubt/models/tree/tree.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/src/doubt/models/tree/utils.py` & `doubt-4.5.0/src/doubt/models/tree/utils.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.1/PKG-INFO` & `doubt-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubt
-Version: 4.4.1
+Version: 4.5.0
 Summary: Bringing back uncertainty to machine learning.
 Home-page: https://github.com/saattrupdan/doubt
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: saattrupdan@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: tables (>=3.7.0,<4.0.0)
+Requires-Dist: scikit-learn (>=1.1.0,<1.3.0)
+Requires-Dist: tables (>=3.7.0,<3.8.0)
 Requires-Dist: tqdm (>=4.62.0,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/saattrupdan/doubt
 Description-Content-Type: text/markdown
 
 # Doubt
```

