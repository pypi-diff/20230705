# Comparing `tmp/icat-iml-0.1.2.tar.gz` & `tmp/icat-iml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icat-iml-0.1.2.tar", last modified: Mon Apr 17 19:49:25 2023, max compression
+gzip compressed data, was "icat-iml-0.2.0.tar", last modified: Wed Jul  5 17:11:35 2023, max compression
```

## Comparing `icat-iml-0.1.2.tar` & `icat-iml-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:49:25.091920 icat-iml-0.1.2/
--rw-r--r--   0 81n      (42021) users      (100)     1524 2023-04-17 14:53:45.000000 icat-iml-0.1.2/LICENSE
--rw-r--r--   0 81n      (42021) users      (100)     1115 2023-04-17 19:49:25.091920 icat-iml-0.1.2/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)      614 2023-04-17 17:30:21.000000 icat-iml-0.1.2/README.md
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:49:25.091920 icat-iml-0.1.2/icat/
--rw-r--r--   0 81n      (42021) users      (100)       22 2023-04-17 19:48:23.000000 icat-iml-0.1.2/icat/__init__.py
--rw-r--r--   0 81n      (42021) users      (100)    23409 2023-04-17 14:58:08.000000 icat-iml-0.1.2/icat/anchorlist.py
--rw-r--r--   0 81n      (42021) users      (100)    17062 2023-04-17 14:58:08.000000 icat-iml-0.1.2/icat/anchors.py
--rw-r--r--   0 81n      (42021) users      (100)    17837 2023-04-17 14:58:12.000000 icat-iml-0.1.2/icat/data.py
--rw-r--r--   0 81n      (42021) users      (100)     3297 2023-04-17 13:46:04.000000 icat-iml-0.1.2/icat/histogram.py
--rw-r--r--   0 81n      (42021) users      (100)     3738 2023-04-17 14:58:08.000000 icat-iml-0.1.2/icat/histograms.py
--rw-r--r--   0 81n      (42021) users      (100)     7117 2023-04-17 14:58:08.000000 icat-iml-0.1.2/icat/instance.py
--rw-r--r--   0 81n      (42021) users      (100)    13184 2023-04-17 13:46:04.000000 icat-iml-0.1.2/icat/model.py
--rw-r--r--   0 81n      (42021) users      (100)     5524 2023-04-17 14:58:08.000000 icat-iml-0.1.2/icat/table.py
--rw-r--r--   0 81n      (42021) users      (100)     9433 2023-04-17 14:58:12.000000 icat-iml-0.1.2/icat/view.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:49:25.091920 icat-iml-0.1.2/icat_iml.egg-info/
--rw-r--r--   0 81n      (42021) users      (100)     1115 2023-04-17 19:49:25.000000 icat-iml-0.1.2/icat_iml.egg-info/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)      547 2023-04-17 19:49:25.000000 icat-iml-0.1.2/icat_iml.egg-info/SOURCES.txt
--rw-r--r--   0 81n      (42021) users      (100)        1 2023-04-17 19:49:25.000000 icat-iml-0.1.2/icat_iml.egg-info/dependency_links.txt
--rw-r--r--   0 81n      (42021) users      (100)      116 2023-04-17 19:49:25.000000 icat-iml-0.1.2/icat_iml.egg-info/requires.txt
--rw-r--r--   0 81n      (42021) users      (100)        5 2023-04-17 19:49:25.000000 icat-iml-0.1.2/icat_iml.egg-info/top_level.txt
--rw-r--r--   0 81n      (42021) users      (100)       31 2023-04-17 14:58:06.000000 icat-iml-0.1.2/pyproject.toml
--rw-r--r--   0 81n      (42021) users      (100)       38 2023-04-17 19:49:25.095920 icat-iml-0.1.2/setup.cfg
--rw-r--r--   0 81n      (42021) users      (100)     1158 2023-04-17 19:48:11.000000 icat-iml-0.1.2/setup.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-04-17 19:49:25.091920 icat-iml-0.1.2/tests/
--rw-r--r--   0 81n      (42021) users      (100)     6467 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_anchorlist.py
--rw-r--r--   0 81n      (42021) users      (100)     9102 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_anchors.py
--rw-r--r--   0 81n      (42021) users      (100)     3813 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_datamanager.py
--rw-r--r--   0 81n      (42021) users      (100)     4099 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_histograms.py
--rw-r--r--   0 81n      (42021) users      (100)     2522 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_instance.py
--rw-r--r--   0 81n      (42021) users      (100)      374 2023-04-17 13:46:04.000000 icat-iml-0.1.2/tests/test_integrations.py
--rw-r--r--   0 81n      (42021) users      (100)     9266 2023-04-17 14:58:07.000000 icat-iml-0.1.2/tests/test_model.py
--rw-r--r--   0 81n      (42021) users      (100)     3885 2023-04-17 14:58:07.000000 icat-iml-0.1.2/tests/test_view.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-07-05 17:11:35.017894 icat-iml-0.2.0/
+-rw-r--r--   0 81n      (42021) users      (100)     1524 2023-07-05 13:15:33.000000 icat-iml-0.2.0/LICENSE
+-rw-r--r--   0 81n      (42021) users      (100)     1115 2023-07-05 17:11:35.017894 icat-iml-0.2.0/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)      614 2023-07-05 13:15:33.000000 icat-iml-0.2.0/README.md
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-07-05 17:11:35.013894 icat-iml-0.2.0/icat/
+-rw-r--r--   0 81n      (42021) users      (100)       22 2023-07-05 16:51:37.000000 icat-iml-0.2.0/icat/__init__.py
+-rw-r--r--   0 81n      (42021) users      (100)    23935 2023-07-05 15:23:08.000000 icat-iml-0.2.0/icat/anchorlist.py
+-rw-r--r--   0 81n      (42021) users      (100)    19254 2023-07-05 13:50:59.000000 icat-iml-0.2.0/icat/anchors.py
+-rw-r--r--   0 81n      (42021) users      (100)    18289 2023-07-05 13:50:59.000000 icat-iml-0.2.0/icat/data.py
+-rw-r--r--   0 81n      (42021) users      (100)     3297 2023-07-05 13:15:33.000000 icat-iml-0.2.0/icat/histogram.py
+-rw-r--r--   0 81n      (42021) users      (100)     3856 2023-07-05 13:50:59.000000 icat-iml-0.2.0/icat/histograms.py
+-rw-r--r--   0 81n      (42021) users      (100)     7117 2023-07-05 13:15:33.000000 icat-iml-0.2.0/icat/instance.py
+-rw-r--r--   0 81n      (42021) users      (100)    13687 2023-07-05 13:50:59.000000 icat-iml-0.2.0/icat/model.py
+-rw-r--r--   0 81n      (42021) users      (100)     5524 2023-07-05 13:15:33.000000 icat-iml-0.2.0/icat/table.py
+-rw-r--r--   0 81n      (42021) users      (100)    10259 2023-07-05 15:25:50.000000 icat-iml-0.2.0/icat/view.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-07-05 17:11:35.017894 icat-iml-0.2.0/icat_iml.egg-info/
+-rw-r--r--   0 81n      (42021) users      (100)     1115 2023-07-05 17:11:35.000000 icat-iml-0.2.0/icat_iml.egg-info/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)      547 2023-07-05 17:11:35.000000 icat-iml-0.2.0/icat_iml.egg-info/SOURCES.txt
+-rw-r--r--   0 81n      (42021) users      (100)        1 2023-07-05 17:11:35.000000 icat-iml-0.2.0/icat_iml.egg-info/dependency_links.txt
+-rw-r--r--   0 81n      (42021) users      (100)       74 2023-07-05 17:11:35.000000 icat-iml-0.2.0/icat_iml.egg-info/requires.txt
+-rw-r--r--   0 81n      (42021) users      (100)        5 2023-07-05 17:11:35.000000 icat-iml-0.2.0/icat_iml.egg-info/top_level.txt
+-rw-r--r--   0 81n      (42021) users      (100)       31 2023-07-05 13:15:33.000000 icat-iml-0.2.0/pyproject.toml
+-rw-r--r--   0 81n      (42021) users      (100)       38 2023-07-05 17:11:35.017894 icat-iml-0.2.0/setup.cfg
+-rw-r--r--   0 81n      (42021) users      (100)     1116 2023-07-05 13:50:59.000000 icat-iml-0.2.0/setup.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-07-05 17:11:35.017894 icat-iml-0.2.0/tests/
+-rw-r--r--   0 81n      (42021) users      (100)     6467 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_anchorlist.py
+-rw-r--r--   0 81n      (42021) users      (100)     9102 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_anchors.py
+-rw-r--r--   0 81n      (42021) users      (100)     3813 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_datamanager.py
+-rw-r--r--   0 81n      (42021) users      (100)     4099 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_histograms.py
+-rw-r--r--   0 81n      (42021) users      (100)     2522 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_instance.py
+-rw-r--r--   0 81n      (42021) users      (100)      374 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_integrations.py
+-rw-r--r--   0 81n      (42021) users      (100)     9266 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_model.py
+-rw-r--r--   0 81n      (42021) users      (100)     3885 2023-07-05 13:15:33.000000 icat-iml-0.2.0/tests/test_view.py
```

### Comparing `icat-iml-0.1.2/LICENSE` & `icat-iml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/PKG-INFO` & `icat-iml-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat-iml
-Version: 0.1.2
+Version: 0.2.0
 Summary: Interactive Corpus Analysis Tool
 Home-page: https://github.com/ORNL/icat
 Author: Nathan Martindale, Scott L. Stewart
 Author-email: icat-help@ornl.gov
 Project-URL: Documentation, https://ornl.github.io/icat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `icat-iml-0.1.2/README.md` & `icat-iml-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/icat/anchorlist.py` & `icat-iml-0.2.0/icat/anchorlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import pandas as pd
 import panel as pn
 import param
 import traitlets
 from sklearn.feature_extraction.text import TfidfVectorizer
 
-from icat.anchors import Anchor, DictionaryAnchor, TFIDFAnchor
+from icat.anchors import Anchor, DictionaryAnchor, SimilarityFunctionAnchor, TFIDFAnchor
 
 
 class AnchorListTemplate(v.VuetifyTemplate):
     """The ipyvuetify contents of the anchorlist table. This handles all the special considerations
     like the slot for the expanded rows containing the anchor widgets, and the coverage v-html etc.
     """
 
@@ -31,14 +31,15 @@
             {"text": "% Neg", "value": "pct_negative"},
             {"text": "% Pos", "value": "pct_positive"},
             {"text": "Viz", "value": "in_viz", "width": 10, "sortable": False},
             {"text": "Model", "value": "in_model", "width": 10, "sortable": False},
             {"text": "Delete", "value": "delete", "width": 10, "sortable": False},
         ]
     ).tag(sync=True)
+    # TODO: height and width don't seem to be used?
     height = traitlets.Int(700).tag(sync=True)
     width = traitlets.Int(150).tag(sync=True)
     expanded = traitlets.List([]).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -162,15 +163,15 @@
                 height: 2px !important;
                 min-height: 2px !important;
             }
         </style>
         """
 
 
-class AnchorList(pn.viewable.Viewer):
+class AnchorList(pn.viewable.Layoutable, pn.viewable.Viewer):
     """A model's list tracking and managing a collection of anchors for creating features off
     a dataset. This class is also a visual component for interacting with and modifying those
     anchors in a table format, and is used as part of the greater model interactive view.
 
     Args:
         model: The parent model.
         table_width (int): Static width of the visual component table.
@@ -212,19 +213,25 @@
         self.dictionary_button.on_click(self._handle_pnl_new_dictionary_btn_clicked)
         self.tfidf_button = pn.widgets.Button(
             name="Add TF-IDF Anchor",
             button_type="primary",
         )
         self.tfidf_button.on_click(self._handle_pnl_new_tfidf_btn_clicked)
 
+        self.similarity_button = pn.widgets.Button(
+            name="Add Similarity Anchor",
+            button_type="primary",
+        )
+        self.similarity_button.on_click(self._handle_pnl_new_similarity_btn_clicked)
+
         self.table = AnchorListTemplate()
         self.table.on_anchor_removal(self._handle_table_anchor_deleted)
 
         self.layout = pn.Column(
-            pn.Row(self.dictionary_button, self.tfidf_button),
+            pn.Row(self.dictionary_button, self.tfidf_button, self.similarity_button),
             self.table,
             height=table_height,
             width=table_width,
         )
         """The full component layout for panel to display."""
 
         self.coverage: dict[dict] = None
@@ -255,14 +262,18 @@
         name = self.get_unique_anchor_name()
         self.add_anchor(DictionaryAnchor(anchor_name=name))
 
     def _handle_pnl_new_tfidf_btn_clicked(self, event):
         name = self.get_unique_anchor_name()
         self.add_anchor(TFIDFAnchor(anchor_name=name))
 
+    def _handle_pnl_new_similarity_btn_clicked(self, event):
+        name = self.get_unique_anchor_name()
+        self.add_anchor(SimilarityFunctionAnchor(anchor_name=name))
+
     # ============================================================
     # EVENT SPAWNERS
     # ============================================================
 
     def on_anchor_added(self, callback: Callable):
         """Register a callback function for the "anchor added" event.
```

### Comparing `icat-iml-0.1.2/icat/anchors.py` & `icat-iml-0.2.0/icat/anchors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Anchors are the interactive featuring component of ICAT, an anchor class
 determines how a feature is computed on the data, and the user interacts with
 the UI widget of the anchor to modify the feature (e.g. what keywords it
 searches for.)
 """
 
+# NOTE: "container" refers to the containing anchorlist instance
+
 from collections.abc import Callable
 
 import ipyvuetify as v
 import numpy as np
 import pandas as pd
 import panel as pn
 import param
@@ -232,15 +234,15 @@
     def row_view(self) -> pn.Row:
         return pn.Row(
             self.param.weight,
             self.param.keywords_str,
         )
 
 
-class TFIDFAnchor(Anchor):
+class SimilarityAnchorBase(Anchor):
     # TODO: have to have the texts _and_ the indices from the original data
     # that this is based on? (because the indices are what we'll want to base
     # the widget off of, but the texts should be what we actually care about/store)
     # is there concern about these getting off from each other?
 
     # alternatively, maybe just do away with indices entirely? The goal for
     # anchors is to be relatively pure
@@ -259,15 +261,16 @@
         self._chips_container = v.Container(
             dense=True, children=[], style_="padding: 0;"
         )  # munch munch
 
         self._id_text = v.TextField(
             label="Row ID", v_model="", dense=True, single_line=True, width=40
         )
-        self._id_text.on_event("change", self._handle_ipv_id_text_changed)
+        # self._id_text.on_event("change", self._handle_ipv_id_text_changed)
+        # self._id_text.on_event("keydown", self._handle_ipv_id_text_changed)
         self._add_button = v.Btn(children=["Add"])
         self._add_button.on_event("click", self._handle_ipv_add_btn_clicked)
 
         self.new_id = 0
 
         self.widget = v.Container(
             fluid=True,
@@ -300,18 +303,22 @@
                             children=[self._add_button],
                         ),
                     ],
                 )
             ],
         )
 
-    def _handle_ipv_id_text_changed(self, widget, event, data):
-        self.new_id = data
+    # def _handle_ipv_id_text_changed(self, widget, event, data):
+    #     print(widget)
+    #     self.new_id = self._id_text.v_model
+    #     print(self.new_id)
 
     def _handle_ipv_add_btn_clicked(self, widget, event, data):
+        self.new_id = self._id_text.v_model
+
         # get the text of the row id specified, or use as the text itself if not an id/no model
         if self.container is not None and self.container.model is not None:
             active_data = self.container.model.data.active_data
             new_text = active_data.loc[int(self.new_id), self.text_col]
         else:
             new_text = self.new_id
         self.reference_texts = [*self.reference_texts, new_text]
@@ -370,14 +377,29 @@
         if index != -1:
             new_list = []
             for i, item in enumerate(self.reference_texts):
                 if i != index:
                     new_list.append(item)
             self.reference_texts = new_list
 
+    def featurize(self, data: pd.DataFrame) -> pd.Series:
+        raise NotImplementedError()
+
+    # def save(self, path: str, prefix: str):
+    #     raise NotImplementedError("these are not the droids you are looking for")
+
+    # @staticmethod
+    # def load(path: str, prefix: str):
+    #     raise NotImplementedError("these are not the droids you are looking for")
+
+
+class TFIDFAnchor(SimilarityAnchorBase):
+    def __init__(self, container=None, *args, **kwargs):
+        super().__init__(container, *args, **kwargs)
+
     def _tfidf_similarities(self, vector, comparison_vectors):
         # TODO: what is instance/instances?
         # these are already numpy arrays/the tfidf vectors I think.
         sims = cosine_similarity(vector, comparison_vectors)
         return sims
 
     # TODO: I really need more integration tests for this, there's a lot
@@ -411,27 +433,64 @@
             # will potentially create very differently shaped vectors
             tfidf_features = tfidf_vectorizer.transform(data[self.text_col])
 
         reference_features = tfidf_vectorizer.transform(self.reference_texts)
 
         combined_reference_features = reference_features.mean(axis=0)
         similarities = self._tfidf_similarities(
-            combined_reference_features, tfidf_features
+            np.asarray(combined_reference_features), tfidf_features
         )
 
-        # if it does, transform the passed data based on it.
-
         # store/save/cache the vectorizer and features
         # NOTE: we don't really have a way to detect when the data has sufficiently
         # changed that we should refit/transform vectorizer and features.
         # if self.container is not None:
         #     self.container.tfidf_vectorizer = tfidf_vectorizer
         #     self.container.tfidf_features = tfidf_features
 
         return pd.Series(similarities[0], index=data.index)
 
-    # def save(self, path: str, prefix: str):
-    #     raise NotImplementedError("these are not the droids you are looking for")
 
-    # @staticmethod
-    # def load(path: str, prefix: str):
-    #     raise NotImplementedError("these are not the droids you are looking for")
+# TODO: probably instead of this extending TF-IDFAnchor, we should have them extend from same root?
+class SimilarityFunctionAnchor(SimilarityAnchorBase):
+    similarity_function = param.String("")
+
+    # TODO: need a dropdown for the possible similarity functions
+    def __init__(self, container=None, *args, **kwargs):
+        super().__init__(container, *args, **kwargs)
+
+        self.sim_function_options = v.Select(label="Similarity function", items=[{}])
+        self.sim_function_options.on_event(
+            "change", self._handle_ipv_sim_function_change
+        )
+
+        self.widget.children = [
+            *self.widget.children,
+            v.Row(
+                dense=True,
+                children=[self.sim_function_options],
+            ),
+        ]
+        self._populate_items()
+
+    # TODO: need dropdown event handlers to modify similarity_function
+
+    def _handle_ipv_sim_function_change(self, widget, event, data):
+        self.similarity_function = data
+
+    def _populate_items(self):
+        items = []
+        if self.container is not None and self.container.model is not None:
+            items = list(self.container.model.similarity_functions.keys())
+        self.sim_function_options.items = items
+
+    def featurize(self, data: pd.DataFrame) -> pd.Series:
+        if len(self.reference_texts) == 0:
+            return pd.Series(0, index=data.index)
+
+        if self.similarity_function == "":
+            return pd.Series(0, index=data.index)
+
+        model_fn = self.container.model.similarity_functions[self.similarity_function]
+        # results = model_fn(data, self.container, self.reference_texts[0], self.text_col)
+        results = model_fn(data, self)
+        return results
```

### Comparing `icat-iml-0.1.2/icat/data.py` & `icat-iml-0.2.0/icat/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,18 +174,24 @@
     # TODO: coupling: directly calling refresh data on the model view. Instead, we
     # could have a "sample_changed" event that view listens to.
     def _handle_ipv_resample_btn_click(self, widget, event, data):
         self.set_random_sample()
         self.model.view.refresh_data()
 
     def _handle_ipv_tab_changed(self, widget, event, data: int):
-        """Event handler for the vuetify tabs change. This chagnes the current_data_tab
+        """Event handler for the vuetify tabs change. This changes the current_data_tab
         param, which will automatically trigger the apply_filter."""
         self.table.options["page"] = 1
-        self.current_data_tab = self.data_tab_list[data]
+        # BUG: https://github.com/ORNL/icat/issues/3
+        # Sometimes when clicking on the first tab, the data being sent is a blank dictionary
+        # {} instead of the integer 0. Bypassing this by directly setting the tab based on
+        # data_tabs v_model which does correctly get set to 0. This is possibly an issue within
+        # ipyvuetify itself?
+        # self.current_data_tab = self.data_tab_list[data]
+        self.current_data_tab = self.data_tab_list[self.data_tabs.v_model]
 
     def _handle_ipv_search_changed(self, widget, event, data):
         """Event handler for the vuetify search box change. This changes the search_value
         param, which will automatically trigger the apply_filter."""
         self.search_value = widget.v_model if widget.v_model is not None else ""
 
     def _handle_ipv_search_cleared(self, widget, event, data):
@@ -363,15 +369,15 @@
         column: str,
     ) -> pd.DataFrame:
         """This function searches for a given string in code:`pattern` and applies it to the code:`column` within the
         code:`df`."""
         # TODO: possibly move to a utils.py
         if not pattern:
             return df
-        return df[df[column].str.contains(pattern)]
+        return df[df[column].str.contains(pattern, case=False)]
 
     # TODO: either make this static and add prediction col,
     # or embrace that it's a self filter and don't support passing min/max/take it from the self params
     def _prediction_range_filter(self, df: pd.DataFrame) -> pd.DataFrame:
         """Filters out rows that don't have a predicted value within the specified range."""
 
         if self.prediction_col not in df:
```

### Comparing `icat-iml-0.1.2/icat/histogram.py` & `icat-iml-0.2.0/icat/histogram.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/icat/histograms.py` & `icat-iml-0.2.0/icat/histograms.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.hist_global.layout.margin = (-35, 0, 0, 0)
         self.slider = v.RangeSlider(
             v_model=[0, 100],
             min=0,
             max=100,
             step=1,
             thumb_label=True,
-            style_="padding: 0; padding-top: 35px; margin: 0; z-index: 10000;",
+            style_=f"padding: 0; padding-top: 35px; margin: 0; z-index: 10000; width: {width-25}px;",
         )
         self.slider.on_event("change", self._handle_ipv_range_changed)
 
         self.transparent_bg_css = v.Html(
             tag="style",
             children=[
                 ".vuetify-styles .theme--dark.v-application {background: transparent}"
@@ -76,17 +76,20 @@
 
     def __panel__(self):
         return self.layout
 
     def _set_layout(self):
         self.layout = pn.Column(
             self.hist_local.layout,
-            v.Container(
-                children=[self.slider, self.transparent_bg_css],
-                style_="padding: 0; margin: 0; overflow: hidden;",
+            pn.Row(
+                v.Container(
+                    children=[self.slider, self.transparent_bg_css],
+                    style_="padding: 0; margin: 0; overflow: hidden;",
+                ),
+                sizing_mode="stretch_width",
             ),
             self.hist_global.layout,
             width=self.width,
             height=227,
         )
 
     # ============================================================
```

### Comparing `icat-iml-0.1.2/icat/instance.py` & `icat-iml-0.2.0/icat/instance.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/icat/model.py` & `icat-iml-0.2.0/icat/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """The model class, this handles both the machine learning model, as well as
 contains an associated anchorlist, datamanager, and view. This is sort of the
 primary parent class for interacting with icat.
 """
 
+from collections.abc import Callable
+
 import numpy as np
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 
 from icat.anchorlist import AnchorList
-from icat.anchors import Anchor, DictionaryAnchor, TFIDFAnchor
+from icat.anchors import Anchor, DictionaryAnchor, SimilarityFunctionAnchor, TFIDFAnchor
 from icat.data import DataManager
 from icat.view import InteractiveView
 
 
 class Model:
-    def __init__(self, data: pd.DataFrame, text_col: str):
+    def __init__(
+        self,
+        data: pd.DataFrame,
+        text_col: str,
+        similarity_functions: list[Callable] = [],
+    ):
         self.training_data: pd.DataFrame = None
         """The rows (and only those rows) of the original data explicitly used for training."""
         self.text_col = text_col
 
         self.classifier: LogisticRegression = LogisticRegression(
             class_weight="balanced"
         )
@@ -34,14 +41,19 @@
         self.data.on_data_labeled(self._on_data_label)
         self.view.on_selected_points_change(self._on_selected_points_change)
 
         self._last_anchor_names: dict[str, str] = []
         """Keep track of anchor names so when the name of one updates we can
         remove the previous column name. The key is the panel id."""
 
+        # self.similarity_functions = similarity_functions
+        self.similarity_functions: dict[str, Callable] = {
+            str(func.__name__): func for func in similarity_functions
+        }
+
         self.anchor_list.build_tfidf_features()
 
     def _on_data_label(self, index: int, new_label: int):
         """Event handler for datamanager."""
         if self.training_data is None:
             self.training_data = pd.DataFrame([self.data.active_data.loc[index, :]])
 
@@ -87,18 +99,22 @@
         self.fit()
         self.view.refresh_data()
 
     def _on_anchor_add(self, anchor: Anchor):
         """Event handler for anchorlist."""
         # TODO: it's possible this should be handled inside the anchorlist?
         if (
-            type(anchor) == DictionaryAnchor or type(anchor) == TFIDFAnchor
+            type(anchor) == DictionaryAnchor
+            or type(anchor) == TFIDFAnchor
+            or type(anchor) == SimilarityFunctionAnchor
         ) and anchor.text_col == "":
             anchor.text_col = self.text_col
             self.anchor_list.anchors[-1].text_col = self.text_col
+        if type(anchor) == SimilarityFunctionAnchor:
+            anchor._populate_items()
         self.fit()
         self.view.refresh_data()
 
     # TODO: I wonder if this should directly be in the view?
     def _on_selected_points_change(self, selected_ids: list[str]):
         """Event handler for interactive view."""
         self.data.selected_indices = [int(selected_id) for selected_id in selected_ids]
```

### Comparing `icat-iml-0.1.2/icat/table.py` & `icat-iml-0.2.0/icat/table.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/icat/view.py` & `icat-iml-0.2.0/icat/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Module for the view code that manages interactions between ipyanchorviz/various
 widgets and the rest of the model gui components."""
 
 import copy
+import random
 from collections.abc import Callable
 from typing import Any
 
 import ipywidgets as ipw
 import pandas as pd
 import panel as pn
 from ipyanchorviz import AnchorViz
 
-from icat.anchors import Anchor, DictionaryAnchor, TFIDFAnchor
+from icat.anchors import Anchor, DictionaryAnchor, SimilarityFunctionAnchor, TFIDFAnchor
 from icat.histograms import Histograms
 
 
 class InteractiveView(pn.viewable.Viewer):
     # TODO: coupling: technically coupling model and view, I think I care a lot less about it
     # here since view is already loosely orchestrating all of the gui stuff. If anything,
     # _more_ of the model event handlers should be handled in here instead of in the model?
@@ -33,22 +34,25 @@
         self.debug = ipw.Output()
 
         self._selected_points_change_callbacks: list[Callable] = []
 
         self.layout = pn.Row(
             pn.Column(self.anchorviz, self.model.anchor_list, self.debug),
             pn.Column(self.model.data.widget, self.histograms, width=700),
-            height=1000,
+            height=1150,
         )
 
         # set up all of the event handlers
         self.model.anchor_list.on_anchor_added(self._add_list_anchor_to_viz)
         self.model.anchor_list.on_anchor_changed(
             self._send_anchorlist_anchor_modification_to_viz
         )
+        self.model.anchor_list.on_anchor_changed(
+            self._update_data_table_on_anchor_change
+        )
         self.model.anchor_list.on_anchor_removed(self._remove_list_anchor_from_viz)
         self.anchorviz.on_anchor_add(self._add_viz_anchor_to_list)
         self.anchorviz.observe(
             self._trigger_selected_points_change, names="lassoedPointIDs"
         )
         self.model.data.table.on_point_hover(self._set_anchorviz_selected_point)
         self.histograms.on_range_changed(self._histograms_range_changed)
@@ -71,18 +75,23 @@
         # difference between thetas and put the new one in the middle of it.
 
         # make sure this isn't a double call from when you click on the anchorviz ring
         for av_anchor in self.anchorviz.anchors:
             if av_anchor["id"] == anchor.name:
                 return
 
-        theta = anchor.theta if hasattr(anchor, "theta") else 0.5
+        # TODO: randomize theta here
+        theta = (
+            anchor.theta if hasattr(anchor, "theta") else random.uniform(0, 2 * 3.14)
+        )
         anchor_dict = dict(id=anchor.name, name=anchor.anchor_name, theta=theta)
         if type(anchor) == TFIDFAnchor:
             anchor_dict["color"] = "#8e24aa"
+        elif type(anchor) == SimilarityFunctionAnchor:
+            anchor_dict["color"] = "#248eaa"
         self.anchorviz.add_anchor(anchor_dict)
 
     def _remove_list_anchor_from_viz(self, anchor: Anchor):
         """When an anchor is removed from the anchorlist, propagate
         that removal to the visualization."""
         # TODO: this can be cleaned when ipyanchorviz#6 is implemented
         current_anchors = copy.deepcopy(self.anchorviz.anchors)
@@ -104,39 +113,42 @@
 
         # send the actual name to be the id for the visualization
         self.anchorviz.modify_anchor_by_id(new_anchor_dict["id"], "id", new_anchor.name)
         self.anchorviz.modify_anchor_by_id(new_anchor.name, "name", name)
 
         self.model.anchor_list.add_anchor(new_anchor)
 
+    # TODO: need tests for this one
     def _send_anchorlist_anchor_modification_to_viz(
         self, id: str, property: str, value: Any
     ):
         """Whenever a modification is made to an anchor in the anchorlist (here
         we only care about name changes, since that's the only visual change),
         propagate it to the anchorviz visualization."""
         if property == "anchor_name":
             self.anchorviz.modify_anchor_by_id(id, "name", value)
         elif property == "in_view":
             if not value:
                 # add theta to the anchor so that when we "re-check" the anchor and re-add it to the viz,
                 # it adds it back where it was when we removed it.
                 for anchor in self.anchorviz.anchors:
                     if anchor["id"] == id:
-                        actual_anchor = self.model.anchor_list.get_anchor_by_id(id)
+                        actual_anchor = self.model.anchor_list.get_anchor_by_panel_id(
+                            id
+                        )
                         actual_anchor.theta = anchor["theta"]
                 # remove the anchor, but only from the visualization.
                 # TODO: this can be cleaned when ipyanchorviz#6 is implemented
                 updated_anchors = copy.deepcopy(self.anchorviz.anchors)
                 for anchor_dict in updated_anchors:
                     if anchor_dict["id"] == id:
                         updated_anchors.remove(anchor_dict)
                 self.anchorviz.set_anchors(updated_anchors)
             else:
-                actual_anchor = self.model.anchor_list.get_anchor_by_id(id)
+                actual_anchor = self.model.anchor_list.get_anchor_by_panel_id(id)
                 self._add_list_anchor_to_viz(actual_anchor)
 
     def _serialize_data_to_dicts(self) -> dict:
         feature_names = self.model.feature_names()
 
         # first we need to see if we are filtering data based on prediction range
         # we reference the sample indices a lot, so just compute this once and reference
@@ -194,14 +206,21 @@
         return points.to_dict(orient="records")
 
     def _trigger_selected_points_change(self, change):
         selected_ids = self.anchorviz.lassoedPointIDs
         for callback in self._selected_points_change_callbacks:
             callback(selected_ids)
 
+    def _update_data_table_on_anchor_change(self, id: str, property: str, value: Any):
+        """Whenever an anchor changes, refresh the data table (this is so that any
+        keyword changes correctly update highlighting)"""
+        # NOTE: unsure if this will cause any "jumping" or lag, if so, look for a keywords
+        # property?
+        self.model.data.update_trigger = True
+
     def on_selected_points_change(self, callback: Callable):
         """Register a callback function for the "anchor added" event.
 
         Callbacks for this event should take a single parameter which is list of
         selected point IDs (strings most likely).
         """
         self._selected_points_change_callbacks.append(callback)
```

### Comparing `icat-iml-0.1.2/icat_iml.egg-info/PKG-INFO` & `icat-iml-0.2.0/icat_iml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icat-iml
-Version: 0.1.2
+Version: 0.2.0
 Summary: Interactive Corpus Analysis Tool
 Home-page: https://github.com/ORNL/icat
 Author: Nathan Martindale, Scott L. Stewart
 Author-email: icat-help@ornl.gov
 Project-URL: Documentation, https://ornl.github.io/icat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `icat-iml-0.1.2/icat_iml.egg-info/SOURCES.txt` & `icat-iml-0.2.0/icat_iml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/setup.py` & `icat-iml-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
     packages=["icat"],
     install_requires=[
-        "panel~=0.14.4",
-        "numpy~=1.23.4",
-        "pandas~=1.5.1",
-        "scikit-learn~=1.1.3",
-        "ipyvuetify~=1.8.4",
-        "ipywidgets<=8.0",
+        "panel",
+        "numpy",
+        "pandas",
+        "scikit-learn",
+        "ipyvuetify",
+        "ipywidgets",
         "ipyanchorviz",
         "altair",
     ],
 )
```

### Comparing `icat-iml-0.1.2/tests/test_anchorlist.py` & `icat-iml-0.2.0/tests/test_anchorlist.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_anchors.py` & `icat-iml-0.2.0/tests/test_anchors.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_datamanager.py` & `icat-iml-0.2.0/tests/test_datamanager.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_histograms.py` & `icat-iml-0.2.0/tests/test_histograms.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_instance.py` & `icat-iml-0.2.0/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_model.py` & `icat-iml-0.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `icat-iml-0.1.2/tests/test_view.py` & `icat-iml-0.2.0/tests/test_view.py`

 * *Files identical despite different names*

