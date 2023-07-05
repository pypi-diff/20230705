# Comparing `tmp/antm-0.1.1.tar.gz` & `tmp/antm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antm-0.1.1.tar", last modified: Thu Feb 16 17:14:16 2023, max compression
+gzip compressed data, was "antm-0.1.2.tar", last modified: Wed Jul  5 09:37:58 2023, max compression
```

## Comparing `antm-0.1.1.tar` & `antm-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-02-16 17:14:16.596743 antm-0.1.1/
--rw-r--r--   0 hamed      (501) staff       (20)     1068 2023-02-08 01:50:11.000000 antm-0.1.1/LICENSE
--rw-r--r--   0 hamed      (501) staff       (20)     5288 2023-02-16 17:14:16.596633 antm-0.1.1/PKG-INFO
--rw-r--r--   0 hamed      (501) staff       (20)     4688 2023-02-16 17:14:08.000000 antm-0.1.1/README.md
-drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-02-16 17:14:16.595858 antm-0.1.1/antm/
--rw-r--r--   0 hamed      (501) staff       (20)       24 2023-02-11 06:26:53.000000 antm-0.1.1/antm/__init__.py
--rw-r--r--   0 hamed      (501) staff       (20)     5117 2023-02-16 15:25:43.000000 antm-0.1.1/antm/aligned_clustering_layer.py
--rw-r--r--   0 hamed      (501) staff       (20)      343 2023-02-15 12:34:42.000000 antm-0.1.1/antm/cm.py
--rw-r--r--   0 hamed      (501) staff       (20)      410 2023-02-16 10:26:26.000000 antm-0.1.1/antm/contextual_embedding_layer.py
--rw-r--r--   0 hamed      (501) staff       (20)     2700 2022-12-22 04:37:17.000000 antm-0.1.1/antm/ctfidf.py
--rw-r--r--   0 hamed      (501) staff       (20)     1193 2023-02-16 10:58:11.000000 antm-0.1.1/antm/data2vec.py
--rw-r--r--   0 hamed      (501) staff       (20)     1183 2023-02-15 12:46:36.000000 antm-0.1.1/antm/diversity_metrics.py
--rw-r--r--   0 hamed      (501) staff       (20)    12290 2023-02-16 17:10:58.000000 antm-0.1.1/antm/main.py
--rw-r--r--   0 hamed      (501) staff       (20)     2170 2023-02-16 14:31:43.000000 antm-0.1.1/antm/sws.py
--rw-r--r--   0 hamed      (501) staff       (20)     1762 2023-02-15 13:13:56.000000 antm-0.1.1/antm/text_processing.py
--rw-r--r--   0 hamed      (501) staff       (20)     2025 2023-02-16 15:55:14.000000 antm-0.1.1/antm/topic_representation_layer.py
-drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-02-16 17:14:16.596485 antm-0.1.1/antm.egg-info/
--rw-r--r--   0 hamed      (501) staff       (20)     5288 2023-02-16 17:14:16.000000 antm-0.1.1/antm.egg-info/PKG-INFO
--rw-r--r--   0 hamed      (501) staff       (20)      403 2023-02-16 17:14:16.000000 antm-0.1.1/antm.egg-info/SOURCES.txt
--rw-r--r--   0 hamed      (501) staff       (20)        1 2023-02-16 17:14:16.000000 antm-0.1.1/antm.egg-info/dependency_links.txt
--rw-r--r--   0 hamed      (501) staff       (20)      109 2023-02-16 17:14:16.000000 antm-0.1.1/antm.egg-info/requires.txt
--rw-r--r--   0 hamed      (501) staff       (20)        5 2023-02-16 17:14:16.000000 antm-0.1.1/antm.egg-info/top_level.txt
--rw-r--r--   0 hamed      (501) staff       (20)       38 2023-02-16 17:14:16.596777 antm-0.1.1/setup.cfg
--rw-r--r--   0 hamed      (501) staff       (20)      983 2023-02-16 17:12:45.000000 antm-0.1.1/setup.py
+drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-07-05 09:37:58.296102 antm-0.1.2/
+-rw-r--r--   0 hamed      (501) staff       (20)     1068 2023-02-08 01:50:11.000000 antm-0.1.2/LICENSE
+-rw-r--r--   0 hamed      (501) staff       (20)     5288 2023-07-05 09:37:58.295989 antm-0.1.2/PKG-INFO
+-rw-r--r--   0 hamed      (501) staff       (20)     4688 2023-02-16 17:14:08.000000 antm-0.1.2/README.md
+drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-07-05 09:37:58.295173 antm-0.1.2/antm/
+-rw-r--r--   0 hamed      (501) staff       (20)       24 2023-06-30 00:31:22.000000 antm-0.1.2/antm/__init__.py
+-rw-r--r--   0 hamed      (501) staff       (20)     5117 2023-02-16 15:25:43.000000 antm-0.1.2/antm/aligned_clustering_layer.py
+-rw-r--r--   0 hamed      (501) staff       (20)      343 2023-02-15 12:34:42.000000 antm-0.1.2/antm/cm.py
+-rw-r--r--   0 hamed      (501) staff       (20)      410 2023-06-30 00:31:22.000000 antm-0.1.2/antm/contextual_embedding_layer.py
+-rw-r--r--   0 hamed      (501) staff       (20)     2700 2023-06-30 00:31:22.000000 antm-0.1.2/antm/ctfidf.py
+-rw-r--r--   0 hamed      (501) staff       (20)     1193 2023-06-30 00:31:22.000000 antm-0.1.2/antm/data2vec.py
+-rw-r--r--   0 hamed      (501) staff       (20)     1183 2023-06-30 00:31:22.000000 antm-0.1.2/antm/diversity_metrics.py
+-rw-r--r--   0 hamed      (501) staff       (20)    13016 2023-06-30 00:31:22.000000 antm-0.1.2/antm/main.py
+-rw-r--r--   0 hamed      (501) staff       (20)     2170 2023-06-30 00:31:22.000000 antm-0.1.2/antm/sws.py
+-rw-r--r--   0 hamed      (501) staff       (20)     1762 2023-06-30 00:31:22.000000 antm-0.1.2/antm/text_processing.py
+-rw-r--r--   0 hamed      (501) staff       (20)     2025 2023-06-30 00:31:22.000000 antm-0.1.2/antm/topic_representation_layer.py
+drwxr-xr-x   0 hamed      (501) staff       (20)        0 2023-07-05 09:37:58.295827 antm-0.1.2/antm.egg-info/
+-rw-r--r--   0 hamed      (501) staff       (20)     5288 2023-07-05 09:37:58.000000 antm-0.1.2/antm.egg-info/PKG-INFO
+-rw-r--r--   0 hamed      (501) staff       (20)      403 2023-07-05 09:37:58.000000 antm-0.1.2/antm.egg-info/SOURCES.txt
+-rw-r--r--   0 hamed      (501) staff       (20)        1 2023-07-05 09:37:58.000000 antm-0.1.2/antm.egg-info/dependency_links.txt
+-rw-r--r--   0 hamed      (501) staff       (20)      109 2023-07-05 09:37:58.000000 antm-0.1.2/antm.egg-info/requires.txt
+-rw-r--r--   0 hamed      (501) staff       (20)        5 2023-07-05 09:37:58.000000 antm-0.1.2/antm.egg-info/top_level.txt
+-rw-r--r--   0 hamed      (501) staff       (20)       38 2023-07-05 09:37:58.296138 antm-0.1.2/setup.cfg
+-rw-r--r--   0 hamed      (501) staff       (20)      983 2023-07-05 09:36:16.000000 antm-0.1.2/setup.py
```

### Comparing `antm-0.1.1/LICENSE` & `antm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/PKG-INFO` & `antm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Aligned Neural Topic Model for Exploring Evolving Topics
 Home-page: https://github.com/hamedR96/ANTM
 Author: Hamed Rahimi
 Author-email: <hamed.rahimi@sorbonne-universite.fr
 Project-URL: Bug Tracker, https://github.com/hamedR96/ANTM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `antm-0.1.1/README.md` & `antm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/aligned_clustering_layer.py` & `antm-0.1.2/antm/aligned_clustering_layer.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/ctfidf.py` & `antm-0.1.2/antm/ctfidf.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/data2vec.py` & `antm-0.1.2/antm/data2vec.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/diversity_metrics.py` & `antm-0.1.2/antm/diversity_metrics.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/main.py` & `antm-0.1.2/antm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from antm.sws import sws
 from antm.contextual_embedding_layer import contextual_embedding
 from antm.topic_representation_layer import rep_prep,ctfidf_rp, topic_evolution
 from antm.cm import coherence_model
 from antm.diversity_metrics import proportion_unique_words,pairwise_jaccard_diversity
 
 class ANTM:
-    def __init__(self, df, overlap, window_length, mode="data2vec", umap_dimension_size=5, umap_n_neighbors=15,
+    def __init__(self, df, overlap, window_length, mode="data2vec", umap_dimension_size=5, umap_n_neighbors=15, df_embedded=None, umap_embeddings_clustering=None, umap_embeddings_visulization=None,
                  partioned_clusttering_size=10, num_words=10, show_2d_plot=False,path=os.getcwd()):
         self.df = df
         self.overlap = overlap
         self.window_length = window_length
         self.mode = mode
         self.umap_dimension_size = umap_dimension_size
         self.umap_n_neighbors = umap_n_neighbors
@@ -27,17 +27,17 @@
         self.num_words = num_words
         self.show_2d_plot = show_2d_plot
 
         if not path== os.getcwd():
             if not os.path.exists(path): os.mkdir(path)
         self.path = path
 
-        self.df_embedded = None
-        self.umap_embeddings_clustering = None
-        self.umap_embeddings_visulization = None
+        self.df_embedded = df_embedded
+        self.umap_embeddings_clustering = umap_embeddings_clustering
+        self.umap_embeddings_visulization = umap_embeddings_visulization
         self.clusters=None
         self.slices=None
         self.arg1_umap=None
         self.arg2_umap=None
         self.cluster_df=None
         self.clustered_df_cent=None
         self.clustered_np_cent=None
@@ -54,44 +54,61 @@
         self.topics=None
         self.slice_num=None
 
         self.periodwise_puw_diversity=None
         self.periodwise_pairwise_jaccard_diversity=None
         self.periodwise_topic_coherence=None
 
-    def fit(self,save=True):
-        print("contextual document embedding is initiated...")
-        self.df_embedded = contextual_embedding(self.df, mode=self.mode)
+    def fit(self, save=True):
+
+        # Contextual embedding
+        if self.df_embedded is None:
+            print("contextual document embedding is initiated...")
+            self.df_embedded = contextual_embedding(self.df, mode=self.mode)
+        else:
+            print("contextual document embedding provided ---> skip")
+
+        # Sliding window segmentation
         print("Sliding Window Segmentation is initialized...")
         self.slices, self.arg1_umap, self.arg2_umap = sws(self.df_embedded, self.overlap, self.window_length)
-        print("Aligned Dimension Reduction is initialized...")
-        self.umap_embeddings_clustering, self.umap_embeddings_visulization = aligned_umap(
-            self.arg1_umap, self.arg2_umap, n_neighbors=self.umap_n_neighbors,
-            umap_dimension_size=self.umap_dimension_size)
+
+        # Aligned dimensionality reduction
+        if self.umap_embeddings_clustering is None or self.umap_embeddings_visulization is None:
+            print("Aligned Dimension Reduction is initialized...")
+            self.umap_embeddings_clustering, self.umap_embeddings_visulization = aligned_umap(
+                self.arg1_umap, self.arg2_umap, n_neighbors=self.umap_n_neighbors,
+                umap_dimension_size=self.umap_dimension_size)
+        else:
+            print("umap embeddings provided ---> skip")
+
         print("Sequential Document-cluster association is initialized...")
-        self.clusters = hdbscan_cluster(self.umap_embeddings_clustering, self.partioned_clusttering_size)
-        if not os.path.exists(self.path+"/results"): os.mkdir(self.path+"/results")
+        self.clusters = hdbscan_cluster(self.umap_embeddings_clustering,
+                                                            self.partioned_clusttering_size)
+        if not os.path.exists(self.path + "/results"): os.mkdir(self.path + "/results")
         for i in range(len(self.clusters)):
             draw_cluster(self.clusters[i], self.umap_embeddings_visulization[i], "time_frame_" + str(i),
-                         show_2d_plot=self.show_2d_plot,path=self.path)
+                         show_2d_plot=self.show_2d_plot, path=self.path)
         self.cluster_df = clustered_df(self.slices, self.clusters)
         self.clustered_df_cent, self.clustered_np_cent = clustered_cent_df(self.cluster_df)
         self.dt, self.concat_cent = dt_creator(self.clustered_df_cent)
         print("Cluster Alignment Procedure is initialized...")
         self.df_tm = alignment_procedure(self.dt, self.concat_cent)
-        self.list_tm = plot_alignment(self.df_tm, self.umap_embeddings_visulization, self.clusters,self.path)
+        self.list_tm = plot_alignment(self.df_tm, self.umap_embeddings_visulization, self.clusters, self.path)
         self.documents_per_topic_per_time = rep_prep(self.cluster_df)
         self.tokens, self.dictionary, self.corpus = text_processing(self.df.content.values)
         print("Topic Representation is initialized...")
-        self.output = ctfidf_rp(self.dictionary, self.documents_per_topic_per_time, num_doc=len(self.df), num_words=self.num_words)
+        self.output = ctfidf_rp(self.dictionary, self.documents_per_topic_per_time, num_doc=len(self.df),
+                                num_words=self.num_words)
         print("Topic Modeling is done")
-        self.evolving_topics=topic_evolution(self.list_tm, self.output)
+        self.evolving_topics = topic_evolution(self.list_tm, self.output)
         if save: self.save()
-        self.slice_num = len(set(self.output["slice_num"]))
-        self.topics = [self.output[self.output["slice_num"] == i].topic_representation.to_list() for i in range(1, self.slice_num + 1)]
+        self.slice_num = set(self.output["slice_num"])
+        self.topics = [self.output[self.output["slice_num"] == i].topic_representation.to_list() for i in
+                       self.slice_num]
+        self.topics = list(filter(None, self.topics))
         return self.topics
 
     def save(self):
         print("Model is saving...")
         if not os.path.exists(self.path+"/model"): os.mkdir(self.path+"/model")
 
         self.df_embedded.to_pickle(self.path+"/model/embedding_df")
```

### Comparing `antm-0.1.1/antm/sws.py` & `antm-0.1.2/antm/sws.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/text_processing.py` & `antm-0.1.2/antm/text_processing.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm/topic_representation_layer.py` & `antm-0.1.2/antm/topic_representation_layer.py`

 * *Files identical despite different names*

### Comparing `antm-0.1.1/antm.egg-info/PKG-INFO` & `antm-0.1.2/antm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Aligned Neural Topic Model for Exploring Evolving Topics
 Home-page: https://github.com/hamedR96/ANTM
 Author: Hamed Rahimi
 Author-email: <hamed.rahimi@sorbonne-universite.fr
 Project-URL: Bug Tracker, https://github.com/hamedR96/ANTM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `antm-0.1.1/setup.py` & `antm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antm',
-    version='0.1.1',
+    version='0.1.2',
     author='Hamed Rahimi',
     author_email='<hamed.rahimi@sorbonne-universite.fr',
     description='Aligned Neural Topic Model for Exploring Evolving Topics',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/hamedR96/ANTM',
     packages=find_packages(),
```

