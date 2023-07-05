# Comparing `tmp/nebula-dgl-0.1.1.tar.gz` & `tmp/nebula-dgl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebula-dgl-0.1.1.tar", last modified: Thu Nov 17 03:05:56 2022, max compression
+gzip compressed data, was "nebula-dgl-0.1.2.tar", last modified: Wed Jul  5 07:05:09 2023, max compression
```

## Comparing `nebula-dgl-0.1.1.tar` & `nebula-dgl-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0 weyl       (501) staff       (20)    11357 2022-07-11 07:09:01.395116 nebula-dgl-0.1.1/LICENSE
--rw-r--r--   0 weyl       (501) staff       (20)     4181 2022-11-17 02:58:47.344518 nebula-dgl-0.1.1/README.md
--rw-r--r--   0 weyl       (501) staff       (20)      277 2022-07-11 08:29:42.072507 nebula-dgl-0.1.1/nebula_dgl/__init__.py
--rw-r--r--   0 weyl       (501) staff       (20)       32 2022-07-27 03:56:23.462477 nebula-dgl-0.1.1/nebula_dgl/nebula_exporter.py
--rw-r--r--   0 weyl       (501) staff       (20)    22285 2022-07-26 09:28:54.520265 nebula-dgl-0.1.1/nebula_dgl/nebula_loader.py
--rw-r--r--   0 weyl       (501) staff       (20)      399 2022-11-17 02:58:47.345507 nebula-dgl-0.1.1/pyproject.toml
--rw-r--r--   0 weyl       (501) staff       (20)     1698 2022-07-19 01:34:21.315725 nebula-dgl-0.1.1/tests/unit/nebula_loader.py
--rw-------   0 weyl       (501) staff       (20)     4411 2022-11-17 03:05:56.457165 nebula-dgl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-11 07:09:01.395116 nebula-dgl-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5311 2023-07-05 07:01:37.675409 nebula-dgl-0.1.2/README.md
+-rw-r--r--   0        0        0      452 2023-07-02 08:13:50.469496 nebula-dgl-0.1.2/nebula_dgl/__init__.py
+-rw-r--r--   0        0        0       32 2022-07-27 03:56:23.462477 nebula-dgl-0.1.2/nebula_dgl/nebula_exporter.py
+-rw-r--r--   0        0        0    32934 2023-07-05 07:01:33.847247 nebula-dgl-0.1.2/nebula_dgl/nebula_loader.py
+-rw-r--r--   0        0        0     9428 2023-07-05 07:01:33.847848 nebula-dgl-0.1.2/nebula_dgl/nebula_part_loader.py
+-rw-r--r--   0        0        0    16691 2023-07-02 08:13:50.470137 nebula-dgl-0.1.2/nebula_dgl/nebula_reduced_loader.py
+-rw-r--r--   0        0        0      398 2023-07-05 07:01:37.676166 nebula-dgl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1698 2022-07-19 01:34:21.315725 nebula-dgl-0.1.2/tests/unit/nebula_loader.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 nebula-dgl-0.1.2/PKG-INFO
```

### Comparing `nebula-dgl-0.1.1/LICENSE` & `nebula-dgl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nebula-dgl-0.1.1/README.md` & `nebula-dgl-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,37 @@
+Metadata-Version: 2.1
+Name: nebula-dgl
+Version: 0.1.2
+Summary: Lib for NebulaGraph integration with Deep Graph Library (DGL).
+License: Apache-2.0
+Author-email: Wey Gu <weyl.gu@gmail.com>
+Description-Content-Type: text/markdown
+
 # nebula-dgl
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
 
 nebula-dgl is the Lib for Nebula Graph integration with Deep Graph Library (DGL).
 
 > nebula-dgl is still WIP, there is a demo project [here](https://github.com/wey-gu/NebulaGraph-Fraud-Detection-GNN/) .
 
 # Guide
 
 ## Installation
 
+### Install from PyPi
+
+```bash
+python3 -m pip install nebula-dgl
+python3 -m pip install dgl dglgo -f https://data.dgl.ai/wheels/repo.html
+```
+
+### Install from codebase for dev
 ```bash
-# this is needed until nebula-python release to fix storageclient issue by including https://github.com/vesoft-inc/nebula-python/pull/219
-python3 -m pip install nebula3-python==3.3.0
+python3 -m pip install nebula3-python
 python3 -m pip install dgl dglgo -f https://data.dgl.ai/wheels/repo.html
 
 # build and install
 python3 -m pip install .
 ```
 
 ## Playground
@@ -94,14 +109,21 @@
 
 with open('example/homogeneous_graph.yaml', 'r') as f:
     feature_mapper = yaml.safe_load(f)
 
 nebula_loader = NebulaLoader(nebula_config, feature_mapper)
 homo_dgl_graph = nebula_loader.load()
 
+# or query based
+query = """
+MATCH p=()-[:follow]->() RETURN p
+"""
+nebula_loader = NebulaLoader(nebula_config, feature_mapper, query=query, query_space="basketballplayer")
+homo_dgl_graph = nebula_loader.load()
+
 nx_g = homo_dgl_graph.to_networkx()
 nx.draw(nx_g, with_labels=True, pos=nx.spring_layout(nx_g))
 ```
 
 Result:
 
 ![nx_draw](https://user-images.githubusercontent.com/1651790/181154556-c25532f9-33ff-4cc8-85d9-62cb559d7f1a.png)
@@ -210,7 +232,40 @@
 
 # get degree
 networkx.degree(nx_g)
 
 # get degree centrality
 networkx.degree_centrality(nx_g)
 ```
+
+
+## Multi-Part Loader for Nebula Graph
+
+1. For now, the Multi-Part Loader is slow like sequence scan, need to profile the performance.
+
+```python
+import yaml
+import networkx as nx
+import matplotlib.pyplot as plt
+
+from nebula_dgl import NebulaReducedLoader
+
+
+nebula_config = {
+    "graph_hosts": [
+                ('127.0.0.1', 9669)
+            ],
+    "nebula_user": "root",
+    "nebula_password": "nebula",
+}
+
+with open('example/homogeneous_graph.yaml', 'r') as f:
+    feature_mapper = yaml.safe_load(f)
+
+# you only need change the following line: from NebulaLoader to NebulaReducedLoader
+# Easy for you to use the multi-part loader 
+nebula_reduced_loader = NebulaReducedLoader(nebula_config, feature_mapper)
+homo_dgl_graph = nebula_reduced_loader.load()
+nx_g = homo_dgl_graph.to_networkx()
+nx.draw(nx_g, with_labels=True, pos=nx.spring_layout(nx_g))
+plt.savefig("multi_graph.png")
+```
```

### Comparing `nebula-dgl-0.1.1/nebula_dgl/nebula_loader.py` & `nebula-dgl-0.1.2/nebula_dgl/nebula_reduced_loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 from nebula3.sclient.GraphStorageClient import GraphStorageClient
 from nebula3.gclient.net import ConnectionPool
 from nebula3.Config import Config as NebulaConfig
 from nebula3.common import ttypes
 
 from dgl import DGLHeteroGraph, heterograph
 from torch import tensor
+from concurrent.futures import ThreadPoolExecutor
 
-from typing import Dict, List, Callable
+from typing import Dict
 
 import logging
 
+from nebula_dgl.nebula_part_loader import NebulaPartLoader
 
 VALID_FILTERS = ['function', 'enumeration', 'value']
 logger = logging.getLogger(__package__)
-ENUMERATION_DEFAULT_VALUE = -1
-NEBULA_TYPE_MAP = {
-    "int": "as_int",
-    "double": "as_double",
-    "str": "as_string",
-    "float": "as_double",
-}
 
 
-class NebulaLoader():
+class NebulaReducedLoader():
     """
-    NebulaLoader is a class that loads the Nebula Graph as a DGLGraph.
+    NebulaReducedLoader is a class that reduces vertexes and edges data from Nebula Graph as a DGLGraph.
 
     feature_mapper: a dictionary that maps the feature names to the feature,
                     its equivalent example in YAML is:
                     ../example/nebula_to_dgl_mapper.yaml
 
     """
 
     def __init__(self, nebula_config: Dict, feature_mapper: Dict):
         """
         Initialize the NebulaLoader class.
         """
         self.nebula_config = nebula_config
+        self.feature_mapper = feature_mapper
+        self.part_nums = None
+        self.tag_feature_dict = None
+        self.edge_feature_dict = None
+        self.meta_hosts = None
         self.init_connection()
         self.remap_vertex_id = feature_mapper.get('remap_vertex_id', True)
         if self.remap_vertex_id:
             self.vertex_id_dict = dict()
         self.validate_feature_mapper(feature_mapper)
 
     def init_connection(self):
@@ -71,30 +71,29 @@
             for row in result.rows():
                 meta_hosts.append(
                     (row.values[0].get_sVal().decode(),
                      row.values[1].get_iVal())
                 )
         self.meta_hosts = meta_hosts
 
+        # get part_nums
+        space_name = self.feature_mapper.get('space', None)
+        with self.connection_pool.session_context(user, password) as session:
+            result = session.execute('USE {}; SHOW PARTS'.format(space_name))
+            assert result.is_succeeded() and result.error_code() == 0
+            self.part_nums = len(result.rows())
+
     def get_meta_client(self):
         """
         Get the MetaClient.
         """
         meta_client = MetaClient(self.meta_hosts, 50000)
         meta_client.open()
         return meta_client
 
-    def get_storage_client(self):
-        """
-        Get the GraphStorageClient.
-        """
-        meta_cache = MetaCache(self.meta_hosts, 50000)
-        storage_client = GraphStorageClient(meta_cache)
-        return storage_client
-
     def validate_feature_mapper(self, feature_mapper: Dict):
         """
         Validate the feature mapper, parse the feature_mapper.yaml file.
 
         feature_mapper: a dictionary that maps the feature names to the feature
         """
         # ensure all properties exist in nebula graph schema
@@ -222,18 +221,18 @@
                     edge_name: {
                         "start_vertex_tag": edge_type.get('start_vertex_tag'),
                         "end_vertex_tag": edge_type.get('end_vertex_tag'),
                         "features": {}
                     }}
             if edge_name not in self.edge_feature_dict[space_name]:
                 self.edge_feature_dict[space_name][edge_name] = {
-                        "start_vertex_tag": edge_type.get('start_vertex_tag'),
-                        "end_vertex_tag": edge_type.get('end_vertex_tag'),
-                        "features": {}
-                    }
+                    "start_vertex_tag": edge_type.get('start_vertex_tag'),
+                    "end_vertex_tag": edge_type.get('end_vertex_tag'),
+                    "features": {}
+                }
             for feature in edge_type.get('features', []):
                 feature_name = feature.get('name')
                 assert feature_name is not None, \
                     'feature name is not specified in {}'.format(feature)
                 # ensure properties exists and type is correct
                 edge = self.edge_type_schema_dict[space_name][edge_name]
                 edge_props_types = {
@@ -287,177 +286,70 @@
         assert len(self.edge_type_schema_dict) == 1, \
             f'There should be only 1 graph space involved, '\
             f'but now: {self.edge_type_schema_dict.keys()}'
         assert self.edge_type_schema_dict.keys() == self.edge_feature_dict.keys(), \
             f'edge type schema and feature dict should have the same graph space, '\
             f'but now: {self.edge_type_schema_dict.keys()} and {self.edge_feature_dict.keys()}'
 
-    def get_feature_transform_function(self, features: Dict, prop_names: List) -> Callable:
-        """
-        Get the transform function for all the features.
-        """
-        prop_pos_index = {prop_name: i for i,
-                          prop_name in enumerate(prop_names)}
-        def transform_function(prop_values):
-            ret_feature = []
-            for feature_name in features:
-                feature = features[feature_name]
-                feature_props = feature.get('prop')
-                if feature_props is None:
-                    import pdb; pdb.set_trace()
-
-                feature_prop_names = [prop.get('name')
-                                      for prop in feature_props]
-                feature_prop_types = [prop.get('type')
-                                      for prop in feature_props]
-                feature_prop_values = []
-                for index, prop_name in enumerate(feature_prop_names):
-                    raw_value = prop_values[prop_pos_index[prop_name]]
-                    # convert byte value according to type
-                    feature_prop_values.append(
-                        getattr(raw_value, NEBULA_TYPE_MAP[feature_prop_types[index]])()
-                        )
-                if feature.get('type') == 'value':
-                    ret_feature.append(feature_prop_values[0])
-                elif feature.get('type') == 'enumeration':
-                    enumeration_dict = feature.get('enumeration')
-                    ret_feature.append(enumeration_dict.get(
-                        feature_prop_values[0], ENUMERATION_DEFAULT_VALUE))
-                elif feature.get('type') == 'function':
-                    feature_filter_function = feature.get('function')
-                    ret_feature.append(
-                        feature_filter_function(*feature_prop_values))
-            if len(ret_feature) == 0:
-                return None
-            else:
-                return ret_feature
-
-        return transform_function
-
     def load(self) -> DGLHeteroGraph:
-        """
-        Load the data from Nebula Graph Cluster, return a DGL heterograph.
-        ref: https://github.com/dmlc/dgl/blob/master/python/dgl/convert.py::heterograph
-        """
-        # generate vertices per tag
+        # load vertexes
+        part_loaders = []
+        for i in range(1, self.part_nums + 1):
+            part = NebulaPartLoader(
+                i, self.meta_hosts, self.edge_feature_dict, self.tag_feature_dict)
+            part_loaders.append(part)
+
+        vertexes_futures = []
+
+        with ThreadPoolExecutor(max_workers=self.part_nums) as executor:
+            for p in part_loaders:
+                fu = executor.submit(p.load_vertexes)
+                vertexes_futures.append(fu)
+
+        vertex_ids = vertexes_futures[0].result()[0]
+        ndata = vertexes_futures[0].result()[1]
+
+        for p in vertexes_futures[1:]:
+            vertexes = p.result()[0]
+            for space, tag_vertexes in vertexes.items():
+                for tag, ids in tag_vertexes.items():
+                    vid_index = len(vertex_ids[space][tag])
+                    for vid, _ in ids.items():
+                        vertex_ids[space][tag][vid] = vid_index
+                        vid_index += 1
+            vertexes_pro = p.result()[1]
+            for prop, tag_vertexes in vertexes_pro.items():
+                for tag, ids in tag_vertexes.items():
+                    ndata[prop][tag].extend(ids)
+
+        # load edges
+        edges_futures = []
+        with ThreadPoolExecutor(max_workers=self.part_nums) as executor:
+            for p in part_loaders:
+                fu = executor.submit(p.load_edges, vertex_ids)
+                edges_futures.append(fu)
+
+        data_dict = edges_futures[0].result()[0]
+        edata = edges_futures[0].result()[1]
+        for f in edges_futures[1:]:
+            edges = f.result()[0]
+            for key, value in edges.items():
+                data_dict[key][0].extend(value[0])
+                data_dict[key][1].extend(value[1])
+            edges_pro = f.result()[1]
+            for prop, edge_prop in edges_pro.items():
+                for key, value in edge_prop.items():
+                    edata[prop][key].extend(value)
 
-        data_dict = dict()
+        for edge, edge_data in data_dict.items():
+            data_dict[edge] = (tensor(edge_data[0]), tensor(edge_data[1]))
 
-        vertex_id_dict = dict()
-        ndata = dict()
-        edata = dict()
-
-        # assumed only one graph space though, we iterate it here.
-        for space_name in self.tag_feature_dict:
-            if space_name not in vertex_id_dict:
-                vertex_id_dict[space_name] = dict()
-            for tag_name in self.tag_feature_dict[space_name]:
-                if tag_name not in vertex_id_dict[space_name]:
-                    vertex_id_dict[space_name][tag_name] = dict()
-                _vertex_id_dict = vertex_id_dict[space_name][tag_name]
-                tag_features = self.tag_feature_dict[space_name][tag_name]
-                props = set()
-                for feature_name in tag_features:
-                    feature = tag_features[feature_name]
-                    if feature_name not in ndata:
-                        ndata[feature_name] = {tag_name: []}
-                    else:
-                        assert tag_name not in ndata[feature_name], \
-                            f'tag {tag_name} already exists in ndata[{feature_name}]'
-                        ndata[feature_name][tag_name] = []
-                    for prop in feature.get('prop', []):
-                        props.add(prop['name'])
-                prop_names = list(props)
-
-                graph_storage_client = self.get_storage_client()
-                resp = graph_storage_client.scan_vertex(
-                    space_name=space_name,
-                    tag_name=tag_name,
-                    prop_names=prop_names)
-                vertex_index = 0
-                transform_function = self.get_feature_transform_function(
-                    tag_features, prop_names)
-                while resp.has_next():
-                    result = resp.next()
-                    for vertex_data in result:
-                        _vertex_id_dict[vertex_data.get_id()] = vertex_index
-                        vertex_index += 1
-                        # feature data for vertex(node)
-                        if not tag_features:
-                            continue
-                        prop_values = vertex_data.get_prop_values()
-                        feature_values = transform_function(prop_values)
-                        for index, feature_name in enumerate(tag_features):
-                            feature = tag_features[feature_name]
-                            if feature_name not in ndata:
-                                ndata[feature_name] = {tag_name: []}
-                            ndata[feature_name][tag_name].append(feature_values[index])
-                if prop_names:
-                    assert vertex_index == len(
-                        ndata[feature_name][tag_name]), \
-                        f'vertex index {vertex_index} != len(ndata[{prop_names[0]}][{tag_name}])'
-
-        for space_name in self.edge_feature_dict:
-
-            for edge_name in self.edge_feature_dict[space_name]:
-                edge = self.edge_feature_dict[space_name][edge_name]
-                edge_features = edge.get('features', {})
-                start_vertex_tag, end_vertex_tag = edge.get(
-                    'start_vertex_tag'), edge.get('end_vertex_tag')
-                assert (start_vertex_tag, edge_name, end_vertex_tag) not in data_dict, \
-                    f'edge {start_vertex_tag}-{edge_name}-{end_vertex_tag} already exists'
-                props = set()
-                for feature_name in edge_features:
-                    feature = edge_features[feature_name]
-                    if feature_name not in edata:
-                        edata[feature_name] = {edge_name: []}
-                    else:
-                        assert edge_name not in edata[feature_name], \
-                            f'tag {edge_name} already exists in edata[{feature_name}]'
-                        edata[feature_name][edge_name] = []
-                    for prop in feature.get('prop', []):
-                        props.add(prop['name'])
-                prop_names = list(props)
-
-                graph_storage_client = self.get_storage_client()
-                resp = graph_storage_client.scan_edge(
-                    space_name=space_name,
-                    edge_name=edge_name,
-                    prop_names=prop_names)
-                transform_function = self.get_feature_transform_function(
-                    edge_features, prop_names)
-                start_vertices, end_vertices = [], []
-                start_vertex_id_dict = vertex_id_dict[space_name][start_vertex_tag]
-                end_vertex_id_dict = vertex_id_dict[space_name][end_vertex_tag]
-                while resp.has_next():
-                    result = resp.next()
-                    for edge_data in result:
-                        # edge data for edge
-                        start_vertices.append(
-                            start_vertex_id_dict[edge_data.get_src_id()]
-                        )
-                        end_vertices.append(
-                            end_vertex_id_dict[edge_data.get_dst_id()]
-                        )
-
-                        # feature data for edge
-                        if not edge_features:
-                            continue
-                        prop_values = edge_data.get_prop_values()
-                        feature_values = transform_function(prop_values)
-                        for index, feature_name in enumerate(edge_features):
-                            feature = edge_features[feature_name]
-                            if feature_name not in edata:
-                                edata[feature_name] = {edge_name: []}
-                            edata[feature_name][edge_name].append(feature_values[index])
-
-                data_dict[(start_vertex_tag, edge_name, end_vertex_tag)] = (
-                    tensor(start_vertices), tensor(end_vertices))
+        # Convert to DGLHeteroGraph
+        space_name = self.feature_mapper.get('space', None)
         dgl_graph: DGLHeteroGraph = heterograph(data_dict)
-
         for prop_name, tag_dict in ndata.items():
             for tag_name, prop_values in tag_dict.items():
                 dgl_graph.ndata[prop_name] = tensor(prop_values) if len(self.tag_feature_dict[space_name]) == 1 else \
                     {tag_name: tensor(prop_values)}
         for prop_name, edge_dict in edata.items():
             for edge_name, prop_values in edge_dict.items():
                 dgl_graph.edata[prop_name] = tensor(prop_values) if len(self.edge_feature_dict[space_name]) == 1 else \
```

### Comparing `nebula-dgl-0.1.1/tests/unit/nebula_loader.py` & `nebula-dgl-0.1.2/tests/unit/nebula_loader.py`

 * *Files identical despite different names*

