# Comparing `tmp/feynml-0.2.2.tar.gz` & `tmp/feynml-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.2.2.tar", max compression
+gzip compressed data, was "feynml-0.2.3.tar", max compression
```

## Comparing `feynml-0.2.2.tar` & `feynml-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35149 2023-07-05 11:23:18.656151 feynml-0.2.2/LICENSE
--rw-r--r--   0        0        0     2359 2023-07-05 11:23:18.656151 feynml-0.2.2/README.md
--rw-r--r--   0        0        0      179 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/__init__.py
--rw-r--r--   0        0        0      986 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/connector.py
--rw-r--r--   0        0        0     5497 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     2764 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/feynml.py
--rw-r--r--   0        0        0     2669 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/head.py
--rw-r--r--   0        0        0      651 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/id.py
--rw-r--r--   0        0        0        0 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/__init__.py
--rw-r--r--   0        0        0     1863 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/fermion.py
--rw-r--r--   0        0        0     1843 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/feynmangraph.py
--rw-r--r--   0        0        0      612 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/field.py
--rw-r--r--   0        0        0     3366 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/insertions.py
--rw-r--r--   0        0        0      129 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/particle.py
--rw-r--r--   0        0        0     2384 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/propagator.py
--rw-r--r--   0        0        0     1729 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/rule.py
--rw-r--r--   0        0        0      635 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/sequenceform.py
--rw-r--r--   0        0        0     2392 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/topology.py
--rw-r--r--   0        0        0     7319 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/topologylist.py
--rw-r--r--   0        0        0     1427 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/vector.py
--rw-r--r--   0        0        0      840 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/vertex.py
--rw-r--r--   0        0        0     2641 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     4694 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/lhe.py
--rw-r--r--   0        0        0     1569 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/qgraf.py
--rw-r--r--   0        0        0      260 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/labeled.py
--rw-r--r--   0        0        0     1035 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/line.py
--rw-r--r--   0        0        0      290 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/link.py
--rw-r--r--   0        0        0      288 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/meta.py
--rw-r--r--   0        0        0      563 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/particles.py
--rw-r--r--   0        0        0     3776 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/point.py
--rw-r--r--   0        0        0      207 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/propagator.py
--rw-r--r--   0        0        0      349 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/shape.py
--rw-r--r--   0        0        0     7878 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/sheet.py
--rw-r--r--   0        0        0      363 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/sourcing.py
--rw-r--r--   0        0        0     2804 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/styled.py
--rw-r--r--   0        0        0      364 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/targeting.py
--rw-r--r--   0        0        0      780 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/type.py
--rw-r--r--   0        0        0     1339 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/util.py
--rw-r--r--   0        0        0      425 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/vertex.py
--rw-r--r--   0        0        0      730 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/xml.py
--rw-r--r--   0        0        0     1874 2023-07-05 11:23:21.400152 feynml-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 feynml-0.2.2/setup.py
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-05 11:27:51.299803 feynml-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2359 2023-07-05 11:27:51.299803 feynml-0.2.3/README.md
+-rw-r--r--   0        0        0      179 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/connector.py
+-rw-r--r--   0        0        0     5361 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     2764 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/feynml.py
+-rw-r--r--   0        0        0     2669 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/head.py
+-rw-r--r--   0        0        0      651 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/fermion.py
+-rw-r--r--   0        0        0     1843 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/feynmangraph.py
+-rw-r--r--   0        0        0      612 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/field.py
+-rw-r--r--   0        0        0     3366 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/insertions.py
+-rw-r--r--   0        0        0      129 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/particle.py
+-rw-r--r--   0        0        0     2384 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/propagator.py
+-rw-r--r--   0        0        0     1729 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/rule.py
+-rw-r--r--   0        0        0      635 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/sequenceform.py
+-rw-r--r--   0        0        0     2392 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/topology.py
+-rw-r--r--   0        0        0     7319 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/topologylist.py
+-rw-r--r--   0        0        0     1427 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/vector.py
+-rw-r--r--   0        0        0      840 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/formcalc/vertex.py
+-rw-r--r--   0        0        0     2641 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     4694 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/lhe.py
+-rw-r--r--   0        0        0     1569 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0      260 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/line.py
+-rw-r--r--   0        0        0      290 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/link.py
+-rw-r--r--   0        0        0      288 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/meta.py
+-rw-r--r--   0        0        0      563 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/particles.py
+-rw-r--r--   0        0        0     3776 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/propagator.py
+-rw-r--r--   0        0        0      349 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/shape.py
+-rw-r--r--   0        0        0     7878 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/sheet.py
+-rw-r--r--   0        0        0      363 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/sourcing.py
+-rw-r--r--   0        0        0     2804 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/targeting.py
+-rw-r--r--   0        0        0      780 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/type.py
+-rw-r--r--   0        0        0     1339 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/util.py
+-rw-r--r--   0        0        0      425 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/vertex.py
+-rw-r--r--   0        0        0      730 2023-07-05 11:27:51.299803 feynml-0.2.3/feynml/xml.py
+-rw-r--r--   0        0        0     1874 2023-07-05 11:27:53.703941 feynml-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 feynml-0.2.3/setup.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.3/PKG-INFO
```

### Comparing `feynml-0.2.2/LICENSE` & `feynml-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/README.md` & `feynml-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/connector.py` & `feynml-0.2.3/feynml/connector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/feynmandiagram.py` & `feynml-0.2.3/feynml/feynmandiagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,22 +147,20 @@
     @doc.append_doc(Head.get_style)
     def get_style(self, obj, xml: XML = None) -> cssutils.css.CSSStyleDeclaration:
         if self.parent_fml is not None:
             return super().get_style(obj, self.parent_fml)
         elif xml is not None:
             return super().get_style(obj, xml)
         else:
-            warnings.warn("No parent fml, returning default style")
             return super().get_style(obj, self)
 
     def get_sheets(self):
         if self.parent_fml is not None:
             return self.parent_fml.get_sheets() + [self.sheet]
         else:
-            warnings.warn("No parent fml, returning default sheet")
             return super().get_sheets() + [self.sheet]
 
     def get_sheet(self):
         return self.sheet
 
     def with_sheet(self, sheet):
         self.sheet = sheet
```

### Comparing `feynml-0.2.2/feynml/feynml.py` & `feynml-0.2.3/feynml/feynml.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/head.py` & `feynml-0.2.3/feynml/head.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/id.py` & `feynml-0.2.3/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/fermion.py` & `feynml-0.2.3/feynml/interface/formcalc/fermion.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/feynmangraph.py` & `feynml-0.2.3/feynml/interface/formcalc/feynmangraph.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/field.py` & `feynml-0.2.3/feynml/interface/formcalc/field.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/insertions.py` & `feynml-0.2.3/feynml/interface/formcalc/insertions.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/propagator.py` & `feynml-0.2.3/feynml/interface/formcalc/propagator.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/rule.py` & `feynml-0.2.3/feynml/interface/formcalc/rule.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/sequenceform.py` & `feynml-0.2.3/feynml/interface/formcalc/sequenceform.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/topology.py` & `feynml-0.2.3/feynml/interface/formcalc/topology.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/topologylist.py` & `feynml-0.2.3/feynml/interface/formcalc/topologylist.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/vector.py` & `feynml-0.2.3/feynml/interface/formcalc/vector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/formcalc/vertex.py` & `feynml-0.2.3/feynml/interface/formcalc/vertex.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/hepmc.py` & `feynml-0.2.3/feynml/interface/hepmc.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/lhe.py` & `feynml-0.2.3/feynml/interface/lhe.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/interface/qgraf.py` & `feynml-0.2.3/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/leg.py` & `feynml-0.2.3/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/momentum.py` & `feynml-0.2.3/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/particles.py` & `feynml-0.2.3/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/pdgid.py` & `feynml-0.2.3/feynml/pdgid.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/point.py` & `feynml-0.2.3/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/sheet.py` & `feynml-0.2.3/feynml/sheet.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/styled.py` & `feynml-0.2.3/feynml/styled.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/type.py` & `feynml-0.2.3/feynml/type.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/util.py` & `feynml-0.2.3/feynml/util.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/feynml/xml.py` & `feynml-0.2.3/feynml/xml.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.2/pyproject.toml` & `feynml-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynml"
-version = "0.2.2"
+version = "0.2.3"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynml-0.2.2/setup.py` & `feynml-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
 {'interfaces': ['pyqgraf>=0.0.3', 'pyhepmc', 'pylhe']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.2.2/PKG-INFO` & `feynml-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.2.2
+Version: 0.2.3
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

