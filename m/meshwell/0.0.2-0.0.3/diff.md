# Comparing `tmp/meshwell-0.0.2.tar.gz` & `tmp/meshwell-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshwell-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meshwell-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meshwell-0.0.2.tar` & `meshwell-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-06-23 20:43:34.791260 meshwell-0.0.2/LICENSE
--rw-r--r--   0        0        0     2866 2023-06-23 20:43:34.791260 meshwell-0.0.2/README.md
--rw-r--r--   0        0        0      137 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/__init__.py
--rw-r--r--   0        0        0      465 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/config.py
--rw-r--r--   0        0        0     1315 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/labeledentity.py
--rw-r--r--   0        0        0    10669 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/model.py
--rw-r--r--   0        0        0     2435 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/polysurface.py
--rw-r--r--   0        0        0     5973 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/prism.py
--rw-r--r--   0        0        0      715 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/refinement.py
--rw-r--r--   0        0        0     2220 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/tag.py
--rw-r--r--   0        0        0      527 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/validation.py
--rw-r--r--   0        0        0     3235 2023-06-23 20:43:34.799260 meshwell-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 meshwell-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 23:34:55.242387 meshwell-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2886 2023-07-04 23:34:55.242387 meshwell-0.0.3/README.md
+-rw-r--r--   0        0        0      137 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/config.py
+-rw-r--r--   0        0        0     1608 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/gmsh_entity.py
+-rw-r--r--   0        0        0     1315 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/labeledentity.py
+-rw-r--r--   0        0        0    10545 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/model.py
+-rw-r--r--   0        0        0     2180 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/polysurface.py
+-rw-r--r--   0        0        0     5694 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/prism.py
+-rw-r--r--   0        0        0      715 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/refinement.py
+-rw-r--r--   0        0        0     2220 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/tag.py
+-rw-r--r--   0        0        0      527 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/validation.py
+-rw-r--r--   0        0        0     3235 2023-07-04 23:34:55.250387 meshwell-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 meshwell-0.0.3/PKG-INFO
```

### Comparing `meshwell-0.0.2/LICENSE` & `meshwell-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.2/README.md` & `meshwell-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,24 @@
 See the documentation for more information and examples. If you encounter a big, you can make an issue so we can improve the software over time. Contributions are also welcome, see open issues for current bugs and requested features.
 
 ### Background
 
 This code was originally developed to define meshes out of the GDSII descriptions of integrated photonic circuits. A particularity of such devices is rich 2.5D topology, featuring multiple layers of smooth curves in the plane and etching profiles vertically.  Maxwell's equations (hence the name) are solved on these geometries to study how light propagates. It is also of critical interest to simulate how this is affected under other physical effects that can be resolved through finite-element or finite-volume analysis.
 
 ### Related projects
+
 * [gdsfactory](https://github.com/gdsfactory/gdsfactory): open-source plugin-rich layout software
 * [femwell](https://github.com/HelgeGehring/femwell): open-source scikit-fem based finite-element simulations, with emphasis on photonics
 * [DEVSIM](https://github.com/devsim/devsim): open-source finite-volume simulator, with emphasis on semiconductor TCAD
 
 ### Other notable GMSH Python interfaces:
+
 * [gmsh](https://gitlab.onelab.info/gmsh/gmsh): the gmsh Python API itself has significantly improved over the years
 * [pygmsh](https://github.com/meshpro/pygmsh): manipulate Python objects instead of gmsh entity tags
 * [objectgmsh](https://github.com/nemocrys/objectgmsh): class wrappers around entities
 * [gyptis](https://gyptis.gitlab.io/): uses basic gmsh for photonic geometries
 
-###
+### Acknowledgements
+
 * Simon Bilodeau (Princeton): maintainer
 * Helge Gehring (Google X): beta testing, use cases, bug fixes
 * Joaquin Matres Abril (Google X): code improvements
```

### Comparing `meshwell-0.0.2/meshwell/labeledentity.py` & `meshwell-0.0.3/meshwell/labeledentity.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.2/meshwell/model.py` & `meshwell-0.0.3/meshwell/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,39 +18,28 @@
     """Model class."""
 
     def __init__(
         self,
         point_tolerance=1e-3,
     ):
         # Initialize model
-        gmsh.clear()
+        if gmsh.is_initialized():
+            gmsh.clear()
         gmsh.initialize()
 
         # Point snapping
         self.point_tolerance = point_tolerance
 
         # CAD engine
         self.model = gmsh.model
-        self.occ = gmsh.model.occ
+        self.occ = self.model.occ
 
         # Track some gmsh entities for bottom-up volume definition
         self.points = {}
         self.segments = {}
-        # self.points_coordinates = np.empty((1,3))
-        # self.points_entities = []
-        # self.segment_coordinates =  np.empty((1,6))
-        # self.segment_entities = []
-
-    # def find_point(self, xyz):
-    #     """Returns an existing point entity if the provided point coordinates are within atol of the entity coordinates.
-
-    #     TODO
-    #     """
-    #     diffs = np.array(xyz) - self.points_coordinates
-    #     mask = np.where(diffs < self.point_tolerance)
 
     def add_get_point(self, x, y, z):
         """Add a point to the model, or reuse a previously-defined point.
         Args:
             x: float, x-coordinate
             y: float, y-coordinate
             z: float, z-coordinate
@@ -131,26 +120,28 @@
 
     def mesh(
         self,
         entities_dict: OrderedDict,
         boundaries_dict: Dict = None,
         resolutions: Optional[Dict] = None,
         default_characteristic_length: float = 0.5,
+        global_scaling: float = 1.0,
         filename: Optional[str] = None,
         verbosity: Optional[int] = 0,
         interface_delimiter: str = "___",
         boundary_delimiter: str = "None",
         finalize: bool = True,
     ):
         """Creates a GMSH mesh with proper physical tagging from a dict of {labels: list( (GMSH entity dimension, GMSH entity tag) )}.
 
         Args:
             entities_dict: OrderedDict of key: physical name, and value: meshwell entity
             resolutions (Dict): Pairs {"physical name": {"resolution": float, "distance": "float}}
             default_characteristic_length (float): if resolutions is not specified for this physical, will use this value instead
+            global_scaling: factor to scale all mesh coordinates by (e.g. 1E-6 to go from um to m)
             filename (str, path): if True, filepath where to save the mesh
             verbosity: GMSH stdout while meshing (True or False)
             interface_delimiter: string characters to use when naming interfaces between entities
             boundary_delimiter: string characters to use when defining an interface between an entity and nothing (simulation boundary)
             finalize: if True (default), finalizes the GMSH model after execution
 
         Returns:
@@ -182,14 +173,15 @@
         # Iterate through OrderedDict of entities, generating and logging the volumes/surfaces in order
         # Manually remove intersections so that BooleanFragments from removeAllDuplicates does not reassign entity tags
         final_entity_list = []
         max_dim = 0
         for index, (label, (entity_obj, keep)) in enumerate(full_entities_dict.items()):
             # First create the shape
             dimtags_out = entity_obj.instanciate()
+
             # Parse dimension
             dim = validate_dimtags(dimtags_out)
             max_dim = max(dim, max_dim)
             dimtags = unpack_dimtags(dimtags_out)
 
             # Assemble with other shapes
             base_resolution = (
@@ -217,14 +209,15 @@
                                 removeTool=False,  # Tool (previous entities) should remain untouched
                             ):
                                 current_dimtags_cut.extend(cut[0])
                             self.sync_model()
                     # Heal interfaces now that there are no volume conflicts
                     self.occ.removeAllDuplicates()
                     self.sync_model()
+                    # Make sure the most up-to-date surfaces are logged as boundaries
                     previous_entities.update_boundaries()
                 current_entities.dimtags = current_dimtags_cut
             current_entities.update_boundaries()
             final_entity_list.append(current_entities)
 
         # Tag entities, interfaces, and boundaries
         tag_entities(final_entity_list)
@@ -234,38 +227,41 @@
         tag_boundaries(
             final_entity_list, max_dim, interface_delimiter, boundary_delimiter
         )
 
         # Remove boundary entities
         for entity in final_entity_list:
             if not entity.keep:
-                gmsh.model.occ.remove(entity.dimtags, recursive=True)
+                self.model.occ.remove(entity.dimtags, recursive=True)
 
         # Perform refinement
         refinement_fields = []
         refinement_index = 0
         refinement_fields_constant, refinement_index = constant_refinement(
             final_entity_list, refinement_field_index=0, model=self.model
         )
         refinement_fields.extend(refinement_fields_constant)
 
         # Use the smallest element size overall
-        gmsh.model.mesh.field.add("Min", refinement_index)
-        gmsh.model.mesh.field.setNumbers(
+        self.model.mesh.field.add("Min", refinement_index)
+        self.model.mesh.field.setNumbers(
             refinement_index, "FieldsList", refinement_fields
         )
-        gmsh.model.mesh.field.setAsBackgroundMesh(refinement_index)
+        self.model.mesh.field.setAsBackgroundMesh(refinement_index)
 
         # Turn off default meshing options
-        gmsh.model.mesh.MeshSizeFromPoints = 0
-        gmsh.model.mesh.MeshSizeFromCurvature = 0
-        gmsh.model.mesh.MeshSizeExtendFromBoundary = 0
+        self.model.mesh.MeshSizeFromPoints = 0
+        self.model.mesh.MeshSizeFromCurvature = 0
+        self.model.mesh.MeshSizeExtendFromBoundary = 0
+
+        # Global resizing
+        gmsh.option.setNumber("Mesh.ScalingFactor", global_scaling)
 
         self.occ.synchronize()
-        gmsh.model.mesh.generate(max_dim)
+        self.model.mesh.generate(max_dim)
 
         if filename:
             gmsh.write(f"{filename}")
 
         with contextlib.redirect_stdout(None):
             with tempfile.TemporaryDirectory() as tmpdirname:
                 gmsh.write(f"{tmpdirname}/mesh.msh")
```

### Comparing `meshwell-0.0.2/meshwell/polysurface.py` & `meshwell-0.0.3/meshwell/polysurface.py`

 * *Files 25% similar despite different names*

```diff
@@ -57,17 +57,7 @@
             exterior = exterior[0][0][1]  # Parse `outDimTags', `outDimTagsMap'
         return exterior
 
     def instanciate(self):
         polysurface = self.get_gmsh_polygons()
         self.model.occ.synchronize()
         return [(2, polysurface)]
-
-
-# def PolySurface(
-#     polygons,
-#     model,
-# ):
-#     """Functional wrapper around PolySurfaceClass."""
-#     polysurface = PolySurfaceClass(polygons=polygons, model=model).get_gmsh_polygons()
-#     model.occ.synchronize()
-#     return polysurface
```

### Comparing `meshwell-0.0.2/meshwell/prism.py` & `meshwell-0.0.3/meshwell/prism.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,20 +145,7 @@
         return exterior
 
     def instanciate(self):
         """Returns dim tag from entity."""
         prism = self.get_gmsh_volumes()
         self.model.occ.synchronize()
         return [(3, prism)]
-
-
-# def Prism(
-#     polygons,
-#     model,
-#     buffers=None,
-# ):
-#     """Functional wrapper around PrismClass."""
-#     prism = PrismClass(
-#         polygons=polygons, buffers=buffers, model=model
-#     ).get_gmsh_volumes()
-#     model.occ.synchronize()
-#     return prism
```

### Comparing `meshwell-0.0.2/meshwell/refinement.py` & `meshwell-0.0.3/meshwell/refinement.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.2/meshwell/tag.py` & `meshwell-0.0.3/meshwell/tag.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.2/meshwell/validation.py` & `meshwell-0.0.3/meshwell/validation.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.2/pyproject.toml` & `meshwell-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version="0.0.2"
+version="0.0.3"
 authors = [
     {name = "Simon Bilodeau", email = "sb30@princeton.edu"},
 ]
 keywords = ["python"]
 license = {file = "LICENSE"}
 dependencies = [
     "shapely",
```

### Comparing `meshwell-0.0.2/PKG-INFO` & `meshwell-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshwell
-Version: 0.0.2
+Version: 0.0.3
 Summary: GMSH wrapper, with integrated photonics focus
 Keywords: python
 Author-email: Simon Bilodeau <sb30@princeton.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -64,22 +64,25 @@
 See the documentation for more information and examples. If you encounter a big, you can make an issue so we can improve the software over time. Contributions are also welcome, see open issues for current bugs and requested features.
 
 ### Background
 
 This code was originally developed to define meshes out of the GDSII descriptions of integrated photonic circuits. A particularity of such devices is rich 2.5D topology, featuring multiple layers of smooth curves in the plane and etching profiles vertically.  Maxwell's equations (hence the name) are solved on these geometries to study how light propagates. It is also of critical interest to simulate how this is affected under other physical effects that can be resolved through finite-element or finite-volume analysis.
 
 ### Related projects
+
 * [gdsfactory](https://github.com/gdsfactory/gdsfactory): open-source plugin-rich layout software
 * [femwell](https://github.com/HelgeGehring/femwell): open-source scikit-fem based finite-element simulations, with emphasis on photonics
 * [DEVSIM](https://github.com/devsim/devsim): open-source finite-volume simulator, with emphasis on semiconductor TCAD
 
 ### Other notable GMSH Python interfaces:
+
 * [gmsh](https://gitlab.onelab.info/gmsh/gmsh): the gmsh Python API itself has significantly improved over the years
 * [pygmsh](https://github.com/meshpro/pygmsh): manipulate Python objects instead of gmsh entity tags
 * [objectgmsh](https://github.com/nemocrys/objectgmsh): class wrappers around entities
 * [gyptis](https://gyptis.gitlab.io/): uses basic gmsh for photonic geometries
 
-###
+### Acknowledgements
+
 * Simon Bilodeau (Princeton): maintainer
 * Helge Gehring (Google X): beta testing, use cases, bug fixes
 * Joaquin Matres Abril (Google X): code improvements
```

