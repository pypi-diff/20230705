# Comparing `tmp/polykin-0.1.0.tar.gz` & `tmp/polykin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polykin-0.1.0.tar", max compression
+gzip compressed data, was "polykin-0.2.0.tar", max compression
```

## Comparing `polykin-0.1.0.tar` & `polykin-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1087 2022-12-26 20:22:07.495866 polykin-0.1.0/LICENSE
--rw-r--r--   0        0        0     1512 2023-02-18 22:37:36.379360 polykin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1719 2023-02-18 22:36:14.952023 polykin-0.1.0/README.md
--rw-r--r--   0        0        0      474 2023-01-21 16:34:39.582515 polykin-0.1.0/src/polykin/__init__.py
--rw-r--r--   0        0        0        5 2023-01-05 21:18:05.152806 polykin-0.1.0/src/polykin/_version.txt
--rw-r--r--   0        0        0      530 2023-02-12 15:25:16.567010 polykin-0.1.0/src/polykin/base.py
--rw-r--r--   0        0        0      209 2023-01-28 16:51:11.435139 polykin-0.1.0/src/polykin/copolymerization/__init__.py
--rw-r--r--   0        0        0     3049 2023-02-13 21:54:58.229803 polykin-0.1.0/src/polykin/copolymerization/basesclasses.py
--rw-r--r--   0        0        0      459 2023-02-18 14:58:00.168279 polykin-0.1.0/src/polykin/distributions/__init__.py
--rw-r--r--   0        0        0     7106 2023-02-01 21:01:24.563105 polykin-0.1.0/src/polykin/distributions/analyticaldistributions.py
--rw-r--r--   0        0        0    27271 2023-02-18 13:49:00.071297 polykin-0.1.0/src/polykin/distributions/baseclasses.py
--rw-r--r--   0        0        0     6762 2023-02-12 15:35:40.146697 polykin-0.1.0/src/polykin/distributions/datadistribution.py
--rw-r--r--   0        0        0    31167 2023-02-18 14:57:16.062665 polykin-0.1.0/src/polykin/distributions/sampledata.py
--rw-r--r--   0        0        0     5955 2023-02-12 15:25:54.375922 polykin-0.1.0/src/polykin/utils.py
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 polykin-0.1.0/setup.py
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 polykin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-12-26 20:22:07.495866 polykin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1575 2023-07-05 21:06:21.070869 polykin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1743 2023-07-05 19:57:51.247594 polykin-0.2.0/README.md
+-rw-r--r--   0        0        0      457 2023-07-05 21:06:04.375348 polykin-0.2.0/src/polykin/__init__.py
+-rw-r--r--   0        0        0      530 2023-02-12 15:25:16.567010 polykin-0.2.0/src/polykin/base.py
+-rw-r--r--   0        0        0    26025 2023-07-05 21:02:53.476740 polykin-0.2.0/src/polykin/coefficients.py
+-rw-r--r--   0        0        0      209 2023-01-28 16:51:11.435139 polykin-0.2.0/src/polykin/copolymerization/__init__.py
+-rw-r--r--   0        0        0     4229 2023-04-12 21:20:42.583262 polykin-0.2.0/src/polykin/copolymerization/baseclasses.py
+-rw-r--r--   0        0        0      459 2023-02-18 14:58:00.168279 polykin-0.2.0/src/polykin/distributions/__init__.py
+-rw-r--r--   0        0        0     7183 2023-06-29 20:06:12.120501 polykin-0.2.0/src/polykin/distributions/analyticaldistributions.py
+-rw-r--r--   0        0        0    27570 2023-06-30 22:35:56.969160 polykin-0.2.0/src/polykin/distributions/baseclasses.py
+-rw-r--r--   0        0        0     7241 2023-06-29 20:12:40.712335 polykin-0.2.0/src/polykin/distributions/datadistribution.py
+-rw-r--r--   0        0        0    31167 2023-02-18 14:57:16.062665 polykin-0.2.0/src/polykin/distributions/sampledata.py
+-rw-r--r--   0        0        0     6912 2023-07-01 15:24:49.608300 polykin-0.2.0/src/polykin/utils.py
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 polykin-0.2.0/PKG-INFO
```

### Comparing `polykin-0.1.0/LICENSE` & `polykin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polykin-0.1.0/pyproject.toml` & `polykin-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polykin"
-version = "0.1.0"
+version = "0.2.0"
 description = "A polymerization kinetics library."
 authors = ["HugoMVale <57530119+HugoMVale@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hugomvale.github.io/polykin/"
 repository = "https://github.com/HugoMVale/polykin"
 documentation = "https://hugomvale.github.io/polykin/"
@@ -16,39 +16,40 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Chemistry",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4"
-
-numpy = ">=1.23"
-scipy = "^1.9.3"
-matplotlib = "^3.6.2"
+python = ">=3.9,<3.11"
 mpmath = "^1.2.1"
-pydantic = "^1.10.4"
-numba = "^0.56.4"
+pydantic = "^1.10.5"
+numpy = "^1.24.2"
+scipy = "^1.10.1"
+matplotlib = "^3.7.1"
+nptyping = "^2.5.0"
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 flake8 = "^6.0.0"
 autopep8 = "^2.0.1"
-black = "^22.12.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 ipykernel = "^6.20.0"
 mkdocs = "^1.4.2"
-mkdocstrings = { extras = ["python"], version = "^0.19.1" }
 mkdocs-material = "^8.5.11"
 mkdocs-jupyter = "^0.22.0"
 mkdocs-autolinks-plugin = "^0.6.0"
+mkdocs-gen-files = "^0.5.0"
+mkdocs-literate-nav = "^0.6.0"
+black = "^23.3.0"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `polykin-0.1.0/README.md` & `polykin-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # PolyKin
 
-[![CI](https://github.com/HugoMVale/polykin/actions/workflows/CI.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions)
+[![Test](https://github.com/HugoMVale/polykin/actions/workflows/test.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions)
 [![codecov](https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin)
 [![Latest Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-commit/HugoMVale/polykin)
 
 PolyKin is an open-source polymerization kinetics library for Python. It is still at an early
 development stage, but the following modules can already be used:
 
 - [x] distributions
+- [x] coefficients
 - [ ] copolymerization
 - [ ] kinetics
 - [ ] database
 - [ ] models
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-# PolyKin [![CI](https://github.com/HugoMVale/polykin/actions/workflows/CI.yml/
-badge.svg)](https://github.com/HugoMVale/polykin/actions) [![codecov](https://
-codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)]
-(https://codecov.io/gh/HugoMVale/polykin) [![Latest Commit](https://
-img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/
-github/last-commit/HugoMVale/polykin) PolyKin is an open-source polymerization
-kinetics library for Python. It is still at an early development stage, but the
-following modules can already be used: - [x] distributions - [ ]
-copolymerization - [ ] kinetics - [ ] database - [ ] models ## Documentation
-Please refer to the package [homepage](https://hugomvale.github.io/polykin/).
-## Tutorials The main features of PolyKin are explained and illustrated through
-a series of [tutorials](https://hugomvale.github.io/polykin/tutorials/
-distributions/) based on Jupyter [notebooks](https://github.com/HugoMVale/
-polykin/tree/main/docs/tutorials), which can be launched online via Binder.
+# PolyKin [![Test](https://github.com/HugoMVale/polykin/actions/workflows/
+test.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions) [![codecov]
+(https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/
+badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin) [![Latest
+Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://
+img.shields.io/github/last-commit/HugoMVale/polykin) PolyKin is an open-source
+polymerization kinetics library for Python. It is still at an early development
+stage, but the following modules can already be used: - [x] distributions - [x]
+coefficients - [ ] copolymerization - [ ] kinetics - [ ] database - [ ] models
+## Documentation Please refer to the package [homepage](https://
+hugomvale.github.io/polykin/). ## Tutorials The main features of PolyKin are
+explained and illustrated through a series of [tutorials](https://
+hugomvale.github.io/polykin/tutorials/distributions/) based on Jupyter
+[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
+which can be launched online via Binder.
                            [MWD_of_a_polymer_blend]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

### Comparing `polykin-0.1.0/src/polykin/base.py` & `polykin-0.2.0/src/polykin/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.1.0/src/polykin/distributions/analyticaldistributions.py` & `polykin-0.2.0/src/polykin/distributions/analyticaldistributions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import numpy as np
 import scipy.special as sp
 import scipy.stats as st
 import functools
 
 
 class Flory(AnalyticalDistributionP1):
-    r"""Flory-Schulz (aka most-probable) chain-length distribution, with
-    _number_ probability mass function given by:
+    r"""Flory-Schulz (aka most-probable) chain-length distribution.
+    
+    The Flory-Schulz _number_ probability mass function is given by:
 
     $$ p(k) = (1-a)a^{k-1} $$
 
     where $a=1-1/DP_n$. Mathematically speaking, this is a [geometric
     distribution](https://en.wikipedia.org/wiki/Geometric_distribution).
     """
     _continuous = False
@@ -59,16 +60,17 @@
 
     @functools.cached_property
     def _range_length_default(self):
         return st.geom.ppf(self._ppf_bounds, p=(1-self._a))
 
 
 class Poisson(AnalyticalDistributionP1):
-    r"""Poisson chain-length distribution, with _number_ probability mass
-    function given by:
+    r"""Poisson chain-length distribution.
+    
+    The Poisson _number_ probability mass function is given by:
 
     $$ p(k) = \frac{a^{k-1} e^{-a}}{\Gamma(k)} $$
 
     where $a=DP_n-1$.
     """
 
     _continuous = False
@@ -112,16 +114,17 @@
 
     @functools.cached_property
     def _range_length_default(self):
         return st.poisson.ppf(self._ppf_bounds, mu=self._a, loc=1)
 
 
 class LogNormal(AnalyticalDistributionP2):
-    r"""Log-normal chain-length distribution, with _number_ probability density
-    function given by:
+    r"""Log-normal chain-length distribution.
+    
+    The Log-normal _number_ probability density function is given by:
 
     $$ p(x) = \frac{1}{x \sigma \sqrt{2 \pi}}
     \exp\left (- \frac{(\ln{x}-\mu)^2}{2\sigma^2} \right ) $$
 
     where $\mu = \ln{(DP_n/\sqrt{PDI})}$ and $\sigma=\sqrt{\ln(PDI)}$.
     """
     # https://reference.wolfram.com/language/ref/LogNormalDistribution.html
@@ -170,16 +173,17 @@
     def _range_length_default(self):
         mu = self._mu
         sigma = self._sigma
         return st.lognorm.ppf(self._ppf_bounds, s=sigma, scale=exp(mu), loc=1)
 
 
 class SchulzZimm(AnalyticalDistributionP2):
-    r"""Schulz-Zimm chain-length distribution, with _number_ probability
-    density function given by:
+    r"""Schulz-Zimm chain-length distribution.
+     
+    The Schulz-Zimm _number_ probability density function is given by:
 
     $$ p(x) = \frac{x^{k-1} e^{-x/\theta}}{\Gamma(k) \theta^k} $$
 
     where $k = 1/(DP_n-1)$ and $\theta = DP_n(PDI-1)$. Mathematically speaking,
     this is a
     [Gamma distribution](https://en.wikipedia.org/wiki/Gamma_distribution).
     """
```

### Comparing `polykin-0.1.0/src/polykin/distributions/baseclasses.py` & `polykin-0.2.0/src/polykin/distributions/baseclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # %% Base distribution classes
 
 from polykin.base import Base
 from polykin.utils import check_bounds, check_type, check_in_set, \
-    custom_error, add_dicts, vectorize, Vector
+    custom_error, add_dicts, vectorize, FloatOrArrayLike, FloatOrArray, \
+    IntOrArray, FloatRange
 
 from math import log10
 import numpy as np
+from numpy import ndarray
 import mpmath
-from numpy import int64, float64, dtype, ndarray
 from scipy import integrate
 import matplotlib.pyplot as plt
-from typing import Any, Literal, Union
+from matplotlib.figure import Figure
+from typing import Literal, Union
 from abc import ABC, abstractmethod
 import functools
 
 # %% Types
 
 Kind = Literal['number', 'mass', 'gpc']
 
 # %% Classes
 
 
-class GeneralDistribution(Base, ABC):
-    """Abstract class for all chain-length distributions."""
+class Distribution(Base, ABC):
+    r"""_Abstract_ class for all chain-length distributions."""
 
     kind_order = {'number': 0, 'mass': 1, 'gpc': 2}
     units = {'molar_mass': 'g/mol'}
 
     def __str__(self) -> str:
         unit_M = self.units['molar_mass']
         return f"type: {self.__class__.__name__}\n" + \
@@ -36,14 +38,20 @@
             f"DPz:  {self.DPz:.1f}\n" + \
             f"PDI:  {self.PDI:.2f}\n" + \
             f"M0:   {self.M0:,.1f} {unit_M}\n" + \
             f"Mn:   {self.Mn:,.0f} {unit_M}\n" + \
             f"Mw:   {self.Mw:,.0f} {unit_M}\n" + \
             f"Mz:   {self.Mz:,.0f} {unit_M}"
 
+    def __lt__(self, other) -> bool:
+        if isinstance(other, Distribution):
+            return self.Mw < other.Mw
+        else:
+            return NotImplemented
+
     @property
     def DPn(self) -> float:
         r"""Number-average degree of polymerization, $DP_n$."""
         return self._moment_mass(1, 1)/self._moment_mass(0)
 
     @property
     def DPw(self) -> float:
@@ -77,72 +85,72 @@
 
     @property
     def M0(self) -> float:
         """Number-average molar mass of the repeating units, $M_0=M_n/DP_n$."""
         return self.Mn / self.DPn
 
     def pdf(self,
-            size: Union[float, Vector],
+            size: FloatOrArrayLike,
             kind: Kind = 'mass',
             sizeasmass: bool = False,
-            ) -> Union[float, ndarray[Any, dtype[float64]]]:
+            ) -> FloatOrArray:
         r"""Evaluate the probability density function, $p(k)$.
 
         Parameters
         ----------
-        size : float | list | ndarray
+        size : FloatOrArrayLike
             Chain length or molar mass.
         kind : Literal['number', 'mass', 'gpc']
             Kind of distribution.
         sizeasmass : bool
             Switch size input between chain-*length* (if `False`) or molar
             *mass* (if `True`).
 
         Returns
         -------
-        float | ndarray
+        FloatOrArray
             Probability density.
         """
         # Check inputs
         self._verify_sizeasmass(sizeasmass)
         order = self.kind_order[self._verify_kind(kind)]
         # Convert list to ndarray
         if isinstance(size, list):
             size = np.asarray(size)
         # Math is done by the corresponding subclass method
         return self._pdf(size, order, sizeasmass)
 
     def cdf(self,
-            size: Union[float, Vector],
+            size: FloatOrArrayLike,
             kind: Literal['number', 'mass'] = 'mass',
             sizeasmass: bool = False,
-            ) -> Union[float, ndarray[Any, dtype[float64]]]:
+            ) -> FloatOrArray:
         r"""Evaluate the cumulative distribution function:
 
         $$ F(s) = \frac{\sum_{k=1}^{s}k^m\,p(k)}{\lambda_m} $$
 
         or
 
         $$ F(s) = \frac{\int_{0}^{s}x^m\,p(x)\mathrm{d}x}{\lambda_m} $$
 
         where $m$ is the order (0: number, 1: mass).
 
         Parameters
         ----------
-        size : float | list | ndarray
+        size : FloatOrArrayLike
             Chain length or molar mass.
         kind : Literal['number', 'mass']
             Kind of distribution.
         sizeasmass : bool
             Switch size input between chain-*length* (if `False`) or molar
             *mass* (if `True`).
 
         Returns
         -------
-        float | ndarray
+        FloatOrArray
             Cumulative probability.
         """
         # Check inputs
         kind = self._verify_kind(kind)
         if kind == 'gpc':
             custom_error('kind', kind, ValueError,
                          "Please use `mass` instead.")
@@ -155,16 +163,15 @@
         result = self._cdf(size, order, sizeasmass)
         return result
 
     def plot(self,
              kinds: Union[Kind, list[Kind]] = 'mass',
              sizeasmass: bool = False,
              xscale: Literal['auto', 'linear', 'log'] = 'auto',
-             xrange: Union[list[float], tuple[float, float],
-                           ndarray[Any, dtype[float64]]] = [],
+             xrange: FloatRange = [],
              cdf: Literal[0, 1, 2] = 0,
              title: Union[str, None] = None,
              axes: Union[list[plt.Axes], None] = None,
              ) -> None:
         """Plot the chain-length distribution.
 
         Parameters
@@ -172,23 +179,23 @@
         kind : Literal['number', 'mass', 'gpc']
             Kind of distribution.
         sizeasmass : bool
             Switch size input between chain-*length* (if `False`) or molar
             *mass* (if `True`).
         xscale : Literal['auto', 'linear', 'log']
             x-axis scale.
-        xrange : Union[list, tuple, ndarray]
+        xrange : list | tuple | ndarray
             x-axis range.
         cdf : Literal[0, 1, 2]
             y-axis where cdf is displayed. If `0` the cdf if not displayed; if
             `1` the cdf is displayed on the primary y-axis; if `2` the cdf is
             displayed on the secondary axis.
-        title: Union[str, None]
+        title: str | None
             Title
-        axes : Union[plt.Axes, None]
+        axes : list[plt.Axes] | None
             Matplotlib Axes object.
         """
         # Check inputs
         kinds = self._verify_kind(kinds, accept_list=True)
         self._verify_sizeasmass(sizeasmass)
         check_in_set(xscale, {'linear', 'log', 'auto'}, 'xscale')
         check_in_set(cdf, {0, 1, 2}, 'cdf')
@@ -308,28 +315,28 @@
 
     def _verify_sizeasmass(self, sizeasmass):
         """Verify `sizeasmass` input."""
         return check_type(sizeasmass, bool, 'sizeasmass')
 
     @abstractmethod
     def _pdf(self,
-             size: Union[float, ndarray],
+             size: FloatOrArray,
              order: int,
              sizeasmass: bool = False
-             ) -> Union[float, ndarray[Any, dtype[float64]]]:
+             ) -> FloatOrArray:
         """$m$-th order chain-length / molar mass probability density
         function."""
         pass
 
     @abstractmethod
     def _cdf(self,
-             size: Union[float, ndarray],
+             size: FloatOrArray,
              order: int,
              sizeasmass: bool = False
-             ) -> Union[float, ndarray[Any, dtype[float64]]]:
+             ) -> FloatOrArray:
         """$m$-th order chain-length / molar mass cumulative distribution
         function."""
         pass
 
     @abstractmethod
     def _moment_mass(self,
                      order: int,
@@ -345,16 +352,16 @@
                      sizeasmass: bool
                      ) -> ndarray:
         """Default chain-length or molar mass range for distribution plots.
         """
         pass
 
 
-class IndividualDistribution(GeneralDistribution):
-    """Abstract class for all individual chain-length distributions."""
+class IndividualDistribution(Distribution):
+    """_Abstract_ class for all individual chain-length distributions."""
 
     _continuous = True
 
     def __mul__(self, other):
         if isinstance(other, (int, float)):
             if other > 0:
                 return MixtureDistribution({self: other}, name=self.name)
@@ -449,65 +456,65 @@
         $$ F(a,b) = \frac{\int_{a}^{b}x^m\,p(x)\mathrm{d}x}{\lambda_m} $$
 
         where $m$ is the moment order.
 
         Parameters
         ----------
         xa : float
-            lower limit of the partial sum / integral.
+            Lower limit of the partial sum / integral.
         xb : float
-            upper limit of the partial sum / integral.
+            Upper limit of the partial sum / integral.
         order : int
-            moment order.
+            Moment order.
 
         Returns
         -------
         float
-            numerical approximation to partial moment.
+            Numerical approximation to partial moment.
         """
         # cast to float is required to use mpmath with ufuncs
         def f(z): return (z**order)*self._pdf0_length(float(z))
 
         if self._continuous:
             result, _ = integrate.quad(f, xa, xb, limit=50, epsrel=1e-4)
         else:
             result = float(mpmath.nsum(f, [max(1, int(xa)), xb]))
         return result
 
     def _cdf_length(self,
-                    x: Union[float, ndarray],
+                    x: FloatOrArray,
                     order: int
-                    ) -> Union[float, ndarray[Any, dtype[float64]]]:
-        """Cumulative distribution function.
+                    ) -> FloatOrArray:
+        r"""Cumulative distribution function.
 
         This implementation is a general low-performance fallback solution.
         Preferably, child classes should implement a specific (e.g., analytic)
         method delivering the cumulative distribution function for the number
         _and_ mass distribution.
 
         Parameters
         ----------
-        x : float | ndarray
+        x : FloatOrArray
             Chain length.
         order : int
             Order of the distribution (0: number, 1: mass).
 
         Returns
         -------
-        float | ndarray
+        FloatOrArray
             Cumulative distribution value.
         """
         return self._moment_quadrature(np.zeros_like(x), x, order) \
             / self._moment_length(order)
 
     @functools.cache
     def _moment_length(self,
                        order: int
                        ) -> float:
-        """Chain-length moments of the _number_ probability density/mass
+        r"""Chain-length moments of the _number_ probability density/mass
         function.
 
         This implementation is a general low-performance fallback solution.
         Preferably, child classes should implement a specific (e.g., analytic)
         method delivering the first four moments (0-3) of the number pdf.
 
         Parameters
@@ -521,57 +528,57 @@
             Moment of the number distribution.
         """
         # print("Warning: using low performance 'moment_length' method.")
         return self._moment_quadrature(0, np.Inf, order)
 
     @abstractmethod
     def _pdf0_length(self,
-                     k: Union[float, ndarray]
-                     ) -> Union[float, ndarray[Any, dtype[float64]]]:
-        """Probability density/mass function.
+                     k: FloatOrArray
+                     ) -> FloatOrArray:
+        r"""Probability density/mass function.
 
         Each child class must implement a method delivering the _number_
         probability density/mass function.
 
         Parameters
         ----------
-        k : float | ndarray
+        k : FloatOrArray
             Chain length.
 
         Returns
         -------
-        float | ndarray
+        FloatOrArray
             Probability density/mass value.
         """
         pass
 
 
 class AnalyticalDistribution(IndividualDistribution):
-    """Abstract class for all analytical chain-length distributions."""
+    r"""_Abstract_ class for all analytical chain-length distributions.
+
+    Parameters
+    ----------
+    DPn : int
+        Number-average degree of polymerization, $DP_n$.
+    M0 : float
+        Molar mass of the repeating unit, $M_0$.
+    name : str
+        Name
+    """
 
     # (min-DPn, max-DPn)
     _pbounds = ((2,), (np.Inf,))
     _ppf_bounds = (1e-4, 0.9999)
 
     def __init__(self,
                  DPn: int,
                  M0: float = 100.0,
                  name: str = ''
                  ) -> None:
-        """Initialize 1-parameter analytical distribution.
 
-        Parameters
-        ----------
-        DPn : int
-            Number-average degree of polymerization, $DP_n$.
-        M0 : float
-            Molar mass of the repeating unit, $M_0$.
-        name : str
-            Name
-        """
         self.DPn = DPn
         self.M0 = M0
         self.name = name
         self._rng = None  # type: ignore
 
     @property
     def DPn(self) -> float:
@@ -589,15 +596,15 @@
     def _pvalues(self) -> tuple:
         """Value(s) defining the chain-length pdf. Used for generalized access
         by fit method."""
         return (self.DPn,)
 
     def random(self,
                size: Union[int, tuple[int, ...], None] = None
-               ) -> Union[int, ndarray[Any, dtype[int64]]]:
+               ) -> IntOrArray:
         r"""Generate random sample of chain lengths according to the
         corresponding number probability density/mass function.
 
         Parameters
         ----------
         size : int | tuple[int, ...] | None
             Sample size.
@@ -609,17 +616,17 @@
         """
         if self._rng is None:
             self._rng = np.random.default_rng()
         return self._random_length(size)
 
     @abstractmethod
     def _random_length(self,
-                       size: Union[int, tuple, None],
-                       ) -> Union[int, ndarray[Any, dtype[int64]]]:
-        """Random chain-length generator.
+                       size: Union[int, tuple[int, ...], None],
+                       ) -> IntOrArray:
+        r"""Random chain-length generator.
 
         Each child class must implement a method to generate random chain
         lengths according to the statistics of the corresponding number
         density/mass function.
 
         Parameters
         ----------
@@ -631,43 +638,45 @@
         int | ndarray
             Random sample of chain lengths.
         """
         pass
 
 
 class AnalyticalDistributionP1(AnalyticalDistribution):
-    """Abstract class for 1-parameter analytical chain-length distributions."""
+    r"""_Abstract_ class for 1-parameter analytical chain-length distributions.
+    """
     pass
 
 
 class AnalyticalDistributionP2(AnalyticalDistribution):
-    """Abstract class for 2-parameter analytical chain-length distributions."""
+    r"""_Abstract_ class for 2-parameter analytical chain-length distributions.
+
+    Parameters
+    ----------
+    DPn : int
+        Number-average degree of polymerization, $DP_n$.
+    PDI : float
+        Polydispersity index, $PDI$.
+    M0 : float
+        Molar mass of the repeating unit, $M_0$.
+    name : str
+        Name.
+
+    """
 
     # ((min-DPn, min-PDI), (max-DPn, max-PDI))
     _pbounds = ((2, 1.000001), (np.Inf, np.Inf))
 
     def __init__(self,
                  DPn: int,
                  PDI: float,
                  M0: float = 100.0,
                  name: str = ''
                  ) -> None:
-        """Initialize 2-parameter analytical chain-length distribution.
 
-        Parameters
-        ----------
-        DPn : int
-            Number-average degree of polymerization, $DP_n$.
-        PDI : float
-            Polydispersity index, $PDI$.
-        M0 : float
-            Molar mass of the repeating unit, $M_0$.
-        name : str
-            Name.
-        """
         super().__init__(DPn=DPn, M0=M0, name=name)
         self.PDI = PDI
 
     @property
     def PDI(self) -> float:
         """Polydispersity index, $M_w/M_n$."""
         return self.__PDI  # type: ignore
@@ -681,16 +690,24 @@
 
     @property
     def _pvalues(self) -> tuple:
         """Value(s) defining the chain-length pdf."""
         return (self.DPn, self.PDI)
 
 
-class MixtureDistribution(GeneralDistribution):
-    """Mixture chain-length distribution."""
+class MixtureDistribution(Distribution):
+    r"""Mixture chain-length distribution.
+
+    This kind of distributions are instantiated _indirectly_ by doing linear
+    combinations of `IndividualDistribution` objects.
+
+    Example:
+    >>> blend = 2.0*Flory(100, name='A') + 1.0*Poisson(50, name='B')
+
+    """
 
     def __init__(self,
                  components: dict[IndividualDistribution, float],
                  name: str = ''
                  ) -> None:
 
         self.__components = components
@@ -720,37 +737,40 @@
 
     def __str__(self):
         if len(self.components) > 0:
             return super().__str__()
         else:
             return 'empty'
 
+    def __bool__(self):
+        return bool(self.components)
+
     @property
     def components(self) -> dict:
-        """Individual components of the mixture distribution.
+        r"""Individual components of the mixture distribution.
 
         Returns
         -------
         dict[IndividualDistribution: float]
             Dictionary of individual distributions and corresponding mass
             weight.
         """
         return self.__components
 
     @property
-    def components_table(self) -> Union[str, None]:
-        """Table of individual components of the mixture distribution.
+    def components_table(self) -> str:
+        r"""Table of individual components of the mixture distribution.
 
         Returns
         -------
         str
             Table with key properties of each component.
         """
         result = 'empty'
-        if len(self.components) > 0:
+        if self.components:
             spacer = f"{' '*3}"
             header = [f"{'#':>2}", f"{'Weight':>6}", f"{'Distribution':>12}",
                       f"{'DPn':>8}", f"{'DPw':>8}", f"{'PDI':>4}"]
             header = (spacer).join(header)
             ruler = f"{'-'*len(header)}"
             table = [header, ruler]
             for i, (d, w) in enumerate(self.components.items()):
@@ -808,31 +828,48 @@
         xrange[1] = max([d._xrange_plot(sizeasmass)[1]
                          for d in self.__iter__()])
         return xrange
 
 # %% Aux functions
 
 
-def plotdists(dists: list[GeneralDistribution],
-              kind: Literal['number', 'mass', 'gpc'],
+def plotdists(dists: list[Distribution],
+              kind: Kind,
               title: Union[str, None] = None,
-              **kwargs):
+              **kwargs
+              ) -> Figure:
+    """Plot a list of distributions in a joint plot.
+
+    Parameters
+    ----------
+    dists : list[GeneralDistribution]
+        List of distributions to be ploted together.
+    kind : Literal['number', 'mass', 'gpc']
+        Kind of distribution.
+    title : str | None
+        Title of plot.
+
+    Returns
+    -------
+    Figure
+        Matplotlib Figure object holding the joint plot.
+    """
 
     # Check input
-    kind = GeneralDistribution._verify_kind(kind)
+    kind = Distribution._verify_kind(kind)
 
-    # Create matplot and axes objects
+    # Create matplotlib objects
     fig, ax = plt.subplots(1, 1)
     if kwargs.get('cdf', 1) == 2:
         ax.twinx()
 
     # Title
-    titles = {'number': 'Number', 'mass': 'Mass', 'gpc': 'GPC'}
     if title is None:
+        titles = {'number': 'Number', 'mass': 'Mass', 'gpc': 'GPC'}
         title = f"{titles.get(kind,'')} distributions"
     fig.suptitle(title)
 
-    # Build plots sequentially
+    # Draw plots sequentially
     for d in dists:
         d.plot(kinds=kind, axes=fig.axes, **kwargs)
 
     return fig
```

### Comparing `polykin-0.1.0/src/polykin/distributions/datadistribution.py` & `polykin-0.2.0/src/polykin/distributions/datadistribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 # %% Data distribution
 
-from polykin.utils import vectorize, check_subclass, Vector
+from polykin.utils import vectorize, check_subclass, FloatArrayLike
 from polykin.distributions import Flory, Poisson, LogNormal, SchulzZimm
 from polykin.distributions.baseclasses import Kind, \
     IndividualDistribution, MixtureDistribution,\
     AnalyticalDistribution, AnalyticalDistributionP2
 
 import numpy as np
 from scipy import interpolate, integrate, optimize
 from typing import Union
 import functools
 
 
 class DataDistribution(IndividualDistribution):
     """Arbitrary numerical chain-length distribution, defined by chain size
     and pdf data.
+
+    Parameters
+    ----------
+    size_data : FloatArrayLike
+        Chain length or molar mass data.
+    pdf_data : FloatArrayLike
+        Distribution data.
+    kind : Literal['number', 'mass', 'gpc']
+        Kind of distribution.
+    sizeasmass : bool
+        Switch size input between chain-*length* (if `False`) or molar
+        *mass* (if `True`).
+    M0 : float
+        Molar mass of the repeating unit, $M_0$.
+    name : str
+        Name.
     """
     _continuous = True
 
     def __init__(self,
-                 size_data: Vector,
-                 pdf_data: Vector,
+                 size_data: FloatArrayLike,
+                 pdf_data: FloatArrayLike,
                  kind: Kind = 'mass',
                  sizeasmass: bool = False,
                  M0: float = 100,
                  name: str = ''
                  ) -> None:
 
         # Check and clean input
@@ -85,25 +101,25 @@
             display_table: bool = True
             ) -> Union[AnalyticalDistribution, MixtureDistribution, None]:
         """Fit (deconvolute) a `DataDistribution` into a linear combination of
         `AnalyticalDistribution`(s).
 
         Parameters
         ----------
-        dist_class : Union[type[Flory], type[Poisson], type[LogNormal], type[SchulzZimm]]
+        dist_class : type[Flory] | type[Poisson] | type[LogNormal] | type[SchulzZimm]
             Type of distribution to be used in the fit.
         dim : int
             Number of individual components to use in the fit.
         display_table : bool
             Option to display results table with information about individual
             components.
 
         Returns
         -------
-        Union[AnalyticalDistribution, MixtureDistribution, None]
+        AnalyticalDistribution | MixtureDistribution | None
             If fit successful, it returns the fitted distribution.
         """
 
         check_subclass(dist_class, AnalyticalDistribution, 'dist_class')
         isP2 = issubclass(dist_class, AnalyticalDistributionP2)
 
         # Init fit distribution
```

### Comparing `polykin-0.1.0/src/polykin/distributions/sampledata.py` & `polykin-0.2.0/src/polykin/distributions/sampledata.py`

 * *Files identical despite different names*

### Comparing `polykin-0.1.0/src/polykin/utils.py` & `polykin-0.2.0/src/polykin/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,53 @@
 from collections.abc import Iterable
 import numbers
 import functools
 import numpy as np
-from numpy import ndarray, dtype, float64
 from typing import Union, Any
+from nptyping import NDArray, Shape, Int32, Float64
 
 # %% Own types
-Vector = Union[list[float], ndarray[Any, dtype[float64]]]
 
+IntArray = NDArray[Any, Int32]
+IntArrayLike = Union[list[int], IntArray]
+IntOrArray = Union[int, IntArray]
+IntOrArrayLike = Union[int, IntArrayLike]
+
+FloatArray = NDArray[Any, Float64]
+FloatArrayLike = Union[list[float], FloatArray]
+FloatOrArray = Union[float, FloatArray]
+FloatOrArrayLike = Union[float, FloatArrayLike]
+
+FloatVector = NDArray[Shape['*'], Float64]
+FloatVectorLike = Union[list[float], FloatVector]
+
+FloatRange = Union[list[float], tuple[float, float],
+                   NDArray[Shape['1, 2'], Float64]]
+
+# %% Maths
+
+eps = float(np.finfo(np.float64).eps)
+
+# %% Custom exceptions
+
+
+class RangeWarning(Warning):
+    pass
+
+
+class RangeError(ValueError):
+    pass
+
+
+class ShapeError(ValueError):
+    pass
 
 # %% Check tools
 
+
 def custom_error(var_name: str,
                  var_value: Any,
                  kind: type,
                  message: str = ""
                  ) -> None:
     """
     Custom error message function.
@@ -39,15 +72,15 @@
         error_message += " " + message
     # print(f"{kind}: {error_message}")
     # sys.exit(1)
     raise kind(error_message)
 
 
 def check_type(var_value: Any,
-               valid_types: Any,
+               valid_types: Union[type, tuple[type, ...]],
                var_name: str,
                check_inside: bool = False
                ) -> Any:
     """
     Check if a variable is of a given type.
 
     Parameters
@@ -120,51 +153,52 @@
             myobject_name,
             myobject,
             TypeError,
             f"Valid `{myobject_name}` types are: {valid_class}.",
         )
 
 
-def check_bounds(x: float,
+def check_bounds(x: Union[float, np.ndarray],
                  xmin: float,
                  xmax: float,
                  xname: str
-                 ) -> Union[float, None]:
+                 ) -> Union[float, np.ndarray, None]:
     """Check if a numerical value is between given bounds.
 
     Example:
     -------
     >>> check_bounds(1.0, 0.1, 2.0, 'x') -> 1.0
     >>> check_bounds(-1.0, 0.1, 2.0, 'x') -> ValueError
 
     Parameters
     ----------
-    x : float
+    x : float | ndarray
         Variable.
     xmin : float
         Lower bound.
     xmax : float
         Upper bound.
     xname : str
         Variable name.
 
     Returns
     -------
-    x : float
+    x : float | ndarray
         Variable.
 
     """
-
-    x = check_type(x, numbers.Number, xname)
-
-    if x >= xmin and x <= xmax:
+    if isinstance(x, numbers.Number) and (x >= xmin) and (x <= xmax):
+        return x
+    elif isinstance(x, np.ndarray) and \
+            np.all(np.logical_and.reduce((x >= xmin, x <= xmax))):
         return x
     else:
+        check_type(x, (numbers.Number, np.ndarray), xname)
         custom_error(
-            xname, x, ValueError, f"Valid `{xname}` range is [{xmin}, {xmax}]."
+            xname, x, RangeError, f"Valid `{xname}` range is [{xmin}, {xmax}]."
         )
 
 
 def check_in_set(var_value: Any,
                  valid_set: set,
                  var_name: str = "#"
                  ) -> Any:
```

### Comparing `polykin-0.1.0/PKG-INFO` & `polykin-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: polykin
-Version: 0.1.0
+Version: 0.2.0
 Summary: A polymerization kinetics library.
 Home-page: https://hugomvale.github.io/polykin/
 License: MIT
 Keywords: polymer,polymerization,kinetics,reaction
 Author: HugoMVale
 Author-email: 57530119+HugoMVale@users.noreply.github.com
-Requires-Python: >=3.9,<4
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mpmath (>=1.2.1,<2.0.0)
-Requires-Dist: numba (>=0.56.4,<0.57.0)
-Requires-Dist: numpy (>=1.23)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: nptyping (>=2.5.0,<3.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Documentation, https://hugomvale.github.io/polykin/
 Project-URL: Repository, https://github.com/HugoMVale/polykin
 Description-Content-Type: text/markdown
 
 # PolyKin
 
-[![CI](https://github.com/HugoMVale/polykin/actions/workflows/CI.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions)
+[![Test](https://github.com/HugoMVale/polykin/actions/workflows/test.yml/badge.svg)](https://github.com/HugoMVale/polykin/actions)
 [![codecov](https://codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/polykin)
 [![Latest Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-commit/HugoMVale/polykin)
 
 PolyKin is an open-source polymerization kinetics library for Python. It is still at an early
 development stage, but the following modules can already be used:
 
 - [x] distributions
+- [x] coefficients
 - [ ] copolymerization
 - [ ] kinetics
 - [ ] database
 - [ ] models
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: polykin Version: 0.1.0 Summary: A polymerization
+Metadata-Version: 2.1 Name: polykin Version: 0.2.0 Summary: A polymerization
 kinetics library. Home-page: https://hugomvale.github.io/polykin/ License: MIT
 Keywords: polymer,polymerization,kinetics,reaction Author: HugoMVale Author-
-email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<4
+email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-Dist:
-matplotlib (>=3.6.2,<4.0.0) Requires-Dist: mpmath (>=1.2.1,<2.0.0) Requires-
-Dist: numba (>=0.56.4,<0.57.0) Requires-Dist: numpy (>=1.23) Requires-Dist:
-pydantic (>=1.10.4,<2.0.0) Requires-Dist: scipy (>=1.9.3,<2.0.0) Project-URL:
-Documentation, https://hugomvale.github.io/polykin/ Project-URL: Repository,
-https://github.com/HugoMVale/polykin Description-Content-Type: text/markdown #
-PolyKin [![CI](https://github.com/HugoMVale/polykin/actions/workflows/CI.yml/
-badge.svg)](https://github.com/HugoMVale/polykin/actions) [![codecov](https://
-codecov.io/gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)]
-(https://codecov.io/gh/HugoMVale/polykin) [![Latest Commit](https://
-img.shields.io/github/last-commit/HugoMVale/polykin)](https://img.shields.io/
-github/last-commit/HugoMVale/polykin) PolyKin is an open-source polymerization
-kinetics library for Python. It is still at an early development stage, but the
-following modules can already be used: - [x] distributions - [ ]
-copolymerization - [ ] kinetics - [ ] database - [ ] models ## Documentation
-Please refer to the package [homepage](https://hugomvale.github.io/polykin/).
-## Tutorials The main features of PolyKin are explained and illustrated through
-a series of [tutorials](https://hugomvale.github.io/polykin/tutorials/
-distributions/) based on Jupyter [notebooks](https://github.com/HugoMVale/
-polykin/tree/main/docs/tutorials), which can be launched online via Binder.
+Python :: 3.10 Classifier: Programming Language :: Python :: 3 Classifier:
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Chemistry Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: mpmath
+(>=1.2.1,<2.0.0) Requires-Dist: nptyping (>=2.5.0,<3.0.0) Requires-Dist: numpy
+(>=1.24.2,<2.0.0) Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist:
+scipy (>=1.10.1,<2.0.0) Project-URL: Documentation, https://
+hugomvale.github.io/polykin/ Project-URL: Repository, https://github.com/
+HugoMVale/polykin Description-Content-Type: text/markdown # PolyKin [![Test]
+(https://github.com/HugoMVale/polykin/actions/workflows/test.yml/badge.svg)]
+(https://github.com/HugoMVale/polykin/actions) [![codecov](https://codecov.io/
+gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://
+codecov.io/gh/HugoMVale/polykin) [![Latest Commit](https://img.shields.io/
+github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-
+commit/HugoMVale/polykin) PolyKin is an open-source polymerization kinetics
+library for Python. It is still at an early development stage, but the
+following modules can already be used: - [x] distributions - [x] coefficients -
+[ ] copolymerization - [ ] kinetics - [ ] database - [ ] models ##
+Documentation Please refer to the package [homepage](https://
+hugomvale.github.io/polykin/). ## Tutorials The main features of PolyKin are
+explained and illustrated through a series of [tutorials](https://
+hugomvale.github.io/polykin/tutorials/distributions/) based on Jupyter
+[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
+which can be launched online via Binder.
                            [MWD_of_a_polymer_blend]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

