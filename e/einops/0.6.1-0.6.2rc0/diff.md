# Comparing `tmp/einops-0.6.1.tar.gz` & `tmp/einops-0.6.2rc0.tar.gz`

## Comparing `einops-0.6.1.tar` & `einops-0.6.2rc0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 einops-0.6.1/mkdocs.yml
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.6.1/test.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 einops-0.6.1/einops/__init__.py
--rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 einops-0.6.1/einops/_backends.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 einops-0.6.1/einops/_torch_specific.py
--rw-r--r--   0        0        0    33690 2020-02-02 00:00:00.000000 einops-0.6.1/einops/einops.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.6.1/einops/packing.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.6.1/einops/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.1/einops/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/__init__.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/data_api_packing.py
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/indexing.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/__init__.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/_einmix.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/chainer.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/flax.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/gluon.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/keras.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/oneflow.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/paddle.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/tensorflow.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/torch.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.6.1/scripts/convert_readme.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 einops-0.6.1/scripts/setup.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 einops-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_einsum.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_examples.py
--rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_layers.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_notebooks.py
--rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_ops.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_other.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_packing.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_parsing.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 einops-0.6.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.6.1/LICENSE
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 einops-0.6.1/README.md
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 einops-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 einops-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 einops-0.6.2rc0/mkdocs.yml
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.6.2rc0/test.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/__init__.py
+-rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/_backends.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/_torch_specific.py
+-rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/einops.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/packing.py
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/__init__.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/data_api_packing.py
+-rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/experimental/indexing.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/__init__.py
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/_einmix.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/chainer.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/flax.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/gluon.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/keras.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/oneflow.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/paddle.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/tensorflow.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 einops-0.6.2rc0/einops/layers/torch.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.6.2rc0/scripts/convert_readme.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 einops-0.6.2rc0/scripts/setup.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/__init__.py
+-rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_einsum.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_examples.py
+-rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_layers.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_notebooks.py
+-rw-r--r--   0        0        0    22261 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_ops.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_other.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_packing.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.6.2rc0/tests/test_parsing.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 einops-0.6.2rc0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.6.2rc0/LICENSE
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 einops-0.6.2rc0/README.md
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 einops-0.6.2rc0/pyproject.toml
+-rw-r--r--   0        0        0    12829 2020-02-02 00:00:00.000000 einops-0.6.2rc0/PKG-INFO
```

### Comparing `einops-0.6.1/mkdocs.yml` & `einops-0.6.2rc0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/test.py` & `einops-0.6.2rc0/test.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/_backends.py` & `einops-0.6.2rc0/einops/_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
       importing may drive to crashes
 - backend should be either symbolic or imperative (tensorflow is for both, but that causes problems)
     - this determines which methods (from_numpy/to_numpy or create_symbol/eval_symbol) should be defined
 - if backend can't (temporarily) provide symbols for shape dimensions, UnknownSize objects are used
 """
 
 import sys
-import warnings
 
 __author__ = 'Alex Rogozhnikov'
 
 _backends: dict = {}
 _debug_importing = False
```

### Comparing `einops-0.6.1/einops/_torch_specific.py` & `einops-0.6.2rc0/einops/_torch_specific.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """
 Specialization of einops for torch.
 
 Unfortunately, torch's jit scripting mechanism isn't strong enough,
 and to have scripting supported at least for layers,
-a number of changes is required, and this layer helps.
+a number of additional moves is needed.
 
-Importantly, whole lib is designed so that you can't use it
+Design of main operations (dynamic resolution by lookup) is unlikely
+to be implemented by torch.jit.script, but torch.compile seems to work completely fine.
 """
 import warnings
-from typing import Dict, List
+from typing import Dict, List, Tuple
 
 import torch
 from einops.einops import TransformRecipe, _reconstruct_from_shape_uncached
 
 
 class TorchJitBackend:
     """
     Completely static backend that mimics part of normal backend functionality
-    but restricted to torch stuff only
+    but restricted to be within torchscript.
     """
 
     @staticmethod
     def reduce(x: torch.Tensor, operation: str, reduced_axes: List[int]):
-        if operation == 'min':
+        if operation == "min":
             return x.amin(dim=reduced_axes)
-        elif operation == 'max':
+        elif operation == "max":
             return x.amax(dim=reduced_axes)
-        elif operation == 'sum':
+        elif operation == "sum":
             return x.sum(dim=reduced_axes)
-        elif operation == 'mean':
+        elif operation == "mean":
             return x.mean(dim=reduced_axes)
-        elif operation == 'prod':
+        elif operation == "prod":
             for i in list(sorted(reduced_axes))[::-1]:
                 x = x.prod(dim=i)
             return x
         else:
-            raise NotImplementedError('Unknown reduction ', operation)
+            raise NotImplementedError("Unknown reduction ", operation)
 
     @staticmethod
     def transpose(x, axes: List[int]):
         return x.permute(axes)
 
     @staticmethod
     def stack_on_zeroth_dimension(tensors: List[torch.Tensor]):
@@ -67,32 +68,43 @@
 
     @staticmethod
     def reshape(x, shape: List[int]):
         return x.reshape(shape)
 
 
 # mirrors einops.einops._apply_recipe
-def apply_for_scriptable_torch(recipe: TransformRecipe, tensor: torch.Tensor, reduction_type: str) -> torch.Tensor:
+def apply_for_scriptable_torch(
+    recipe: TransformRecipe, tensor: torch.Tensor, reduction_type: str, axes_dims: List[Tuple[str, int]]
+) -> torch.Tensor:
     backend = TorchJitBackend
-    init_shapes, reduced_axes, axes_reordering, added_axes, final_shapes = \
-        _reconstruct_from_shape_uncached(recipe, backend.shape(tensor))
-    tensor = backend.reshape(tensor, init_shapes)
+    (
+        init_shapes,
+        axes_reordering,
+        reduced_axes,
+        added_axes,
+        final_shapes,
+        n_axes_w_added,
+    ) = _reconstruct_from_shape_uncached(recipe, backend.shape(tensor), axes_dims=axes_dims)
+    if init_shapes is not None:
+        tensor = backend.reshape(tensor, init_shapes)
+    if axes_reordering is not None:
+        tensor = backend.transpose(tensor, axes_reordering)
     if len(reduced_axes) > 0:
         tensor = backend.reduce(tensor, operation=reduction_type, reduced_axes=reduced_axes)
-    tensor = backend.transpose(tensor, axes_reordering)
     if len(added_axes) > 0:
-        tensor = backend.add_axes(tensor, n_axes=len(axes_reordering) + len(added_axes), pos2len=added_axes)
-    return backend.reshape(tensor, final_shapes)
+        tensor = backend.add_axes(tensor, n_axes=n_axes_w_added, pos2len=added_axes)
+    if final_shapes is not None:
+        tensor = backend.reshape(tensor, final_shapes)
+    return tensor
 
 
 def allow_ops_in_compiled_graph():
     try:
         from torch._dynamo import allow_in_graph
     except ImportError:
-        from warnings import warn
         warnings.warn("allow_ops_in_compiled_graph failed to import torch: ensure pytorch >=2.0", ImportWarning)
 
     from .einops import rearrange, reduce, repeat, einsum
     from .packing import pack, unpack
 
     allow_in_graph(rearrange)
     allow_in_graph(reduce)
```

### Comparing `einops-0.6.1/einops/einops.py` & `einops-0.6.2rc0/einops/einops.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,28 @@
 if typing.TYPE_CHECKING:
     import numpy as np
 
 from . import EinopsError
 from ._backends import get_backend
 from .parsing import ParsedExpression, _ellipsis, AnonymousAxis
 
-Tensor = TypeVar('Tensor')
+Tensor = TypeVar("Tensor")
 ReductionCallable = Callable[[Tensor, Tuple[int, ...]], Tensor]
 Reduction = Union[str, ReductionCallable]
 
-_reductions = ('min', 'max', 'sum', 'mean', 'prod')
+_reductions = ("min", "max", "sum", "mean", "prod")
+
 # magic integers are required to stay within
 # traceable subset of language
-_ellipsis_not_in_parenthesis: List[int] = [-999]
 _unknown_axis_length = -999999
-
-
-def is_ellipsis_not_in_parenthesis(group: List[int]) -> bool:
-    if len(group) != 1:
-        return False
-    return group[0] == -999
+_expected_axis_length = -99999
 
 
 def _product(sequence: List[int]) -> int:
-    """ minimalistic product that works both with numbers and symbols. Supports empty lists """
+    """minimalistic product that works both with numbers and symbols. Supports empty lists"""
     result = 1
     for element in sequence:
         result *= element
     return result
 
 
 def _reduce_axes(tensor, reduction_type: Reduction, reduced_axes: List[int], backend):
@@ -42,34 +37,34 @@
         # custom callable
         return reduction_type(tensor, tuple(reduced_axes))
     else:
         # one of built-in operations
         if len(reduced_axes) == 0:
             return tensor
         assert reduction_type in _reductions
-        if reduction_type == 'mean':
+        if reduction_type == "mean":
             if not backend.is_float_type(tensor):
-                raise NotImplementedError('reduce_mean is not available for non-floating tensors')
+                raise NotImplementedError("reduce_mean is not available for non-floating tensors")
         return backend.reduce(tensor, reduction_type, tuple(reduced_axes))
 
 
 def _optimize_transformation(init_shapes, reduced_axes, axes_reordering, final_shapes):
     # 'collapses' neighboring axes if those participate in the result pattern in the same order
     # TODO add support for added_axes
     assert len(axes_reordering) + len(reduced_axes) == len(init_shapes)
     # joining consecutive axes that will be reduced
     # possibly we can skip this if all backends can optimize this (not sure)
     reduced_axes = tuple(sorted(reduced_axes))
     for i in range(len(reduced_axes) - 1)[::-1]:
         if reduced_axes[i] + 1 == reduced_axes[i + 1]:
             removed_axis = reduced_axes[i + 1]
             removed_length = init_shapes[removed_axis]
-            init_shapes = init_shapes[:removed_axis] + init_shapes[removed_axis + 1:]
+            init_shapes = init_shapes[:removed_axis] + init_shapes[removed_axis + 1 :]
             init_shapes[removed_axis - 1] *= removed_length
-            reduced_axes = reduced_axes[:i + 1] + tuple(axis - 1 for axis in reduced_axes[i + 2:])
+            reduced_axes = reduced_axes[: i + 1] + tuple(axis - 1 for axis in reduced_axes[i + 2 :])
 
     # removing axes that are moved together during reshape
     def build_mapping():
         init_to_final = {}
         for axis in range(len(init_shapes)):
             if axis in reduced_axes:
                 init_to_final[axis] = None
@@ -87,15 +82,15 @@
             continue
         if init_axis_to_final_axis[init_axis] + 1 == init_axis_to_final_axis[init_axis + 1]:
             removed_axis = init_axis + 1
             removed_length = init_shapes[removed_axis]
             removed_axis_after_reduction = sum(x not in reduced_axes for x in range(removed_axis))
 
             reduced_axes = tuple(axis if axis < removed_axis else axis - 1 for axis in reduced_axes)
-            init_shapes = init_shapes[:removed_axis] + init_shapes[removed_axis + 1:]
+            init_shapes = init_shapes[:removed_axis] + init_shapes[removed_axis + 1 :]
             init_shapes[removed_axis - 1] *= removed_length
             old_reordering = axes_reordering
             axes_reordering = []
             for axis in old_reordering:
                 if axis == removed_axis_after_reduction:
                     pass
                 elif axis < removed_axis_after_reduction:
@@ -103,188 +98,240 @@
                 else:
                     axes_reordering.append(axis - 1)
             init_axis_to_final_axis = build_mapping()
 
     return init_shapes, reduced_axes, axes_reordering, final_shapes
 
 
-CookedRecipe = Tuple[List[int], List[int], List[int], Dict[int, int], List[int]]
+# This
+CookedRecipe = Tuple[Optional[List[int]], Optional[List[int]], List[int], Dict[int, int], Optional[List[int]], int]
+
+HashableAxesLengths = List[Tuple[str, int]]
 
 
 class TransformRecipe:
     """
     Recipe describes actual computation pathway.
     Recipe can be applied to a tensor or variable.
     """
 
     # structure is non-mutable. In future, this can be non-mutable dataclass (python 3.7+)
+    # update: pytorch 2.0 torch.jit.script seems to have problems with dataclasses unless they were explicitly provided
 
-    def __init__(self,
-                 # list of expressions (or just sizes) for elementary axes as they appear in left expression.
-                 # this is what (after computing unknown parts) will be a shape after first transposition.
-                 # If ellipsis is present, it forms one dimension here (in the right position).
-                 elementary_axes_lengths: List[int],
-                 # each dimension in input can help to reconstruct length of one elementary axis
-                 # or verify one of dimensions. Each element points to element of elementary_axes_lengths
-                 input_composite_axes: List[Tuple[List[int], List[int]]],
-                 # indices of axes to be squashed
-                 reduced_elementary_axes: List[int],
-                 # in which order should axes be reshuffled after reduction
-                 axes_permutation: List[int],
-                 # at which positions which of elementary axes should appear
-                 added_axes: Dict[int, int],
-                 # ids of axes as they appear in result, again pointers to elementary_axes_lengths,
-                 # only used to infer result dimensions
-                 output_composite_axes: List[List[int]],
-                 # positions of ellipsis in lhs and rhs of expression
-                 ellipsis_position_in_lhs: Optional[int] = None,
-                 ):
+    def __init__(
+        self,
+        # list of sizes (or just sizes) for elementary axes as they appear in left expression.
+        # this is what (after computing unknown parts) will be a shape after first transposition.
+        # This does not include any ellipsis dimensions.
+        elementary_axes_lengths: List[int],
+        # if additional axes are provided, they should be set in prev array
+        # This shows mapping from name to position
+        axis_name2elementary_axis: Dict[str, int],
+        # each dimension in input can help to reconstruct length of one elementary axis
+        # or verify one of dimensions. Each element points to element of elementary_axes_lengths.
+        input_composition_known_unknown: List[Tuple[List[int], List[int]]],
+        # permutation applied to elementary axes, if ellipsis is absent
+        axes_permutation: List[int],
+        # permutation puts reduced axes in the end, we only need to know the first position.
+        first_reduced_axis: int,
+        # at which positions which of elementary axes should appear. Axis position -> axis index.
+        added_axes: Dict[int, int],
+        # ids of axes as they appear in result, again pointers to elementary_axes_lengths,
+        # only used to infer result dimensions
+        output_composite_axes: List[List[int]],
+    ):
         self.elementary_axes_lengths: List[int] = elementary_axes_lengths
-        self.input_composite_axes: List[Tuple[List[int], List[int]]] = input_composite_axes
-        self.output_composite_axes: List[List[int]] = output_composite_axes
+        self.axis_name2elementary_axis: Dict[str, int] = axis_name2elementary_axis
+        self.input_composition_known_unknown: List[Tuple[List[int], List[int]]] = input_composition_known_unknown
         self.axes_permutation: List[int] = axes_permutation
+
+        self.first_reduced_axis: int = first_reduced_axis
         self.added_axes: Dict[int, int] = added_axes
-        # This is redundant information, but more convenient to use
-        self.reduced_elementary_axes: List[int] = reduced_elementary_axes
-        # setting to a large number to avoid handling Nones in reconstruct_from_shape
-        self.ellipsis_position_in_lhs: int = ellipsis_position_in_lhs if ellipsis_position_in_lhs is not None else 10000
+        self.output_composite_axes: List[List[int]] = output_composite_axes
 
 
-def _reconstruct_from_shape_uncached(self: TransformRecipe, shape: List[int]) -> CookedRecipe:
+def _reconstruct_from_shape_uncached(
+    self: TransformRecipe, shape: List[int], axes_dims: HashableAxesLengths
+) -> CookedRecipe:
     """
     Reconstruct all actual parameters using shape.
-    Shape is a tuple that may contain integers, shape symbols (tf, keras, theano) and UnknownSize (keras, mxnet)
+    Shape is a tuple that may contain integers, shape symbols (tf, theano) and UnknownSize (tf, previously mxnet)
     known axes can be integers or symbols, but not Nones.
     """
+    # magic number
+    need_init_reshape = False
+
+    # last axis is allocated for collapsed ellipsis
     axes_lengths: List[int] = list(self.elementary_axes_lengths)
-    if self.ellipsis_position_in_lhs != 10000:
-        if len(shape) < len(self.input_composite_axes) - 1:
-            raise EinopsError('Expected at least {} dimensions, got {}'.format(
-                len(self.input_composite_axes) - 1, len(shape)))
-    else:
-        if len(shape) != len(self.input_composite_axes):
-            raise EinopsError('Expected {} dimensions, got {}'.format(len(self.input_composite_axes), len(shape)))
+    for axis, dim in axes_dims:
+        axes_lengths[self.axis_name2elementary_axis[axis]] = dim
+
+    for input_axis, (known_axes, unknown_axes) in enumerate(self.input_composition_known_unknown):
+        length = shape[input_axis]
+        if len(known_axes) == 0 and len(unknown_axes) == 1:
+            # shortcut for the most common case
+            axes_lengths[unknown_axes[0]] = length
+            continue
 
-    ellipsis_shape: List[int] = []
-    for input_axis, (known_axes, unknown_axes) in enumerate(self.input_composite_axes):
-        before_ellipsis = input_axis
-        after_ellipsis = input_axis + len(shape) - len(self.input_composite_axes)
-        if input_axis == self.ellipsis_position_in_lhs:
-            assert len(known_axes) == 0 and len(unknown_axes) == 1
-            unknown_axis: int = unknown_axes[0]
-            ellipsis_shape = shape[before_ellipsis:after_ellipsis + 1]
-            for d in ellipsis_shape:
-                if d is None:
-                    raise EinopsError("Couldn't infer shape for one or more axes represented by ellipsis")
-            total_dim_size: int = _product(ellipsis_shape)
-            axes_lengths[unknown_axis] = total_dim_size
+        known_product = 1
+        for axis in known_axes:
+            known_product *= axes_lengths[axis]
+
+        if len(unknown_axes) == 0:
+            if isinstance(length, int) and isinstance(known_product, int) and length != known_product:
+                raise EinopsError(f"Shape mismatch, {length} != {known_product}")
         else:
-            if input_axis < self.ellipsis_position_in_lhs:
-                length = shape[before_ellipsis]
-            else:
-                length = shape[after_ellipsis]
-            known_product = 1
-            for axis in known_axes:
-                known_product *= axes_lengths[axis]
-
-            if len(unknown_axes) == 0:
-                if isinstance(length, int) and isinstance(known_product, int) and length != known_product:
-                    raise EinopsError('Shape mismatch, {} != {}'.format(length, known_product))
-            # this is enforced when recipe is created
-            # elif len(unknown_axes) > 1:
-            #     raise EinopsError(
-            #         "Lengths of two or more axes in parenthesis not provided (dim={}), can't infer dimensions".
-            #             format(known_product)
-            #     )
-            else:
-                if isinstance(length, int) and isinstance(known_product, int) and length % known_product != 0:
-                    raise EinopsError("Shape mismatch, can't divide axis of length {} in chunks of {}".format(
-                        length, known_product))
-
-                unknown_axis = unknown_axes[0]
-                inferred_length: int = length // known_product
-                axes_lengths[unknown_axis] = inferred_length
+            # assert len(unknown_axes) == 1, 'this is enforced when recipe is created, so commented out'
+            if isinstance(length, int) and isinstance(known_product, int) and length % known_product != 0:
+                raise EinopsError(f"Shape mismatch, can't divide axis of length {length} in chunks of {known_product}")
+
+            unknown_axis = unknown_axes[0]
+            inferred_length: int = length // known_product
+            axes_lengths[unknown_axis] = inferred_length
+
+        if len(known_axes) + len(unknown_axes) != 1:
+            need_init_reshape = True
 
     # at this point all axes_lengths are computed (either have values or variables, but not Nones)
 
-    # TODO more readable expression
-    init_shapes = axes_lengths[:len(axes_lengths) - len(self.added_axes)]
+    # elementary axes are ordered as they appear in input, then all added axes
+    init_shapes: Optional[List[int]] = axes_lengths[: len(self.axes_permutation)] if need_init_reshape else None
+
+    need_final_reshape = False
     final_shapes: List[int] = []
-    for output_axis, grouping in enumerate(self.output_composite_axes):
-        if is_ellipsis_not_in_parenthesis(grouping):
-            final_shapes.extend(ellipsis_shape)
-        else:
-            lengths = [axes_lengths[elementary_axis] for elementary_axis in grouping]
-            final_shapes.append(_product(lengths))
-    reduced_axes = self.reduced_elementary_axes
-    axes_reordering = self.axes_permutation
+    for grouping in self.output_composite_axes:
+        lengths = [axes_lengths[elementary_axis] for elementary_axis in grouping]
+        final_shapes.append(_product(lengths))
+        if len(lengths) != 1:
+            need_final_reshape = True
+
     added_axes: Dict[int, int] = {
-        pos: axes_lengths[pos_in_elementary] for pos, pos_in_elementary in self.added_axes.items()}
-    # if optimize:
-    #     assert len(self.added_axes) == 0
-    #     return _optimize_transformation(init_shapes, reduced_axes, axes_reordering, final_shapes)
-    return init_shapes, reduced_axes, axes_reordering, added_axes, final_shapes
+        pos: axes_lengths[pos_in_elementary] for pos, pos_in_elementary in self.added_axes.items()
+    }
+
+    # this list can be empty
+    reduced_axes = list(range(self.first_reduced_axis, len(self.axes_permutation)))
+
+    n_axes_after_adding_axes = len(added_axes) + len(self.axes_permutation)
+
+    axes_reordering: Optional[List[int]] = self.axes_permutation
+    if self.axes_permutation == list(range(len(self.axes_permutation))):
+        axes_reordering = None
+
+    _final_shapes = final_shapes if need_final_reshape else None
+    return init_shapes, axes_reordering, reduced_axes, added_axes, _final_shapes, n_axes_after_adding_axes
 
 
 _reconstruct_from_shape = functools.lru_cache(1024)(_reconstruct_from_shape_uncached)
 
 
-def _apply_recipe(recipe: TransformRecipe, tensor: Tensor, reduction_type: Reduction) -> Tensor:
+def _apply_recipe(
+    backend, recipe: TransformRecipe, tensor: Tensor, reduction_type: Reduction, axes_lengths: HashableAxesLengths
+) -> Tensor:
     # this method works for all backends but not compilable with
-    backend = get_backend(tensor)
-    init_shapes, reduced_axes, axes_reordering, added_axes, final_shapes = \
-        _reconstruct_from_shape(recipe, backend.shape(tensor))
-    tensor = backend.reshape(tensor, init_shapes)
-    tensor = _reduce_axes(tensor, reduction_type=reduction_type, reduced_axes=reduced_axes, backend=backend)
-    tensor = backend.transpose(tensor, axes_reordering)
+    init_shapes, axes_reordering, reduced_axes, added_axes, final_shapes, n_axes_w_added = _reconstruct_from_shape(
+        recipe, backend.shape(tensor), axes_lengths
+    )
+    if init_shapes is not None:
+        tensor = backend.reshape(tensor, init_shapes)
+    if axes_reordering is not None:
+        tensor = backend.transpose(tensor, axes_reordering)
+    if len(reduced_axes) > 0:
+        tensor = _reduce_axes(tensor, reduction_type=reduction_type, reduced_axes=reduced_axes, backend=backend)
     if len(added_axes) > 0:
-        tensor = backend.add_axes(tensor, n_axes=len(axes_reordering) + len(added_axes), pos2len=added_axes)
-    return backend.reshape(tensor, final_shapes)
+        tensor = backend.add_axes(tensor, n_axes=n_axes_w_added, pos2len=added_axes)
+    if final_shapes is not None:
+        tensor = backend.reshape(tensor, final_shapes)
+    return tensor
 
 
 @functools.lru_cache(256)
-def _prepare_transformation_recipe(pattern: str,
-                                   operation: Reduction,
-                                   axes_lengths: Tuple[Tuple, ...]) -> TransformRecipe:
-    """ Perform initial parsing of pattern and provided supplementary info
+def _prepare_transformation_recipe(
+    pattern: str,
+    operation: Reduction,
+    axes_names: Tuple[str, ...],
+    ndim: int,
+) -> TransformRecipe:
+    """Perform initial parsing of pattern and provided supplementary info
     axes_lengths is a tuple of tuples (axis_name, axis_length)
     """
-    left_str, rght_str = pattern.split('->')
+    left_str, rght_str = pattern.split("->")
     left = ParsedExpression(left_str)
     rght = ParsedExpression(rght_str)
 
     # checking that axes are in agreement - new axes appear only in repeat, while disappear only in reduction
     if not left.has_ellipsis and rght.has_ellipsis:
-        raise EinopsError('Ellipsis found in right side, but not left side of a pattern {}'.format(pattern))
+        raise EinopsError("Ellipsis found in right side, but not left side of a pattern {}".format(pattern))
     if left.has_ellipsis and left.has_ellipsis_parenthesized:
-        raise EinopsError('Ellipsis is parenthesis in the left side is not allowed: {}'.format(pattern))
-    if operation == 'rearrange':
-        difference = set.symmetric_difference(left.identifiers, rght.identifiers)
+        raise EinopsError("Ellipsis inside parenthesis in the left side is not allowed: {}".format(pattern))
+    if operation == "rearrange":
         if left.has_non_unitary_anonymous_axes or rght.has_non_unitary_anonymous_axes:
-            raise EinopsError('Non-unitary anonymous axes are not supported in rearrange (exception is length 1)')
+            raise EinopsError("Non-unitary anonymous axes are not supported in rearrange (exception is length 1)")
+        difference = set.symmetric_difference(left.identifiers, rght.identifiers)
         if len(difference) > 0:
-            raise EinopsError('Identifiers only on one side of expression (should be on both): {}'.format(difference))
-    elif operation == 'repeat':
+            raise EinopsError("Identifiers only on one side of expression (should be on both): {}".format(difference))
+    elif operation == "repeat":
         difference = set.difference(left.identifiers, rght.identifiers)
         if len(difference) > 0:
-            raise EinopsError('Unexpected identifiers on the left side of repeat: {}'.format(difference))
-        axes_without_size = set.difference({ax for ax in rght.identifiers if not isinstance(ax, AnonymousAxis)},
-                                           {*left.identifiers, *(ax for ax, _ in axes_lengths)})
+            raise EinopsError("Unexpected identifiers on the left side of repeat: {}".format(difference))
+        axes_without_size = set.difference(
+            {ax for ax in rght.identifiers if not isinstance(ax, AnonymousAxis)},
+            {*left.identifiers, *axes_names},
+        )
         if len(axes_without_size) > 0:
-            raise EinopsError('Specify sizes for new axes in repeat: {}'.format(axes_without_size))
+            raise EinopsError("Specify sizes for new axes in repeat: {}".format(axes_without_size))
     elif operation in _reductions or callable(operation):
         difference = set.difference(rght.identifiers, left.identifiers)
         if len(difference) > 0:
-            raise EinopsError('Unexpected identifiers on the right side of reduce {}: {}'.format(operation, difference))
+            raise EinopsError("Unexpected identifiers on the right side of reduce {}: {}".format(operation, difference))
     else:
-        raise EinopsError('Unknown reduction {}. Expect one of {}.'.format(operation, _reductions))
+        raise EinopsError("Unknown reduction {}. Expect one of {}.".format(operation, _reductions))
+
+    if left.has_ellipsis:
+        n_other_dims = len(left.composition) - 1
+        if ndim < n_other_dims:
+            raise EinopsError(f"Wrong shape: expected >={n_other_dims} dims. Received {ndim}-dim tensor.")
+        ellipsis_ndim = ndim - n_other_dims
+        ell_axes = [_ellipsis + str(i) for i in range(ellipsis_ndim)]
+        left_composition = []
+        for composite_axis in left.composition:
+            if composite_axis == _ellipsis:
+                for axis in ell_axes:
+                    left_composition.append([axis])
+            else:
+                left_composition.append(composite_axis)
+
+        rght_composition = []
+        for composite_axis in rght.composition:
+            if composite_axis == _ellipsis:
+                for axis in ell_axes:
+                    rght_composition.append([axis])
+            else:
+                group = []
+                for axis in composite_axis:
+                    if axis == _ellipsis:
+                        group.extend(ell_axes)
+                    else:
+                        group.append(axis)
+                rght_composition.append(group)
+
+        left.identifiers.update(ell_axes)
+        left.identifiers.remove(_ellipsis)
+        if rght.has_ellipsis:
+            rght.identifiers.update(ell_axes)
+            rght.identifiers.remove(_ellipsis)
+    else:
+        if ndim != len(left.composition):
+            raise EinopsError(f"Wrong shape: expected {len(left.composition)} dims. Received {ndim}-dim tensor.")
+        left_composition = left.composition
+        rght_composition = rght.composition
 
     # parsing all dimensions to find out lengths
     axis_name2known_length: Dict[Union[str, AnonymousAxis], int] = OrderedDict()
-    for composite_axis in left.composition:
+    for composite_axis in left_composition:
         for axis_name in composite_axis:
             if isinstance(axis_name, AnonymousAxis):
                 axis_name2known_length[axis_name] = axis_name.value
             else:
                 axis_name2known_length[axis_name] = _unknown_axis_length
 
     # axis_ids_after_first_reshape = range(len(axis_name2known_length)) at this point
@@ -295,69 +342,86 @@
             if isinstance(axis_name, AnonymousAxis):
                 axis_name2known_length[axis_name] = axis_name.value
             else:
                 axis_name2known_length[axis_name] = _unknown_axis_length
             repeat_axes_names.append(axis_name)
 
     axis_name2position = {name: position for position, name in enumerate(axis_name2known_length)}
-    reduced_axes: List[int] = [position for axis, position in axis_name2position.items() if
-                               axis not in rght.identifiers]
-    reduced_axes = list(sorted(reduced_axes))
 
-    for elementary_axis, axis_length in axes_lengths:
+    # axes provided as kwargs
+    for elementary_axis in axes_names:
         if not ParsedExpression.check_axis_name(elementary_axis):
-            raise EinopsError('Invalid name for an axis', elementary_axis)
+            raise EinopsError("Invalid name for an axis", elementary_axis)
         if elementary_axis not in axis_name2known_length:
-            raise EinopsError('Axis {} is not used in transform'.format(elementary_axis))
-        axis_name2known_length[elementary_axis] = axis_length
+            raise EinopsError("Axis {} is not used in transform".format(elementary_axis))
+        axis_name2known_length[elementary_axis] = _expected_axis_length
 
     input_axes_known_unknown = []
-    # some of shapes will be inferred later - all information is prepared for faster inference
-    for composite_axis in left.composition:
+    # some shapes are inferred later - all information is prepared for faster inference
+    for i, composite_axis in enumerate(left_composition):
         known: Set[str] = {axis for axis in composite_axis if axis_name2known_length[axis] != _unknown_axis_length}
         unknown: Set[str] = {axis for axis in composite_axis if axis_name2known_length[axis] == _unknown_axis_length}
         if len(unknown) > 1:
-            raise EinopsError('Could not infer sizes for {}'.format(unknown))
+            raise EinopsError("Could not infer sizes for {}".format(unknown))
         assert len(unknown) + len(known) == len(composite_axis)
         input_axes_known_unknown.append(
-            ([axis_name2position[axis] for axis in known],
-             [axis_name2position[axis] for axis in unknown])
+            ([axis_name2position[axis] for axis in known], [axis_name2position[axis] for axis in unknown])
         )
 
     axis_position_after_reduction: Dict[str, int] = {}
-    for axis_name in itertools.chain(*left.composition):
+    for axis_name in itertools.chain(*left_composition):
         if axis_name in rght.identifiers:
             axis_position_after_reduction[axis_name] = len(axis_position_after_reduction)
 
-    result_axes_grouping: List[List[int]] = []
-    for composite_axis in rght.composition:
-        if composite_axis == _ellipsis:
-            result_axes_grouping.append(_ellipsis_not_in_parenthesis)
-        else:
-            result_axes_grouping.append([axis_name2position[axis] for axis in composite_axis])
+    result_axes_grouping: List[List[int]] = [
+        [axis_name2position[axis] for axis in composite_axis] for i, composite_axis in enumerate(rght_composition)
+    ]
 
-    ordered_axis_right = list(itertools.chain(*rght.composition))
-    axes_permutation = [
-        axis_position_after_reduction[axis] for axis in ordered_axis_right if axis in left.identifiers]
-    added_axes = {i: axis_name2position[axis_name] for i, axis_name in enumerate(ordered_axis_right)
-                  if axis_name not in left.identifiers}
+    ordered_axis_left = list(itertools.chain(*left_composition))
+    ordered_axis_rght = list(itertools.chain(*rght_composition))
+    reduced_axes = [axis for axis in ordered_axis_left if axis not in rght.identifiers]
+    order_after_transposition = [axis for axis in ordered_axis_rght if axis in left.identifiers] + reduced_axes
+    axes_permutation = [ordered_axis_left.index(axis) for axis in order_after_transposition]
+    added_axes = {
+        i: axis_name2position[axis_name]
+        for i, axis_name in enumerate(ordered_axis_rght)
+        if axis_name not in left.identifiers
+    }
 
-    ellipsis_left = None if _ellipsis not in left.composition else left.composition.index(_ellipsis)
+    first_reduced_axis = len(order_after_transposition) - len(reduced_axes)
 
     return TransformRecipe(
         elementary_axes_lengths=list(axis_name2known_length.values()),
-        input_composite_axes=input_axes_known_unknown,
-        reduced_elementary_axes=reduced_axes,
+        axis_name2elementary_axis={axis: axis_name2position[axis] for axis in axes_names},
+        input_composition_known_unknown=input_axes_known_unknown,
         axes_permutation=axes_permutation,
+        first_reduced_axis=first_reduced_axis,
         added_axes=added_axes,
         output_composite_axes=result_axes_grouping,
-        ellipsis_position_in_lhs=ellipsis_left,
     )
 
 
+# TODO multi-recipe should be recomputed when a layer is unpickled.
+
+
+def _prepare_recipes_for_all_dims(
+    pattern: str, operation: Reduction, axes_names: Tuple[str, ...]
+) -> Dict[int, TransformRecipe]:
+    """
+    Function to be used in layers.
+    Layer makes all recipe creation when it is initialized, thus to keep recipes simple we pre-compute for all dimensions.
+    """
+    left_str, rght_str = pattern.split("->")
+    left = ParsedExpression(left_str)
+    dims = [len(left.composition)]
+    if left.has_ellipsis:
+        dims = [len(left.composition) - 1 + ellipsis_dims for ellipsis_dims in range(8)]
+    return {ndim: _prepare_transformation_recipe(pattern, operation, axes_names, ndim=ndim) for ndim in dims}
+
+
 def reduce(tensor: Tensor, pattern: str, reduction: Reduction, **axes_lengths: int) -> Tensor:
     """
     einops.reduce provides combination of reordering and reduction using reader-friendly notation.
 
     Examples for reduce operation:
 
     ```python
@@ -404,25 +468,26 @@
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         tensor of the same type as input
     """
     try:
         hashable_axes_lengths = tuple(sorted(axes_lengths.items()))
-        recipe = _prepare_transformation_recipe(pattern, reduction, axes_lengths=hashable_axes_lengths)
-        return _apply_recipe(recipe, tensor, reduction_type=reduction)
+        backend = get_backend(tensor)
+        shape = backend.shape(tensor)
+        recipe = _prepare_transformation_recipe(pattern, reduction, axes_names=tuple(axes_lengths), ndim=len(shape))
+        return _apply_recipe(backend, recipe, tensor, reduction_type=reduction, axes_lengths=hashable_axes_lengths)
     except EinopsError as e:
         message = ' Error while processing {}-reduction pattern "{}".'.format(reduction, pattern)
         if not isinstance(tensor, list):
-            message += '\n Input tensor shape: {}. '.format(get_backend(tensor).shape(tensor))
+            message += "\n Input tensor shape: {}. ".format(shape)
         else:
-            message += '\n Input is list. '
-        message += 'Additional info: {}.'.format(axes_lengths)
-        raise EinopsError(message + '\n {}'.format(e))
-
+            message += "\n Input is list. "
+        message += "Additional info: {}.".format(axes_lengths)
+        raise EinopsError(message + "\n {}".format(e))
 
 
 def rearrange(tensor: Union[Tensor, List[Tensor]], pattern: str, **axes_lengths) -> Tensor:
     """
     einops.rearrange is a reader-friendly smart element reordering for multidimensional tensors.
     This operation includes functionality of transpose (axes permutation), reshape (view), squeeze, unsqueeze,
     stack, concatenate and other operations.
@@ -476,15 +541,15 @@
         tensor of the same type as input. If possible, a view to the original tensor is returned.
 
     """
     if isinstance(tensor, list):
         if len(tensor) == 0:
             raise TypeError("Rearrange can't be applied to an empty list")
         tensor = get_backend(tensor[0]).stack_on_zeroth_dimension(tensor)
-    return reduce(cast(Tensor, tensor), pattern, reduction='rearrange', **axes_lengths)
+    return reduce(cast(Tensor, tensor), pattern, reduction="rearrange", **axes_lengths)
 
 
 def repeat(tensor: Tensor, pattern: str, **axes_lengths) -> Tensor:
     """
     einops.repeat allows reordering elements and repeating them in arbitrary combinations.
     This operation includes functionality of repeat, tile, broadcast functions.
 
@@ -526,15 +591,15 @@
         pattern: string, rearrangement pattern
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         Tensor of the same type as input. If possible, a view to the original tensor is returned.
 
     """
-    return reduce(tensor, pattern, reduction='repeat', **axes_lengths)
+    return reduce(tensor, pattern, reduction="repeat", **axes_lengths)
 
 
 def parse_shape(x, pattern: str) -> dict:
     """
     Parse a tensor shape to dictionary mapping axes names to their lengths.
 
     ```python
@@ -558,39 +623,38 @@
 
     Returns:
         dict, maps axes names to their lengths
     """
     exp = ParsedExpression(pattern, allow_underscore=True)
     shape = get_backend(x).shape(x)
     if exp.has_composed_axes():
-        raise RuntimeError("Can't parse shape with composite axes: {pattern} {shape}".format(
-            pattern=pattern, shape=shape))
+        raise RuntimeError(f"Can't parse shape with composite axes: {pattern} {shape}")
     if len(shape) != len(exp.composition):
         if exp.has_ellipsis:
             if len(shape) < len(exp.composition) - 1:
-                raise RuntimeError("Can't parse shape with this number of dimensions: {pattern} {shape}".format(
-                    pattern=pattern, shape=shape))
+                raise RuntimeError(f"Can't parse shape with this number of dimensions: {pattern} {shape}")
         else:
-            raise RuntimeError("Can't parse shape with different number of dimensions: {pattern} {shape}".format(
-                pattern=pattern, shape=shape))
+            raise RuntimeError(f"Can't parse shape with different number of dimensions: {pattern} {shape}")
     if exp.has_ellipsis:
         ellipsis_idx = exp.composition.index(_ellipsis)
-        composition = (exp.composition[:ellipsis_idx] +
-                       ['_'] * (len(shape) - len(exp.composition) + 1) +
-                       exp.composition[ellipsis_idx + 1:])
+        composition = (
+            exp.composition[:ellipsis_idx]
+            + ["_"] * (len(shape) - len(exp.composition) + 1)
+            + exp.composition[ellipsis_idx + 1 :]
+        )
     else:
         composition = exp.composition
     result = {}
     for (axis_name,), axis_length in zip(composition, shape):  # type: ignore
-        if axis_name != '_':
+        if axis_name != "_":
             result[axis_name] = axis_length
     return result
 
 
-# this one is probably not needed in the public API
+# _enumerate_directions is not exposed in the public API
 def _enumerate_directions(x):
     """
     For an n-dimensional tensor, returns tensors to enumerate each axis.
     ```python
     x = np.zeros([2, 3, 4]) # or any other tensor
     i, j, k = _enumerate_directions(x)
     result = i + 2*j + 3*k
@@ -644,35 +708,31 @@
 
 @functools.lru_cache(256)
 def _compactify_pattern_for_einsum(pattern: str) -> str:
     if "->" not in pattern:
         # numpy allows this, so make sure users
         # don't accidentally do something like this.
         raise ValueError("Einsum pattern must contain '->'.")
-    lefts_str, right_str = pattern.split('->')
+    lefts_str, right_str = pattern.split("->")
 
-    lefts = [
-        ParsedExpression(left, allow_underscore=True, allow_duplicates=True)
-        for left in lefts_str.split(',')
-    ]
+    lefts = [ParsedExpression(left, allow_underscore=True, allow_duplicates=True) for left in lefts_str.split(",")]
 
     right = ParsedExpression(right_str, allow_underscore=True)
 
     # Start from 'a' and go up to 'Z'
     output_axis_names = string.ascii_letters
     i = 0
     axis_name_mapping = {}
 
     left_patterns = []
     for left in lefts:
         left_pattern = ""
         for raw_axis_name in left.composition:
-
             if raw_axis_name == _ellipsis:
-                left_pattern += '...'
+                left_pattern += "..."
                 continue
 
             _validate_einsum_axis_name(raw_axis_name)
             axis_name = raw_axis_name[0]
             if axis_name not in axis_name_mapping:
                 if i >= len(output_axis_names):
                     raise RuntimeError("Too many axes in einsum.")
@@ -682,39 +742,46 @@
             left_pattern += axis_name_mapping[axis_name]
         left_patterns.append(left_pattern)
 
     compact_pattern = ",".join(left_patterns) + "->"
 
     for raw_axis_name in right.composition:
         if raw_axis_name == _ellipsis:
-            compact_pattern += '...'
+            compact_pattern += "..."
             continue
 
         _validate_einsum_axis_name(raw_axis_name)
         axis_name = raw_axis_name[0]
 
         if axis_name not in axis_name_mapping:
             raise EinopsError(f"Unknown axis {axis_name} on right side of einsum {pattern}.")
 
         compact_pattern += axis_name_mapping[axis_name]
 
     return compact_pattern
 
 
-# dunders in overloads turn arguments into positional-only.
-# After python 3.7 EOL this should be replaced with '/' as the last argument.
-
 @typing.overload
-def einsum(__tensor: Tensor, __pattern: str) -> Tensor: ...
+def einsum(tensor: Tensor, pattern: str, /) -> Tensor:
+    ...
+
+
 @typing.overload
-def einsum(__tensor1: Tensor, __tensor2: Tensor, __pattern: str) -> Tensor: ...
+def einsum(tensor1: Tensor, tensor2: Tensor, pattern: str, /) -> Tensor:
+    ...
+
+
 @typing.overload
-def einsum(__tensor1: Tensor, __tensor2: Tensor, __tensor3: Tensor, __pattern: str) -> Tensor: ...
+def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, pattern: str, /) -> Tensor:
+    ...
+
+
 @typing.overload
-def einsum(__tensor1: Tensor, __tensor2: Tensor, __tensor3: Tensor, __tensor4: Tensor, __pattern: str) -> Tensor: ...
+def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, tensor4: Tensor, pattern: str, /) -> Tensor:
+    ...
 
 
 def einsum(*tensors_and_pattern: Union[Tensor, str]) -> Tensor:
     """
     einops.einsum calls einsum operations with einops-style named
     axes indexing, computing tensor products with an arbitrary
     number of tensors. Unlike typical einsum syntax, here you must
@@ -775,19 +842,17 @@
 
     Returns:
         Tensor of the same type as input, after processing with einsum.
 
     """
     if len(tensors_and_pattern) <= 1:
         raise ValueError(
-            "`einops.einsum` takes at minimum two arguments: the tensors (at least one),"
-            " followed by the pattern."
+            "`einops.einsum` takes at minimum two arguments: the tensors (at least one), followed by the pattern."
         )
     pattern = tensors_and_pattern[-1]
     if not isinstance(pattern, str):
         raise ValueError(
-            "The last argument passed to `einops.einsum` must be a string,"
-            " representing the einsum pattern."
+            "The last argument passed to `einops.einsum` must be a string, representing the einsum pattern."
         )
     tensors = tensors_and_pattern[:-1]
     pattern = _compactify_pattern_for_einsum(pattern)
     return get_backend(tensors[0]).einsum(pattern, *tensors)
```

### Comparing `einops-0.6.1/einops/packing.py` & `einops-0.6.2rc0/einops/packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/parsing.py` & `einops-0.6.2rc0/einops/parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/experimental/data_api_packing.py` & `einops-0.6.2rc0/einops/experimental/data_api_packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/experimental/indexing.py` & `einops-0.6.2rc0/einops/experimental/indexing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/_einmix.py` & `einops-0.6.2rc0/einops/layers/_einmix.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
         This layer manages weights for you, syntax highlights separate role of weight matrix
         >>> EinMix('time batch channel_in -> time batch channel_out', weight_shape='channel_in channel_out')
         But otherwise it is the same einsum under the hood.
 
         Simple linear layer with bias term (you have one like that in your framework)
         >>> EinMix('t b cin -> t b cout', weight_shape='cin cout', bias_shape='cout', cin=10, cout=20)
-        There is restriction to mix the last axis. Let's mix along height
+        There is no restriction to mix the last axis. Let's mix along height
         >>> EinMix('h w c-> hout w c', weight_shape='h hout', bias_shape='hout', h=32, hout=32)
         Channel-wise multiplication (like one used in normalizations)
         >>> EinMix('t b c -> t b c', weight_shape='c', c=128)
-        Separate dense layer within each head, no connection between different heads
+        Multi-head linear layer (each head is own linear layer):
         >>> EinMix('t b (head cin) -> t b (head cout)', weight_shape='head cin cout', ...)
 
         ... ah yes, you need to specify all dimensions of weight shape/bias shape in parameters.
 
         Use cases:
         - when channel dimension is not last, use EinMix, not transposition
         - patch/segment embeddings
```

### Comparing `einops-0.6.1/einops/layers/chainer.py` & `einops-0.6.2rc0/einops/layers/chainer.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/flax.py` & `einops-0.6.2rc0/einops/layers/flax.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/gluon.py` & `einops-0.6.2rc0/einops/layers/gluon.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/oneflow.py` & `einops-0.6.2rc0/einops/layers/oneflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/paddle.py` & `einops-0.6.2rc0/einops/layers/paddle.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/tensorflow.py` & `einops-0.6.2rc0/einops/layers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/einops/layers/torch.py` & `einops-0.6.2rc0/einops/layers/torch.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,30 @@
 from .._torch_specific import apply_for_scriptable_torch
 
 __author__ = 'Alex Rogozhnikov'
 
 
 class Rearrange(RearrangeMixin, torch.nn.Module):
     def forward(self, input):
-        return apply_for_scriptable_torch(self._recipe, input, reduction_type='rearrange')
+        recipe = self._multirecipe[input.ndim]
+        return apply_for_scriptable_torch(
+            recipe, input, reduction_type='rearrange', axes_dims=self._axes_lengths
+        )
 
     def _apply_recipe(self, x):
         # overriding parent method to prevent it's scripting
         pass
 
 
 class Reduce(ReduceMixin, torch.nn.Module):
     def forward(self, input):
-        return apply_for_scriptable_torch(self._recipe, input, reduction_type=self.reduction)
+        recipe = self._multirecipe[input.ndim]
+        return apply_for_scriptable_torch(
+            recipe, input, reduction_type=self.reduction, axes_dims=self._axes_lengths
+        )
 
     def _apply_recipe(self, x):
         # overriding parent method to prevent it's scripting
         pass
 
 
 class EinMix(_EinmixMixin, torch.nn.Module):
```

### Comparing `einops-0.6.1/scripts/convert_readme.py` & `einops-0.6.2rc0/scripts/convert_readme.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/scripts/setup.py` & `einops-0.6.2rc0/scripts/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 __author__ = 'Alex Rogozhnikov'
 
 from setuptools import setup
 
 setup(
     name="einops",
-    version='0.6.1',
+    version='0.6.2rc',
     description="A new flavour of deep learning operations",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/arogozhnikov/einops',
     author='Alex Rogozhnikov',
     classifiers=[
         'Intended Audience :: Science/Research',
```

### Comparing `einops-0.6.1/tests/__init__.py` & `einops-0.6.2rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_einsum.py` & `einops-0.6.2rc0/tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_examples.py` & `einops-0.6.2rc0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_layers.py` & `einops-0.6.2rc0/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_notebooks.py` & `einops-0.6.2rc0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_ops.py` & `einops-0.6.2rc0/tests/test_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                  getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
                 ['(a a2) ... -> (a2 a) ...', dict(a2=1),
                  input],
             ]
             for pattern, axes_lengths, expected_result in test_cases:
                 result = reduce(backend.from_numpy(input.copy()), pattern, reduction=reduction, **axes_lengths)
                 result = backend.to_numpy(result)
-                assert numpy.allclose(result, expected_result)
+                assert numpy.allclose(result, expected_result), f'Failed at {pattern}'
 
 
 def test_reduction_symbolic():
     for backend in sym_op_backends:
         print('Reduction tests for ', backend.framework_name)
         for reduction in _reductions:
             input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype='int64').reshape([2, 3, 4, 5, 6])
```

### Comparing `einops-0.6.1/tests/test_other.py` & `einops-0.6.2rc0/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_packing.py` & `einops-0.6.2rc0/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/tests/test_parsing.py` & `einops-0.6.2rc0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/.gitignore` & `einops-0.6.2rc0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -119,8 +119,11 @@
 # oneflow's output trash
 log
 
 # this file is auto-generated
 docs_src/index.md
 
 # vs code 
-*.code-workspace
+*.code-workspace
+
+# macos files
+.DS_Store
```

### Comparing `einops-0.6.1/LICENSE` & `einops-0.6.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `einops-0.6.1/README.md` & `einops-0.6.2rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: einops
+Version: 0.6.2rc0
+Summary: A new flavour of deep learning operations
+Project-URL: Homepage, https://github.com/arogozhnikov/einops
+Author: Alex Rogozhnikov
+License: MIT
+License-File: LICENSE
+Keywords: deep learning,einops,machine learning,neural networks,scientific computations,tensor manipulation
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 
 <!--
 <a href='http://arogozhnikov.github.io/images/einops/einops_video.mp4' >
 <div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_video.gif" alt="einops package examples" />
   <br>
   <small><a href='http://arogozhnikov.github.io/images/einops/einops_video.mp4'>This video in high quality (mp4)</a></small>
@@ -25,20 +40,31 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
+- 10'000: github reports that more than 10k project use einops 🎂
+- see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
+- einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
-- [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading)
-- flax and oneflow backend added
-- torch.jit.script is supported for pytorch layers
-- powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+- [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
+  Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
+
+
+<details>
+  <summary>Previous updates</summary>
+  
+  
+  - flax and oneflow backend added
+  - torch.jit.script is supported for pytorch layers
+  - powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+</details>
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
 
@@ -51,31 +77,33 @@
 [Andrej Karpathy, AI at Tesla](https://twitter.com/karpathy/status/1290826075916779520)
 
 > Slowly but surely, einops is seeping in to every nook and cranny of my code. If you find yourself shuffling around bazillion dimensional tensors, this might change your life
 [Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/1216022614755463169)
 
 [More testimonials](https://einops.rocks/pages/testimonials/)
 
+<!--
 ## Recordings of talk at ICLR 2022
 
 <a href='https://iclr.cc/virtual/2022/oral/6603'>
 <img width="922" alt="Screen Shot 2022-07-03 at 1 00 15 AM" src="https://user-images.githubusercontent.com/6318811/177030789-89d349bf-ef75-4af5-a71f-609896d1c8d9.png">
 </a>
 
 Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603) focused on main problems of standard tensor manipulation methods, and how einops improves this process.
-
+-->
 
 ## Contents
 
 - [Installation](#Installation)
 - [Documentation](https://einops.rocks/)
 - [Tutorial](#Tutorials) 
 - [API micro-reference](#API)
 - [Why using einops](#Why-using-einops-notation)
 - [Supported frameworks](#Supported-frameworks)
+- [Citing](#Citing)
 - [Repository](https://github.com/arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/discussions)
 
 ## Installation  <a name="Installation"></a>
 
 Plain and simple:
 ```bash
 pip install einops
@@ -113,64 +141,80 @@
 # rearrange elements according to the pattern
 output_tensor = rearrange(input_tensor, 't b c -> b c t')
 # combine rearrangement and reduction
 output_tensor = reduce(input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2)
 # copy along a new axis
 output_tensor = repeat(input_tensor, 'h w -> h w c', c=3)
 ```
-And two corresponding layers (`einops` keeps a separate version for each framework) with the same API.
-
-```python
-from einops.layers.torch      import Rearrange, Reduce
-from einops.layers.tensorflow import Rearrange, Reduce
-from einops.layers.flax       import Rearrange, Reduce
-from einops.layers.gluon      import Rearrange, Reduce
-from einops.layers.keras      import Rearrange, Reduce
-from einops.layers.chainer    import Rearrange, Reduce
-```
 
-Layers behave similarly to operations and have the same parameters 
-(with the exception of the first argument, which is passed during call).
+Later additions to the family are `pack` and `unpack` functions (better than stack/split/concatenate):
 
-Example of using layers within a model:
 ```python
-# example given for pytorch, but code in other frameworks is almost identical  
-from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
-from einops.layers.torch import Rearrange
-
-model = Sequential(
-    ...,
-    Conv2d(6, 16, kernel_size=5),
-    MaxPool2d(kernel_size=2),
-    # flattening without need to write forward
-    Rearrange('b c h w -> b (c h w)'),  
-    Linear(16*5*5, 120), 
-    ReLU(),
-    Linear(120, 10), 
-)
+from einops import pack, unpack
+# pack and unpack allow reversibly 'packing' multiple tensors into one.
+# Packed tensors may be of different dimensionality:
+packed,  ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
+class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b * c')
 ```
 
-Later additions to the family are `einsum`, `pack` and `unpack` functions:
+Finally, einops provides einsum with a support of multi-lettered names: 
 
 ```python
 from einops import einsum, pack, unpack
 # einsum is like ... einsum, generic and flexible dot-product 
 # but 1) axes can be multi-lettered  2) pattern goes last 3) works with multiple frameworks
 C = einsum(A, B, 'b t1 head c, b t2 head c -> b head t1 t2')
-
-# pack and unpack allow reversibly 'packing' multiple tensors into one.
-# Packed tensors may be of different dimensionality:
-packed,  ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
-class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b * c')
-# Pack/Unpack are more convenient than concat and split, see tutorial
 ```
 
-Last, but not the least `EinMix` layer is available! <br />
+### EinMix
+
 `EinMix` is a generic linear layer, perfect for MLP Mixers and similar architectures.
 
+### Layers
+
+Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
+
+```python
+from einops.layers.torch      import Rearrange, Reduce
+from einops.layers.tensorflow import Rearrange, Reduce
+from einops.layers.flax       import Rearrange, Reduce
+from einops.layers.gluon      import Rearrange, Reduce
+from einops.layers.keras      import Rearrange, Reduce
+from einops.layers.chainer    import Rearrange, Reduce
+```
+
+<details>
+  <summary>Example of using layers within a pytorch model</summary>
+  
+  
+  ```python
+  # example given for pytorch, but code in other frameworks is almost identical  
+  from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
+  from einops.layers.torch import Rearrange
+
+  model = Sequential(
+      ...,
+      Conv2d(6, 16, kernel_size=5),
+      MaxPool2d(kernel_size=2),
+      # flattening without need to write forward
+      Rearrange('b c h w -> b (c h w)'),  
+      Linear(16*5*5, 120), 
+      ReLU(),
+      Linear(120, 10), 
+  )
+  ```
+  
+  No more flatten needed! 
+  
+  Additionally, torch users will benefit from layers as those are script-able and compile-able.
+</details>
+
+
+
+
 ## Naming <a name="Naming"></a>
 
 `einops` stands for Einstein-Inspired Notation for operations 
 (though "Einstein operations" is more attractive and easier to remember).
 
 Notation was loosely inspired by Einstein summation (in particular by `numpy.einsum` operation).
 
@@ -274,15 +318,15 @@
 repeat(image, 'h w -> h (tile w)', tile=2)  # in pytorch
 repeat(image, 'h w -> h (tile w)', tile=2)  # in tf
 repeat(image, 'h w -> h (tile w)', tile=2)  # in jax
 repeat(image, 'h w -> h (tile w)', tile=2)  # in cupy
 ... (etc.)
 ```
 
-Testimonials provide user's perspective on the same question. 
+[Testimonials](https://einops.rocks/pages/testimonials/) provide users' perspective on the same question. 
 
 ## Supported frameworks <a name="Supported-frameworks"></a>
 
 Einops works with ...
 
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
@@ -292,15 +336,15 @@
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
 - [gluon](https://gluon.mxnet.io/) (deprecated)
 
-## Citing einops <a name="Contributing"></a>
+## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
     rogozhnikov2022einops,
     title={Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
```

#### html2text {}

```diff
@@ -1,41 +1,49 @@
-   https://user-images.githubusercontent.com/6318811/177030658-66f0eb5d-e136-
-44d8-99c9-86ae298ead5b.mp4 # einops [![Run tests](https://github.com/
-arogozhnikov/einops/actions/workflows/run_tests.yml/badge.svg)](https://
-github.com/arogozhnikov/einops/actions/workflows/run_tests.yml) [![PyPI
-version](https://badge.fury.io/py/einops.svg)](https://badge.fury.io/py/einops)
-[![Documentation](https://img.shields.io/badge/documentation-link-blue.svg)]
-(https://einops.rocks/) ![Supported python versions](https://
-raw.githubusercontent.com/arogozhnikov/einops/master/docs/resources/
-python_badge.svg) Flexible and powerful tensor operations for readable and
-reliable code.
+Metadata-Version: 2.1 Name: einops Version: 0.6.2rc0 Summary: A new flavour of
+deep learning operations Project-URL: Homepage, https://github.com/
+arogozhnikov/einops Author: Alex Rogozhnikov License: MIT License-File: LICENSE
+Keywords: deep learning,einops,machine learning,neural networks,scientific
+computations,tensor manipulation Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
+Type: text/markdown   https://user-images.githubusercontent.com/6318811/
+177030658-66f0eb5d-e136-44d8-99c9-86ae298ead5b.mp4 # einops [![Run tests]
+(https://github.com/arogozhnikov/einops/actions/workflows/run_tests.yml/
+badge.svg)](https://github.com/arogozhnikov/einops/actions/workflows/
+run_tests.yml) [![PyPI version](https://badge.fury.io/py/einops.svg)](https://
+badge.fury.io/py/einops) [![Documentation](https://img.shields.io/badge/
+documentation-link-blue.svg)](https://einops.rocks/) ![Supported python
+versions](https://raw.githubusercontent.com/arogozhnikov/einops/master/docs/
+resources/python_badge.svg) Flexible and powerful tensor operations for
+readable and reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - einops 0.6 introduces [packing and unpacking](https://
+## Recent updates: - 10'000: github reports that more than 10k project use
+einops ð - see how to use einops with [torch.compile](https://github.com/
+arogozhnikov/einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1:
+paddle backend added - einops 0.6 introduces [packing and unpacking](https://
 github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) -
 einops 0.5: einsum is now a part of einops - [Einops paper](https://
 openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR
-2022 (yes, it worth reading) - flax and oneflow backend added -
+2022 (yes, it worth reading). Talk recordings are [available](https://iclr.cc/
+virtual/2022/oral/6603)  Previous updates - flax and oneflow backend added -
 torch.jit.script is supported for pytorch layers - powerful EinMix added to
 einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/
-master/docs/3-einmix-layer.ipynb)  ## Tweets > In case you need convincing
+master/docs/3-einmix-layer.ipynb)   ## Tweets > In case you need convincing
 arguments for setting aside time to learn about einsum and einops... [Tim
 RocktÃ¤schel, FAIR](https://twitter.com/_rockt/status/1230818967205425152) >
 Writing better code with PyTorch and einops ð [Andrej Karpathy, AI at Tesla]
 (https://twitter.com/karpathy/status/1290826075916779520) > Slowly but surely,
 einops is seeping in to every nook and cranny of my code. If you find yourself
 shuffling around bazillion dimensional tensors, this might change your life
 [Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/
 1216022614755463169) [More testimonials](https://einops.rocks/pages/
-testimonials/) ## Recordings of talk at ICLR 2022 [Screen_Shot_2022-07-03_at_1
-00_15_AM] Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603)
-focused on main problems of standard tensor manipulation methods, and how
-einops improves this process. ## Contents - [Installation](#Installation) -
-[Documentation](https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-
-reference](#API) - [Why using einops](#Why-using-einops-notation) - [Supported
-frameworks](#Supported-frameworks) - [Repository](https://github.com/
+testimonials/)  ## Contents - [Installation](#Installation) - [Documentation]
+(https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-reference](#API)
+- [Why using einops](#Why-using-einops-notation) - [Supported frameworks]
+(#Supported-frameworks) - [Citing](#Citing) - [Repository](https://github.com/
 arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
 discussions) ## Installation  Plain and simple: ```bash pip install einops ```
 ## Tutorials  Tutorials are the most convenient way to see `einops` in action -
 part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
 master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
 /github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
 learning.ipynb) - part 3: [packing and unpacking](https://github.com/
@@ -46,91 +54,93 @@
 Three core operations provided ([einops tutorial](https://github.com/
 arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
 transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
 reductions) ```python from einops import rearrange, reduce, repeat # rearrange
 elements according to the pattern output_tensor = rearrange(input_tensor, 't b
 c -> b c t') # combine rearrangement and reduction output_tensor = reduce
 (input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
-a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` And
-two corresponding layers (`einops` keeps a separate version for each framework)
-with the same API. ```python from einops.layers.torch import Rearrange, Reduce
-from einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
+a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` Later
+additions to the family are `pack` and `unpack` functions (better than stack/
+split/concatenate): ```python from einops import pack, unpack # pack and unpack
+allow reversibly 'packing' multiple tensors into one. # Packed tensors may be
+of different dimensionality: packed, ps = pack([class_token_bc,
+image_tokens_bhwc, text_tokens_btc], 'b * c') class_emb_bc, image_emb_bhwc,
+text_emb_btc = unpack(transformer(packed), ps, 'b * c') ``` Finally, einops
+provides einsum with a support of multi-lettered names: ```python from einops
+import einsum, pack, unpack # einsum is like ... einsum, generic and flexible
+dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
+with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
+t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
+Mixers and similar architectures. ### Layers Einops provides layers (`einops`
+keeps a separate version for each framework) that reflect corresponding
+functions ```python from einops.layers.torch import Rearrange, Reduce from
+einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
 import Rearrange, Reduce from einops.layers.gluon import Rearrange, Reduce from
 einops.layers.keras import Rearrange, Reduce from einops.layers.chainer import
-Rearrange, Reduce ``` Layers behave similarly to operations and have the same
-parameters (with the exception of the first argument, which is passed during
-call). Example of using layers within a model: ```python # example given for
-pytorch, but code in other frameworks is almost identical from torch.nn import
-Sequential, Conv2d, MaxPool2d, Linear, ReLU from einops.layers.torch import
-Rearrange model = Sequential( ..., Conv2d(6, 16, kernel_size=5), MaxPool2d
-(kernel_size=2), # flattening without need to write forward Rearrange('b c h w
--> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear(120, 10), ) ``` Later
-additions to the family are `einsum`, `pack` and `unpack` functions: ```python
-from einops import einsum, pack, unpack # einsum is like ... einsum, generic
-and flexible dot-product # but 1) axes can be multi-lettered 2) pattern goes
-last 3) works with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head
-c -> b head t1 t2') # pack and unpack allow reversibly 'packing' multiple
-tensors into one. # Packed tensors may be of different dimensionality: packed,
-ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
-class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b
-* c') # Pack/Unpack are more convenient than concat and split, see tutorial ```
-Last, but not the least `EinMix` layer is available!
-`EinMix` is a generic linear layer, perfect for MLP Mixers and similar
-architectures. ## Naming  `einops` stands for Einstein-Inspired Notation for
-operations (though "Einstein operations" is more attractive and easier to
-remember). Notation was loosely inspired by Einstein summation (in particular
-by `numpy.einsum` operation). ## Why use `einops` notation?!  ### Semantic
-information (being verbose in expectations) ```python y = x.view(x.shape[0], -
-1) y = rearrange(x, 'b c h w -> b (c h w)') ``` While these two lines are doing
-the same job in *some* context, the second one provides information about the
-input and output. In other words, `einops` focuses on interface: *what is the
-input and output*, not *how* the output is computed. The next operation looks
-similar: ```python y = rearrange(x, 'time c h w -> time (c h w)') ``` but it
-gives the reader a hint: this is not an independent batch of images we are
-processing, but rather a sequence (video). Semantic information makes the code
-easier to read and maintain. ### Convenient checks Reconsider the same example:
-```python y = x.view(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x,
-'b c h w -> b (c h w)') ``` The second line checks that the input has four
-dimensions, but you can also specify particular dimensions. That's opposed to
-just writing comments about shapes since comments don't prevent mistakes, not
-tested, and without code review tend to be outdated ```python y = x.view
-(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b (c h
-w)', c=256, h=19, w=19) ``` ### Result is strictly determined Below we have at
-least two ways to define the depth-to-space operation ```python # depth-to-
-space rearrange(x, 'b c (h h2) (w w2) -> b (c h2 w2) h w', h2=2, w2=2)
-rearrange(x, 'b c (h h2) (w w2) -> b (h2 w2 c) h w', h2=2, w2=2) ``` There are
-at least four more ways to do it. Which one is used by the framework? These
-details are ignored, since *usually* it makes no difference, but it can make a
-big difference (e.g. if you use grouped convolutions in the next stage), and
-you'd like to specify this in your code. ### Uniformity ```python reduce(x, 'b
-c (x dx) -> b c x', 'max', dx=2) reduce(x, 'b c (x dx) (y dy) -> b c x y',
-'max', dx=2, dy=3) reduce(x, 'b c (x dx) (y dy) (z dz) -> b c x y z', 'max',
-dx=2, dy=3, dz=4) ``` These examples demonstrated that we don't use separate
-operations for 1d/2d/3d pooling, those are all defined in a uniform way. Space-
-to-depth and depth-to space are defined in many frameworks but how about width-
-to-height? Here you go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w',
-w2=2) ``` ### Framework independent behavior Even simple functions are defined
-differently by different frameworks ```python y = x.flatten() # or flatten(x)
-``` Suppose `x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy,
-chainer, pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops`
-works the same way in all frameworks. ### Independence of framework terminology
+Rearrange, Reduce ```  Example of using layers within a pytorch model ```python
+# example given for pytorch, but code in other frameworks is almost identical
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
+kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
+forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
+(120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
+from layers as those are script-able and compile-able.  ## Naming  `einops`
+stands for Einstein-Inspired Notation for operations (though "Einstein
+operations" is more attractive and easier to remember). Notation was loosely
+inspired by Einstein summation (in particular by `numpy.einsum` operation). ##
+Why use `einops` notation?!  ### Semantic information (being verbose in
+expectations) ```python y = x.view(x.shape[0], -1) y = rearrange(x, 'b c h w -
+> b (c h w)') ``` While these two lines are doing the same job in *some*
+context, the second one provides information about the input and output. In
+other words, `einops` focuses on interface: *what is the input and output*, not
+*how* the output is computed. The next operation looks similar: ```python y =
+rearrange(x, 'time c h w -> time (c h w)') ``` but it gives the reader a hint:
+this is not an independent batch of images we are processing, but rather a
+sequence (video). Semantic information makes the code easier to read and
+maintain. ### Convenient checks Reconsider the same example: ```python y =
+x.view(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b
+(c h w)') ``` The second line checks that the input has four dimensions, but
+you can also specify particular dimensions. That's opposed to just writing
+comments about shapes since comments don't prevent mistakes, not tested, and
+without code review tend to be outdated ```python y = x.view(x.shape[0], -1) #
+x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b (c h w)', c=256, h=19,
+w=19) ``` ### Result is strictly determined Below we have at least two ways to
+define the depth-to-space operation ```python # depth-to-space rearrange(x, 'b
+c (h h2) (w w2) -> b (c h2 w2) h w', h2=2, w2=2) rearrange(x, 'b c (h h2) (w
+w2) -> b (h2 w2 c) h w', h2=2, w2=2) ``` There are at least four more ways to
+do it. Which one is used by the framework? These details are ignored, since
+*usually* it makes no difference, but it can make a big difference (e.g. if you
+use grouped convolutions in the next stage), and you'd like to specify this in
+your code. ### Uniformity ```python reduce(x, 'b c (x dx) -> b c x', 'max',
+dx=2) reduce(x, 'b c (x dx) (y dy) -> b c x y', 'max', dx=2, dy=3) reduce(x, 'b
+c (x dx) (y dy) (z dz) -> b c x y z', 'max', dx=2, dy=3, dz=4) ``` These
+examples demonstrated that we don't use separate operations for 1d/2d/3d
+pooling, those are all defined in a uniform way. Space-to-depth and depth-to
+space are defined in many frameworks but how about width-to-height? Here you
+go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w', w2=2) ``` ###
+Framework independent behavior Even simple functions are defined differently by
+different frameworks ```python y = x.flatten() # or flatten(x) ``` Suppose
+`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy, chainer,
+pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
+the same way in all frameworks. ### Independence of framework terminology
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along
 width: ```python np.tile(image, (1, 2)) # in numpy image.repeat(1, 2) #
 pytorch's repeat ~ numpy's tile ``` With einops you don't need to decipher
 which axis was repeated: ```python repeat(image, 'h w -> h (tile w)', tile=2) #
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
-Testimonials provide user's perspective on the same question. ## Supported
-frameworks  Einops works with ... - [numpy](http://www.numpy.org/) - [pytorch]
-(https://pytorch.org/) - [tensorflow](https://www.tensorflow.org/) - [jax]
-(https://github.com/google/jax) - [cupy](https://cupy.chainer.org/) - [chainer]
-(https://chainer.org/) - [tf.keras](https://www.tensorflow.org/guide/keras) -
-[oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental) - [flax]
-(https://github.com/google/flax) (experimental) - [paddle](https://github.com/
-PaddlePaddle/Paddle) (experimental) - [gluon](https://gluon.mxnet.io/)
-(deprecated) ## Citing einops  Please use the following bibtex record ```text
-@inproceedings{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor
-Manipulations with Einstein-like Notation}, author={Alex Rogozhnikov},
-booktitle={International Conference on Learning Representations}, year={2022},
-url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
+[Testimonials](https://einops.rocks/pages/testimonials/) provide users'
+perspective on the same question. ## Supported frameworks  Einops works with
+... - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
+[tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
+jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
+[tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
+github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
+google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
+(experimental) - [gluon](https://gluon.mxnet.io/) (deprecated) ## Citing einops
+Please use the following bibtex record ```text @inproceedings
+{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
+with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
+{International Conference on Learning Representations}, year={2022}, url=
+{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
 versions `einops` works with python 3.7 or later.
```

### Comparing `einops-0.6.1/pyproject.toml` & `einops-0.6.2rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling>=1.10.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "einops"
 description = "A new flavour of deep learning operations"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 keywords = [
     'deep learning',
     'neural networks',
     'tensor manipulation',
     'machine learning',
     'scientific computations',
```

### Comparing `einops-0.6.1/PKG-INFO` & `einops-0.6.2rc0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: einops
-Version: 0.6.1
-Summary: A new flavour of deep learning operations
-Project-URL: Homepage, https://github.com/arogozhnikov/einops
-Author: Alex Rogozhnikov
-License: MIT
-License-File: LICENSE
-Keywords: deep learning,einops,machine learning,neural networks,scientific computations,tensor manipulation
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 
 <!--
 <a href='http://arogozhnikov.github.io/images/einops/einops_video.mp4' >
 <div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_video.gif" alt="einops package examples" />
   <br>
   <small><a href='http://arogozhnikov.github.io/images/einops/einops_video.mp4'>This video in high quality (mp4)</a></small>
@@ -40,20 +25,31 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
+- 10'000: github reports that more than 10k project use einops 🎂
+- see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
+- einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
-- [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading)
-- flax and oneflow backend added
-- torch.jit.script is supported for pytorch layers
-- powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+- [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
+  Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
+
+
+<details>
+  <summary>Previous updates</summary>
+  
+  
+  - flax and oneflow backend added
+  - torch.jit.script is supported for pytorch layers
+  - powerful EinMix added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb) 
+</details>
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
 
@@ -66,31 +62,33 @@
 [Andrej Karpathy, AI at Tesla](https://twitter.com/karpathy/status/1290826075916779520)
 
 > Slowly but surely, einops is seeping in to every nook and cranny of my code. If you find yourself shuffling around bazillion dimensional tensors, this might change your life
 [Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/1216022614755463169)
 
 [More testimonials](https://einops.rocks/pages/testimonials/)
 
+<!--
 ## Recordings of talk at ICLR 2022
 
 <a href='https://iclr.cc/virtual/2022/oral/6603'>
 <img width="922" alt="Screen Shot 2022-07-03 at 1 00 15 AM" src="https://user-images.githubusercontent.com/6318811/177030789-89d349bf-ef75-4af5-a71f-609896d1c8d9.png">
 </a>
 
 Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603) focused on main problems of standard tensor manipulation methods, and how einops improves this process.
-
+-->
 
 ## Contents
 
 - [Installation](#Installation)
 - [Documentation](https://einops.rocks/)
 - [Tutorial](#Tutorials) 
 - [API micro-reference](#API)
 - [Why using einops](#Why-using-einops-notation)
 - [Supported frameworks](#Supported-frameworks)
+- [Citing](#Citing)
 - [Repository](https://github.com/arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/discussions)
 
 ## Installation  <a name="Installation"></a>
 
 Plain and simple:
 ```bash
 pip install einops
@@ -128,64 +126,80 @@
 # rearrange elements according to the pattern
 output_tensor = rearrange(input_tensor, 't b c -> b c t')
 # combine rearrangement and reduction
 output_tensor = reduce(input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2)
 # copy along a new axis
 output_tensor = repeat(input_tensor, 'h w -> h w c', c=3)
 ```
-And two corresponding layers (`einops` keeps a separate version for each framework) with the same API.
-
-```python
-from einops.layers.torch      import Rearrange, Reduce
-from einops.layers.tensorflow import Rearrange, Reduce
-from einops.layers.flax       import Rearrange, Reduce
-from einops.layers.gluon      import Rearrange, Reduce
-from einops.layers.keras      import Rearrange, Reduce
-from einops.layers.chainer    import Rearrange, Reduce
-```
 
-Layers behave similarly to operations and have the same parameters 
-(with the exception of the first argument, which is passed during call).
+Later additions to the family are `pack` and `unpack` functions (better than stack/split/concatenate):
 
-Example of using layers within a model:
 ```python
-# example given for pytorch, but code in other frameworks is almost identical  
-from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
-from einops.layers.torch import Rearrange
-
-model = Sequential(
-    ...,
-    Conv2d(6, 16, kernel_size=5),
-    MaxPool2d(kernel_size=2),
-    # flattening without need to write forward
-    Rearrange('b c h w -> b (c h w)'),  
-    Linear(16*5*5, 120), 
-    ReLU(),
-    Linear(120, 10), 
-)
+from einops import pack, unpack
+# pack and unpack allow reversibly 'packing' multiple tensors into one.
+# Packed tensors may be of different dimensionality:
+packed,  ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
+class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b * c')
 ```
 
-Later additions to the family are `einsum`, `pack` and `unpack` functions:
+Finally, einops provides einsum with a support of multi-lettered names: 
 
 ```python
 from einops import einsum, pack, unpack
 # einsum is like ... einsum, generic and flexible dot-product 
 # but 1) axes can be multi-lettered  2) pattern goes last 3) works with multiple frameworks
 C = einsum(A, B, 'b t1 head c, b t2 head c -> b head t1 t2')
-
-# pack and unpack allow reversibly 'packing' multiple tensors into one.
-# Packed tensors may be of different dimensionality:
-packed,  ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
-class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b * c')
-# Pack/Unpack are more convenient than concat and split, see tutorial
 ```
 
-Last, but not the least `EinMix` layer is available! <br />
+### EinMix
+
 `EinMix` is a generic linear layer, perfect for MLP Mixers and similar architectures.
 
+### Layers
+
+Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
+
+```python
+from einops.layers.torch      import Rearrange, Reduce
+from einops.layers.tensorflow import Rearrange, Reduce
+from einops.layers.flax       import Rearrange, Reduce
+from einops.layers.gluon      import Rearrange, Reduce
+from einops.layers.keras      import Rearrange, Reduce
+from einops.layers.chainer    import Rearrange, Reduce
+```
+
+<details>
+  <summary>Example of using layers within a pytorch model</summary>
+  
+  
+  ```python
+  # example given for pytorch, but code in other frameworks is almost identical  
+  from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
+  from einops.layers.torch import Rearrange
+
+  model = Sequential(
+      ...,
+      Conv2d(6, 16, kernel_size=5),
+      MaxPool2d(kernel_size=2),
+      # flattening without need to write forward
+      Rearrange('b c h w -> b (c h w)'),  
+      Linear(16*5*5, 120), 
+      ReLU(),
+      Linear(120, 10), 
+  )
+  ```
+  
+  No more flatten needed! 
+  
+  Additionally, torch users will benefit from layers as those are script-able and compile-able.
+</details>
+
+
+
+
 ## Naming <a name="Naming"></a>
 
 `einops` stands for Einstein-Inspired Notation for operations 
 (though "Einstein operations" is more attractive and easier to remember).
 
 Notation was loosely inspired by Einstein summation (in particular by `numpy.einsum` operation).
 
@@ -289,15 +303,15 @@
 repeat(image, 'h w -> h (tile w)', tile=2)  # in pytorch
 repeat(image, 'h w -> h (tile w)', tile=2)  # in tf
 repeat(image, 'h w -> h (tile w)', tile=2)  # in jax
 repeat(image, 'h w -> h (tile w)', tile=2)  # in cupy
 ... (etc.)
 ```
 
-Testimonials provide user's perspective on the same question. 
+[Testimonials](https://einops.rocks/pages/testimonials/) provide users' perspective on the same question. 
 
 ## Supported frameworks <a name="Supported-frameworks"></a>
 
 Einops works with ...
 
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
@@ -307,15 +321,15 @@
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
 - [gluon](https://gluon.mxnet.io/) (deprecated)
 
-## Citing einops <a name="Contributing"></a>
+## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
     rogozhnikov2022einops,
     title={Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
```

#### html2text {}

```diff
@@ -1,48 +1,42 @@
-Metadata-Version: 2.1 Name: einops Version: 0.6.1 Summary: A new flavour of
-deep learning operations Project-URL: Homepage, https://github.com/
-arogozhnikov/einops Author: Alex Rogozhnikov License: MIT License-File: LICENSE
-Keywords: deep learning,einops,machine learning,neural networks,scientific
-computations,tensor manipulation Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
-Type: text/markdown   https://user-images.githubusercontent.com/6318811/
-177030658-66f0eb5d-e136-44d8-99c9-86ae298ead5b.mp4 # einops [![Run tests]
-(https://github.com/arogozhnikov/einops/actions/workflows/run_tests.yml/
-badge.svg)](https://github.com/arogozhnikov/einops/actions/workflows/
-run_tests.yml) [![PyPI version](https://badge.fury.io/py/einops.svg)](https://
-badge.fury.io/py/einops) [![Documentation](https://img.shields.io/badge/
-documentation-link-blue.svg)](https://einops.rocks/) ![Supported python
-versions](https://raw.githubusercontent.com/arogozhnikov/einops/master/docs/
-resources/python_badge.svg) Flexible and powerful tensor operations for
-readable and reliable code.
+   https://user-images.githubusercontent.com/6318811/177030658-66f0eb5d-e136-
+44d8-99c9-86ae298ead5b.mp4 # einops [![Run tests](https://github.com/
+arogozhnikov/einops/actions/workflows/run_tests.yml/badge.svg)](https://
+github.com/arogozhnikov/einops/actions/workflows/run_tests.yml) [![PyPI
+version](https://badge.fury.io/py/einops.svg)](https://badge.fury.io/py/einops)
+[![Documentation](https://img.shields.io/badge/documentation-link-blue.svg)]
+(https://einops.rocks/) ![Supported python versions](https://
+raw.githubusercontent.com/arogozhnikov/einops/master/docs/resources/
+python_badge.svg) Flexible and powerful tensor operations for readable and
+reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - einops 0.6 introduces [packing and unpacking](https://
+## Recent updates: - 10'000: github reports that more than 10k project use
+einops ð - see how to use einops with [torch.compile](https://github.com/
+arogozhnikov/einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1:
+paddle backend added - einops 0.6 introduces [packing and unpacking](https://
 github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) -
 einops 0.5: einsum is now a part of einops - [Einops paper](https://
 openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR
-2022 (yes, it worth reading) - flax and oneflow backend added -
+2022 (yes, it worth reading). Talk recordings are [available](https://iclr.cc/
+virtual/2022/oral/6603)  Previous updates - flax and oneflow backend added -
 torch.jit.script is supported for pytorch layers - powerful EinMix added to
 einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/einops/blob/
-master/docs/3-einmix-layer.ipynb)  ## Tweets > In case you need convincing
+master/docs/3-einmix-layer.ipynb)   ## Tweets > In case you need convincing
 arguments for setting aside time to learn about einsum and einops... [Tim
 RocktÃ¤schel, FAIR](https://twitter.com/_rockt/status/1230818967205425152) >
 Writing better code with PyTorch and einops ð [Andrej Karpathy, AI at Tesla]
 (https://twitter.com/karpathy/status/1290826075916779520) > Slowly but surely,
 einops is seeping in to every nook and cranny of my code. If you find yourself
 shuffling around bazillion dimensional tensors, this might change your life
 [Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/
 1216022614755463169) [More testimonials](https://einops.rocks/pages/
-testimonials/) ## Recordings of talk at ICLR 2022 [Screen_Shot_2022-07-03_at_1
-00_15_AM] Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603)
-focused on main problems of standard tensor manipulation methods, and how
-einops improves this process. ## Contents - [Installation](#Installation) -
-[Documentation](https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-
-reference](#API) - [Why using einops](#Why-using-einops-notation) - [Supported
-frameworks](#Supported-frameworks) - [Repository](https://github.com/
+testimonials/)  ## Contents - [Installation](#Installation) - [Documentation]
+(https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-reference](#API)
+- [Why using einops](#Why-using-einops-notation) - [Supported frameworks]
+(#Supported-frameworks) - [Citing](#Citing) - [Repository](https://github.com/
 arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
 discussions) ## Installation  Plain and simple: ```bash pip install einops ```
 ## Tutorials  Tutorials are the most convenient way to see `einops` in action -
 part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
 master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
 /github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
 learning.ipynb) - part 3: [packing and unpacking](https://github.com/
@@ -53,91 +47,93 @@
 Three core operations provided ([einops tutorial](https://github.com/
 arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
 transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
 reductions) ```python from einops import rearrange, reduce, repeat # rearrange
 elements according to the pattern output_tensor = rearrange(input_tensor, 't b
 c -> b c t') # combine rearrangement and reduction output_tensor = reduce
 (input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
-a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` And
-two corresponding layers (`einops` keeps a separate version for each framework)
-with the same API. ```python from einops.layers.torch import Rearrange, Reduce
-from einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
+a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` Later
+additions to the family are `pack` and `unpack` functions (better than stack/
+split/concatenate): ```python from einops import pack, unpack # pack and unpack
+allow reversibly 'packing' multiple tensors into one. # Packed tensors may be
+of different dimensionality: packed, ps = pack([class_token_bc,
+image_tokens_bhwc, text_tokens_btc], 'b * c') class_emb_bc, image_emb_bhwc,
+text_emb_btc = unpack(transformer(packed), ps, 'b * c') ``` Finally, einops
+provides einsum with a support of multi-lettered names: ```python from einops
+import einsum, pack, unpack # einsum is like ... einsum, generic and flexible
+dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
+with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
+t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
+Mixers and similar architectures. ### Layers Einops provides layers (`einops`
+keeps a separate version for each framework) that reflect corresponding
+functions ```python from einops.layers.torch import Rearrange, Reduce from
+einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
 import Rearrange, Reduce from einops.layers.gluon import Rearrange, Reduce from
 einops.layers.keras import Rearrange, Reduce from einops.layers.chainer import
-Rearrange, Reduce ``` Layers behave similarly to operations and have the same
-parameters (with the exception of the first argument, which is passed during
-call). Example of using layers within a model: ```python # example given for
-pytorch, but code in other frameworks is almost identical from torch.nn import
-Sequential, Conv2d, MaxPool2d, Linear, ReLU from einops.layers.torch import
-Rearrange model = Sequential( ..., Conv2d(6, 16, kernel_size=5), MaxPool2d
-(kernel_size=2), # flattening without need to write forward Rearrange('b c h w
--> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear(120, 10), ) ``` Later
-additions to the family are `einsum`, `pack` and `unpack` functions: ```python
-from einops import einsum, pack, unpack # einsum is like ... einsum, generic
-and flexible dot-product # but 1) axes can be multi-lettered 2) pattern goes
-last 3) works with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head
-c -> b head t1 t2') # pack and unpack allow reversibly 'packing' multiple
-tensors into one. # Packed tensors may be of different dimensionality: packed,
-ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b * c')
-class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed), ps, 'b
-* c') # Pack/Unpack are more convenient than concat and split, see tutorial ```
-Last, but not the least `EinMix` layer is available!
-`EinMix` is a generic linear layer, perfect for MLP Mixers and similar
-architectures. ## Naming  `einops` stands for Einstein-Inspired Notation for
-operations (though "Einstein operations" is more attractive and easier to
-remember). Notation was loosely inspired by Einstein summation (in particular
-by `numpy.einsum` operation). ## Why use `einops` notation?!  ### Semantic
-information (being verbose in expectations) ```python y = x.view(x.shape[0], -
-1) y = rearrange(x, 'b c h w -> b (c h w)') ``` While these two lines are doing
-the same job in *some* context, the second one provides information about the
-input and output. In other words, `einops` focuses on interface: *what is the
-input and output*, not *how* the output is computed. The next operation looks
-similar: ```python y = rearrange(x, 'time c h w -> time (c h w)') ``` but it
-gives the reader a hint: this is not an independent batch of images we are
-processing, but rather a sequence (video). Semantic information makes the code
-easier to read and maintain. ### Convenient checks Reconsider the same example:
-```python y = x.view(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x,
-'b c h w -> b (c h w)') ``` The second line checks that the input has four
-dimensions, but you can also specify particular dimensions. That's opposed to
-just writing comments about shapes since comments don't prevent mistakes, not
-tested, and without code review tend to be outdated ```python y = x.view
-(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b (c h
-w)', c=256, h=19, w=19) ``` ### Result is strictly determined Below we have at
-least two ways to define the depth-to-space operation ```python # depth-to-
-space rearrange(x, 'b c (h h2) (w w2) -> b (c h2 w2) h w', h2=2, w2=2)
-rearrange(x, 'b c (h h2) (w w2) -> b (h2 w2 c) h w', h2=2, w2=2) ``` There are
-at least four more ways to do it. Which one is used by the framework? These
-details are ignored, since *usually* it makes no difference, but it can make a
-big difference (e.g. if you use grouped convolutions in the next stage), and
-you'd like to specify this in your code. ### Uniformity ```python reduce(x, 'b
-c (x dx) -> b c x', 'max', dx=2) reduce(x, 'b c (x dx) (y dy) -> b c x y',
-'max', dx=2, dy=3) reduce(x, 'b c (x dx) (y dy) (z dz) -> b c x y z', 'max',
-dx=2, dy=3, dz=4) ``` These examples demonstrated that we don't use separate
-operations for 1d/2d/3d pooling, those are all defined in a uniform way. Space-
-to-depth and depth-to space are defined in many frameworks but how about width-
-to-height? Here you go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w',
-w2=2) ``` ### Framework independent behavior Even simple functions are defined
-differently by different frameworks ```python y = x.flatten() # or flatten(x)
-``` Suppose `x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy,
-chainer, pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops`
-works the same way in all frameworks. ### Independence of framework terminology
+Rearrange, Reduce ```  Example of using layers within a pytorch model ```python
+# example given for pytorch, but code in other frameworks is almost identical
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
+kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
+forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
+(120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
+from layers as those are script-able and compile-able.  ## Naming  `einops`
+stands for Einstein-Inspired Notation for operations (though "Einstein
+operations" is more attractive and easier to remember). Notation was loosely
+inspired by Einstein summation (in particular by `numpy.einsum` operation). ##
+Why use `einops` notation?!  ### Semantic information (being verbose in
+expectations) ```python y = x.view(x.shape[0], -1) y = rearrange(x, 'b c h w -
+> b (c h w)') ``` While these two lines are doing the same job in *some*
+context, the second one provides information about the input and output. In
+other words, `einops` focuses on interface: *what is the input and output*, not
+*how* the output is computed. The next operation looks similar: ```python y =
+rearrange(x, 'time c h w -> time (c h w)') ``` but it gives the reader a hint:
+this is not an independent batch of images we are processing, but rather a
+sequence (video). Semantic information makes the code easier to read and
+maintain. ### Convenient checks Reconsider the same example: ```python y =
+x.view(x.shape[0], -1) # x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b
+(c h w)') ``` The second line checks that the input has four dimensions, but
+you can also specify particular dimensions. That's opposed to just writing
+comments about shapes since comments don't prevent mistakes, not tested, and
+without code review tend to be outdated ```python y = x.view(x.shape[0], -1) #
+x: (batch, 256, 19, 19) y = rearrange(x, 'b c h w -> b (c h w)', c=256, h=19,
+w=19) ``` ### Result is strictly determined Below we have at least two ways to
+define the depth-to-space operation ```python # depth-to-space rearrange(x, 'b
+c (h h2) (w w2) -> b (c h2 w2) h w', h2=2, w2=2) rearrange(x, 'b c (h h2) (w
+w2) -> b (h2 w2 c) h w', h2=2, w2=2) ``` There are at least four more ways to
+do it. Which one is used by the framework? These details are ignored, since
+*usually* it makes no difference, but it can make a big difference (e.g. if you
+use grouped convolutions in the next stage), and you'd like to specify this in
+your code. ### Uniformity ```python reduce(x, 'b c (x dx) -> b c x', 'max',
+dx=2) reduce(x, 'b c (x dx) (y dy) -> b c x y', 'max', dx=2, dy=3) reduce(x, 'b
+c (x dx) (y dy) (z dz) -> b c x y z', 'max', dx=2, dy=3, dz=4) ``` These
+examples demonstrated that we don't use separate operations for 1d/2d/3d
+pooling, those are all defined in a uniform way. Space-to-depth and depth-to
+space are defined in many frameworks but how about width-to-height? Here you
+go: ```python rearrange(x, 'b c h (w w2) -> b c (h w2) w', w2=2) ``` ###
+Framework independent behavior Even simple functions are defined differently by
+different frameworks ```python y = x.flatten() # or flatten(x) ``` Suppose
+`x`'s shape was `(3, 4, 5)`, then `y` has shape ... - numpy, cupy, chainer,
+pytorch: `(60,)` - keras, tensorflow.layers, gluon: `(3, 20)` `einops` works
+the same way in all frameworks. ### Independence of framework terminology
 Example: `tile` vs `repeat` causes lots of confusion. To copy image along
 width: ```python np.tile(image, (1, 2)) # in numpy image.repeat(1, 2) #
 pytorch's repeat ~ numpy's tile ``` With einops you don't need to decipher
 which axis was repeated: ```python repeat(image, 'h w -> h (tile w)', tile=2) #
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
-Testimonials provide user's perspective on the same question. ## Supported
-frameworks  Einops works with ... - [numpy](http://www.numpy.org/) - [pytorch]
-(https://pytorch.org/) - [tensorflow](https://www.tensorflow.org/) - [jax]
-(https://github.com/google/jax) - [cupy](https://cupy.chainer.org/) - [chainer]
-(https://chainer.org/) - [tf.keras](https://www.tensorflow.org/guide/keras) -
-[oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental) - [flax]
-(https://github.com/google/flax) (experimental) - [paddle](https://github.com/
-PaddlePaddle/Paddle) (experimental) - [gluon](https://gluon.mxnet.io/)
-(deprecated) ## Citing einops  Please use the following bibtex record ```text
-@inproceedings{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor
-Manipulations with Einstein-like Notation}, author={Alex Rogozhnikov},
-booktitle={International Conference on Learning Representations}, year={2022},
-url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
+[Testimonials](https://einops.rocks/pages/testimonials/) provide users'
+perspective on the same question. ## Supported frameworks  Einops works with
+... - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
+[tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
+jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
+[tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
+github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
+google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
+(experimental) - [gluon](https://gluon.mxnet.io/) (deprecated) ## Citing einops
+Please use the following bibtex record ```text @inproceedings
+{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
+with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
+{International Conference on Learning Representations}, year={2022}, url=
+{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
 versions `einops` works with python 3.7 or later.
```

