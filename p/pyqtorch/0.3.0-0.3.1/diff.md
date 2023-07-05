# Comparing `tmp/pyqtorch-0.3.0.tar.gz` & `tmp/pyqtorch-0.3.1.tar.gz`

## Comparing `pyqtorch-0.3.0.tar` & `pyqtorch-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/publish.sh
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_converters.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22858 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    12266 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_converters.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/PKG-INFO
```

### Comparing `pyqtorch-0.3.0/.pre-commit-config.yaml` & `pyqtorch-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/CODE_OF_CONDUCT.md` & `pyqtorch-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/CONTRIBUTING.md` & `pyqtorch-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/mkdocs.yml` & `pyqtorch-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.3.1/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/QAOA.ipynb` & `pyqtorch-0.3.1/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/essentials.ipynb` & `pyqtorch-0.3.1/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/fit_function.ipynb` & `pyqtorch-0.3.1/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/gate_composition.ipynb` & `pyqtorch-0.3.1/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/hamevo.md` & `pyqtorch-0.3.1/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.3.1/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/bench.py` & `pyqtorch-0.3.1/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.3.1/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.3.1/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.3.1/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.3.1/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/__init__.py` & `pyqtorch-0.3.1/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/ansatz.py` & `pyqtorch-0.3.1/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/embedding.py` & `pyqtorch-0.3.1/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/matrices.py` & `pyqtorch-0.3.1/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/matrices_sparse.py` & `pyqtorch-0.3.1/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/converters/store_ops.py` & `pyqtorch-0.3.1/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.3.1/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/core/__init__.py` & `pyqtorch-0.3.1/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/core/batched_operation.py` & `pyqtorch-0.3.1/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/core/circuit.py` & `pyqtorch-0.3.1/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/core/measurement.py` & `pyqtorch-0.3.1/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/core/operation.py` & `pyqtorch-0.3.1/pyqtorch/core/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,34 @@
         store_operation("S", qubits)
 
     dev = state.device
     mat = OPERATIONS_DICT["S"].to(dev)
     return _apply_gate(state, mat, qubits, N_qubits)
 
 
+def Sdagger(state: torch.Tensor, qubits: ArrayLike, N_qubits: int) -> torch.Tensor:
+    """Sdagger single-qubit gate
+
+    Args:
+        state (torch.Tensor): the input quantum state, of shape `(N_0, N_1,..., N_N, batch_size)`
+        qubits (ArrayLike): list of qubit indices where the gate will operate
+        N_qubits (int): the number of qubits in the system
+
+    Returns:
+        torch.Tensor: the resulting state after applying the gate
+    """
+
+    if ops_cache.enabled:
+        store_operation("Sdagger", qubits)
+
+    dev = state.device
+    mat = OPERATIONS_DICT["SDAGGER"].to(dev)
+    return _apply_gate(state, mat, qubits, N_qubits)
+
+
 def T(state: torch.Tensor, qubits: ArrayLike, N_qubits: int) -> torch.Tensor:
     """T single-qubit gate
 
     Args:
         state (torch.Tensor): the input quantum state, of shape `(N_0, N_1,..., N_N, batch_size)`
         qubits (ArrayLike): list of qubit indices where the gate will operate
         N_qubits (int): the number of qubits in the system
```

### Comparing `pyqtorch-0.3.0/pyqtorch/core/utils.py` & `pyqtorch-0.3.1/pyqtorch/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 
 
 IMAT = torch.eye(2, dtype=torch.cdouble)
 XMAT = torch.tensor([[0, 1], [1, 0]], dtype=torch.cdouble)
 YMAT = torch.tensor([[0, -1j], [1j, 0]], dtype=torch.cdouble)
 ZMAT = torch.tensor([[1, 0], [0, -1]], dtype=torch.cdouble)
 SMAT = torch.tensor([[1, 0], [0, 1j]], dtype=torch.cdouble)
+SDAGGERMAT = torch.tensor([[1, 0], [0, -1j]], dtype=torch.cdouble)
 TMAT = torch.tensor([[1, 0], [0, torch.exp(torch.tensor(1.0j * torch.pi / 4))]])
 SWAPMAT = torch.tensor(
     [[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]], dtype=torch.cdouble
 )
 HMAT = 1 / torch.sqrt(torch.tensor(2)) * torch.tensor([[1, 1], [1, -1]], dtype=torch.cdouble)
 
 
 OPERATIONS_DICT = {
     "I": IMAT,
     "X": XMAT,
     "Y": YMAT,
     "Z": ZMAT,
     "S": SMAT,
+    "SDAGGER": SDAGGERMAT,
     "T": TMAT,
     "H": HMAT,
     "SWAP": SWAPMAT,
 }
 
 
 def _apply_gate(
@@ -148,15 +150,15 @@
     - batch_size (int): the size of the batch
 
     Output:
     - state (torch.Tensor): the quantum state after application of the gate.
     Same shape as `input_state`
     """
     mat = mat.reshape([2] * len(qubits) * 2 + [batch_size])
-    qubits = N_qubits - 1 - np.array(qubits)
+    qubits = np.array(N_qubits - 1 - np.array(qubits), dtype=np.int64)
 
     state_indices = ABC_ARRAY[0 : N_qubits + 1].copy()
     mat_indices = ABC_ARRAY[N_qubits + 2 : N_qubits + 2 + 2 * len(qubits) + 1].copy()
     mat_indices[len(qubits) : 2 * len(qubits)] = state_indices[qubits]
     mat_indices[-1] = state_indices[-1]
 
     new_state_indices = state_indices.copy()
```

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/abstract.py` & `pyqtorch-0.3.1/pyqtorch/modules/abstract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from typing import Any
 
 import torch
 from numpy.typing import ArrayLike
 from torch.nn import Module
 
-import pyqtorch.modules
+import pyqtorch.modules as pyq
 
 
 class AbstractGate(ABC, Module):
     def __init__(self, qubits: ArrayLike, n_qubits: int):
         super().__init__()
         self.qubits = qubits
         self.n_qubits = n_qubits
 
-    def __mul__(
-        self, other: AbstractGate | pyqtorch.modules.QuantumCircuit
-    ) -> pyqtorch.modules.QuantumCircuit:
+    def __mul__(self, other: AbstractGate | pyq.QuantumCircuit) -> pyq.QuantumCircuit:
         if isinstance(other, AbstractGate):
-            return pyqtorch.modules.QuantumCircuit(
-                max(self.n_qubits, other.n_qubits), [self, other]
-            )
-
-        if isinstance(other, pyqtorch.modules.QuantumCircuit):
-            return pyqtorch.modules.QuantumCircuit(
-                max(self.n_qubits, other.n_qubits), [self, *other.operations]
-            )
-
+            ml = torch.nn.ModuleList([self, other])
+            return pyq.QuantumCircuit(max(self.n_qubits, other.n_qubits), ml)
+        elif isinstance(other, pyq.QuantumCircuit):
+            ml = torch.nn.ModuleList([self]) + other.operations
+            return pyq.QuantumCircuit(max(self.n_qubits, other.n_qubits), ml)
         else:
-            return NotImplemented
+            return TypeError(f"Cannot compose {type(self)} with {type(other)}")
+
+    def __key(self) -> tuple:
+        return (self.n_qubits, *self.qubits)
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, type(self)):
+            return self.__key() == other.__key()
+        return NotImplemented
+
+    def __hash__(self) -> int:
+        return hash(self.__key())
 
     @abstractmethod
     def matrices(self, tensors: torch.Tensor) -> torch.Tensor:
         # NOTE: thetas are assumed to be of shape (1,batch_size) or (batch_size,) because we
         # want to allow e.g. (3,batch_size) in the U gate.
         ...
 
@@ -43,14 +49,7 @@
 
     @abstractmethod
     def forward(self, state: torch.Tensor, thetas: torch.Tensor) -> torch.Tensor:
         ...
 
     def extra_repr(self) -> str:
         return f"qubits={self.qubits}, n_qubits={self.n_qubits}"
-
-    def is_same_gate(self, other: AbstractGate) -> bool:
-        return (
-            self.qubits == other.qubits
-            and self.n_qubits == other.n_qubits
-            and type(self) == type(other)
-        )
```

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/circuit.py` & `pyqtorch-0.3.1/pyqtorch/modules/circuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,23 +124,34 @@
         """
         super().__init__()
         self.n_qubits = n_qubits
         self.operations = torch.nn.ModuleList(operations)
 
     def __mul__(self, other: AbstractGate | QuantumCircuit) -> QuantumCircuit:
         if isinstance(other, QuantumCircuit):
-            return QuantumCircuit(
-                max(self.n_qubits, other.n_qubits), self.operations.extend(other.operations)
-            )
+            n_qubits = max(self.n_qubits, other.n_qubits)
+            return QuantumCircuit(n_qubits, self.operations.extend(other.operations))
 
         if isinstance(other, AbstractGate):
-            return QuantumCircuit(max(self.n_qubits, other.n_qubits), self.operations.append(other))
+            n_qubits = max(self.n_qubits, other.n_qubits)
+            return QuantumCircuit(n_qubits, self.operations.append(other))
 
         else:
-            return NotImplemented
+            return ValueError(f"Cannot compose {type(self)} with {type(other)}")
+
+    def __key(self) -> tuple:
+        return (self.n_qubits, *self.operations)
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, QuantumCircuit):
+            return self.__key() == other.__key()
+        return NotImplemented
+
+    def __hash__(self) -> int:
+        return hash(self.__key())
 
     def forward(self, state: torch.Tensor, thetas: torch.Tensor = None) -> torch.Tensor:
         """
         Forward pass of the quantum circuit.
 
         Arguments:
             state (torch.Tensor): The input quantum state tensor.
@@ -161,22 +172,14 @@
             return buffer.device
         except StopIteration:
             return torch.device("cpu")
 
     def init_state(self, batch_size: int) -> torch.Tensor:
         return zero_state(self.n_qubits, batch_size, device=self._device)
 
-    def is_same_circuit(self, other: QuantumCircuit) -> bool:
-        return (
-            all(
-                gate1.is_same_gate(gate2) for gate1, gate2 in zip(self.operations, other.operations)
-            )
-            and self.n_qubits == other.n_qubits
-        )
-
 
 def FeaturemapLayer(n_qubits: int, Op: Any) -> QuantumCircuit:
     """
     Creates a feature map layer in a quantum neural network.
     The FeaturemapLayer is a convenience constructor for a QuantumCircuit
     which accepts an operation to put on every qubit.
```

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/hamevo.py` & `pyqtorch-0.3.1/pyqtorch/modules/hamevo.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,29 +32,42 @@
     ):
         super().__init__()
         self.H: torch.Tensor
         self.t: torch.Tensor
         self.qubits = qubits
         self.n_qubits = n_qubits
         self.n_steps = n_steps
-        self.register_buffer("H", H)
-        self.register_buffer("t", t)
+        if H.ndim == 2:
+            H = H.unsqueeze(2)
+        if H.size(-1) == t.size(0) or t.size(0) == 1:
+            self.register_buffer("H", H)
+            self.register_buffer("t", t)
+        elif H.size(-1) == 1:
+            (x, y, _) = H.size()
+            self.register_buffer("H", H.expand(x, y, t.size(0)))
+            self.register_buffer("t", t)
+        else:
+            msg = "H and t batchsizes either have to match or (one of them has to) be equal to one."
+            raise ValueError(msg)
 
     def apply(self, state: torch.Tensor) -> torch.Tensor:
         """
         Applies the Hamiltonian evolution operation on the given state using RK4 method.
 
         Args:
             state (tensor): Input quantum state.
 
         Returns:
             tensor: Output state after Hamiltonian evolution.
         """
 
-        batch_size = state.size(-1)
+        batch_size = max(state.size(-1), self.H.size(-1))
+        if state.size(-1) == 1:
+            state = state.repeat(*[1 for _ in range(len(state.size()) - 1)], batch_size)
+
         h = self.t.reshape((1, -1)) / self.n_steps
         for _ in range(self.n_qubits - 1):
             h = h.unsqueeze(0)
 
         h = h.expand_as(state)
         _state = state.clone()
         for _ in range(self.n_steps):
@@ -123,64 +136,61 @@
     def __init__(
         self, H: torch.Tensor, t: torch.Tensor, qubits: Any, n_qubits: int, n_steps: int = 100
     ):
         super().__init__(H, t, qubits, n_qubits, n_steps)
         if len(self.H.size()) < 3:
             self.H = self.H.unsqueeze(2)
         batch_size_h = self.H.size()[BATCH_DIM]
-        self.l_vec = []
-        self.l_val = []
-        for i in range(batch_size_h):
-            eig_values, eig_vectors = diagonalize(self.H[..., i])
+        batch_size_t = self.t.size(0)
 
-            self.l_vec.append(eig_vectors)
-            self.l_val.append(eig_values)
+        self._eigs = []
+        if batch_size_h == batch_size_t or batch_size_t == 1:
+            for i in range(batch_size_h):
+                eig_values, eig_vectors = diagonalize(self.H[..., i])
+                self._eigs.append((eig_values, eig_vectors))
+        elif batch_size_h == 1:
+            eig_values, eig_vectors = diagonalize(self.H[..., 0])
+            for i in range(batch_size_t):
+                self._eigs.append((eig_values, eig_vectors))
+        else:
+            msg = "H and t batchsizes either have to match or (one of them has to) be equal to one."
+            raise ValueError(msg)
+        self.batch_size = max(batch_size_h, batch_size_t)
 
     def apply(self, state: torch.Tensor) -> torch.Tensor:
         """
         Applies the Hamiltonian evolution operation on the given state
         using Eigenvalue Decomposition method.
 
         Args:
             state (tensor): Input quantum state.
 
         Returns:
             tensor: Output state after Hamiltonian evolution.
         """
 
-        batch_size_t = len(self.t)
-        batch_size_h = self.H.size()[BATCH_DIM]
-        t_evo = torch.zeros(batch_size_h).to(torch.cdouble)
-        evol_operator = torch.zeros(self.H.size()).to(torch.cdouble)
-
-        if batch_size_t >= batch_size_h:
-            t_evo = self.t[:batch_size_h]
-        else:
-            if batch_size_t == 1:
-                t_evo[:] = self.t[0]
-            else:
-                t_evo[:batch_size_t] = self.t
-
-        for i in range(batch_size_h):
-            eig_values, eig_vectors = self.l_val[i], self.l_vec[i]
+        (x, y, _) = self.H.size()
+        evol_operator = torch.zeros(x, y, self.batch_size).to(torch.cdouble)
+        t_evo = self.t.repeat(self.batch_size) if self.t.size(0) == 1 else self.t
 
+        for i, (eig_values, eig_vectors) in enumerate(self._eigs):
             if eig_vectors is None:
                 # Compute e^(-i H t)
                 evol_operator[..., i] = torch.diag(torch.exp(-1j * eig_values * t_evo[i]))
 
             else:
                 # Compute e^(-i D t)
                 eig_exp = torch.diag(torch.exp(-1j * eig_values * t_evo[i]))
                 # e^(-i H t) = V.e^(-i D t).V^\dagger
                 evol_operator[..., i] = torch.matmul(
                     torch.matmul(eig_vectors, eig_exp),
                     torch.conj(eig_vectors.transpose(0, 1)),
                 )
 
-        return _apply_batch_gate(state, evol_operator, self.qubits, self.n_qubits, batch_size_h)
+        return _apply_batch_gate(state, evol_operator, self.qubits, self.n_qubits, self.batch_size)
 
 
 class HamEvoExp(HamEvo):
     """
     Class for Hamiltonian evolution operation, using matrix exponential method.
 
     Args:
@@ -213,37 +223,30 @@
 
         Returns:
             tensor: Output state after Hamiltonian evolution.
         """
 
         batch_size_t = len(self.t)
         batch_size_h = self.H.size()[BATCH_DIM]
-        t_evo = torch.zeros(batch_size_h).to(torch.cdouble)
-
-        if batch_size_t >= batch_size_h:
-            t_evo = self.t[:batch_size_h]
-        else:
-            if batch_size_t == 1:
-                t_evo[:] = self.t[0]
-            else:
-                t_evo[:batch_size_t] = self.t
+        t_evo = self.t
 
         if self.batch_is_diag:
             # Skips the matrix exponential for diagonal hamiltonians
             H_diagonals = torch.diagonal(self.H)
             evol_exp_arg = H_diagonals * (-1j * t_evo).view((-1, 1))
             evol_operator_T = torch.diag_embed(torch.exp(evol_exp_arg))
             evol_operator = torch.transpose(evol_operator_T, 0, -1)
         else:
             H_T = torch.transpose(self.H, 0, -1)
             evol_exp_arg = H_T * (-1j * t_evo).view((-1, 1, 1))
             evol_operator_T = torch.linalg.matrix_exp(evol_exp_arg)
             evol_operator = torch.transpose(evol_operator_T, 0, -1)
 
-        return _apply_batch_gate(state, evol_operator, self.qubits, self.n_qubits, batch_size_h)
+        batch_size = max(batch_size_h, batch_size_t)
+        return _apply_batch_gate(state, evol_operator, self.qubits, self.n_qubits, batch_size)
 
 
 class HamEvoType(Enum):
     """
     An Enumeration to represent types of Hamiltonian Evolution
 
     RK4: Hamiltonian evolution performed using the 4th order Runge-Kutta method.
@@ -334,10 +337,9 @@
             H (tensor): The Hamiltonian to be used in the evolution.
             t (tensor): The evolution time.
             state (tensor): The state on which to perform Hamiltonian evolution.
 
         Returns:
             The state (tensor) after Hamiltonian evolution.
         """
-
         ham_evo_instance = self.get_hamevo_instance(H, t)
         return ham_evo_instance.forward(state)
```

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/parametric.py` & `pyqtorch-0.3.1/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/primitive.py` & `pyqtorch-0.3.1/pyqtorch/modules/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,42 @@
         result = s_gate(z_state)
         print(result)
         ```
         """
         super().__init__("S", qubits, n_qubits)
 
 
+class Sdagger(PrimitiveGate):
+    def __init__(self, qubits: ArrayLike, n_qubits: int):
+        """
+        Represents an Sdagger gate (-PI/2 phase gate) in a quantum circuit.
+
+        Arguments:
+            qubits (ArrayLike): The qubits to which the S gate is applied.
+            n_qubits (int): The total number of qubits in the circuit.
+
+        Examples:
+        ```python exec="on" source="above" result="json"
+        import torch
+        import pyqtorch.modules as pyq
+
+        # Create an Sdagger gate
+        sdagger_gate = pyq.Sdagger(qubits=[0], n_qubits=1)
+
+        # Create a zero state
+        z_state = pyq.zero_state(n_qubits=1)
+
+        # Apply the Sdagger gate to the zero state
+        result = sdagger_gate(z_state)
+        print(result)
+        ```
+        """
+        super().__init__("SDAGGER", qubits, n_qubits)
+
+
 class SWAP(PrimitiveGate):
     def __init__(self, qubits: ArrayLike, n_qubits: int):
         """
         Represents a SWAP gate in a quantum circuit.
         The SwapGate swaps the qubit states of two quantum wires.
```

### Comparing `pyqtorch-0.3.0/pyqtorch/modules/utils.py` & `pyqtorch-0.3.1/pyqtorch/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/conftest.py` & `pyqtorch-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/test_batched_operations.py` & `pyqtorch-0.3.1/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/test_converters.py` & `pyqtorch-0.3.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/test_module_hamevo.py` & `pyqtorch-0.3.1/tests/test_operations_hamevo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,186 @@
 from __future__ import annotations
 
 import random
 from math import isclose
-from typing import Callable
 
+import networkx as nx
 import numpy as np
-import pytest
 import torch
 
-import pyqtorch.modules as pyq
+from pyqtorch.core import batched_operation, circuit, operation
+from pyqtorch.core.batched_operation import (
+    batched_hamiltonian_evolution,
+    batched_hamiltonian_evolution_eig,
+)
+from pyqtorch.core.circuit import QuantumCircuit
+from pyqtorch.core.operation import hamiltonian_evolution, hamiltonian_evolution_eig
+from pyqtorch.matrices import generate_ising_from_graph
 
 random.seed(0)
 np.random.seed(0)
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
+state_00 = torch.tensor([[1, 0], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
+state_10 = torch.tensor([[0, 1], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
+state_01 = torch.tensor([[0, 0], [1, 0]], dtype=torch.cdouble).unsqueeze(2)
+state_11 = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
 
 pi = torch.tensor(torch.pi, dtype=torch.cdouble)
 
+CNOT_mat: torch.Tensor = torch.tensor(
+    [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]], dtype=torch.cdouble
+)
 
-def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float | list[float]:
-    N = len(state1.shape) - 1
-    state1_T = torch.transpose(state1, N, 0)
-    overlap = torch.tensordot(state1_T, state2, dims=N)
-    res: list[float] = list(map(float, torch.abs(overlap**2).flatten()))
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
 
+def test_hamevo_single() -> None:
+    N = 4
+    qc = circuit.QuantumCircuit(N)
+    psi = qc.uniform_state(1)
+
+    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float:
+        N = len(state1.shape) - 1
+        state1_T = torch.transpose(state1, N, 0)
+        overlap = torch.tensordot(state1_T, state2, dims=N)
+        return float(torch.abs(overlap**2).flatten())
 
-def Hamiltonian(batch_size: int = 1) -> torch.Tensor:
     sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
     Hbase = torch.kron(sigmaz, sigmaz)
     H = torch.kron(Hbase, Hbase)
-    if batch_size == 1:
-        return H
-    else:
-        return torch.stack((H, H.conj()), dim=2)
-
-
-def Hamiltonian_general(n_qubits: int = 2, batch_size: int = 1) -> torch.Tensor:
-    H_batch = torch.zeros((2**n_qubits, 2**n_qubits, batch_size), dtype=torch.cdouble)
-    for i in range(batch_size):
-        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
-        H = (H_0 + torch.conj(H_0.transpose(0, 1))).cdouble()
-        H_batch[..., i] = H
-    return H_batch
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    psi_star = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
+    result: float = overlap(psi_star, psi)
 
+    assert isclose(result, 0.5)
 
-def Hamiltonian_diag(n_qubits: int = 2, batch_size: int = 1) -> torch.Tensor:
-    H_batch = torch.zeros((2**n_qubits, 2**n_qubits, batch_size), dtype=torch.cdouble)
-    for i in range(batch_size):
-        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
-        H = (H_0 + torch.conj(H_0.transpose(0, 1))).cdouble()
-        get_diag = torch.diag(H)
-        H_diag = torch.diag(get_diag)
-        H_batch[..., i] = H_diag
-    return H_batch
 
+def test_hamevo_eig_single() -> None:
+    N = 4
+    qc = circuit.QuantumCircuit(N)
+    psi = qc.uniform_state(1)
+
+    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float:
+        N = len(state1.shape) - 1
+        state1_T = torch.transpose(state1, N, 0)
+        overlap = torch.tensordot(state1_T, state2, dims=N)
+        return float(torch.abs(overlap**2).flatten())
 
-@pytest.mark.parametrize(
-    "ham_evo",
-    [pyq.HamiltonianEvolution],
-)
-def test_ham_modules_single(ham_evo: torch.nn.Module) -> None:
-    n_qubits = 4
-    H = Hamiltonian(1)
+    sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
+    Hbase = torch.kron(sigmaz, sigmaz)
+    H = torch.kron(Hbase, Hbase)
     t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
-    hamevo = ham_evo(range(n_qubits), n_qubits)
-    psi = pyq.uniform_state(n_qubits)
-    psi_star = hamevo(H, t_evo, psi)
-    result = overlap(psi_star, psi)
-    result = result if isinstance(result, float) else result[0]
+    psi_star = operation.hamiltonian_evolution_eig(H, psi, t_evo, range(N), N)
+    result: float = overlap(psi_star, psi)
+
     assert isclose(result, 0.5)
 
 
-@pytest.mark.parametrize(
-    "ham_evo",
-    [pyq.HamiltonianEvolution],
-)
-def test_hamiltonianevolution_batch(ham_evo: torch.nn.Module) -> None:
-    n_qubits = 4
-    batch_size = 2
-    H = Hamiltonian(batch_size)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+def test_hamevo_batch() -> None:
+    N = 4
+    qc = circuit.QuantumCircuit(N)
+    psi = qc.uniform_state(batch_size=2)
+
+    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> list[float]:
+        N = len(state1.shape) - 1
+        state1_T = torch.transpose(state1, N, 0)
+        overlap = torch.tensordot(state1_T, state2, dims=N)
+        return list(map(float, torch.abs(overlap**2).flatten()))
 
-    hamevo = ham_evo(range(n_qubits), n_qubits)
-    psi = pyq.uniform_state(n_qubits, batch_size)
-    psi_star = hamevo(H, t_evo, psi)
-    result = overlap(psi_star, psi)
+    sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
+    Hbase = torch.kron(sigmaz, sigmaz)
+    H = torch.kron(Hbase, Hbase)
+    H_conj = H.conj()
+
+    t_evo = torch.tensor([0], dtype=torch.cdouble)
+    psi = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
+
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    psi_star = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
+    H_batch = torch.stack((H, H_conj), dim=2)
+    batched_operation.batched_hamiltonian_evolution(H_batch, psi, t_evo, range(N), N)
+    result: list[float] = overlap(psi_star, psi)
 
     assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
 
 
-@pytest.mark.parametrize(
-    "ham_evo",
-    [pyq.HamEvo, pyq.HamEvoEig, pyq.HamEvoExp],
-)
-def test_hamevo_modules_single(ham_evo: torch.nn.Module) -> None:
-    n_qubits = 4
-    H = Hamiltonian(1)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
-    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
-    psi = pyq.uniform_state(n_qubits)
-    psi_star = hamevo.forward(psi)
-    result = overlap(psi_star, psi)
-    result = result if isinstance(result, float) else result[0]
-    assert isclose(result, 0.5)
+def test_hamevo_rk4_vs_eig_diag_H() -> None:
+    n_qubits: int = 7
+    batch_size: int = 10
+    graph: nx.Graph = nx.fast_gnp_random_graph(n_qubits, 0.7)
+    qc = QuantumCircuit(n_qubits)
+    psi = qc.uniform_state(batch_size)
 
+    H_diag = generate_ising_from_graph(graph)
+    H = torch.diag(H_diag)
 
-@pytest.mark.parametrize(
-    "ham_evo",
-    [pyq.HamEvo, pyq.HamEvoEig, pyq.HamEvoExp],
-)
-def test_hamevo_modules_batch(ham_evo: torch.nn.Module) -> None:
-    n_qubits = 4
-    batch_size = 2
-    H = Hamiltonian(batch_size)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    n_trials = 10
+    wf_save_rk = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
+    wf_save_eig = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
 
-    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
-    psi = pyq.uniform_state(n_qubits, batch_size)
-    psi_star = hamevo.forward(psi)
-    result = overlap(psi_star, psi)
-    print(result)
+    for i in range(n_trials):
+        t_evo = torch.rand(batch_size) * 0.5
 
-    assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
+        psi_star = hamiltonian_evolution(H, psi, t_evo, range(n_qubits), n_qubits)
+        wf_save_rk[i] = psi_star
 
+        psi_star = hamiltonian_evolution_eig(H, psi, t_evo, range(n_qubits), n_qubits)
+        wf_save_eig[i] = psi_star
 
-@pytest.mark.parametrize("get_hamiltonians", [Hamiltonian_general, Hamiltonian_diag])
-def test_hamevo_consistency(get_hamiltonians: Callable) -> None:
-    n_qubits = 4
-    batch_size = 5
-
-    H_batch = get_hamiltonians(n_qubits, batch_size)
-
-    t_evo = torch.tensor([torch.pi / 8], dtype=torch.cdouble)
-    psi_0 = pyq.uniform_state(batch_size=batch_size, n_qubits=n_qubits)
-
-    hamevo_rk4 = pyq.HamEvo(H_batch, t_evo, range(n_qubits), n_qubits)
-    psi_rk4 = hamevo_rk4.forward(psi_0)
-    hamevo_eig = pyq.HamEvoEig(H_batch, t_evo, range(n_qubits), n_qubits)
-    psi_eig = hamevo_eig.forward(psi_0)
-    hamevo_exp = pyq.HamEvoExp(H_batch, t_evo, range(n_qubits), n_qubits)
-    psi_exp = hamevo_exp.forward(psi_0)
-
-    hamiltonian_evolution = pyq.HamiltonianEvolution(range(n_qubits), n_qubits)
-    psi_ham = hamiltonian_evolution(H_batch, t_evo, psi_0)
-
-    # assert torch.allclose(psi_rk4, psi_eig)
-    # assert torch.allclose(psi_rk4, psi_eig)
-    # assert torch.allclose(psi_eig, psi_exp)
-    tensors = [psi_rk4, psi_eig, psi_exp, psi_ham]
-    assert all(torch.allclose(tensors[i], tensors[0]) for i in range(1, len(tensors)))
-
-
-@pytest.mark.parametrize(
-    "ham_evo_type, ham_evo_class",
-    [
-        (pyq.HamEvoType.RK4, pyq.HamEvo),
-        (pyq.HamEvoType.EIG, pyq.HamEvoEig),
-        (pyq.HamEvoType.EXP, pyq.HamEvoExp),
-        ("rk4", pyq.HamEvo),
-        ("eig", pyq.HamEvoEig),
-        ("exp", pyq.HamEvoExp),
-    ],
-)
-def test_hamiltonianevolution_with_types(
-    ham_evo_type: pyq.HamEvoType, ham_evo_class: torch.nn.Module
-) -> None:
-    n_qubits = 4
-    H = Hamiltonian(1)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    diff = torch.tensor(
+        [torch.max(abs(wf_save_rk[i, ...] - wf_save_eig[i, ...])) for i in range(n_trials)]
+    )
 
-    hamevo = pyq.HamiltonianEvolution(range(n_qubits), n_qubits, hamevo_type=ham_evo_type)
-    ham_evo_instance = hamevo.get_hamevo_instance(H, t_evo)
-    assert isinstance(ham_evo_instance, ham_evo_class)
-
-    psi = pyq.uniform_state(n_qubits)
-    psi_star = hamevo(H, t_evo, psi)
-    result = overlap(psi_star, psi)
-    result = result if isinstance(result, float) else result[0]
-    assert isclose(result, 0.5)
+    assert torch.max(diff) <= 10 ** (-6)
+
+
+def test_hamevo_rk4_vs_eig_general_H() -> None:
+    n_qubits: int = 6
+    batch_size: int = 10
+
+    qc = QuantumCircuit(n_qubits)
+    psi = qc.uniform_state(batch_size)
+
+    H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
+    H = (H_0 + torch.conj(H_0.transpose(0, 1))).to(torch.cdouble)
+
+    n_trials = 10
+    wf_save_rk = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
+    wf_save_eig = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
+
+    for i in range(n_trials):
+        t_evo = torch.rand(batch_size) * 0.5
+        psi_star = hamiltonian_evolution(H, psi, t_evo, range(n_qubits), n_qubits)
+        wf_save_rk[i] = psi_star
+        psi_star = hamiltonian_evolution_eig(H, psi, t_evo, range(n_qubits), n_qubits)
+        wf_save_eig[i] = psi_star
+
+    diff = torch.tensor(
+        [torch.max(abs(wf_save_rk[i, ...] - wf_save_eig[i, ...])) for i in range(n_trials)]
+    )
+
+    assert torch.max(diff) <= 10 ** (-5)
+
+
+def test_hamevo_rk4_vs_eig_general_H_batched() -> None:
+    n_qubits: int = 5
+    batch_size: int = 20
+
+    qc = QuantumCircuit(n_qubits)
+    psi = qc.uniform_state(batch_size)
+
+    H_batch = torch.zeros(2**n_qubits, 2**n_qubits, batch_size).to(torch.cdouble)
+    for i in range(batch_size):
+        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
+        H_batch[..., i] = (H_0 + torch.conj(H_0.transpose(0, 1))).to(torch.cdouble)
+
+    t_evo = (torch.rand(batch_size) * 0.5).to(torch.cdouble)
+
+    psi_star_norm = batched_hamiltonian_evolution(H_batch, psi, t_evo, range(n_qubits), n_qubits)
+
+    psi_star_eig = batched_hamiltonian_evolution_eig(H_batch, psi, t_evo, range(n_qubits), n_qubits)
+
+    diff = torch.tensor(
+        [torch.max(abs(psi_star_norm[..., b] - psi_star_eig[..., b])) for b in range(batch_size)]
+    )
+
+    assert torch.max(diff) <= 10 ** (-6)
```

### Comparing `pyqtorch-0.3.0/tests/test_modules.py` & `pyqtorch-0.3.1/tests/test_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import pytest
 import torch
 
 import pyqtorch.core as func_pyq
 import pyqtorch.modules as pyq
+from pyqtorch.modules.abstract import AbstractGate
 
 
-@pytest.mark.parametrize("gate", ["X", "Y", "Z"])
+@pytest.mark.parametrize("gate", ["X", "Y", "Z", "H", "I", "S", "T", "Sdagger"])
 def test_constant_gates(gate: str) -> None:
     dtype = torch.cdouble
     device = "cpu"
     batch_size = 100
     qubits = [0]
     n_qubits = 2
 
@@ -75,15 +76,15 @@
 
     # g = torch.autograd.grad(circ, thetas)
     dres_theta = torch.autograd.grad(res, phi, torch.ones_like(res), create_graph=True)[0]
     assert not torch.all(torch.isnan(dres_theta))
 
 
 @pytest.mark.parametrize("batch_size", [1, 2, 4, 6])
-def test_empy_circuit(batch_size: int) -> None:
+def test_empty_circuit(batch_size: int) -> None:
     n_qubits = 2
     device = "cuda" if torch.cuda.is_available() else "cpu"
     dtype = torch.cdouble
 
     ops: list = []
     circ = pyq.QuantumCircuit(n_qubits, ops).to(device=device, dtype=dtype)
 
@@ -103,58 +104,88 @@
     n_qubits = 1
     u = pyq.U([0], n_qubits)
     x = torch.rand(3, batch_size)
     state = pyq.zero_state(n_qubits, batch_size=batch_size, device="cpu", dtype=torch.cdouble)
     assert not torch.all(torch.isnan(u(state, x)))
 
 
+@pytest.mark.parametrize(
+    "a,b,val",
+    [
+        (pyq.X([0], 1), pyq.X([0], 1), True),
+        (pyq.RY([0], 1), pyq.RY([0], 1), True),
+        (pyq.RY([0], 1), pyq.RY([0], 1), True),
+        (pyq.X([0], 1), pyq.Y([0], 1), False),
+        (pyq.RX([0], 2), pyq.RX([0], 1), False),
+        (pyq.RX([1], 1), pyq.RX([0], 1), False),
+    ],
+)
+def test_gate_equality(a: AbstractGate, b: AbstractGate, val: bool) -> None:
+    x = a == b
+    assert x == val
+
+
+def test_circuit_equality() -> None:
+    c1 = pyq.QuantumCircuit(2, [pyq.RX([0], 2), pyq.Z([1], 2)])
+    c2 = pyq.QuantumCircuit(2, [pyq.RX([0], 2), pyq.Z([1], 2)])
+    assert c1 == c2
+
+    c3 = pyq.QuantumCircuit(2, [pyq.RX([1], 2), pyq.Z([1], 2)])
+    assert c1 != c3
+
+    c4 = pyq.QuantumCircuit(2, [pyq.Z([1], 2)])
+    assert c3 != c4
+
+    c5 = pyq.QuantumCircuit(2, [pyq.RX([0], 2)])
+    assert c1 != c5
+
+
 @pytest.mark.parametrize("n_qubits", [1, 2, 3])
 def test_gate_composition(n_qubits: int) -> None:
-    X = pyq.X(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
-    Y = pyq.Y(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
-    XYcirc = X * Y
-    XYcirc_ref = pyq.QuantumCircuit(n_qubits, [X, Y])
-    assert XYcirc.is_same_circuit(XYcirc_ref)
-
-    RX = pyq.RX(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
-    RY = pyq.RY(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
-    RXRYcirc = RX * RY
-    RXRYcirc_ref = pyq.QuantumCircuit(n_qubits, [RX, RY])
-    assert RXRYcirc.is_same_circuit(RXRYcirc_ref)
+    x = pyq.X(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
+    y = pyq.Y(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
+    circ = x * y
+    truth = pyq.QuantumCircuit(n_qubits, [x, y])
+    assert circ == truth
+
+    rx = pyq.RX(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
+    ry = pyq.RY(torch.randint(0, n_qubits, (1,)).tolist(), n_qubits)
+    circ = rx * ry
+    truth = pyq.QuantumCircuit(n_qubits, [rx, ry])
+    assert circ == truth
 
     r1, r2, r3 = 1, n_qubits, max(n_qubits - 1, 1)
-    Z1 = pyq.Z(torch.randint(0, r1, (1,)).tolist(), r1)
-    Y = pyq.Y(torch.randint(0, r2, (1,)).tolist(), r2)
-    Z2 = pyq.Z(torch.randint(0, r3, (1,)).tolist(), r3)
-
-    ZYZcirc = Z1 * Y * Z2
-    ZYZcirc_ref = pyq.QuantumCircuit(max(r1, r2, r3), [Z1, Y, Z2])
-    assert ZYZcirc.is_same_circuit(ZYZcirc_ref)
+    z1 = pyq.Z(torch.randint(0, r1, (1,)).tolist(), r1)
+    y = pyq.Y(torch.randint(0, r2, (1,)).tolist(), r2)
+    z2 = pyq.Z(torch.randint(0, r3, (1,)).tolist(), r3)
+    circ = z1 * y * z2
+    truth = pyq.QuantumCircuit(max(r1, r2, r3), [z1, y, z2])
+    assert circ == truth
 
     rr1, rr2, rr3 = 1, n_qubits, max(n_qubits - 1, 1)
-    RZ1 = pyq.RZ(torch.randint(0, rr1, (1,)).tolist(), rr1)
-    RY1 = pyq.RY(torch.randint(0, rr2, (1,)).tolist(), rr2)
-    RZ2 = pyq.RZ(torch.randint(0, rr3, (1,)).tolist(), rr3)
-
-    Ucirc = RZ1 * RY1 * RZ2
-    Ucirc_ref = pyq.QuantumCircuit(max(r1, r2, r3), [RZ1, RY1, RZ2])
-    assert Ucirc.is_same_circuit(Ucirc_ref)
+    rz1 = pyq.RZ(torch.randint(0, rr1, (1,)).tolist(), rr1)
+    ry1 = pyq.RY(torch.randint(0, rr2, (1,)).tolist(), rr2)
+    rz2 = pyq.RZ(torch.randint(0, rr3, (1,)).tolist(), rr3)
+
+    circ = rz1 * ry1 * rz2
+    truth = pyq.QuantumCircuit(max(r1, r2, r3), [rz1, ry1, rz2])
+    assert circ == truth
 
 
 @pytest.mark.parametrize("n_qubits", [1, 2, 3])
-def test_QuantumCircuit_composition(n_qubits: int) -> None:
+def test_circuit_composition(n_qubits: int) -> None:
     r = torch.randint(1, n_qubits + 1, (1,)).tolist()
-    RX = pyq.RX(r, n_qubits)
+    rx = pyq.RX(r, n_qubits)
 
-    RXcirc = RX * pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)])
-    RXcirc_ref = pyq.QuantumCircuit(n_qubits, [RX, pyq.X([0], 1), pyq.Y([0], 1)])
-    assert RXcirc.is_same_circuit(RXcirc_ref)
-
-    circRX = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * RX
-    circRX_ref = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), RX])
-    assert circRX.is_same_circuit(circRX_ref)
+    circ = rx * pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)])
+    truth = pyq.QuantumCircuit(n_qubits, [rx, pyq.X([0], 1), pyq.Y([0], 1)])
+    assert circ == truth
+
+    circ = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * rx
+    truth = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), rx])
+    assert circ == truth
 
-    circ_mult = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * pyq.QuantumCircuit(
-        n_qubits, [RX, pyq.RY([0], 1)]
+    circ = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * pyq.QuantumCircuit(
+        n_qubits, [rx, pyq.RY([0], 1)]
     )
-    circ_mult_ref = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), RX, pyq.RY([0], 1)])
-    assert circ_mult.is_same_circuit(circ_mult_ref)
+    truth = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), rx, pyq.RY([0], 1)])
+    assert circ == truth
```

### Comparing `pyqtorch-0.3.0/tests/test_notebooks.py` & `pyqtorch-0.3.1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/test_operations.py` & `pyqtorch-0.3.1/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/tests/test_operations_hamevo.py` & `pyqtorch-0.3.1/tests/test_module_hamevo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,186 +1,224 @@
 from __future__ import annotations
 
 import random
 from math import isclose
+from typing import Callable
 
-import networkx as nx
 import numpy as np
+import pytest
 import torch
 
-from pyqtorch.core import batched_operation, circuit, operation
-from pyqtorch.core.batched_operation import (
-    batched_hamiltonian_evolution,
-    batched_hamiltonian_evolution_eig,
-)
-from pyqtorch.core.circuit import QuantumCircuit
-from pyqtorch.core.operation import hamiltonian_evolution, hamiltonian_evolution_eig
-from pyqtorch.matrices import generate_ising_from_graph
+import pyqtorch.modules as pyq
 
 random.seed(0)
 np.random.seed(0)
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
-state_00 = torch.tensor([[1, 0], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
-state_10 = torch.tensor([[0, 1], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
-state_01 = torch.tensor([[0, 0], [1, 0]], dtype=torch.cdouble).unsqueeze(2)
-state_11 = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
 
 pi = torch.tensor(torch.pi, dtype=torch.cdouble)
 
-CNOT_mat: torch.Tensor = torch.tensor(
-    [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]], dtype=torch.cdouble
-)
-
 
-def test_hamevo_single() -> None:
-    N = 4
-    qc = circuit.QuantumCircuit(N)
-    psi = qc.uniform_state(1)
+def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float | list[float]:
+    N = len(state1.shape) - 1
+    state1_T = torch.transpose(state1, N, 0)
+    overlap = torch.tensordot(state1_T, state2, dims=N)
+    res: list[float] = list(map(float, torch.abs(overlap**2).flatten()))
+    if len(res) == 1:
+        return res[0]
+    else:
+        return res
 
-    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float:
-        N = len(state1.shape) - 1
-        state1_T = torch.transpose(state1, N, 0)
-        overlap = torch.tensordot(state1_T, state2, dims=N)
-        return float(torch.abs(overlap**2).flatten())
 
+def Hamiltonian(batch_size: int = 1) -> torch.Tensor:
     sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
     Hbase = torch.kron(sigmaz, sigmaz)
     H = torch.kron(Hbase, Hbase)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
-    psi_star = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
-    result: float = overlap(psi_star, psi)
+    if batch_size == 1:
+        return H
+    elif batch_size == 2:
+        return torch.stack((H, H.conj()), dim=2)
+    else:
+        raise NotImplementedError
 
-    assert isclose(result, 0.5)
 
+def Hamiltonian_general(n_qubits: int = 2, batch_size: int = 1) -> torch.Tensor:
+    H_batch = torch.zeros((2**n_qubits, 2**n_qubits, batch_size), dtype=torch.cdouble)
+    for i in range(batch_size):
+        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
+        H = (H_0 + torch.conj(H_0.transpose(0, 1))).cdouble()
+        H_batch[..., i] = H
+    return H_batch
 
-def test_hamevo_eig_single() -> None:
-    N = 4
-    qc = circuit.QuantumCircuit(N)
-    psi = qc.uniform_state(1)
 
-    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float:
-        N = len(state1.shape) - 1
-        state1_T = torch.transpose(state1, N, 0)
-        overlap = torch.tensordot(state1_T, state2, dims=N)
-        return float(torch.abs(overlap**2).flatten())
+def Hamiltonian_diag(n_qubits: int = 2, batch_size: int = 1) -> torch.Tensor:
+    H_batch = torch.zeros((2**n_qubits, 2**n_qubits, batch_size), dtype=torch.cdouble)
+    for i in range(batch_size):
+        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
+        H = (H_0 + torch.conj(H_0.transpose(0, 1))).cdouble()
+        get_diag = torch.diag(H)
+        H_diag = torch.diag(get_diag)
+        H_batch[..., i] = H_diag
+    return H_batch
 
-    sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
-    Hbase = torch.kron(sigmaz, sigmaz)
-    H = torch.kron(Hbase, Hbase)
-    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
-    psi_star = operation.hamiltonian_evolution_eig(H, psi, t_evo, range(N), N)
-    result: float = overlap(psi_star, psi)
 
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamiltonianEvolution],
+)
+def test_ham_modules_single(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    H = Hamiltonian(1)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    hamevo = ham_evo(range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits)
+    psi_star = hamevo(H, t_evo, psi)
+    result = overlap(psi_star, psi)
+    result = result if isinstance(result, float) else result[0]
     assert isclose(result, 0.5)
 
 
-def test_hamevo_batch() -> None:
-    N = 4
-    qc = circuit.QuantumCircuit(N)
-    psi = qc.uniform_state(batch_size=2)
-
-    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> list[float]:
-        N = len(state1.shape) - 1
-        state1_T = torch.transpose(state1, N, 0)
-        overlap = torch.tensordot(state1_T, state2, dims=N)
-        return list(map(float, torch.abs(overlap**2).flatten()))
-
-    sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
-    Hbase = torch.kron(sigmaz, sigmaz)
-    H = torch.kron(Hbase, Hbase)
-    H_conj = H.conj()
-
-    t_evo = torch.tensor([0], dtype=torch.cdouble)
-    psi = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
-
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamiltonianEvolution],
+)
+def test_hamiltonianevolution_batch(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    batch_size = 2
+    H = Hamiltonian(batch_size)
     t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
-    psi_star = operation.hamiltonian_evolution(H, psi, t_evo, range(N), N)
-    H_batch = torch.stack((H, H_conj), dim=2)
-    batched_operation.batched_hamiltonian_evolution(H_batch, psi, t_evo, range(N), N)
-    result: list[float] = overlap(psi_star, psi)
 
-    assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
-
-
-def test_hamevo_rk4_vs_eig_diag_H() -> None:
-    n_qubits: int = 7
-    batch_size: int = 10
-    graph: nx.Graph = nx.fast_gnp_random_graph(n_qubits, 0.7)
-    qc = QuantumCircuit(n_qubits)
-    psi = qc.uniform_state(batch_size)
-
-    H_diag = generate_ising_from_graph(graph)
-    H = torch.diag(H_diag)
-
-    n_trials = 10
-    wf_save_rk = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
-    wf_save_eig = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
-
-    for i in range(n_trials):
-        t_evo = torch.rand(batch_size) * 0.5
-
-        psi_star = hamiltonian_evolution(H, psi, t_evo, range(n_qubits), n_qubits)
-        wf_save_rk[i] = psi_star
-
-        psi_star = hamiltonian_evolution_eig(H, psi, t_evo, range(n_qubits), n_qubits)
-        wf_save_eig[i] = psi_star
-
-    diff = torch.tensor(
-        [torch.max(abs(wf_save_rk[i, ...] - wf_save_eig[i, ...])) for i in range(n_trials)]
-    )
-
-    assert torch.max(diff) <= 10 ** (-6)
-
-
-def test_hamevo_rk4_vs_eig_general_H() -> None:
-    n_qubits: int = 6
-    batch_size: int = 10
-
-    qc = QuantumCircuit(n_qubits)
-    psi = qc.uniform_state(batch_size)
-
-    H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
-    H = (H_0 + torch.conj(H_0.transpose(0, 1))).to(torch.cdouble)
-
-    n_trials = 10
-    wf_save_rk = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
-    wf_save_eig = torch.zeros((n_trials,) + tuple(psi.shape)).to(torch.cdouble)
-
-    for i in range(n_trials):
-        t_evo = torch.rand(batch_size) * 0.5
-        psi_star = hamiltonian_evolution(H, psi, t_evo, range(n_qubits), n_qubits)
-        wf_save_rk[i] = psi_star
-        psi_star = hamiltonian_evolution_eig(H, psi, t_evo, range(n_qubits), n_qubits)
-        wf_save_eig[i] = psi_star
+    hamevo = ham_evo(range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits, batch_size)
+    psi_star = hamevo(H, t_evo, psi)
+    result = overlap(psi_star, psi)
 
-    diff = torch.tensor(
-        [torch.max(abs(wf_save_rk[i, ...] - wf_save_eig[i, ...])) for i in range(n_trials)]
-    )
-
-    assert torch.max(diff) <= 10 ** (-5)
+    assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
 
 
-def test_hamevo_rk4_vs_eig_general_H_batched() -> None:
-    n_qubits: int = 5
-    batch_size: int = 20
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamEvo, pyq.HamEvoEig, pyq.HamEvoExp],
+)
+def test_hamevo_modules_single(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    H = Hamiltonian(1)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits)
+    psi_star = hamevo.forward(psi)
+    result = overlap(psi_star, psi)
+    result = result if isinstance(result, float) else result[0]
+    assert isclose(result, 0.5)
 
-    qc = QuantumCircuit(n_qubits)
-    psi = qc.uniform_state(batch_size)
 
-    H_batch = torch.zeros(2**n_qubits, 2**n_qubits, batch_size).to(torch.cdouble)
-    for i in range(batch_size):
-        H_0 = torch.randn((2**n_qubits, 2**n_qubits), dtype=torch.cdouble)
-        H_batch[..., i] = (H_0 + torch.conj(H_0.transpose(0, 1))).to(torch.cdouble)
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamEvo, pyq.HamEvoEig, pyq.HamEvoExp],
+)
+def test_hamevo_modules_batch(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    batch_size = 2
+    H = Hamiltonian(batch_size)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
 
-    t_evo = (torch.rand(batch_size) * 0.5).to(torch.cdouble)
+    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits, batch_size)
+    psi_star = hamevo.forward(psi)
+    result = overlap(psi_star, psi)
+    print(result)
 
-    psi_star_norm = batched_hamiltonian_evolution(H_batch, psi, t_evo, range(n_qubits), n_qubits)
+    assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
 
-    psi_star_eig = batched_hamiltonian_evolution_eig(H_batch, psi, t_evo, range(n_qubits), n_qubits)
 
-    diff = torch.tensor(
-        [torch.max(abs(psi_star_norm[..., b] - psi_star_eig[..., b])) for b in range(batch_size)]
-    )
+@pytest.mark.parametrize("get_hamiltonians", [Hamiltonian_general, Hamiltonian_diag])
+def test_hamevo_consistency(get_hamiltonians: Callable) -> None:
+    n_qubits = 4
+    batch_size = 5
+
+    H_batch = get_hamiltonians(n_qubits, batch_size)
+
+    t_evo = torch.tensor([torch.pi / 8], dtype=torch.cdouble)
+    psi_0 = pyq.uniform_state(batch_size=batch_size, n_qubits=n_qubits)
+
+    hamevo_rk4 = pyq.HamEvo(H_batch, t_evo, range(n_qubits), n_qubits)
+    psi_rk4 = hamevo_rk4.forward(psi_0)
+    hamevo_eig = pyq.HamEvoEig(H_batch, t_evo, range(n_qubits), n_qubits)
+    psi_eig = hamevo_eig.forward(psi_0)
+    hamevo_exp = pyq.HamEvoExp(H_batch, t_evo, range(n_qubits), n_qubits)
+    psi_exp = hamevo_exp.forward(psi_0)
+
+    hamiltonian_evolution = pyq.HamiltonianEvolution(range(n_qubits), n_qubits)
+    psi_ham = hamiltonian_evolution(H_batch, t_evo, psi_0)
+
+    # assert torch.allclose(psi_rk4, psi_eig)
+    # assert torch.allclose(psi_rk4, psi_eig)
+    # assert torch.allclose(psi_eig, psi_exp)
+    tensors = [psi_rk4, psi_eig, psi_exp, psi_ham]
+    assert all(torch.allclose(tensors[i], tensors[0]) for i in range(1, len(tensors)))
+
+
+@pytest.mark.parametrize(
+    "ham_evo_type, ham_evo_class",
+    [
+        (pyq.HamEvoType.RK4, pyq.HamEvo),
+        (pyq.HamEvoType.EIG, pyq.HamEvoEig),
+        (pyq.HamEvoType.EXP, pyq.HamEvoExp),
+        ("rk4", pyq.HamEvo),
+        ("eig", pyq.HamEvoEig),
+        ("exp", pyq.HamEvoExp),
+    ],
+)
+@pytest.mark.parametrize(
+    "H, t_evo, target, batch_size",
+    [
+        (  # batchsize 1 | 1
+            Hamiltonian(1),
+            torch.tensor([torch.pi / 4], dtype=torch.cdouble),
+            torch.tensor([0.5]),
+            1,
+        ),
+        (  # batchsize 1 | 4
+            Hamiltonian(1),
+            torch.tensor([torch.pi / 4, 0.0, torch.pi / 2, torch.pi]),
+            torch.tensor([0.5, 1.0, 0.0, 1.0]),
+            4,
+        ),
+        (  # batchsize 2 | 1
+            Hamiltonian(2),
+            torch.tensor([torch.pi / 4], dtype=torch.cdouble),
+            torch.tensor([0.5, 0.5]),
+            2,
+        ),
+        (  # batchsize 2 | 2
+            Hamiltonian(2),
+            torch.tensor([torch.pi / 4, torch.pi]),
+            torch.tensor([0.5, 1.0]),
+            2,
+        ),
+    ],
+)
+def test_hamiltonianevolution_with_types(
+    ham_evo_type: pyq.HamEvoType,
+    ham_evo_class: torch.nn.Module,
+    H: torch.Tensor,
+    t_evo: torch.Tensor,
+    target: torch.Tensor,
+    batch_size: int,
+) -> None:
+    def overlap(state1: torch.Tensor, state2: torch.Tensor) -> torch.Tensor:
+        N = len(state1.shape) - 1
+        state1_T = torch.transpose(state1, N, 0)
+        overlap = torch.tensordot(state1_T, state2, dims=N)
+        return torch.abs(overlap**2).flatten()
 
-    assert torch.max(diff) <= 10 ** (-6)
+    n_qubits = 4
+    hamevo = pyq.HamiltonianEvolution(range(n_qubits), n_qubits, hamevo_type=ham_evo_type)
+    ham_evo_instance = hamevo.get_hamevo_instance(H, t_evo)
+    assert isinstance(ham_evo_instance, ham_evo_class)
+
+    psi = pyq.uniform_state(n_qubits)
+    psi_star = hamevo(H, t_evo, psi)
+    result = overlap(psi_star, psi)
+    assert result.size() == (batch_size,)
+    assert torch.allclose(result, target)
```

### Comparing `pyqtorch-0.3.0/.gitignore` & `pyqtorch-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/LICENSE` & `pyqtorch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.0/pyproject.toml` & `pyqtorch-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.3.0"
+version = "0.3.1"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.3.0/PKG-INFO` & `pyqtorch-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

