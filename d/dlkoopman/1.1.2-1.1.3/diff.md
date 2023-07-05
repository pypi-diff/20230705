# Comparing `tmp/dlkoopman-1.1.2.tar.gz` & `tmp/dlkoopman-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlkoopman-1.1.2.tar", max compression
+gzip compressed data, was "dlkoopman-1.1.3.tar", max compression
```

## Comparing `dlkoopman-1.1.2.tar` & `dlkoopman-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2022-09-14 20:03:37.378852 dlkoopman-1.1.2/LICENSE
--rw-r--r--   0        0        0     6465 2023-02-28 15:51:18.006168 dlkoopman-1.1.2/README.md
--rw-r--r--   0        0        0      228 2023-02-24 18:00:10.916845 dlkoopman-1.1.2/dlkoopman/__init__.py
--rw-r--r--   0        0        0     5112 2023-02-24 18:00:10.917757 dlkoopman-1.1.2/dlkoopman/config.py
--rw-r--r--   0        0        0    13228 2023-02-24 18:00:10.918081 dlkoopman-1.1.2/dlkoopman/hyp_search.py
--rw-r--r--   0        0        0     5243 2023-02-24 18:00:10.918947 dlkoopman-1.1.2/dlkoopman/metrics.py
--rw-r--r--   0        0        0     4888 2023-02-24 18:00:10.919606 dlkoopman-1.1.2/dlkoopman/nets.py
--rw-r--r--   0        0        0    30268 2023-02-24 18:00:10.920670 dlkoopman-1.1.2/dlkoopman/state_pred.py
--rw-r--r--   0        0        0    22638 2023-02-24 18:00:10.921709 dlkoopman-1.1.2/dlkoopman/traj_pred.py
--rw-r--r--   0        0        0     6546 2023-02-24 18:00:10.922357 dlkoopman-1.1.2/dlkoopman/utils.py
--rw-r--r--   0        0        0      935 2023-02-28 15:50:12.160841 dlkoopman-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 dlkoopman-1.1.2/setup.py
--rw-r--r--   0        0        0     7673 1970-01-01 00:00:00.000000 dlkoopman-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-09-14 20:03:37.378852 dlkoopman-1.1.3/LICENSE
+-rw-r--r--   0        0        0     6585 2023-07-05 14:36:02.796801 dlkoopman-1.1.3/README.md
+-rw-r--r--   0        0        0      228 2023-02-24 18:00:10.916845 dlkoopman-1.1.3/dlkoopman/__init__.py
+-rw-r--r--   0        0        0     5112 2023-02-24 18:00:10.917757 dlkoopman-1.1.3/dlkoopman/config.py
+-rw-r--r--   0        0        0    13228 2023-02-24 18:00:10.918081 dlkoopman-1.1.3/dlkoopman/hyp_search.py
+-rw-r--r--   0        0        0     5243 2023-02-24 18:00:10.918947 dlkoopman-1.1.3/dlkoopman/metrics.py
+-rw-r--r--   0        0        0     4888 2023-02-24 18:00:10.919606 dlkoopman-1.1.3/dlkoopman/nets.py
+-rw-r--r--   0        0        0    30268 2023-02-24 18:00:10.920670 dlkoopman-1.1.3/dlkoopman/state_pred.py
+-rw-r--r--   0        0        0    22638 2023-02-24 18:00:10.921709 dlkoopman-1.1.3/dlkoopman/traj_pred.py
+-rw-r--r--   0        0        0     6546 2023-02-24 18:00:10.922357 dlkoopman-1.1.3/dlkoopman/utils.py
+-rw-r--r--   0        0        0      935 2023-07-05 14:36:02.797182 dlkoopman-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7586 1970-01-01 00:00:00.000000 dlkoopman-1.1.3/setup.py
+-rw-r--r--   0        0        0     7793 1970-01-01 00:00:00.000000 dlkoopman-1.1.3/PKG-INFO
```

### Comparing `dlkoopman-1.1.2/LICENSE` & `dlkoopman-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/README.md` & `dlkoopman-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```
 git clone https://github.com/GaloisInc/dlkoopman.git
 cd dlkoopman
 pip install .
 ```
 
 ### Running as a Docker container
-DLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.2`.
+DLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.3`.
 
 
 ## Tutorials and examples
 Available in the [`examples`](https://github.com/GaloisInc/dlkoopman/tree/ed11bef92b90112d9ca90722942a6789e6af7d5a/examples) folder.
 
 
 ## Documentation and API Reference
@@ -86,22 +86,26 @@
 
 
 ## Known issues
 Some common issues and ways to overcome them are described in the [known issues](https://github.com/GaloisInc/dlkoopman/issues?q=is%3Aissue+is%3Aclosed+label%3Aknown-issue).
 
 
 ## How to cite
-Please cite the [accompanying paper](https://arxiv.org/abs/2211.08992):
+Please cite the [accompanying paper](https://proceedings.mlr.press/v211/dey23a.html):
 ```
-@article{Dey2022_dlkoopman,
+@inproceedings{Dey2023_L4DC,
     author = {Sourya Dey and Eric William Davis},
-    title = {DLKoopman: A deep learning software package for Koopman theory},
-    journal = {arXiv preprint arXiv:2211.08992},
-    year = {2022},
-    note = {Submitted to 5th Annual Learning for Dynamics & Control (L4DC) Conference}
+    title = {{DLKoopman: A deep learning software package for Koopman theory}},
+    booktitle = {Proceedings of The 5th Annual Learning for Dynamics and Control Conference},
+    pages = {1467--1479},
+    volume = {211},
+    series = {Proceedings of Machine Learning Research},
+    publisher = {PMLR},
+    year = {2023},
+    month = {Jun}
 }
 ```
 
 
 ## References
 - B. O. Koopman - Hamiltonian systems and transformation in Hilbert space
 - J. Nathan Kutz, Steven L. Brunton, Bingni Brunton, Joshua L. Proctor - Dynamic Mode Decomposition
```

### Comparing `dlkoopman-1.1.2/dlkoopman/config.py` & `dlkoopman-1.1.3/dlkoopman/config.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/hyp_search.py` & `dlkoopman-1.1.3/dlkoopman/hyp_search.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/metrics.py` & `dlkoopman-1.1.3/dlkoopman/metrics.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/nets.py` & `dlkoopman-1.1.3/dlkoopman/nets.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/state_pred.py` & `dlkoopman-1.1.3/dlkoopman/state_pred.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/traj_pred.py` & `dlkoopman-1.1.3/dlkoopman/traj_pred.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/dlkoopman/utils.py` & `dlkoopman-1.1.3/dlkoopman/utils.py`

 * *Files identical despite different names*

### Comparing `dlkoopman-1.1.2/pyproject.toml` & `dlkoopman-1.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlkoopman"
-version = "1.1.2"
+version = "1.1.3"
 description = "A general-purpose Python package for Koopman theory using deep learning."
 authors = ["Sourya Dey <sourya@galois.com>"]
 maintainers = ["Galois dlkoopman team <dlkoopman@galois.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/GaloisInc/dlkoopman"
 documentation = "https://galoisinc.github.io/dlkoopman/"
```

### Comparing `dlkoopman-1.1.2/setup.py` & `dlkoopman-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'pandas>=1.2.3,<2.0.0',
  'shortuuid>=1.0.9,<2.0.0',
  'torch>=1.12.1,<2.0.0',
  'tqdm>=4.61.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'dlkoopman',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'A general-purpose Python package for Koopman theory using deep learning.',
-    'long_description': '<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/36108ffcfd9608a393985ac9af431d3910fe2fc5/logo.png" height=150/>\n</figure>\n\n**DLKoopman: A general-purpose Python package for Koopman theory using deep learning**.\n\nKoopman theory is a technique to encode sampled data (aka states) of a nonlinear dynamical system into a linear domain. This is very powerful as a linear model can:\n- Give insight into the dynamics via eigenvalues and eigenvectors.\n- Leverage linear algebra techniques to easily analyze the system and predict its behavior under unknown conditions.\n\n\n## Why DLKoopman?\n*DLKoopman uses deep learning to learn an encoding of a nonlinear dynamical system into a linear domain, while simultaneously learning the dynamics of the linear model*. DLKoopman bridges the gap between:\n- Software packages that restrict the learning of a good encoding (e.g. [`pykoopman`](https://github.com/dynamicslab/pykoopman)), and\n- Efforts that learn encodings for specific applications instead of being a general-purpose tool (e.g. [`DeepKoopman`](https://github.com/BethanyL/DeepKoopman)).\n\n### Key DLKoopman features\n- State prediction (`StatePred`) - Train on individual states of a system, then predict unknown states.\n    - E.g: What is the pressure vector on this aircraft for $23.5^{\\circ}$ angle of attack?\n- Trajectory prediction (`TrajPred`) - Train on generated trajectories of a system, then predict unknown trajectories for new initial states.\n    - E.g: What is the behavior of this pendulum if I start from the point $[1,-1]$?\n- General-purpose and reusable - supports data from any dynamical system.\n- Novel error function Average Normalized Absolute Error (ANAE) for visualizing performance.\n- Extensive options and a ready-to-use hyperparameter search module to improve performance.\n- Built using [Pytorch](https://pytorch.org/), supports both CPU and GPU platforms.\n\nRead more about DLKoopman in this [blog article](https://galois.com/blog/2023/01/dl-koopman/).\n\n\n## Installation\n\n### With pip (for regular users)\n`pip install dlkoopman`\n\n### From source (for development)\n```\ngit clone https://github.com/GaloisInc/dlkoopman.git\ncd dlkoopman\npip install .\n```\n\n### Running as a Docker container\nDLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.2`.\n\n\n## Tutorials and examples\nAvailable in the [`examples`](https://github.com/GaloisInc/dlkoopman/tree/ed11bef92b90112d9ca90722942a6789e6af7d5a/examples) folder.\n\n\n## Documentation and API Reference\nAvailable at https://galoisinc.github.io/dlkoopman/.\n\n## Changelog\nSee [Releases](https://github.com/GaloisInc/dlkoopman/releases) and their notes.\n\n\n## Description \n\n### Koopman theory\nAssume a dynamical system $x_{i+1} = F(x_i)$, where $x$ is the (genrally multi-dimensional) state of the system at index $i$, and $F$ is the (generally nonlinear) evolution rule describing the dynamics of the system. Koopman theory attempts to *encode* $x$ into a different space $y = g(x)$ where the dynamics are linear, i.e. $y_{i+1} = Ky_i$, where $K$ is the Koopman matrix. This is incredibly powerful since the state $y_i$ at any index $i$ can be predicted from the initial state $y_0$ as $y_i = K^iy_0$. This is then *decoded* back into the original space as $x = g^{-1}(y)$.\n\nFor a thorough mathematical treatment, see [this technical report](https://arxiv.org/abs/2211.07561).\n\n### dlkoopman training\n<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/ed11bef92b90112d9ca90722942a6789e6af7d5a/training_architecture.png" width=750/>\n</figure>\n\nThis is a small example with three input states $\\left[x_0, x_1, x_2\\right]$. These are passed through an encoder neural network to get encoded states $\\left[y_0, y_1, y_2\\right]$. These are passed through a decoder neural network to get $\\left[\\hat{x}_0, \\hat{x}_1, \\hat{x}_2\\right]$, and also used to learn $K$. This is used to derive predicted encoded states $\\left[\\mathsf{y}_1, \\mathsf{y}_2\\right]$, which are then passed through the same decoder to get predicted approximations $\\left[\\hat{\\mathsf{x}}_1, \\hat{\\mathsf{x}}_2\\right]$ to the original input states.\n\nErrors mimimized during training:\n- Train the autoencoder - Reconstruction `recon` between $x$ and $\\hat{x}$.\n- Train the Koopman matrix - Linearity `lin` between $y$ and $\\mathsf{y}$.\n- Combine the above - Prediction `pred` between $x$ and $\\hat{\\mathsf{x}}$.\n\n### dlkoopman prediction\n<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/ed11bef92b90112d9ca90722942a6789e6af7d5a/prediction_architecture.png" width=750/>\n</figure>\n\nPrediction happens after training.\n\n(a) State prediction - Compute predicted states for new indexes such as $i\'$. This uses the eigendecomposition of $K$, so $i\'$ can be any real number - positive (forward extapolation), negative (backward extrapolation), or fractional (interpolation).\n\n(b) Trajectory prediction - Generate predicted trajectories $j\'$ for new starting states such as $x^{j\'}_0$. This uses a linear neural net layer to evolve the initial state.\n\n\n## Known issues\nSome common issues and ways to overcome them are described in the [known issues](https://github.com/GaloisInc/dlkoopman/issues?q=is%3Aissue+is%3Aclosed+label%3Aknown-issue).\n\n\n## How to cite\nPlease cite the [accompanying paper](https://arxiv.org/abs/2211.08992):\n```\n@article{Dey2022_dlkoopman,\n    author = {Sourya Dey and Eric William Davis},\n    title = {DLKoopman: A deep learning software package for Koopman theory},\n    journal = {arXiv preprint arXiv:2211.08992},\n    year = {2022},\n    note = {Submitted to 5th Annual Learning for Dynamics & Control (L4DC) Conference}\n}\n```\n\n\n## References\n- B. O. Koopman - Hamiltonian systems and transformation in Hilbert space\n- J. Nathan Kutz, Steven L. Brunton, Bingni Brunton, Joshua L. Proctor - Dynamic Mode Decomposition\n- Bethany Lusch, J. Nathan Kutz & Steven L. Brunton - Deep learning for universal linear embeddings of nonlinear dynamics\n\n\n## Distribution Statement\nThis material is based upon work supported by the United States Air Force and DARPA under Contract No. FA8750-20-C-0534. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the United States Air Force and DARPA. Distribution Statement A, "Approved for Public Release, Distribution Unlimited."\n',
+    'long_description': '<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/36108ffcfd9608a393985ac9af431d3910fe2fc5/logo.png" height=150/>\n</figure>\n\n**DLKoopman: A general-purpose Python package for Koopman theory using deep learning**.\n\nKoopman theory is a technique to encode sampled data (aka states) of a nonlinear dynamical system into a linear domain. This is very powerful as a linear model can:\n- Give insight into the dynamics via eigenvalues and eigenvectors.\n- Leverage linear algebra techniques to easily analyze the system and predict its behavior under unknown conditions.\n\n\n## Why DLKoopman?\n*DLKoopman uses deep learning to learn an encoding of a nonlinear dynamical system into a linear domain, while simultaneously learning the dynamics of the linear model*. DLKoopman bridges the gap between:\n- Software packages that restrict the learning of a good encoding (e.g. [`pykoopman`](https://github.com/dynamicslab/pykoopman)), and\n- Efforts that learn encodings for specific applications instead of being a general-purpose tool (e.g. [`DeepKoopman`](https://github.com/BethanyL/DeepKoopman)).\n\n### Key DLKoopman features\n- State prediction (`StatePred`) - Train on individual states of a system, then predict unknown states.\n    - E.g: What is the pressure vector on this aircraft for $23.5^{\\circ}$ angle of attack?\n- Trajectory prediction (`TrajPred`) - Train on generated trajectories of a system, then predict unknown trajectories for new initial states.\n    - E.g: What is the behavior of this pendulum if I start from the point $[1,-1]$?\n- General-purpose and reusable - supports data from any dynamical system.\n- Novel error function Average Normalized Absolute Error (ANAE) for visualizing performance.\n- Extensive options and a ready-to-use hyperparameter search module to improve performance.\n- Built using [Pytorch](https://pytorch.org/), supports both CPU and GPU platforms.\n\nRead more about DLKoopman in this [blog article](https://galois.com/blog/2023/01/dl-koopman/).\n\n\n## Installation\n\n### With pip (for regular users)\n`pip install dlkoopman`\n\n### From source (for development)\n```\ngit clone https://github.com/GaloisInc/dlkoopman.git\ncd dlkoopman\npip install .\n```\n\n### Running as a Docker container\nDLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.3`.\n\n\n## Tutorials and examples\nAvailable in the [`examples`](https://github.com/GaloisInc/dlkoopman/tree/ed11bef92b90112d9ca90722942a6789e6af7d5a/examples) folder.\n\n\n## Documentation and API Reference\nAvailable at https://galoisinc.github.io/dlkoopman/.\n\n## Changelog\nSee [Releases](https://github.com/GaloisInc/dlkoopman/releases) and their notes.\n\n\n## Description \n\n### Koopman theory\nAssume a dynamical system $x_{i+1} = F(x_i)$, where $x$ is the (genrally multi-dimensional) state of the system at index $i$, and $F$ is the (generally nonlinear) evolution rule describing the dynamics of the system. Koopman theory attempts to *encode* $x$ into a different space $y = g(x)$ where the dynamics are linear, i.e. $y_{i+1} = Ky_i$, where $K$ is the Koopman matrix. This is incredibly powerful since the state $y_i$ at any index $i$ can be predicted from the initial state $y_0$ as $y_i = K^iy_0$. This is then *decoded* back into the original space as $x = g^{-1}(y)$.\n\nFor a thorough mathematical treatment, see [this technical report](https://arxiv.org/abs/2211.07561).\n\n### dlkoopman training\n<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/ed11bef92b90112d9ca90722942a6789e6af7d5a/training_architecture.png" width=750/>\n</figure>\n\nThis is a small example with three input states $\\left[x_0, x_1, x_2\\right]$. These are passed through an encoder neural network to get encoded states $\\left[y_0, y_1, y_2\\right]$. These are passed through a decoder neural network to get $\\left[\\hat{x}_0, \\hat{x}_1, \\hat{x}_2\\right]$, and also used to learn $K$. This is used to derive predicted encoded states $\\left[\\mathsf{y}_1, \\mathsf{y}_2\\right]$, which are then passed through the same decoder to get predicted approximations $\\left[\\hat{\\mathsf{x}}_1, \\hat{\\mathsf{x}}_2\\right]$ to the original input states.\n\nErrors mimimized during training:\n- Train the autoencoder - Reconstruction `recon` between $x$ and $\\hat{x}$.\n- Train the Koopman matrix - Linearity `lin` between $y$ and $\\mathsf{y}$.\n- Combine the above - Prediction `pred` between $x$ and $\\hat{\\mathsf{x}}$.\n\n### dlkoopman prediction\n<figure>\n<img src="https://raw.githubusercontent.com/GaloisInc/dlkoopman/ed11bef92b90112d9ca90722942a6789e6af7d5a/prediction_architecture.png" width=750/>\n</figure>\n\nPrediction happens after training.\n\n(a) State prediction - Compute predicted states for new indexes such as $i\'$. This uses the eigendecomposition of $K$, so $i\'$ can be any real number - positive (forward extapolation), negative (backward extrapolation), or fractional (interpolation).\n\n(b) Trajectory prediction - Generate predicted trajectories $j\'$ for new starting states such as $x^{j\'}_0$. This uses a linear neural net layer to evolve the initial state.\n\n\n## Known issues\nSome common issues and ways to overcome them are described in the [known issues](https://github.com/GaloisInc/dlkoopman/issues?q=is%3Aissue+is%3Aclosed+label%3Aknown-issue).\n\n\n## How to cite\nPlease cite the [accompanying paper](https://proceedings.mlr.press/v211/dey23a.html):\n```\n@inproceedings{Dey2023_L4DC,\n    author = {Sourya Dey and Eric William Davis},\n    title = {{DLKoopman: A deep learning software package for Koopman theory}},\n    booktitle = {Proceedings of The 5th Annual Learning for Dynamics and Control Conference},\n    pages = {1467--1479},\n    volume = {211},\n    series = {Proceedings of Machine Learning Research},\n    publisher = {PMLR},\n    year = {2023},\n    month = {Jun}\n}\n```\n\n\n## References\n- B. O. Koopman - Hamiltonian systems and transformation in Hilbert space\n- J. Nathan Kutz, Steven L. Brunton, Bingni Brunton, Joshua L. Proctor - Dynamic Mode Decomposition\n- Bethany Lusch, J. Nathan Kutz & Steven L. Brunton - Deep learning for universal linear embeddings of nonlinear dynamics\n\n\n## Distribution Statement\nThis material is based upon work supported by the United States Air Force and DARPA under Contract No. FA8750-20-C-0534. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the United States Air Force and DARPA. Distribution Statement A, "Approved for Public Release, Distribution Unlimited."\n',
     'author': 'Sourya Dey',
     'author_email': 'sourya@galois.com',
     'maintainer': 'Galois dlkoopman team',
     'maintainer_email': 'dlkoopman@galois.com',
     'url': 'https://github.com/GaloisInc/dlkoopman',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlkoopman-1.1.2/PKG-INFO` & `dlkoopman-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlkoopman
-Version: 1.1.2
+Version: 1.1.3
 Summary: A general-purpose Python package for Koopman theory using deep learning.
 Home-page: https://github.com/GaloisInc/dlkoopman
 License: MIT
 Keywords: koopman theory,koopman operator,deep learning,autoencoder
 Author: Sourya Dey
 Author-email: sourya@galois.com
 Maintainer: Galois dlkoopman team
@@ -65,15 +65,15 @@
 ```
 git clone https://github.com/GaloisInc/dlkoopman.git
 cd dlkoopman
 pip install .
 ```
 
 ### Running as a Docker container
-DLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.2`.
+DLKoopman can also be run as a docker container by pulling the image from `galoisinc/dlkoopman:<version>`, e.g. `docker pull galoisinc/dlkoopman:v1.1.3`.
 
 
 ## Tutorials and examples
 Available in the [`examples`](https://github.com/GaloisInc/dlkoopman/tree/ed11bef92b90112d9ca90722942a6789e6af7d5a/examples) folder.
 
 
 ## Documentation and API Reference
@@ -115,22 +115,26 @@
 
 
 ## Known issues
 Some common issues and ways to overcome them are described in the [known issues](https://github.com/GaloisInc/dlkoopman/issues?q=is%3Aissue+is%3Aclosed+label%3Aknown-issue).
 
 
 ## How to cite
-Please cite the [accompanying paper](https://arxiv.org/abs/2211.08992):
+Please cite the [accompanying paper](https://proceedings.mlr.press/v211/dey23a.html):
 ```
-@article{Dey2022_dlkoopman,
+@inproceedings{Dey2023_L4DC,
     author = {Sourya Dey and Eric William Davis},
-    title = {DLKoopman: A deep learning software package for Koopman theory},
-    journal = {arXiv preprint arXiv:2211.08992},
-    year = {2022},
-    note = {Submitted to 5th Annual Learning for Dynamics & Control (L4DC) Conference}
+    title = {{DLKoopman: A deep learning software package for Koopman theory}},
+    booktitle = {Proceedings of The 5th Annual Learning for Dynamics and Control Conference},
+    pages = {1467--1479},
+    volume = {211},
+    series = {Proceedings of Machine Learning Research},
+    publisher = {PMLR},
+    year = {2023},
+    month = {Jun}
 }
 ```
 
 
 ## References
 - B. O. Koopman - Hamiltonian systems and transformation in Hilbert space
 - J. Nathan Kutz, Steven L. Brunton, Bingni Brunton, Joshua L. Proctor - Dynamic Mode Decomposition
```

