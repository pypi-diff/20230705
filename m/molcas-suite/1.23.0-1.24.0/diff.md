# Comparing `tmp/molcas_suite-1.23.0.tar.gz` & `tmp/molcas_suite-1.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.23.0.tar", last modified: Thu Jun  1 10:32:07 2023, max compression
+gzip compressed data, was "molcas_suite-1.24.0.tar", last modified: Wed Jul  5 13:06:05 2023, max compression
```

## Comparing `molcas_suite-1.23.0.tar` & `molcas_suite-1.24.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3618 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.767176 molcas_suite-1.23.0/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-01 10:32:05.000000 molcas_suite-1.23.0/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    28336 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    31919 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18799 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25262 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21698 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3618 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-06-01 10:32:05.000000 molcas_suite-1.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:06:05.721520 molcas_suite-1.24.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-07-05 13:06:05.721520 molcas_suite-1.24.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:06:05.719520 molcas_suite-1.24.0/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-05 13:05:59.000000 molcas_suite-1.24.0/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    28336 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    31919 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18799 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25262 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21698 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:06:05.721520 molcas_suite-1.24.0/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 13:06:05.000000 molcas_suite-1.24.0/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-05 13:05:42.000000 molcas_suite-1.24.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 13:06:05.721520 molcas_suite-1.24.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-07-05 13:05:59.000000 molcas_suite-1.24.0/setup.py
```

### Comparing `molcas_suite-1.23.0/LICENSE` & `molcas_suite-1.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/PKG-INFO` & `molcas_suite-1.24.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: molcas_suite
-Version: 1.23.0
+Name: molcas-suite
+Version: 1.24.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.23.0/README.md` & `molcas_suite-1.24.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/barrier.py` & `molcas_suite-1.24.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/cfp.py` & `molcas_suite-1.24.0/molcas_suite/cfp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from angmom_suite.basis import extract_blocks, dissect_array, \
-    print_sf_term_content
+    print_sf_term_content, print_so_term_content, sf2ws, sf2ws_amfi, \
+    make_angmom_ops_from_mult, unitary_transform
 from angmom_suite.crystal import ProjectModelHamiltonian, evaluate_term_space,\
-    evaluate_term_operators, print_basis
+    evaluate_term_operators, print_basis, HARTREE2INVCM
 from angmom_suite.utils import plot_op
 from .extractor import make_extractor
 
 
 def make_proj_evaluator(h_file, options):
     return ProjectModelHamiltonianMolcas(h_file, options)
 
@@ -33,15 +34,31 @@
         self.field = options.pop("field")
 
         super().__init__(ops, sf_mult, **options)
 
     def __iter__(self):
 
         if self.model_space is None:
-            print_sf_term_content(self.ops['sf_angm'], self.sf_mult)
+            smult = np.repeat(list(self.sf_mult.keys()), list(self.sf_mult.values()))
+
+            ws_angm = sf2ws(self.ops['sf_angm'], self.sf_mult)
+            ws_spin = np.array(make_angmom_ops_from_mult(smult)[0:3])
+            ws_hamiltonian = sf2ws(self.ops['sf_mch'], self.sf_mult) + \
+                sf2ws_amfi(self.ops['sf_amfi'], self.sf_mult)
+
+            eig, vec = np.linalg.eigh(ws_hamiltonian)
+            so_eners = (eig - eig[0]) * HARTREE2INVCM
+
+            sf_eners = [(np.diag(eners) - eners[0, 0]) * HARTREE2INVCM
+                        for eners in self.ops['sf_mch']]
+
+            print_sf_term_content(self.ops['sf_angm'], sf_eners, self.sf_mult)
+            print_so_term_content(unitary_transform(ws_spin, vec),
+                                  unitary_transform(ws_angm, vec),
+                                  so_eners, self.sf_mult)
 
         elif not self.terms:
             term_space, trafo = \
                 evaluate_term_space(self.sf_mult, self.model_space,
                                     coupling=self.coupling, complete=True)
 
             hamiltonian, spin, angm = \
```

### Comparing `molcas_suite-1.23.0/molcas_suite/cli.py` & `molcas_suite-1.24.0/molcas_suite/cli.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/extractor.py` & `molcas_suite-1.24.0/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/generate_input.py` & `molcas_suite-1.24.0/molcas_suite/generate_input.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/generate_job.py` & `molcas_suite-1.24.0/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/h5tools.py` & `molcas_suite-1.24.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite/orbs.py` & `molcas_suite-1.24.0/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.23.0/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: molcas-suite
-Version: 1.23.0
+Name: molcas_suite
+Version: 1.24.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.23.0/setup.py` & `molcas_suite-1.24.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.23.0"
+__version__ = "1.24.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
@@ -31,15 +31,15 @@
         ],
     python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'h5py',
         'xyz_py>=5.6.1',
-        'angmom_suite>=1.11.1',
+        'angmom_suite>=1.13.0',
         'hpc_suite>=1.8.0',
         'matplotlib'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'molcas_suite = molcas_suite.cli:main'
```

