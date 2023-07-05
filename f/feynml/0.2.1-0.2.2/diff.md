# Comparing `tmp/feynml-0.2.1.tar.gz` & `tmp/feynml-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.2.1.tar", max compression
+gzip compressed data, was "feynml-0.2.2.tar", max compression
```

## Comparing `feynml-0.2.1.tar` & `feynml-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35149 2023-05-29 19:03:34.181465 feynml-0.2.1/LICENSE
--rw-r--r--   0        0        0     2359 2023-05-29 19:03:34.181465 feynml-0.2.1/README.md
--rw-r--r--   0        0        0      179 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/__init__.py
--rw-r--r--   0        0        0      986 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/connector.py
--rw-r--r--   0        0        0     5497 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     3116 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/feynml.py
--rw-r--r--   0        0        0     2959 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/head.py
--rw-r--r--   0        0        0      651 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/id.py
--rw-r--r--   0        0        0        0 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/__init__.py
--rw-r--r--   0        0        0     1863 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/fermion.py
--rw-r--r--   0        0        0     1843 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/feynmangraph.py
--rw-r--r--   0        0        0      612 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/field.py
--rw-r--r--   0        0        0     3443 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/insertions.py
--rw-r--r--   0        0        0      129 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/particle.py
--rw-r--r--   0        0        0     2384 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/propagator.py
--rw-r--r--   0        0        0     1729 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/rule.py
--rw-r--r--   0        0        0      635 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/sequenceform.py
--rw-r--r--   0        0        0     2429 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/topology.py
--rw-r--r--   0        0        0     7356 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/topologylist.py
--rw-r--r--   0        0        0     1427 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/vector.py
--rw-r--r--   0        0        0      896 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/formcalc/vertex.py
--rw-r--r--   0        0        0     2641 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     4694 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/lhe.py
--rw-r--r--   0        0        0     1569 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/interface/qgraf.py
--rw-r--r--   0        0        0      260 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/labeled.py
--rw-r--r--   0        0        0     1035 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/line.py
--rw-r--r--   0        0        0      290 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/link.py
--rw-r--r--   0        0        0      294 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/meta.py
--rw-r--r--   0        0        0      563 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/particles.py
--rw-r--r--   0        0        0     3115 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/point.py
--rw-r--r--   0        0        0      207 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/propagator.py
--rw-r--r--   0        0        0      349 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/shape.py
--rw-r--r--   0        0        0     7878 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/sheet.py
--rw-r--r--   0        0        0      363 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/sourcing.py
--rw-r--r--   0        0        0     2804 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/styled.py
--rw-r--r--   0        0        0      364 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/targeting.py
--rw-r--r--   0        0        0      780 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/type.py
--rw-r--r--   0        0        0     1608 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/util.py
--rw-r--r--   0        0        0      425 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/vertex.py
--rw-r--r--   0        0        0      756 2023-05-29 19:03:34.181465 feynml-0.2.1/feynml/xml.py
--rw-r--r--   0        0        0     1893 2023-05-29 19:03:35.821460 feynml-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 feynml-0.2.1/setup.py
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-05 11:23:18.656151 feynml-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2359 2023-07-05 11:23:18.656151 feynml-0.2.2/README.md
+-rw-r--r--   0        0        0      179 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/connector.py
+-rw-r--r--   0        0        0     5497 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     2764 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/feynml.py
+-rw-r--r--   0        0        0     2669 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/head.py
+-rw-r--r--   0        0        0      651 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/fermion.py
+-rw-r--r--   0        0        0     1843 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/feynmangraph.py
+-rw-r--r--   0        0        0      612 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/field.py
+-rw-r--r--   0        0        0     3366 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/insertions.py
+-rw-r--r--   0        0        0      129 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/particle.py
+-rw-r--r--   0        0        0     2384 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/propagator.py
+-rw-r--r--   0        0        0     1729 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/rule.py
+-rw-r--r--   0        0        0      635 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/sequenceform.py
+-rw-r--r--   0        0        0     2392 2023-07-05 11:23:18.656151 feynml-0.2.2/feynml/interface/formcalc/topology.py
+-rw-r--r--   0        0        0     7319 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/topologylist.py
+-rw-r--r--   0        0        0     1427 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/vector.py
+-rw-r--r--   0        0        0      840 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/formcalc/vertex.py
+-rw-r--r--   0        0        0     2641 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     4694 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/lhe.py
+-rw-r--r--   0        0        0     1569 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0      260 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/line.py
+-rw-r--r--   0        0        0      290 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/link.py
+-rw-r--r--   0        0        0      288 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/meta.py
+-rw-r--r--   0        0        0      563 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/particles.py
+-rw-r--r--   0        0        0     3776 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/propagator.py
+-rw-r--r--   0        0        0      349 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/shape.py
+-rw-r--r--   0        0        0     7878 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/sheet.py
+-rw-r--r--   0        0        0      363 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/sourcing.py
+-rw-r--r--   0        0        0     2804 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/targeting.py
+-rw-r--r--   0        0        0      780 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/type.py
+-rw-r--r--   0        0        0     1339 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/util.py
+-rw-r--r--   0        0        0      425 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/vertex.py
+-rw-r--r--   0        0        0      730 2023-07-05 11:23:18.660151 feynml-0.2.2/feynml/xml.py
+-rw-r--r--   0        0        0     1874 2023-07-05 11:23:21.400152 feynml-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 feynml-0.2.2/setup.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.2/PKG-INFO
```

### Comparing `feynml-0.2.1/LICENSE` & `feynml-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/README.md` & `feynml-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/connector.py` & `feynml-0.2.2/feynml/connector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/feynmandiagram.py` & `feynml-0.2.2/feynml/feynmandiagram.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/feynml.py` & `feynml-0.2.2/feynml/feynml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import logging
 import os
 import warnings
 from dataclasses import dataclass, field
 from importlib.metadata import version
 from typing import List, Optional
 
-import cssutils
 import smpl_io.io as io
-from smpl_doc import doc
-from xsdata.formats.dataclass.parsers import XmlParser
-from xsdata.formats.dataclass.serializers import XmlSerializer
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.head import Head
 from feynml.id import Identifiable
 from feynml.meta import Meta
 from feynml.sheet import SheetHandler
 from feynml.styled import CSSSheet
 from feynml.xml import XML
 
-# We don't want to see the cssutils warnings, since we have custom properties
-cssutils.log.setLevel(logging.CRITICAL)
-
-
 feynml_version = version("feynml")
 
 
 @dataclass
 class FeynML(SheetHandler, XML):
     class Meta:
         name = "feynml"
```

### Comparing `feynml-0.2.1/feynml/head.py` & `feynml-0.2.2/feynml/head.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import logging
 import warnings
 from dataclasses import dataclass, field
 from importlib.metadata import version
-from typing import List, Optional, Union
+from typing import List, Optional
 
 import cssutils
 import smpl_io.io as io
-from cssselect import GenericTranslator, SelectorError
-from lxml import etree
 
-from feynml.id import Identifiable
-from feynml.leg import Leg
 from feynml.link import Link
 from feynml.meta import Meta as alias_meta
-from feynml.propagator import Propagator
 from feynml.sheet import SheetHandler
 from feynml.styled import CSSSheet, Styled
-from feynml.type import get_default_sheet
-from feynml.vertex import Vertex
-from feynml.xml import XML
 
 
 @dataclass
 class Head(SheetHandler):
     class Meta:
         name = "head"
```

### Comparing `feynml-0.2.1/feynml/id.py` & `feynml-0.2.2/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/fermion.py` & `feynml-0.2.2/feynml/interface/formcalc/fermion.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/feynmangraph.py` & `feynml-0.2.2/feynml/interface/formcalc/feynmangraph.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/field.py` & `feynml-0.2.2/feynml/interface/formcalc/field.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/insertions.py` & `feynml-0.2.2/feynml/interface/formcalc/insertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 from dataclasses import dataclass
 from typing import List
 
 from feynml.interface.formcalc.feynmangraph import FeynmanGraph
 from feynml.interface.formcalc.field import Field
-from feynml.interface.formcalc.rule import Rule
-from feynml.pdgid import PDG
 
 
 @dataclass
 class Insertions:
     generic: FeynmanGraph
     classes: FeynmanGraph
```

### Comparing `feynml-0.2.1/feynml/interface/formcalc/propagator.py` & `feynml-0.2.2/feynml/interface/formcalc/propagator.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     f: Field
 
     def to_feynml(self, insertions: Insertions) -> Tuple[Connector, List[Vertex]]:
         if self.type == "Internal":
             fmlv1 = self.v1.to_feynml()
             fmlv2 = self.v2.to_feynml()
             return FMLPropagator(
-                source=fmlv1.id, target=fmlv2.id, pdgid=insertions.get_pdgid(self.f)
+                source=fmlv2.id, target=fmlv1.id, pdgid=insertions.get_pdgid(self.f)
             ), [fmlv1, fmlv2]
         elif self.type == "Incoming":
             fmlv1 = self.v1.to_feynml()
             fmlv2 = self.v2.to_feynml()
             return FMLLeg(
                 target=fmlv2.id, sense="incoming", pdgid=insertions.get_pdgid(self.f)
             ), [fmlv2]
```

### Comparing `feynml-0.2.1/feynml/interface/formcalc/rule.py` & `feynml-0.2.2/feynml/interface/formcalc/rule.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/sequenceform.py` & `feynml-0.2.2/feynml/interface/formcalc/sequenceform.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/topology.py` & `feynml-0.2.2/feynml/interface/formcalc/topology.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from dataclasses import dataclass
 from typing import List
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.interface.formcalc.insertions import Insertions
 from feynml.interface.formcalc.propagator import Propagator
-from feynml.util import len_not_none
 
 
 @dataclass
 class Topology:
     order: int
     propagators: List[Propagator]
```

### Comparing `feynml-0.2.1/feynml/interface/formcalc/topologylist.py` & `feynml-0.2.2/feynml/interface/formcalc/topologylist.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import List, Tuple
 
 from feynml.feynml import FeynML
 from feynml.head import Head
 from feynml.interface.formcalc.insertions import Insertions
 from feynml.interface.formcalc.topology import Topology
 from feynml.meta import Meta
-from feynml.util import len_not_none
 
 
 @dataclass
 class TopologyList:
     rest: str
     topologies: List[Tuple[Topology, Insertions]]
```

### Comparing `feynml-0.2.1/feynml/interface/formcalc/vector.py` & `feynml-0.2.2/feynml/interface/formcalc/vector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/formcalc/vertex.py` & `feynml-0.2.2/feynml/interface/formcalc/vertex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from dataclasses import dataclass
 
-from feynml.interface.formcalc.particle import Particle
 from feynml.vertex import Vertex as FMLVertex
 
 
 @dataclass
 class Vertex:
     i: int
     j: int
```

### Comparing `feynml-0.2.1/feynml/interface/hepmc.py` & `feynml-0.2.2/feynml/interface/hepmc.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/lhe.py` & `feynml-0.2.2/feynml/interface/lhe.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/interface/qgraf.py` & `feynml-0.2.2/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/leg.py` & `feynml-0.2.2/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/momentum.py` & `feynml-0.2.2/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/particles.py` & `feynml-0.2.2/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/point.py` & `feynml-0.2.2/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/sheet.py` & `feynml-0.2.2/feynml/sheet.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/styled.py` & `feynml-0.2.2/feynml/styled.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/type.py` & `feynml-0.2.2/feynml/type.py`

 * *Files identical despite different names*

### Comparing `feynml-0.2.1/feynml/xml.py` & `feynml-0.2.2/feynml/xml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-
 import smpl_io.io as io
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 
 class XML:
```

### Comparing `feynml-0.2.1/pyproject.toml` & `feynml-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [tool.poetry]
 name = "feynml"
-version = "0.2.1"
+version = "0.2.2"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 particle = "*"
 xsdata = {version = "*", extras = ["cli","lxml","soap"]}
 cssutils= "*"
 cssselect ="*"
-#pyqgraf = {path= "../pyqgraf", develop = true }
-#ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 smpl_io = "^1.1.2"
 #smpl_io = {path= "../smpl_io", develop = true}
 smpl_doc = "^1.1.3"
 #smpl_doc = {path= "../smpl_doc", develop = true}
 smpl_util= "*"
 
 pyqgraf = {version = ">=0.0.3", optional = true}
+#pyqgraf = {path= "../pyqgraf", develop = true }
 pyhepmc = {version = "*", optional = true}
 pylhe = {version = "*", optional = true}
 
 [tool.poetry.extras]
 interfaces = ["pyqgraf", "pyhepmc", "pylhe"]
 
 [tool.poetry.group.test]
@@ -44,15 +43,15 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.23.0"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.25.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `feynml-0.2.1/setup.py` & `feynml-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
 {'interfaces': ['pyqgraf>=0.0.3', 'pyhepmc', 'pylhe']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.2.1/PKG-INFO` & `feynml-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

