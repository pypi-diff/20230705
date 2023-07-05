# Comparing `tmp/compmec_nurbs-1.0.3.tar.gz` & `tmp/compmec_nurbs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compmec_nurbs-1.0.3.tar", max compression
+gzip compressed data, was "compmec_nurbs-1.0.4.tar", max compression
```

## Comparing `compmec_nurbs-1.0.3.tar` & `compmec_nurbs-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35142 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     1846 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/README.md
--rw-r--r--   0        0        0      543 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3063 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/src/compmec/nurbs/__classes__.py
--rw-r--r--   0        0        0      220 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/src/compmec/nurbs/__init__.py
--rw-r--r--   0        0        0    10541 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/algorithms.py
--rw-r--r--   0        0        0    12759 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/curves.py
--rw-r--r--   0        0        0     8233 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/functions.py
--rw-r--r--   0        0        0     8362 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/knotspace.py
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35142 2023-07-05 10:35:21.767464 compmec_nurbs-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     2142 2023-07-05 10:35:21.767464 compmec_nurbs-1.0.4/README.md
+-rw-r--r--   0        0        0      543 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3316 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/__classes__.py
+-rw-r--r--   0        0        0      175 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/__init__.py
+-rw-r--r--   0        0        0    10541 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/algorithms.py
+-rw-r--r--   0        0        0    12888 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/curves.py
+-rw-r--r--   0        0        0     8153 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/functions.py
+-rw-r--r--   0        0        0     8362 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/knotspace.py
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.4/PKG-INFO
```

### Comparing `compmec_nurbs-1.0.3/LICENSE.md` & `compmec_nurbs-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compmec_nurbs-1.0.3/pyproject.toml` & `compmec_nurbs-1.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compmec-nurbs"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 readme = "README.md"
 authors = ["Carlos Adir <carlos.adir@gmail.com>"]
 packages = [{ include = "compmec/nurbs", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `compmec_nurbs-1.0.3/src/compmec/nurbs/__classes__.py` & `compmec_nurbs-1.0.4/src/compmec/nurbs/__classes__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,51 +38,65 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def __ne__(self, obj: object) -> bool:
         raise NotImplementedError
 
 
-class Intface_BaseFunction_Evaluator_BaseCurve(abc.ABC):
+class Intface_Evaluator(abc.ABC):
     @abc.abstractproperty
-    def knotvector(self) -> Intface_KnotVector:
+    def evalf(self) -> Union[int, slice]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def __call__(self, u: np.ndarray) -> np.ndarray:
         raise NotImplementedError
 
 
-class Intface_Evaluator(Intface_BaseFunction_Evaluator_BaseCurve):
-    @abc.abstractproperty
-    def first_index(self) -> Union[int, slice]:
+class Intface_BaseFunction_BaseCurve(abc.ABC):
+    @abc.abstractmethod
+    def __eq__(self, obj: object) -> bool:
         raise NotImplementedError
 
-    @abc.abstractproperty
-    def second_index(self) -> Union[int, slice]:
+    @abc.abstractmethod
+    def __ne__(self, obj: object) -> bool:
         raise NotImplementedError
 
+    @abc.abstractproperty
+    def knotvector(self) -> Intface_KnotVector:
+        raise NotImplementedError
 
-class Intface_BaseFunction_BaseCurve(Intface_BaseFunction_Evaluator_BaseCurve):
     @abc.abstractproperty
     def degree(self) -> int:
         raise NotImplementedError
 
     @abc.abstractproperty
     def npts(self) -> int:
         raise NotImplementedError
 
+    @abc.abstractproperty
+    def knots(self) -> int:
+        raise NotImplementedError
+
     @abc.abstractmethod
     def knot_insert(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
     @abc.abstractmethod
     def knot_remove(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def degree_increase(self, times: Optional[int] = 1):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def degree_decrease(self, times: Optional[int] = 1):
+        raise NotImplementedError
+
 
 class Intface_BaseFunction(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
     def __init__(self, knotvector: Intface_KnotVector):
         raise NotImplementedError
 
     @abc.abstractmethod
@@ -100,13 +114,13 @@
         raise NotImplementedError
 
     @abc.abstractproperty
     def ctrlpoints(self) -> np.ndarray:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __eq__(self, obj: object) -> bool:
+    def knot_clean(self):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __ne__(self, obj: object) -> bool:
+    def degree_clean(self):
         raise NotImplementedError
```

### Comparing `compmec_nurbs-1.0.3/src/compmec/nurbs/algorithms.py` & `compmec_nurbs-1.0.4/src/compmec/nurbs/algorithms.py`

 * *Files identical despite different names*

### Comparing `compmec_nurbs-1.0.3/src/compmec/nurbs/curves.py` & `compmec_nurbs-1.0.4/src/compmec/nurbs/curves.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 from typing import Optional, Tuple, Union
 
 import numpy as np
 
 from compmec.nurbs import algorithms as algo
 from compmec.nurbs.__classes__ import Intface_BaseCurve
-from compmec.nurbs.functions import RationalFunction, SplineFunction
+from compmec.nurbs.functions import Function
 from compmec.nurbs.knotspace import KnotVector
 
 
 class BaseCurve(Intface_BaseCurve):
-    def __init__(self, knotvector: KnotVector, ctrlpoints: np.ndarray):
-        self.__set_UFP(knotvector, ctrlpoints)
+    def __init__(self, knotvector: KnotVector):
+        self.knotvector = KnotVector(knotvector)
 
     def deepcopy(self) -> Intface_BaseCurve:
-        return self.__class__(self.knotvector, self.ctrlpoints)
+        curve = self.__class__(self.knotvector)
+        curve.ctrlpoints = self.ctrlpoints
+        return curve
 
     def __call__(self, u: np.ndarray) -> np.ndarray:
         return self.evaluate(u)
 
     def evaluate(self, u: np.ndarray) -> np.ndarray:
+        if self.ctrlpoints is None:
+            error_msg = "Cannot evaluate: There are no control points"
+            raise ValueError(error_msg)
         L = self.F(u)
-        return L.T @ self.ctrlpoints
+        return np.moveaxis(L, 0, -1) @ self.ctrlpoints
+
+    @property
+    def knotvector(self):
+        return KnotVector(self.__knotvector)
 
     @property
     def degree(self):
         return self.knotvector.degree
 
     @property
     def npts(self):
         return self.knotvector.npts
 
     @property
-    def knotvector(self):
-        return self.F.knotvector
-
-    @property
     def knots(self):
-        return self.F.knots
-
-    @property
-    def F(self):
-        return self.__F
+        return self.knotvector.knots
 
     @property
     def ctrlpoints(self):
         return self.__ctrlpoints
 
+    @knotvector.setter
+    def knotvector(self, value: KnotVector):
+        self.__knotvector = KnotVector(value)
+
     @degree.setter
     def degree(self, value: int):
         value = int(value)
         if value < 1:
             raise ValueError("The degree must be 1 or higher!")
         if value == self.degree:
             return
         if value > self.degree:
             self.__degree_increase(value - self.degree)
         else:
             self.__degree_decrease(self.degree - value)
 
     @ctrlpoints.setter
     def ctrlpoints(self, value: np.ndarray):
+        if value is None:
+            self.__ctrlpoints = None
+            return
         try:
             iter(value)
         except Exception:
             raise ValueError
         if len(value) != self.npts:
             error_msg = "The number of control points must be the same as"
             error_msg += " degrees of freedom of KnotVector.\n"
@@ -74,19 +82,14 @@
             1.0 * value[0] - 1.5 * value[0] + 3.1 * value[0]
         except Exception:
             error_msg = "For each control point P, it's needed operations"
             error_msg = "with floats like 1.0*P - 1.5*P + 3.1*P"
             raise ValueError(error_msg)
         self.__ctrlpoints = value
 
-    def __set_UFP(self, knotvector: KnotVector, ctrlpoints: np.ndarray):
-        knotvector = KnotVector(knotvector)
-        self.__F = self._create_base_function_instance(knotvector)
-        self.ctrlpoints = ctrlpoints
-
     def __eq__(self, other: object) -> bool:
         if type(self) != type(other):
             return False
         if self.knotvector[0] != other.knotvector[0]:
             return False
         if self.knotvector[-1] != other.knotvector[-1]:
             return False
@@ -169,15 +172,16 @@
         newknotvector = np.array(self.knotvector).tolist()
 
         newknotvector.extend(nodes)
         newknotvector.sort()
         newknotvector = KnotVector(newknotvector)
         T, _ = algo.LeastSquare.spline(self.knotvector, newknotvector)
         newcontrolpoints = T @ self.ctrlpoints
-        self.__set_UFP(newknotvector, newcontrolpoints)
+        self.__knotvector = KnotVector(newknotvector)
+        self.ctrlpoints = newcontrolpoints
 
     def knot_remove(
         self, nodes: Union[float, Tuple[float]], tolerance: float = 1e-9
     ) -> None:
         nodes = np.array(nodes, dtype="float64").flatten()
         nodes_requested = list(set(list(nodes)))
         newknotvector = list(self.knotvector)
@@ -200,15 +204,16 @@
         error = np.moveaxis(self.ctrlpoints, 0, -1) @ E @ self.ctrlpoints
         error = np.max(np.abs(error))
         if error > tolerance:
             error_msg = f"Cannot remove the nodes {nodes} cause the "
             error_msg += f" error ({error:.1e}) is > {tolerance:.1e} "
             raise ValueError(error_msg)
         newctrlpoints = T @ self.ctrlpoints
-        self.__set_UFP(newknotvector, newctrlpoints)
+        self.__knotvector = KnotVector(newknotvector)
+        self.ctrlpoints = newctrlpoints
 
     def knot_clean(self, tolerance: float = 1e-9) -> None:
         """
         Remove all unecessary knots.
         If removing the knot the error is bigger than the tolerance,
         nothing happens
         """
@@ -221,15 +226,16 @@
                 pass
 
     def __degree_increase(self, times: int):
         newknotvector = list(self.knotvector) + times * list(self.knots)
         newknotvector.sort()
         T, _ = algo.LeastSquare.spline(self.knotvector, newknotvector)
         newctrlpoints = T @ self.ctrlpoints
-        self.__set_UFP(newknotvector, newctrlpoints)
+        self.__knotvector = KnotVector(newknotvector)
+        self.ctrlpoints = newctrlpoints
 
     def __degree_decrease(self, times: int = 1, tolerance: float = 1e-9):
         newknotvector = list(self.knotvector)
         for knot in self.knots:
             mult = min(times, self.knotvector.mult(knot))
             for i in range(mult):
                 newknotvector.remove(knot)
@@ -237,15 +243,16 @@
         error = np.moveaxis(self.ctrlpoints, 0, -1) @ E @ self.ctrlpoints
         error = np.max(np.abs(error))
         if error > tolerance:
             error_msg = f"Cannot reduce degree {times} times "
             error_msg += f"cause the error ({error:.1e}) is > {tolerance:.1e} "
             raise ValueError(error_msg)
         newctrlpoints = T @ self.ctrlpoints
-        self.__set_UFP(newknotvector, newctrlpoints)
+        self.__knotvector = newknotvector
+        self.ctrlpoints = newctrlpoints
 
     def degree_decrease(self, times: Optional[int] = 1):
         """
         The same as mycurve.degree -= 1
         But this function forces the degree reductions without looking the error
         """
         self.degree -= times
@@ -301,32 +308,35 @@
             newctrlpts = copycurve.ctrlpoints[lowerind:upperind]
             newcurve = self.__class__(newknotvec, newctrlpts)
             listcurves[i] = newcurve
         del copycurve
         return tuple(listcurves)
 
 
-class SplineCurve(BaseCurve):
-    def __init__(self, knotvector: KnotVector, ctrlpoints: np.ndarray):
-        super().__init__(knotvector, ctrlpoints)
-
-    def __repr__(self):
-        return f"SplineCurve of degree {self.degree} and {self.npts} control points"
-
-    def _create_base_function_instance(self, knotvector: KnotVector):
-        return SplineFunction(knotvector)
-
+class Curve(BaseCurve):
+    def __init__(
+        self,
+        knotvector: KnotVector,
+        ctrlpoints: Optional[np.ndarray] = None,
+        weights: Optional[np.ndarray] = None,
+    ):
+        super().__init__(knotvector)
+        self.ctrlpoints = ctrlpoints
+        self.weights = weights
 
-class RationalCurve(BaseCurve):
-    def __init__(self, knotvector: KnotVector, ctrlpoints: np.ndarray):
-        super().__init__(knotvector, ctrlpoints)
+    @property
+    def F(self):
+        function = Function(self.knotvector)
+        return function
 
-    def _create_base_function_instance(self, knotvector: KnotVector):
-        return RationalFunction(knotvector)
+    def deepcopy(self):
+        curve = super().deepcopy()
+        curve.weights = self.weights
+        return curve
 
     @property
     def weights(self):
-        return self.F.weights
+        return self.__weights
 
     @weights.setter
     def weights(self, value: Tuple[float]):
-        self.F.weights = value
+        self.__weights = value
```

### Comparing `compmec_nurbs-1.0.3/src/compmec/nurbs/functions.py` & `compmec_nurbs-1.0.4/src/compmec/nurbs/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,254 +6,233 @@
 from compmec.nurbs.__classes__ import Intface_BaseFunction, Intface_Evaluator
 from compmec.nurbs.algorithms import N, R
 from compmec.nurbs.knotspace import KnotVector
 
 
 class BaseFunction(Intface_BaseFunction):
     def __init__(self, knotvector: KnotVector):
-        self.__U = KnotVector(knotvector)
+        self.__knotvector = KnotVector(knotvector)
+        self.weights = None
+        self.__degree = self.knotvector.degree
+
+    def __eq__(self, other: Intface_BaseFunction) -> bool:
+        if not isinstance(other, Intface_BaseFunction):
+            return False
+        if self.degree != other.degree:
+            return False
+        if self.knotvector != other.knotvector:
+            return False
+        weightleft = self.weights
+        weightrigh = other.weights
+        weightleft = np.ones(self.npts) if self.weights is None else self.weights
+        weightrigh = np.ones(self.npts) if weightrigh is None else weightrigh
+        return np.all(weightleft == weightrigh)
+
+    def __ne__(self, other: Intface_BaseFunction) -> bool:
+        return not self.__eq__(other)
+
+    @property
+    def knotvector(self) -> KnotVector:
+        return self.__knotvector
 
     @property
     def degree(self) -> int:
-        return self.__U.degree
+        return self.__degree
 
     @property
     def npts(self) -> int:
-        return self.__U.npts
+        return self.knotvector.npts
 
     @property
-    def knotvector(self) -> KnotVector:
-        return self.__U
+    def knots(self) -> Tuple[float]:
+        return self.knotvector.knots
 
     @property
-    def knots(self) -> Tuple[float]:
-        return self.__U.knots
+    def weights(self) -> Union[Tuple[float], None]:
+        return self.__weights
+
+    @weights.setter
+    def weights(self, value: Tuple[float]):
+        if value is None:
+            self.__weights = None
+            return
+        value = np.array(value, dtype="float64")
+        if not np.all(value > 0):
+            error_msg = "All weights must be positive!"
+            raise ValueError(error_msg)
+        if value.shape != (self.npts,):
+            error_msg = f"Weights shape invalid! {value.shape} != ({self.npts})"
+            raise ValueError(error_msg)
+        self.__weights = value
+
+    @degree.setter
+    def degree(self, value: int):
+        self.__degree = int(value)
 
     def knot_insert(self, knot: float, times: Optional[int] = 1):
         self.knotvector.knot_insert(knot, times)
 
     def knot_remove(self, knot: float, times: Optional[int] = 1):
         self.knotvector.knot_remove(knot, times)
 
+    def degree_increase(self, times: Optional[int] = 1):
+        pass
 
-class BaseEvaluator(Intface_Evaluator):
-    def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
-        self.__U = F.knotvector
-        self.__first_index = i
-        self.__second_index = j
-        self.__A = F.A
+    def degree_decrease(self, times: Optional[int] = 1):
+        pass
 
-    @property
-    def knotvector(self) -> KnotVector:
-        return self.__U
+    @abc.abstractmethod
+    def evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        raise NotImplementedError
 
-    @property
-    def first_index(self) -> Union[int, range]:
-        return self.__first_index
+    def __call__(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        return self.evalf(nodes)
 
-    @property
-    def second_index(self) -> int:
-        return self.__second_index
 
-    @abc.abstractmethod
-    def compute_one_value(self, i: int, u: float, span: int) -> float:
-        raise NotImplementedError
+class FunctionEvaluator(Intface_Evaluator):
+    def __init__(self, func: BaseFunction, i: Union[int, slice], j: int):
+        self.__knotvector = func.knotvector
+        self.__weights = func.weights
+        self.__first_index = i
+        self.__second_index = j
 
-    def compute_vector(self, u: float, span: int) -> np.ndarray:
+    def compute_one_value(self, i: int, node: float, span: int) -> float:
+        j = self.__second_index
+        U = tuple(self.__knotvector)
+        if self.__weights is None:
+            return N(i, j, span, node, U)
+        return R(i, j, span, node, U, self.__weights)
+
+    def compute_vector(self, node: float, span: int) -> np.ndarray:
         """
         Given a 'u' float, it returns the vector with all BasicFunctions:
         compute_vector(u, span) = [F_{0j}(u), F_{1j}(u), ..., F_{npts-1,j}(u)]
         """
-        result = np.zeros(self.__U.npts, dtype="float64")
+        npts = self.__knotvector.npts
+        result = np.zeros(npts, dtype="float64")
         # for i in range(span, span+self.second_index):
-        for i in range(self.__U.npts):
-            result[i] = self.compute_one_value(i, u, span)
+        for i in range(npts):
+            result[i] = self.compute_one_value(i, node, span)
         return result
 
-    def compute_all(
-        self, u: Union[float, np.ndarray], span: Union[int, np.ndarray]
-    ) -> np.ndarray:
-        u = np.array(u, dtype="float64")
-        if span.ndim == 0:
-            return self.compute_vector(float(u), int(span))
-        result = np.zeros([self.__U.npts] + list(u.shape))
-        for k, (uk, sk) in enumerate(zip(u, span)):
-            result[:, k] = self.compute_all(uk, sk)
+    def compute_matrix(
+        self, nodes: Tuple[float], spans: Union[int, np.ndarray]
+    ) -> Tuple[Tuple[float]]:
+        """
+        Receives an 1D array of nodes, and returns a 2D array.
+        nodes.shape = (len(nodes), )
+        result.shape = (npts, len(nodes))
+        """
+        nodes = np.array(nodes, dtype="float64")
+        newshape = [self.__knotvector.npts] + list(nodes.shape)
+        result = np.zeros(newshape, dtype="float64")
+        for i, (nodei, spani) in enumerate(zip(nodes, spans)):
+            result[:, i] = self.compute_vector(nodei, spani)
         return result
 
-    def evalf(self, u: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def __evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
         """
         If i is integer, u is float -> float
         If i is integer, u is np.ndarray, ndim = k -> np.ndarray, ndim = k
         If i is slice, u is float -> 1D np.ndarray
         if i is slice, u is np.ndarray, ndim = k -> np.ndarray, ndim = k+1
         """
-        u = np.array(u, dtype="float64")
-        span = self.__U.span(u)
-        span = np.array(span, dtype="int16")
-        return self.compute_all(u, span)
-
-    def __call__(self, u: np.ndarray) -> np.ndarray:
-        result = self.evalf(u)
-        result = self.__A @ result
-        return result[self.first_index]
-
+        nodes = np.array(nodes, dtype="float64")
+        flat_nodes = nodes.flatten()
+        flat_spans = self.__knotvector.span(flat_nodes)
+        flat_spans = np.array(flat_spans, dtype="int16")
+        newshape = [self.__knotvector.npts] + list(nodes.shape)
+        result = self.compute_matrix(flat_nodes, flat_spans)
+        return result.reshape(newshape)
 
-class SplineEvaluatorClass(BaseEvaluator):
-    def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
-        super().__init__(F, i, j)
-
-    def compute_one_value(self, i: int, u: float, span: int) -> float:
-        return N(i, self.second_index, span, u, self.knotvector)
-
-
-class RationalEvaluatorClass(BaseEvaluator):
-    def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
-        super().__init__(F, i, j)
-        self.__weights = F.weights
+    def evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        """
+        If i is integer, u is float -> float
+        If i is integer, u is np.ndarray, ndim = k -> np.ndarray, ndim = k
+        If i is slice, u is float -> 1D np.ndarray
+        if i is slice, u is np.ndarray, ndim = k -> np.ndarray, ndim = k+1
+        """
+        return self.__evalf(nodes)[self.__first_index]
 
-    def compute_one_value(self, i: int, u: float, span: int) -> float:
-        j = self.second_index
-        U = self.knotvector
-        w = self.__weights
-        return R(i, j, span, u, U, w)
+    def __call__(self, nodes: np.ndarray) -> np.ndarray:
+        return self.evalf(nodes)
 
 
-class BaseFunctionDerivable(BaseFunction):
-    def __init__(self, knotvector: KnotVector):
-        super().__init__(knotvector)
-        self.__q = self.degree
-        self.__A = np.eye(self.npts, dtype="float64")
-
-    @property
-    def q(self) -> int:
-        return self.__q
-
-    @property
-    def A(self) -> np.ndarray:
-        return np.copy(self.__A)
-
-    def derivate(self):
-        avals = np.zeros(self.npts)
-        for i in range(self.npts):
-            diff = (
-                self.knotvector[i + self.degree] - self.knotvector[i]
-            )  # Maybe it's wrong
-            if diff != 0:
-                avals[i] = self.degree / diff
-        newA = np.diag(avals)
-        for i in range(self.npts - 1):
-            newA[i, i + 1] = -avals[i + 1]
-        self.__A = self.__A @ newA
-        self.__q -= 1
-
-
-class BaseFunctionGetItem(BaseFunctionDerivable):
+class IndexableFunction(BaseFunction):
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
 
     def __valid_first_index(self, index: Union[int, slice]):
         if not isinstance(index, (int, slice)):
             raise TypeError
         if isinstance(index, int):
-            if not (-self.npts <= index < self.npts):
+            npts = self.npts
+            if not (-npts <= index < npts):
                 raise IndexError
 
     def __valid_second_index(self, index: int):
         if not isinstance(index, int):
             raise TypeError
         if not (0 <= index <= self.degree):
             error_msg = f"Second index (={index}) "
             error_msg += f"must be in [0, {self.degree}]"
             raise IndexError(error_msg)
 
-    @abc.abstractmethod
-    def create_evaluator_instance(self, i: Union[int, slice], j: int):
-        raise NotImplementedError
-
     def __getitem__(self, tup: Any):
         if isinstance(tup, tuple):
             if len(tup) > 2:
                 raise IndexError
             i, j = tup
         else:
-            i, j = tup, self.q
+            i, j = tup, self.degree
         self.__valid_first_index(i)
         self.__valid_second_index(j)
-        return self.create_evaluator_instance(i, j)
-
-    def __call__(self, u: np.ndarray) -> np.ndarray:
-        i, j = slice(None, None, None), self.degree
-        evaluator = self.create_evaluator_instance(i, j)
-        return evaluator(u)
-
-    def __eq__(self, obj: object) -> bool:
-        if type(self) != type(obj):
-            raise TypeError
-        if self.knotvector != obj.knotvector:
-            return False
-        if self.q != obj.q:
-            return False
-        return True
-
-
-class SplineFunction(BaseFunctionGetItem):
-    def __doc__(self):
-        """
-        This function is recursively determined like
-
-        N_{i, 0}(u) = { 1   if  knotvector[i] <= u < knotvector[i+1]
-                      { 0   else
+        return FunctionEvaluator(self, i, j)
 
-                          u - knotvector[i]
-        N_{i, j}(u) = --------------- * N_{i, j-1}(u)
-                       knotvector[i+j] - knotvector[i]
-                            knotvector[i+j+1] - u
-                      + ------------------- * N_{i+1, j-1}(u)
-                         knotvector[i+j+1] - knotvector[i+1]
-
-        As consequence, we have that
-
-        N_{i, j}(u) = 0   if  ( u not in [knotvector[i], knotvector[i+j+1]] )
-
-        """
 
+class DerivableFunction(IndexableFunction):
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
+        self.__matrix = np.eye(self.npts, dtype="float64")
 
-    def create_evaluator_instance(self, i: Union[int, slice], j: int):
-        return SplineEvaluatorClass(self, i, j)
-
+    @property
+    def matrix(self) -> np.ndarray:
+        return np.copy(self.__matrix)
 
-class RationalFunction(BaseFunctionGetItem):
-    def __init__(self, knotvector: KnotVector):
-        super().__init__(knotvector)
+    def derivate(self):
+        """
+        Derivates the function once. If you want more, call it in a loop
+        """
+        avals = np.zeros(self.npts)
+        for i in range(self.npts):
+            diff = (
+                self.knotvector[i + self.degree] - self.knotvector[i]
+            )  # Maybe it's wrong
+            if diff != 0:
+                avals[i] = self.degree / diff
+        newA = np.diag(avals)
+        for i in range(self.npts - 1):
+            newA[i, i + 1] = -avals[i + 1]
+        self.__matrix = self.__matrix @ newA
+        self.degree -= 1
 
-    def create_evaluator_instance(self, i: Union[int, slice], j: int):
-        return RationalEvaluatorClass(self, i, j)
+    def evalf(self, nodes: np.ndarray) -> np.ndarray:
+        evaluator = self[:, self.degree]
+        return self.matrix @ evaluator(nodes)
 
-    def __eq__(self, obj):
-        if not super().__eq__(obj):
-            return False
-        if np.any(self.weights != obj.weights):
-            return False
-        return True
 
-    @property
-    def weights(self):
-        try:
-            return self.__weights
-        except AttributeError:
-            self.__weights = np.ones(self.npts, dtype="float64")
-        return self.__weights
+class Function(DerivableFunction):
+    def __doc__(self):
+        """
+        Spline and rational base function
+        """
 
-    @weights.setter
-    def weights(self, value: Tuple[float]):
-        value = np.array(value, dtype="float64")
-        if value.ndim != 1:
-            raise ValueError("Input must be 1D array")
-        if len(value) != self.npts:
-            error_msg = "Lenght of weights must be equal to knotvector.npts"
-            raise ValueError(error_msg)
-        if np.any(value <= 0):
-            raise ValueError("All the weights must be positive")
-        self.__weights = value
+    def __repr__(self) -> str:
+        if self.npts == self.degree + 1:
+            return f"Bezier function of degree {self.degree}"
+        elif self.weights is None:
+            msg = "Spline"
+        else:
+            msg = "Rational"
+        msg += f" function of degree {self.degree} "
+        msg += f"and {self.npts} points"
+        return msg
```

### Comparing `compmec_nurbs-1.0.3/src/compmec/nurbs/knotspace.py` & `compmec_nurbs-1.0.4/src/compmec/nurbs/knotspace.py`

 * *Files identical despite different names*

