# Comparing `tmp/qcs_phy-1.0.5.tar.gz` & `tmp/qcs_phy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcs_phy-1.0.5.tar", last modified: Wed Jun  7 09:54:40 2023, max compression
+gzip compressed data, was "qcs_phy-1.0.6.tar", last modified: Wed Jul  5 12:53:33 2023, max compression
```

## Comparing `qcs_phy-1.0.5.tar` & `qcs_phy-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:54:40.985155 qcs_phy-1.0.5/
--rw-rw-rw-   0        0        0     1011 2023-06-07 09:54:40.985155 qcs_phy-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 09:54:40.979171 qcs_phy-1.0.5/qcs_phy/
--rw-rw-rw-   0        0        0    55774 2023-06-07 09:53:12.000000 qcs_phy-1.0.5/qcs_phy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:54:40.984158 qcs_phy-1.0.5/qcs_phy.egg-info/
--rw-rw-rw-   0        0        0     1011 2023-06-07 09:54:40.000000 qcs_phy-1.0.5/qcs_phy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-07 09:54:40.000000 qcs_phy-1.0.5/qcs_phy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:54:40.000000 qcs_phy-1.0.5/qcs_phy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-07 09:54:40.000000 qcs_phy-1.0.5/qcs_phy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 09:54:40.000000 qcs_phy-1.0.5/qcs_phy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 09:54:40.985155 qcs_phy-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-06-07 09:51:46.000000 qcs_phy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:53:33.342451 qcs_phy-1.0.6/
+-rw-rw-rw-   0        0        0     1011 2023-07-05 12:53:33.342451 qcs_phy-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 12:53:33.337465 qcs_phy-1.0.6/qcs_phy/
+-rw-rw-rw-   0        0        0    55776 2023-07-05 12:49:17.000000 qcs_phy-1.0.6/qcs_phy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:53:33.341453 qcs_phy-1.0.6/qcs_phy.egg-info/
+-rw-rw-rw-   0        0        0     1011 2023-07-05 12:53:33.000000 qcs_phy-1.0.6/qcs_phy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-05 12:53:33.000000 qcs_phy-1.0.6/qcs_phy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 12:53:33.000000 qcs_phy-1.0.6/qcs_phy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-05 12:53:33.000000 qcs_phy-1.0.6/qcs_phy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 12:53:33.000000 qcs_phy-1.0.6/qcs_phy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 12:53:33.342451 qcs_phy-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-07-05 12:52:51.000000 qcs_phy-1.0.6/setup.py
```

### Comparing `qcs_phy-1.0.5/PKG-INFO` & `qcs_phy-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs_phy
-Version: 1.0.5
+Version: 1.0.6
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.5/qcs_phy/__init__.py` & `qcs_phy-1.0.6/qcs_phy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,40 +460,40 @@
                         break
                 if rep:
                     Heff_nexc[tuple(Hi)] = csr_matrix(Heff_nexc[tuple(H_d)].toarray().T)
                     continue
 
             coff = np.ones((len(bas_fix),))
             bas_cor = np.array(bas_fix)
-            for H in Hi:
+            for H in Hi[::-1]:
                 if H[0] in ["a", "sm"]:
                     loc = self.__Ope_ani.index(H)
-                    bas_cor[:, loc] += 1
                     coff = coff * emath.sqrt(bas_cor[:, loc])
+                    bas_cor[:, loc] -= 1
                 elif H[0] in ["ad", "sp"]:
                     loc = self.__Ope_cre.index(H)
+                    bas_cor[:, loc] += 1
                     coff = coff * emath.sqrt(bas_cor[:, loc])
-                    bas_cor[:, loc] -= 1
                 elif "Sm" in H[0]:
                     N_spin = int("".join(list(filter(str.isdigit, H[0]))))
                     loc = self.__Ope_ani.index(H)
-                    bas_cor[:, loc] += 1
                     coff = coff * emath.sqrt((N_spin - bas_cor[:, loc] + 1) * bas_cor[:, loc])
+                    bas_cor[:, loc] -= 1
                 elif "Sp" in H[0]:
                     N_spin = int("".join(list(filter(str.isdigit, H[0]))))
                     loc = self.__Ope_cre.index(H)
+                    bas_cor[:, loc] += 1
                     coff = coff * emath.sqrt((N_spin - bas_cor[:, loc] + 1) * bas_cor[:, loc])
-                    bas_cor[:, loc] -= 1
                 elif "Sz" in H[0]:
                     N_spin = int("".join(list(filter(str.isdigit, H[0]))))
                     loc = self.__Ope_Szs.index(H)
                     coff = coff * bas_cor[:, loc]
                 else:
                     pass
-                Heff_nexc[tuple(Hi)] = basis_dot(bas_fix, bas_cor, coff)
+            Heff_nexc[tuple(Hi)] = basis_dot(bas_fix, bas_cor, coff)
         qcs.__HeffList[n_exc] = Heff_nexc
 
     def __prestore_InOutList(self, n_exc: int):
         """
         In order to decrease the runtime when user calculates a series of parameters, we
         prestore the Input-Output mode's matrix in the form of sparse matrices.
         :param n_exc: the excitation number
```

### Comparing `qcs_phy-1.0.5/qcs_phy.egg-info/PKG-INFO` & `qcs_phy-1.0.6/qcs_phy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs-phy
-Version: 1.0.5
+Version: 1.0.6
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.5/setup.py` & `qcs_phy-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # # these things are needed for the README.md show on pypi
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'QCS: Quantum Correlation Solver'
 LONG_DESCRIPTION = 'QCS is an open-source Python code that allows to study the single-photon transmission and reflection, ' \
                    'as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.'
 REQUIRES = ['numpy (>=1.8)', 'scipy (>=0.15)']
 INSTALL_REQUIRES = ['numpy>=1.8', 'scipy>=0.15']
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "quantum physics higher-order equal-time correlation function"
```

