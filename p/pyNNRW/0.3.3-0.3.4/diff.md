# Comparing `tmp/pyNNRW-0.3.3.tar.gz` & `tmp/pyNNRW-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNNRW-0.3.3.tar", last modified: Mon Jul  3 09:52:57 2023, max compression
+gzip compressed data, was "pyNNRW-0.3.4.tar", last modified: Wed Jul  5 11:01:17 2023, max compression
```

## Comparing `pyNNRW-0.3.3.tar` & `pyNNRW-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.716614 pyNNRW-0.3.3/
--rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.3/LICENCE
--rw-rw-rw-   0        0        0     4106 2023-07-03 09:52:57.716614 pyNNRW-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.3/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-07-03 09:52:57.719615 pyNNRW-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.657069 pyNNRW-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.706614 pyNNRW-0.3.3/src/pyNNRW/
--rw-rw-rw-   0        0        0     2044 2023-04-07 01:49:33.000000 pyNNRW-0.3.3/src/pyNNRW/__init__.py
--rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/aerw.py
--rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/dtc.py
--rw-rw-rw-   0        0        0    18109 2023-07-03 09:13:36.000000 pyNNRW-0.3.3/src/pyNNRW/elm.py
--rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/knn.py
--rw-rw-rw-   0        0        0    13110 2023-07-03 09:52:09.000000 pyNNRW-0.3.3/src/pyNNRW/knnrw.py
--rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/lr.py
--rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/mlp.py
--rw-rw-rw-   0        0        0    23963 2023-06-11 14:29:33.000000 pyNNRW-0.3.3/src/pyNNRW/nnrw.py
--rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/rbfnn.py
--rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/rbm.py
--rw-rw-rw-   0        0        0    17134 2023-07-03 09:47:35.000000 pyNNRW-0.3.3/src/pyNNRW/rvfl.py
--rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/wann.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.715614 pyNNRW-0.3.3/src/pyNNRW.egg-info/
--rw-rw-rw-   0        0        0     4106 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.274625 pyNNRW-0.3.4/
+-rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.4/LICENCE
+-rw-rw-rw-   0        0        0     4106 2023-07-05 11:01:17.277629 pyNNRW-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.4/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-07-05 11:01:17.286623 pyNNRW-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 11:01:16.817922 pyNNRW-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.254623 pyNNRW-0.3.4/src/pyNNRW/
+-rw-rw-rw-   0        0        0     2044 2023-04-07 01:49:33.000000 pyNNRW-0.3.4/src/pyNNRW/__init__.py
+-rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/aerw.py
+-rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/dtc.py
+-rw-rw-rw-   0        0        0    18109 2023-07-03 09:13:36.000000 pyNNRW-0.3.4/src/pyNNRW/elm.py
+-rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/knn.py
+-rw-rw-rw-   0        0        0    13110 2023-07-03 09:52:09.000000 pyNNRW-0.3.4/src/pyNNRW/knnrw.py
+-rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/lr.py
+-rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/mlp.py
+-rw-rw-rw-   0        0        0    24246 2023-07-05 10:32:40.000000 pyNNRW-0.3.4/src/pyNNRW/nnrw.py
+-rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/rbfnn.py
+-rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/rbm.py
+-rw-rw-rw-   0        0        0    17215 2023-07-05 05:52:42.000000 pyNNRW-0.3.4/src/pyNNRW/rvfl.py
+-rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/wann.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.269621 pyNNRW-0.3.4/src/pyNNRW.egg-info/
+-rw-rw-rw-   0        0        0     4106 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/top_level.txt
```

### Comparing `pyNNRW-0.3.3/PKG-INFO` & `pyNNRW-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyNNRW-0.3.3/README.md` & `pyNNRW-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/setup.cfg` & `pyNNRW-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 794e 4e52 570d 0a76 6572 7369   = pyNNRW..versi
-00000020: 6f6e 203d 2030 2e33 2e33 0d0a 6175 7468  on = 0.3.3..auth
+00000020: 6f6e 203d 2030 2e33 2e34 0d0a 6175 7468  on = 0.3.4..auth
 00000030: 6f72 203d 2059 696e 7368 656e 6720 5a68  or = Yinsheng Zh
 00000040: 616e 6720 2850 682e 442e 290d 0a61 7574  ang (Ph.D.)..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6f6f 407a  hor_email = oo@z
 00000060: 6a75 2e65 6475 2e63 6e0d 0a64 6573 6372  ju.edu.cn..descr
 00000070: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
 00000080: 6e20 6c69 6272 6172 7920 666f 7220 4e4e  n library for NN
 00000090: 5257 2028 6e65 7572 616c 206e 6574 776f  RW (neural netwo
```

### Comparing `pyNNRW-0.3.3/src/pyNNRW/__init__.py` & `pyNNRW-0.3.4/src/pyNNRW/__init__.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/dtc.py` & `pyNNRW-0.3.4/src/pyNNRW/dtc.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/elm.py` & `pyNNRW-0.3.4/src/pyNNRW/elm.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/knnrw.py` & `pyNNRW-0.3.4/src/pyNNRW/knnrw.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/mlp.py` & `pyNNRW-0.3.4/src/pyNNRW/mlp.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/nnrw.py` & `pyNNRW-0.3.4/src/pyNNRW/nnrw.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,21 +445,22 @@
         return yp
     
     def score(self, X, y):
         X = np.nan_to_num(X)
         y = np.nan_to_num(y)
         return LogisticRegression.score(X=X, y=y)   
 
-def homo_stacking(X, y, create_base_estimator, meta_learner = LogisticRegressionX,
+def homo_stacking(X, y, create_base_estimator, 
+                  meta_learner = LogisticRegressionX,
                   Ns = [1, 2, 5], Ls = [1, 2, 5, 10, 20], 
-                  test_size = .3, 
+                  test_size = .3,
                   random_state = None,
-                  WITH_CONTEXT = False, 
+                  WITH_CONTEXT = False,
                   xlabel = '',
-                  YLIM = (.5, 1.05)):
+                  YLIM = None):
     '''
     create_base_estimator # a function that create base learner instanes
     Ns = [1, 2, 5] # number of base estimators
     Ls = [1, 2, 5, 10, 20] # base learner's specific hyper-parameter    
     '''
 
     # pbar = tqdm(total = repeat * len(Ns) * len(Ls), position=0, leave=True) # stay on top
@@ -472,15 +473,15 @@
     repeat = 1 # no need to repeat, each run is now deterministic.
 
     plt.figure(figsize = (14, 6))
 
     for N in Ns:
         ACCs = []
 
-        for L in Ls:        
+        for L in Ls:
 
             accs = []
 
             for _ in range(repeat):
 
                 estimators = []
                 for i in range(N):
@@ -504,18 +505,25 @@
             ACCs.append(averaged_acc)
             dic_acc[(N, L)] = averaged_acc
 
         plt.plot(Ls, ACCs, '--', label = 'N='+str(N), marker='o') # fillstyle='none'
         # plt.scatter(Ls, ACCs, s = 50)
 
     plt.gca().xaxis.set_major_locator(mticker.MultipleLocator(1)) # only show integer
+    plt.gca().yaxis.set_major_locator(mticker.MultipleLocator(.1)) # only show integer
+    
+    Ls = np.array(Ls)
+    plt.xlim( (Ls.min() - .5, Ls.max() + .5) )
     plt.legend()
     plt.xlabel('Hyper-parameter' + xlabel)
     plt.ylabel("Classfication Accuracy")
-    plt.ylim(YLIM)
+    if YLIM is None:
+        plt.ylim( (np.min(list(dic_acc.values())) - .05, 1.05) )
+    else:
+        plt.ylim(YLIM) # e.g., (.4, 1.05)
     plt.show()
 
     print('best test accuracy: ', max(dic_acc.values()), 'N, L = ', [key for key, value in dic_acc.items() if value == max(dic_acc.values())])
 
     return dic_acc
     
 def hetero_stacking(X, y, estimators, repeat = 10, WITH_CONTEXT = True):
```

### Comparing `pyNNRW-0.3.3/src/pyNNRW/rbfnn.py` & `pyNNRW-0.3.4/src/pyNNRW/rbfnn.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/rbm.py` & `pyNNRW-0.3.4/src/pyNNRW/rbm.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW/rvfl.py` & `pyNNRW-0.3.4/src/pyNNRW/rvfl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class RVFL:
     """
     A simple RVFL classifier or regression.
     This implementation is based on https://github.com/Xuyang-Huang/Simple-RVFL-python/tree/main
 
     Attributes:
         n_nodes: An integer of enhancement node number.
-        lam: A floating number of regularization parameter.
+        lam: A floating number of regularization parameter. Controls the direct-link strength.
         w_random_vec_range: A list, [min, max], the range of generating random weights.
         b_random_vec_range: A list, [min, max], the range of generating random bias.
         random_weights: A Numpy array shape is [n_feature, n_nodes], weights of neuron.
         random_bias: A Numpy array shape is [n_nodes], bias of neuron.
         beta: A Numpy array shape is [n_feature + n_nodes, n_class], the projection matrix.
         activation: A string of activation name.
         data_std: A list, store normalization parameters for each layer.
@@ -27,24 +27,24 @@
     """
     def __init__(self, n_nodes, lam, w_random_vec_range = [-1, 1], 
                  b_random_vec_range = [0, 1], activation = 'sigmoid', 
                  same_feature=False,
                  task_type='classification'):
         assert task_type in ['classification', 'regression'], 'task_type should be "classification" or "regression".'
         self.n_nodes = n_nodes
-        self.lam = lam
+        self.lam = lam # controls the direct-link strength
         self.w_random_range = w_random_vec_range
         self.b_random_range = b_random_vec_range
         self.random_weights = None
         self.random_bias = None
         self.beta = None
         a = Activation()
         self.activation_function = getattr(a, activation)
-        self.data_std = None
-        self.data_mean = None
+        # self.data_std = None
+        # self.data_mean = None
         self.same_feature = same_feature
         self.task_type = task_type
 
     def train(self, data, label, n_class):
         """
 
         :param data: Training data.
@@ -53,15 +53,15 @@
         :return: No return
         """
 
         assert len(data.shape) > 1, 'Data shape should be [n, dim].'
         assert len(data) == len(label), 'Label number does not match data number.'
         assert len(label.shape) == 1, 'Label should be 1-D array.'
 
-        data = self.standardize(data)  # Normalization data
+        # data = self.standardize(data)  # Normalization data
         n_sample = len(data) #样本数量
         n_feature = len(data[0]) #特征数量
         self.random_weights = self.get_random_vectors(n_feature, self.n_nodes, self.w_random_range) #构成随机权重值
         self.random_bias = self.get_random_vectors(1, self.n_nodes, self.b_random_range) #构成随机偏置值
         
         #点积，并添加偏置项，使用激活函数处理，得到激活值h
         h = self.activation_function(np.dot(data, self.random_weights) + np.dot(np.ones([n_sample, 1]), self.random_bias))
@@ -79,15 +79,15 @@
     def predict(self, data):
         """
 
         :param data: Predict data.
         :return: When classification, return Prediction result and probability.
                  When regression, return the output of rvfl.
         """
-        data = self.standardize(data)  # Normalization data
+        # data = self.standardize(data)  # Normalization data
         h = self.activation_function(np.dot(data, self.random_weights) + self.random_bias)
         d = np.concatenate([h, data], axis=1)
         d = np.concatenate([d, np.ones_like(d[:, 0:1])], axis=1)
         output = np.dot(d, self.beta)
         if self.task_type == 'classification':
             proba = self.softmax(output)
             result = np.argmax(proba, axis=1)
@@ -104,15 +104,15 @@
                  When regression return MAE.
         """
 
         assert len(data.shape) > 1, 'Data shape should be [n, dim].'
         assert len(data) == len(label), 'Label number does not match data number.'
         assert len(label.shape) == 1, 'Label should be 1-D array.'
 
-        data = self.standardize(data)  # Normalization data
+        # data = self.standardize(data)  # Normalization data
         h = self.activation_function(np.dot(data, self.random_weights) + self.random_bias)
         d = np.concatenate([h, data], axis=1)
         d = np.concatenate([d, np.ones_like(d[:, 0:1])], axis=1)
         output = np.dot(d, self.beta)
         if self.task_type == 'classification':
             result = np.argmax(output, axis=1)
             acc = np.sum(np.equal(result, label)) / len(label)
```

### Comparing `pyNNRW-0.3.3/src/pyNNRW/wann.py` & `pyNNRW-0.3.4/src/pyNNRW/wann.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.3/src/pyNNRW.egg-info/PKG-INFO` & `pyNNRW-0.3.4/src/pyNNRW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

