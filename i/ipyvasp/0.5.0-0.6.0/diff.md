# Comparing `tmp/ipyvasp-0.5.0.tar.gz` & `tmp/ipyvasp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.5.0.tar", last modified: Tue Jul  4 17:30:06 2023, max compression
+gzip compressed data, was "ipyvasp-0.6.0.tar", last modified: Wed Jul  5 00:37:19 2023, max compression
```

## Comparing `ipyvasp-0.5.0.tar` & `ipyvasp-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.805501 ipyvasp-0.5.0/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1862 2023-07-04 17:30:06.804495 ipyvasp-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.767725 ipyvasp-0.5.0/ipyvasp/
--rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.5.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.5.0/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    92905 2023-07-04 17:23:48.000000 ipyvasp-0.5.0/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0       23 2023-07-04 17:29:24.000000 ipyvasp-0.5.0/ipyvasp/_version.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.5.0/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0      565 2023-07-02 21:39:58.000000 ipyvasp-0.5.0/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.803496 ipyvasp-0.5.0/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.5.0/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.5.0/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.5.0/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.5.0/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.5.0/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.5.0/ipyvasp/evals_dataframe.py
--rw-rw-rw-   0        0        0    22391 2023-07-03 16:19:41.000000 ipyvasp-0.5.0/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.5.0/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.5.0/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.5.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.5.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.799100 ipyvasp-0.5.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      190 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 17:30:06.805501 ipyvasp-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3820 2023-07-02 21:35:36.000000 ipyvasp-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.721723 ipyvasp-0.6.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.6.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.0/ipyvasp/__main__.py
+-rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    92969 2023-07-04 23:43:08.000000 ipyvasp-0.6.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-07-05 00:36:32.000000 ipyvasp-0.6.0/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     1590 2023-07-05 00:32:00.000000 ipyvasp-0.6.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.761724 ipyvasp-0.6.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.6.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.6.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.0/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    22397 2023-07-04 23:42:24.000000 ipyvasp-0.6.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.6.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.761724 ipyvasp-0.6.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      203 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.0/setup.py
```

### Comparing `ipyvasp-0.5.0/LICENSE` & `ipyvasp-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/PKG-INFO` & `ipyvasp-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.5.0
+Version: 0.6.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.5.0/README.md` & `ipyvasp-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/__init__.py` & `ipyvasp-0.6.0/ipyvasp/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/_enplots.py` & `ipyvasp-0.6.0/ipyvasp/_enplots.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/_lattice.py` & `ipyvasp-0.6.0/ipyvasp/_lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,15 +571,22 @@
                 _5th = int(data[4])
                 point = point + [data[3], _5th]
 
             hsk_list.append(point)
     return hsk_list
 
 
-def get_kpath(kpoints, n=5, weight=None, ibzkpt=None, outfile=None, rec_basis=None):
+def get_kpath(
+    kpoints,
+    n: int = 5,
+    weight: float = None,
+    ibzkpt: str = None,
+    outfile: str = None,
+    rec_basis=None,
+):
     """Generate list of kpoints along high symmetry path. Options are write to file or return KPOINTS list.
     It generates uniformly spaced point with input `n` as just a scale factor of number of points per average length of `rec_basis`.
 
     Parameters
     ----------
     kpoints : list or str
         Any number points as [(x,y,z,[label],[N]), ...]. N adds as many points in current interval.
```

### Comparing `ipyvasp-0.5.0/ipyvasp/bsdos.py` & `ipyvasp-0.6.0/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/core/parser.py` & `ipyvasp-0.6.0/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.6.0/ipyvasp/core/plot_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/core/serializer.py` & `ipyvasp-0.6.0/ipyvasp/core/serializer.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.6.0/ipyvasp/core/spatial_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/evals_dataframe.py` & `ipyvasp-0.6.0/ipyvasp/evals_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/lattice.py` & `ipyvasp-0.6.0/ipyvasp/lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,9 +592,9 @@
     @_sub_doc(get_kmesh, {"poscar_data :.*\*args :": "*args :"})
     @_sig_kwargs(get_kmesh, ("poscar_data",))
     def get_kmesh(self, *args, **kwargs):
         return get_kmesh(self.data, *args, **kwargs)
 
     @_sub_doc(get_kpath, {"rec_basis :.*\n\n": "\n\n"})
     @_sig_kwargs(get_kpath, ("rec_basis",))
-    def get_kpath(self, kpoints, n=5, **kwargs):
+    def get_kpath(self, kpoints, n : int=5, **kwargs):
         return get_kpath(kpoints, n=n, **kwargs, rec_basis=self.data.rec_basis)
```

### Comparing `ipyvasp-0.5.0/ipyvasp/misc.py` & `ipyvasp-0.6.0/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/potential.py` & `ipyvasp-0.6.0/ipyvasp/potential.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/utils.py` & `ipyvasp-0.6.0/ipyvasp/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp/widgets.py` & `ipyvasp-0.6.0/ipyvasp/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.5.0/ipyvasp.egg-info/PKG-INFO` & `ipyvasp-0.6.0/ipyvasp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.5.0
+Version: 0.6.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.5.0/ipyvasp.egg-info/SOURCES.txt` & `ipyvasp-0.6.0/ipyvasp.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 ipyvasp/__init__.py
+ipyvasp/__main__.py
 ipyvasp/_enplots.py
 ipyvasp/_lattice.py
 ipyvasp/_version.py
 ipyvasp/bsdos.py
 ipyvasp/cli.py
 ipyvasp/evals_dataframe.py
 ipyvasp/lattice.py
```

### Comparing `ipyvasp-0.5.0/setup.py` & `ipyvasp-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "numpy==1.23.2",
     "scipy==1.9.1",
     "ipywidgets>=8.0.4",
     "pillow>=9.3.0",
     "pandas==1.4.4",
     "plotly==5.14.1",
     "requests==2.28.1",
+    "typer==0.9.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     "extra": ["jupyterlab>=3.5.2", "ipython>=8.7", "ase>=3.22.1", "nglview>=3.0.4"],
 }
 
@@ -124,11 +125,11 @@
     # $ setup.py publish support.
     cmdclass={
         "upload": UploadCommand,
     },
     # for command line interface
     entry_points={
         "console_scripts": [
-            "ipyvasp=ipyvasp.cli:main",
+            "ipyvasp=ipyvasp.cli:app",
         ]
     },
 )
```

