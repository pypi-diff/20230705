# Comparing `tmp/pedestal-inference-0.2.1.tar.gz` & `tmp/pedestal-inference-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedestal-inference-0.2.1.tar", last modified: Fri Jun 16 14:46:59 2023, max compression
+gzip compressed data, was "pedestal-inference-0.2.2.tar", last modified: Wed Jul  5 15:41:17 2023, max compression
```

## Comparing `pedestal-inference-0.2.1.tar` & `pedestal-inference-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/pedestal_inference.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-06-16 14:46:59.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-16 14:46:58.000000 pedestal-inference-0.2.1/pedestal_inference.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/pedinf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6299 2023-03-12 12:51:51.000000 pedestal-inference-0.2.1/pedinf/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/pedinf/analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1761 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pedinf/diagnostics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10519 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/pedinf/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4763 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pedinf/spectrum.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-06-16 12:58:40.000000 pedestal-inference-0.2.1/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-06-16 14:46:59.006087 pedestal-inference-0.2.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-16 14:46:59.002087 pedestal-inference-0.2.1/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/tests/test_analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.1/tests/test_models.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.2/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.2/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/pedestal_inference.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/pedinf/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6452 2023-07-05 14:36:16.000000 pedestal-inference-0.2.2/pedinf/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/pedinf/analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1761 2023-06-16 12:58:40.000000 pedestal-inference-0.2.2/pedinf/diagnostics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10546 2023-06-18 01:14:19.000000 pedestal-inference-0.2.2/pedinf/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5642 2023-06-18 01:49:12.000000 pedestal-inference-0.2.2/pedinf/spectrum.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-07-05 15:33:14.000000 pedestal-inference-0.2.2/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/tests/test_analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/tests/test_models.py
```

### Comparing `pedestal-inference-0.2.1/LICENSE` & `pedestal-inference-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.1/PKG-INFO` & `pedestal-inference-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.2.1/pedestal_inference.egg-info/PKG-INFO` & `pedestal-inference-0.2.2/pedestal_inference.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
 Project-URL: documentation, https://inference-tools.readthedocs.io
```

### Comparing `pedestal-inference-0.2.1/pedinf/__init__.py` & `pedestal-inference-0.2.2/pedinf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         assert self.spectra.shape == self.errors.shape
 
         # check for any data which are NaN or inf
         assert self.spectra.shape[0] == self.spatial_channels.shape[0]
         bad_data = ~isfinite(self.spectra) | ~isfinite(self.errors)
         if bad_data.any():
             self.spectra[bad_data] = 0.0
-            self.errors[bad_data] = self.spectra.max() * 1e10
+            self.errors[bad_data] = 1e50
 
         # check validity of data values
         assert (self.errors > 0).all()
         assert (diff(self.spatial_channels) > 0).all()
 
         self.good_data = ~bad_data
         self.n_spectra = self.spectra.shape[1]
@@ -182,16 +182,22 @@
 
 class SpectralPedestalPosterior:
     def __init__(
         self,
         spectrometer_model: SpectrometerModel,
         spectrum_data: SpectrumData,
         likelihood=LogisticLikelihood,
+        prior=None,
     ):
         self.spectrum = spectrometer_model
         self.data = spectrum_data
 
         self.likelihood = likelihood(
             y_data=self.data.spectra.flatten(),
             sigma=self.data.errors.flatten(),
             forward_model=self.spectrum.predictions,
         )
+
+        self.prior = lambda x: 0.0 if prior is None else prior
+
+    def __call__(self, theta):
+        return self.likelihood(theta) + self.prior(theta)
```

### Comparing `pedestal-inference-0.2.1/pedinf/analysis.py` & `pedestal-inference-0.2.2/pedinf/analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.1/pedinf/diagnostics.py` & `pedestal-inference-0.2.2/pedinf/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.1/pedinf/models.py` & `pedestal-inference-0.2.2/pedinf/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @staticmethod
     @abstractmethod
     def jacobian(R: ndarray, theta: ndarray) -> ndarray:
         pass
 
     @staticmethod
     @abstractmethod
-    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray]:
+    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray, ndarray]:
         pass
 
 
 class mtanh(ProfileModel):
     r"""
     The standard 'mtanh' function used for pedestal fitting. Specifically,
     the function is:
@@ -142,15 +142,15 @@
         jac[:, 1] = L
         jac[:, 2] = -0.25 * q * z
         jac[:, 3] = (sigma * z) * L
         jac[:, 4] = 1 - L
         return jac
 
     @staticmethod
-    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray]:
+    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray, ndarray]:
         """
         Calculates the prediction and the jacobian of the ``mtanh`` model. The jacobian
         is a matrix where element :math:`i, j` is the derivative of the model prediction
         at the :math:`i`'th radial position with respect to the :math:`j`'th model parameter.
         See the documentation for ``mtanh`` for details of the model itself.
 
         :param R: \
@@ -301,15 +301,15 @@
         jac[:, 2] = -(z / w) * df_dz + (0.25*a) * S
         jac[:, 3] = sigma * S
         jac[:, 4] = 1 - Lk
         jac[:, 5] = (h - b) * Lk * (1 + ln_L - L)
         return jac
 
     @staticmethod
-    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray]:
+    def prediction_and_jacobian(R: ndarray, theta: ndarray) -> Tuple[ndarray, ndarray]:
         """
         Calculates the prediction and the jacobian of the ``lpm`` model. The jacobian
         is a matrix where element :math:`i, j` is the derivative of the model prediction
         at the :math:`i`'th radial position with respect to the :math:`j`'th model parameter.
         See the documentation for ``lpm`` for details of the model itself.
 
         :param R: \
```

### Comparing `pedestal-inference-0.2.1/pedinf/spectrum.py` & `pedestal-inference-0.2.2/pedinf/spectrum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,37 @@
 from numpy import sqrt, cos, pi, exp
 from numpy import ndarray, linspace, zeros
 from scipy.interpolate import RectBivariateSpline
 
 
-def selden(Te, wavelength, theta, laser_wavelength=1.064e-6):
+def selden(
+    Te: ndarray, wavelength: ndarray, theta: ndarray, laser_wavelength=1.064e-6
+) -> ndarray:
+    """
+    Implementation of the 'Selden' equation, which gives a very accurate approximation
+    of the relativistic Thomson-scattering spectrum for fusion-relevant temperatures.
+
+    :param Te: \
+        The electron temperature in electron-volts.
+
+    :param wavelength: \
+        Wavelength values (in meters) at which the scattering spectrum is calculated.
+
+    :param theta: \
+        The scattering angle in radians.
+
+    :param laser_wavelength: \
+        Wavelength (in meters) of the light being scattered.
+
+    :return: \
+        The scattering spectrum. Note that the integral of the Selden equation across
+        all scattering wavelengths is equal to the laser wavelength, so the returned
+        spectrum must be divided by the laser wavelength to yield a properly normalised
+        probability distribution.
+    """
     coeff = 3.913902367e-06  # 2 divided by the electron rest-mass-energy in eV
     inv_alpha = coeff * Te
     alpha = 1.0 / inv_alpha
 
     # Coefficients
     eps = (wavelength - laser_wavelength) / laser_wavelength
     k = 2 * (1 - cos(theta)) * (1 + eps)
```

### Comparing `pedestal-inference-0.2.1/pyproject.toml` & `pedestal-inference-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pedestal-inference"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Chris Bowman", email="chris.bowman.physics@gmail.com" },
 ]
 description = "A collection of Python tools for plasma-edge Thomson-scattering analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pedestal-inference-0.2.1/setup.cfg` & `pedestal-inference-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.1/tests/test_analysis.py` & `pedestal-inference-0.2.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.1/tests/test_models.py` & `pedestal-inference-0.2.2/tests/test_models.py`

 * *Files identical despite different names*

