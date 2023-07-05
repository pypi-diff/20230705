# Comparing `tmp/pyseistr-win-0.0.1.tar.gz` & `tmp/pyseistr-win-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseistr-win-0.0.1.tar", last modified: Wed Jul  5 13:26:28 2023, max compression
+gzip compressed data, was "pyseistr-win-0.0.1.1.tar", last modified: Wed Jul  5 14:19:14 2023, max compression
```

## Comparing `pyseistr-win-0.0.1.tar` & `pyseistr-win-0.0.1.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 13:26:28.731774 pyseistr-win-0.0.1/
--rw-r--r--   0 chenyk     (501) staff       (20)     1157 2023-07-05 13:26:28.731414 pyseistr-win-0.0.1/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     7481 2023-07-05 13:12:42.000000 pyseistr-win-0.0.1/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 13:26:28.723989 pyseistr-win-0.0.1/pyseistr_win.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1157 2023-07-05 13:26:28.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      731 2023-07-05 13:26:28.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-05 13:26:28.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-05 13:19:47.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-05 13:26:28.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       10 2023-07-05 13:26:28.000000 pyseistr-win-0.0.1/pyseistr_win.egg-info/top_level.txt
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 13:26:28.731053 pyseistr-win-0.0.1/pyseistrw/
--rw-r--r--   0 chenyk     (501) staff       (20)     2126 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6443 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/bp.py
--rw-r--r--   0 chenyk     (501) staff       (20)     3370 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/das.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/dip2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/dip3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9829 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/divne.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1949 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/fk.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4355 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/mf.py
--rw-r--r--   0 chenyk     (501) staff       (20)     5004 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/operators.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2506 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/plot.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2053 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/pwsmooth.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9503 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/pwspray2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9161 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/pwspray3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2699 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/rgt.py
--rw-r--r--   0 chenyk     (501) staff       (20)      756 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/ricker.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2325 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/sint.py
--rw-r--r--   0 chenyk     (501) staff       (20)     5686 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/smooth.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1959 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/soint2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2296 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/soint3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     7701 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/solvers.py
--rw-r--r--   0 chenyk     (501) staff       (20)      503 2023-07-05 13:25:15.000000 pyseistr-win-0.0.1/pyseistrw/somean2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)      506 2023-07-05 13:25:26.000000 pyseistr-win-0.0.1/pyseistrw/somean3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     3116 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/somf2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2877 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/somf3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6125 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1/pyseistrw/synthetics.py
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-05 13:26:28.731876 pyseistr-win-0.0.1/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     1833 2023-07-05 13:19:37.000000 pyseistr-win-0.0.1/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 14:19:14.018762 pyseistr-win-0.0.1.1/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1159 2023-07-05 14:19:14.018418 pyseistr-win-0.0.1.1/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     7333 2023-07-05 14:18:54.000000 pyseistr-win-0.0.1.1/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 14:19:14.005327 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1159 2023-07-05 14:19:13.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      714 2023-07-05 14:19:13.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-05 14:19:13.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-07-05 13:19:47.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-07-05 14:19:13.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       10 2023-07-05 14:19:13.000000 pyseistr-win-0.0.1.1/pyseistr_win.egg-info/top_level.txt
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-07-05 14:19:14.017764 pyseistr-win-0.0.1.1/pyseistrw/
+-rw-r--r--   0 chenyk     (501) staff       (20)     2171 2023-07-05 14:13:22.000000 pyseistr-win-0.0.1.1/pyseistrw/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4917 2023-07-05 14:15:20.000000 pyseistr-win-0.0.1.1/pyseistrw/bp.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2795 2023-07-05 14:15:08.000000 pyseistr-win-0.0.1.1/pyseistrw/das.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3694 2023-07-05 14:14:56.000000 pyseistr-win-0.0.1.1/pyseistrw/dip2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     5207 2023-07-05 14:14:42.000000 pyseistr-win-0.0.1.1/pyseistrw/dip3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9829 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/divne.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1949 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/fk.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4355 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/mf.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     5004 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/operators.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2506 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/plot.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2053 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/pwsmooth.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9503 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/pwspray2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9161 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/pwspray3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      756 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/ricker.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1078 2023-07-05 14:11:49.000000 pyseistr-win-0.0.1.1/pyseistrw/sint.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3155 2023-07-05 14:11:36.000000 pyseistr-win-0.0.1.1/pyseistrw/smooth.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      848 2023-07-05 14:11:26.000000 pyseistr-win-0.0.1.1/pyseistrw/soint2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1251 2023-07-05 14:11:15.000000 pyseistr-win-0.0.1.1/pyseistrw/soint3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7701 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/solvers.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      503 2023-07-05 13:25:15.000000 pyseistr-win-0.0.1.1/pyseistrw/somean2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      506 2023-07-05 13:25:26.000000 pyseistr-win-0.0.1.1/pyseistrw/somean3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1722 2023-07-05 14:10:59.000000 pyseistr-win-0.0.1.1/pyseistrw/somf2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1423 2023-07-05 14:10:48.000000 pyseistr-win-0.0.1.1/pyseistrw/somf3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6125 2023-07-05 13:13:33.000000 pyseistr-win-0.0.1.1/pyseistrw/synthetics.py
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-07-05 14:19:14.018895 pyseistr-win-0.0.1.1/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     1835 2023-07-05 14:19:05.000000 pyseistr-win-0.0.1.1/setup.py
```

### Comparing `pyseistr-win-0.0.1/PKG-INFO` & `pyseistr-win-0.0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr-win
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr-win
 Author: pyseistr-win developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-win-0.0.1/README.md` & `pyseistr-win-0.0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-**Pyseistr**
+**pyseistr-win**
 ======
 
 ## Description
 
-**Pyseistr** is a python package for structural denoising and interpolation of multi-channel seismic data. The latest version has incorporated both Python and C (hundreds of times faster) implementations of the embedded functions. We keep both implementations for both educational and production purposes. This package has a variety of applications in both exploration and earthquake seismology.
+**pyseistr-win** is the Windows version of the pyseistr package, a python package for structural denoising and interpolation of multi-channel seismic data. The latest version has incorporated both Python and C (hundreds of times faster) implementations of the embedded functions. We keep both implementations for both educational and production purposes. This package has a variety of applications in both exploration and earthquake seismology.
 
 ## Reference
-Chen et al., 2023, Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, Seismological Research Letters, 94(3), 1703-1714. 
+Chen et al., 2023, pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, Seismological Research Letters, 94(3), 1703-1714. 
 
 BibTeX:
 
 	@article{pyseistr,
-	  title={Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data},
+	  title={pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data},
 	  author={Yangkang Chen and Alexandros Savvaidis and Sergey Fomel and Yunfeng Chen and Omar M. Saad and Yapo Abol{\'e} Serge Innocent Obou{\'e} and Quan Zhang and Wei Chen},
 	  journal={Seismological Research Letters},
 	  volume={94},
 	  number={3},
 	  pages={1703–1714},
 	  year={2023}
 	}
 
 -----------
 ## Copyright
-    The pyseistr developing team, 2021-present
+    The pyseistr-win developing team, 2021-present
 -----------
 
 ## License
     GNU General Public License, Version 3
     (http://www.gnu.org/copyleft/gpl.html)   
 
 -----------
 
 ## Install
 Using the latest version
 
-    git clone https://github.com/aaspip/pyseistr
-    cd pyseistr
+    git clone https://github.com/aaspip/pyseistr-win
+    cd pyseistr-win
     pip install -v -e .
 or using Pypi
 
-    pip install pyseistr
+    pip install pyseistr-win
 
 -----------
 ## DEMO scripts
-    The "demo" directory contains all runable scripts to demonstrate different applications of pyseistr. 
+    The "demo" directory contains all runable scripts to demonstrate different applications of pyseistr-win. 
 
 -----------
 ## Gallery
-The gallery figures of the pyseistr package can be found at
+The gallery figures of the pyseistr-win package can be found at
     https://github.com/aaspip/gallery/tree/main/pyseistr
 Each figure in the gallery directory corresponds to a DEMO script in the "demo" directory with the exactly the same file name.
 
 -----------
 ## Dependence Packages
 * scipy 
 * numpy 
@@ -83,69 +83,65 @@
     Regarding any questions, bugs, developments, collaborations, please contact  
     Yangkang Chen
     chenyk2016@gmail.com
 
 -----------
 ## Examples
 # Example 1 (2D structure-oriented mean/smoothing filter) 
-Generated by [demos/test_pyseistr_somean2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somean2d.py)
+Generated by [demos/test_pyseistr_somean2d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_somean2d.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somean2d.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_somean2d.png' alt='Slicing' width=960/>
 
 # Example 2 (3D structure-oriented mean/smoothing filter) 
-Generated by [demos/test_pyseistr_somean3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somean3d.py)
+Generated by [demos/test_pyseistr_somean3d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_somean3d.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somean3d.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_somean3d.png' alt='Slicing' width=960/>
 
 # Example 3 (2D structure-oriented median filter) 
-Generated by [demos/test_pyseistr_somf2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somf2d.py)
+Generated by [demos/test_pyseistr_somf2d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_somf2d.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somf2d.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_somf2d.png' alt='Slicing' width=960/>
 
 # Example 4 (3D structure-oriented median filter) 
-Generated by [demos/test_pyseistr_somf3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somf3d.py)
+Generated by [demos/test_pyseistr_somf3d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_somf3d.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somf3d.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_somf3d.png' alt='Slicing' width=960/>
 
 # Example 5 (3D structure-oriented interpolation) 
-Generated by [demos/test_pyseistr_passive_recon3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_passive_recon3d.py)
+Generated by [demos/test_pyseistr_passive_recon3d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_passive_recon3d.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_passive_recon3d.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_passive_recon3d.png' alt='Slicing' width=960/>
 
 # Example 6 (SS precursor data enhancement) 
-Generated by [demos/test_pyseistr_ssprecursor.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_ssprecursor.py)
+Generated by [demos/test_pyseistr_ssprecursor.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_ssprecursor.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_ssprecursor.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_ssprecursor.png' alt='Slicing' width=960/>
 
 # Example 7 (receiver function data enhancement) 
-Generated by [demos/test_pyseistr_rf.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_rf.py)
+Generated by [demos/test_pyseistr_rf.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_rf.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_rf.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_rf.png' alt='Slicing' width=960/>
 
 # Example 8 (structure-oriented distributed acoustic sensing (DAS) data processing) 
-Generated by [demos/test_pyseistr_das.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_das.py)
+Generated by [demos/test_pyseistr_das.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_das.py)
 
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_das.png' alt='Slicing' width=960/>
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_das.png' alt='Slicing' width=960/>
 
 # Below are new examples in addition to the results in the original paper
 
 # Below is an example for 2D structure-oriented interpolation of a multi-channel synthetic seismic data
-Generated by [demos/test_pyseistr_soint2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d.py)
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d.png' alt='comp' width=960/>
+Generated by [demos/test_pyseistr_soint2d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_soint2d.py)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_soint2d.png' alt='comp' width=960/>
 
 # Below is an example for 2D structure-oriented interpolation of a seafloor dataset
-Generated by [demos/test_pyseistr_soint2d_seafloor.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d_seafloor.py)
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d_seafloor.png' alt='comp' width=960/>
+Generated by [demos/test_pyseistr_soint2d_seafloor.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_soint2d_seafloor.py)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_soint2d_seafloor.png' alt='comp' width=960/>
 
 # Below is another example for 2D structure-oriented interpolation of sparse seismic data
-Generated by [demos/test_pyseistr_soint2d2.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d2.py)
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2dnew.png' alt='comp' width=960/>
-
-# Below is an example for calculating relative geological time (RGT) from 2D seismic data
-Generated by [demos/test_pyseistr_rgt2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_rgt2d.py)
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_rgt2d.png' alt='comp' width=960/>
+Generated by [demos/test_pyseistr_soint2d2.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_soint2d2.py)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_soint2dnew.png' alt='comp' width=960/>
 
 # Below is an example for 2D interpolation of sparse seismic data
-Generated by [demos/test_pyseistr_sint2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_sint2d.py)
-<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_sint2d.png' alt='comp' width=960/>
+Generated by [demos/test_pyseistr_sint2d.py](https://github.com/aaspip/pyseistr-win/tree/main/demos/test_pyseistr_sint2d.py)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr-win/test_pyseistr_sint2d.png' alt='comp' width=960/>
```

### Comparing `pyseistr-win-0.0.1/pyseistr_win.egg-info/PKG-INFO` & `pyseistr-win-0.0.1.1/pyseistr_win.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr-win
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr-win
 Author: pyseistr-win developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-win-0.0.1/pyseistr_win.egg-info/SOURCES.txt` & `pyseistr-win-0.0.1.1/pyseistr_win.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 pyseistrw/fk.py
 pyseistrw/mf.py
 pyseistrw/operators.py
 pyseistrw/plot.py
 pyseistrw/pwsmooth.py
 pyseistrw/pwspray2d.py
 pyseistrw/pwspray3d.py
-pyseistrw/rgt.py
 pyseistrw/ricker.py
 pyseistrw/sint.py
 pyseistrw/smooth.py
 pyseistrw/soint2d.py
 pyseistrw/soint3d.py
 pyseistrw/solvers.py
 pyseistrw/somean2d.py
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/__init__.py` & `pyseistr-win-0.0.1.1/pyseistrw/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,35 +57,33 @@
 from .bp import bandpass
 from .fk import fkdip
 from .plot import *
 from .pwsmooth import *
 from .pwspray2d import *
 
 from .das import coh 
-from .das import cohc
+# from .das import cohc
 
 from .synthetics import *
-from .rgt import *
 from .smooth import *
 
-## C versions
-from .dip2d import dip2dc
-from .dip3d import dip3dc
-from .somean2d import somean2dc
-from .somean3d import somean3dc
-from .somf2d import somf2dc
-from .somf3d import somf3dc
-from .soint2d import soint2dc
-from .soint3d import soint3dc
-from .sint import sint2dc
-from .sint import sint3dc
-from .bp import bandpassc
-
-from dipcfun import *
-from sofcfun import *
-from sof3dcfun import *
-from bpcfun import *
+## C versions (deactivated in windows version)
+# from .dip2d import dip2dc
+# from .dip3d import dip3dc
+# from .somean2d import somean2dc
+# from .somean3d import somean3dc
+# from .somf2d import somf2dc
+# from .somf3d import somf3dc
+# from .soint2d import soint2dc
+# from .soint3d import soint3dc
+# from .sint import sint2dc
+# from .sint import sint3dc
+# from .bp import bandpassc
+# from dipcfun import *
+# from sofcfun import *
+# from sof3dcfun import *
+# from bpcfun import *
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/bp.py` & `pyseistr-win-0.0.1.1/pyseistrw/bp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from bpcfun import *
 
 def bandpass(din,dt,flo=0,fhi=0.5,nplo=6,nphi=6,phase=0,verb=1):
 	'''
 	bandpass: Bandpass filtering.
 	
 	Aug, 05, 2020
 	by Yangkang Chen
@@ -121,73 +120,14 @@
 		dout[:,i2]=trace[:,0];
 
 	dout=dout.reshape(n1,n22,n33);
 
 	dout=np.squeeze(dout);
 	return dout
 
-def bandpassc(din,dt,flo=0,fhi=0.5,nplo=6,nphi=6,phase=0,verb=1):
-	'''
-	bandpass: Bandpass filtering.
-	
-	Aug, 05, 2020
-	by Yangkang Chen
-	
-	INPUT
-	din:	  input data
-	dt:       sampling
-	flo:      Low frequency in band, default is 0
-	fhi:      High frequency in band, default is Nyquist
-	nplo=6:   number of poles for low cutoff
-	nphi=6:   number of poles for high cutoff
-	phase=0:  y: minimum phase, n: zero phase
-	verb=0:   verbosity flag
-	
-	OUTPUT
-	dout:     output data
-	
-	RFERENCE
-	November 2012 program of the month: http://ahay.org/blog/2012/11/03/program-of-the-month-sfbandpass/
-	
-	EXAMPLE 1
-	demos/test_pyseistr_das.py
-	
-	EXAMPLE 2
-	from pyseistr import ricker;
-	wav,tw=ricker(20,0.004,2);
-	from pyseistr import bandpassc;
-	wav2=bandpassc(wav,0.004,flo=0,fhi=20);
-	
-	import matplotlib.pyplot as plt;
-	figsize=(8, 8)
-	plt.subplot(2,1,1);
-	plt.plot(tw,wav);plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
-	plt.subplot(2,1,2);
-	plt.plot(tw,wav2);plt.xlabel('Time (s)');plt.ylabel('Amplitude');plt.gca().set_ylim([-0.5,1]);
-	plt.show();
-	
-	'''
-	if din.ndim==1:	#for 1D problems
-		din=np.expand_dims(din, axis=1)
-		
-	if din.ndim==2:	#for 2D problems
-		din=np.expand_dims(din, axis=2)
-		
-	if din.shape[0]==1 and din.shape[1]>1 and din.shape[2]==1: #row vector
-		din=din.flatten();
-
-	[n1,n2,n3]=din.shape;
-		
-	din=np.float32(din).flatten(order='F');
-	dout=cbp(din,n1,n2,n3,dt,flo,fhi,nplo,nphi,phase,verb);
-	dout=dout.reshape(n1,n2,n3,order='F');
-
-	if n3==1:
-		dout=np.squeeze(dout);
-	return dout
 	
 def butter_init(low,cutoff,nn):
 	'''
 	butter_init: initialize
 	Aug, 5, 2020
 	Yangkang Chen
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/das.py` & `pyseistr-win-0.0.1.1/pyseistrw/das.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from cohcfun import *
 
 def coh(inpt,par,operator=-1):
     '''
     Coherency measure based on the 
     Forward and Adjoint operators for Radon RT in the time domain.
     IN   	in:   		intput data 
       	Param:  		parameters combination
@@ -85,37 +84,8 @@
         out = d
     if operator ==-1:
         out = m
 
     return out
     
     
-def cohc(din,par,operator=-1,verb=0):
-	'''
-	Forward and Adjoint operators for Radon RT in the time domain.
-	radon implemented in C
-	'''
-	
-	h = par['h'];
-	v = par['v'];
-	nt = par['nt'];
-	dt = par['dt'];
-	typ = par['typ'];
-
-	nh = len(h);
-	nv = len(v);
-	
-	din=np.float32(din.flatten(order='F'));
-	v=np.float32(v);
-	h=np.float32(h);
-	
-	dout=cohc_fb(din, v, h, typ, nt, nv, nh, dt, operator, verb);
-	
-	if operator==1: #forward
-		dout=dout.reshape(nt,nh,order='F');
-	if operator==-1: #backward/adjoint
-		dout=dout.reshape(nt,nv,order='F');
-	
-	
-	return dout
-
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/dip2d.py` & `pyseistr-win-0.0.1.1/pyseistrw/dip3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,154 +1,160 @@
 import numpy as np
-from dipcfun import *
 
-def dip2d(din,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1):
+def dip3d(din,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1):
 	'''
-	dip2d: dip estimation based on shaping regularized PWD algorithm 
+	dip3d: 3D dip estimation based on shaping regularized PWD algorithm
 	(independent implementation)
 	
+	Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
+	
 	INPUT
 	din: input data (nt*nx)
 	niter: number of nonlinear iterations
 	liter: number of linear iterations (in divn)
 	order: accuracy order
 	eps_dv: eps for divn  (default: 0.01)
-	eps_cg: eps for CG    (default: 1)
+	eps_cg: eps for CG	(default: 1)
 	tol_cg: tolerence for CG (default: 0.000001)
 	rect:  smoothing radius (ndim*1)
 	verb: verbosity flag
 	
 	OUTPUT
-	dip:  2D slope
+	dipi:  inline 3D slope
+	dipx:  xline 3D slope
 	
 	NOTE: mask function is not enabled yet (will do in the future)
 	'''
-	
 	from .divne import divne
 	
-	p0 = 0.0;
-	nj1 = 1;
-	nj2 = 1;
 	dim = 3;
-	
 	n = np.zeros(dim,dtype='int');
 	n1 = din.shape[0];
 	n2 = din.shape[1];
+	n3 = din.shape[2];
 	n[0] = n1;
 	n[1] = n2;
-	n[2] = 1;
+	n[2] = n3;
 
 	n123 = din.size;
 
-	ratio=np.zeros([n1,n2,1]);
-	dip=np.zeros([n1,n2,1]);
+	dip_i=np.zeros([n1,n2,n3]);
+	dip_x=np.zeros([n1,n2,n3]);
 
 	for iter in range(0,niter):
-		"""corresponding to the eq.21 in the paper  (Wang et al., 2022)"""
-		[u1,u2] = conv_allpass(din,dip,order); 
-		ratio = divne(-u2, u1, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
-		dip=dip+ratio;
 
-	return dip
+		#corresponding to the eq.21 in the paper
+		u1_i,u2_i = conv_allpass_i(din,dip_i,order); 	#inline linearization using the updated dip	
+		ratio_i  = divne(-u2_i, u1_i, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
 
-def dip2dc(din,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1,mask=None):
+		#corresponding to the eq.21 in the paper
+		u1_x,u2_x = conv_allpass_x(din,dip_x,order); 	#xline linearization using the updated dip
+		ratio_x  = divne(-u2_x, u1_x, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
+	
+		dip_i=dip_i+ratio_i;
+		dip_x=dip_x+ratio_x;
+
+	return dip_i,dip_x
+
+def conv_allpass_i(din,dip,order):
 	'''
-	dip2dc: dip estimation based on shaping regularized PWD algorithm 
-	(C implementation)
+	conv_allpass_i: Convolutional operator implemented by an allpass filter (iline direction)
 	
-	INPUT
-	din: input data (nt*nx)
-	niter: number of nonlinear iterations
-	liter: number of linear iterations (in divn)
+	Linearized inverse problem
+	C'(\sigma)d\Delta \sigma =  C(\sigma)d
+	
+	IPNUT:
+	din: input data
+	dip: 3D dip
 	order: accuracy order
-	eps_dv: eps for divn  (default: 0.01)
-	eps_cg: eps for CG    (default: 1)
-	tol_cg: tolerence for CG (default: 0.000001)
-	rect:  smoothing radius (ndim*1)
-	verb: verbosity flag
 	
-	OUTPUT
-	dip:  2D slope
+	OUTPUT:
+	u1: C'(\sigma)d (denominator)
+	u2: C(\sigma)d  (numerator)
 	
-	from .divne import divne
 	'''
-	
-	p0 = 0.0;
-	nj1 = 1;
-	nj2 = 1;
-	dim = 3;
-	
-	n1 = din.shape[0];
-	n2 = din.shape[1];
-	n3 = 1;
-	
-	r1=rect[0]
-	r2=rect[1]
-	r3=rect[2]
-
-	if mask is None:
-		din=np.float32(din.flatten(order='F'));
-		hasmask=0
+	[n1,n2,n3]=din.shape;
+	u1=np.zeros([n1,n2,n3]);
+	u2=np.zeros([n1,n2,n3]);
+
+	if order==1:
+		nw=1;
 	else:
-		if din.size != mask.size:
-			Exception("Mask and Data should have the same dimension")
-		else:
-			din=np.float32(np.concatenate([din.flatten(order='F'),mask.flatten(order='F')],axis=0));
-			hasmask=1;
-	dip=dipc(din,n1,n2,n3,niter,liter,order,eps_dv,eps_cg,tol_cg,r1,r2,r3,hasmask,verb);
-	dip=dip.reshape(n1,n2,order='F');
-		
-	return dip
-	
-def conv_allpass(din,dip,order):
+		nw=2;
+
+
+	filt1=np.zeros(2*nw+1);
+	filt2=np.zeros(2*nw+1);
+
+	# cprresponding to eqs.17-19
+	# destruct the data
+	for i1 in range(nw,n1-nw):
+		for i2 in range(0,n2-1):
+			for i3 in range(0,n3):
+				if order==1:
+					filt1=B3d(dip[i1,i2,i3]);
+					filt2=B3(dip[i1,i2,i3]);
+				else:
+					filt1=B5d(dip[i1,i2,i3]);
+					filt2=B5(dip[i1,i2,i3]);
+
+				for iw in range(-nw,nw+1):
+					u1[i1,i2,i3]=u1[i1,i2,i3]+(din[i1+iw,i2+1,i3]-din[i1-iw,i2,i3])*filt1[iw+nw];
+					u2[i1,i2,i3]=u2[i1,i2,i3]+(din[i1+iw,i2+1,i3]-din[i1-iw,i2,i3])*filt2[iw+nw];
+
+	return u1,u2
+
+def conv_allpass_x(din,dip,order):
 	'''
-	conv_allpass: Convolutional operator implemented by an allpass filter
+	conv_allpass_x: Convolutional operator implemented by an allpass filter (xline direction)
 	
 	Linearized inverse problem
 	C'(\sigma)d\Delta \sigma =  C(\sigma)d
 	
 	IPNUT:
 	din: input data
 	dip: 3D dip
 	order: accuracy order
 	
 	OUTPUT:
 	u1: C'(\sigma)d (denominator)
 	u2: C(\sigma)d  (numerator)
 	
 	'''
-	[n1,n2]=din.shape;
-	u1=np.zeros([n1,n2]);
-	u2=np.zeros([n1,n2]);
+	
+	[n1,n2,n3]=din.shape;
+	u1=np.zeros([n1,n2,n3]);
+	u2=np.zeros([n1,n2,n3]);
 
 	if order==1:
 		nw=1;
 	else:
 		nw=2;
 
+
 	filt1=np.zeros(2*nw+1);
 	filt2=np.zeros(2*nw+1);
 
-	#cprresponding to eqs.17-19
-	#destruct the data
+	# cprresponding to eqs.17-19
+	# destruct the data
 	for i1 in range(nw,n1-nw):
-		for i2 in range(0,n2-1):
-			if order==1:
-				filt1=B3d(dip[i1,i2]);
-				filt2=B3(dip[i1,i2]);
-			else:
-				filt1=B5d(dip[i1,i2]);
-				filt2=B5(dip[i1,i2]);
-
-			for iw in range(-nw,nw+1):
-				u1[i1,i2]=u1[i1,i2]+(din[i1+iw,i2+1]-din[i1-iw,i2])*filt1[iw+nw];
-				u2[i1,i2]=u2[i1,i2]+(din[i1+iw,i2+1]-din[i1-iw,i2])*filt2[iw+nw];
-
+		for i2 in range(0,n2):
+			for i3 in range(0,n3-1):
+				if order==1:
+					filt1=B3d(dip[i1,i2,i3]);
+					filt2=B3(dip[i1,i2,i3]);
+				else:
+					filt1=B5d(dip[i1,i2,i3]);
+					filt2=B5(dip[i1,i2,i3]);
+				for iw in range(-nw,nw+1):
+					u1[i1,i2,i3]=u1[i1,i2,i3]+(din[i1+iw,i2,i3+1]-din[i1-iw,i2,i3])*filt1[iw+nw];
+					u2[i1,i2,i3]=u2[i1,i2,i3]+(din[i1+iw,i2,i3+1]-din[i1-iw,i2,i3])*filt2[iw+nw];
 	return u1,u2
 
+
 #cprresponding to eqs.13-16
 #form the filters
 def B3(sigma):
 	'''
 	B3 coefficient
 	sigma: slope
 	'''
@@ -213,7 +219,10 @@
 
 	b5d[4]=(2+sigma)*(3+sigma)*(4+sigma)/1680+\
 	(1+sigma)*(3+sigma)*(4+sigma)/1680+\
 	(1+sigma)*(2+sigma)*(4+sigma)/1680+\
 	(1+sigma)*(2+sigma)*(3+sigma)/1680;
 
 	return b5d
+	
+
+
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/divne.py` & `pyseistr-win-0.0.1.1/pyseistrw/divne.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/fk.py` & `pyseistr-win-0.0.1.1/pyseistrw/fk.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/mf.py` & `pyseistr-win-0.0.1.1/pyseistrw/mf.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/operators.py` & `pyseistr-win-0.0.1.1/pyseistrw/operators.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/plot.py` & `pyseistr-win-0.0.1.1/pyseistrw/plot.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/pwsmooth.py` & `pyseistr-win-0.0.1.1/pyseistrw/pwsmooth.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/pwspray2d.py` & `pyseistr-win-0.0.1.1/pyseistrw/pwspray2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/pwspray3d.py` & `pyseistr-win-0.0.1.1/pyseistrw/pwspray3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/ricker.py` & `pyseistr-win-0.0.1.1/pyseistrw/ricker.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/soint3d.py` & `pyseistr-win-0.0.1.1/pyseistrw/soint3d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from soint3dcfun import *
-
 def soint3d(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,verb=1):
 	'''
 	soint3d: 3D structure-oriented interpolation
 	
 	by Yangkang Chen, 2022
 	
 	INPUT
@@ -58,54 +56,8 @@
 	mm2,tmp=solver(allpass3_lop,cgstep,n123,2*n123,mm,dd,niter,par_L,par_sol);
 	
 	dout=mm2.reshape(n1,n2,n3,order='F');
 
 	return dout
 	
 	
-def soint3dc(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,seed=202223,hasmask=1,var=0,verb=1):
-	'''
-	soint3dc: 3D structure-oriented interpolation implemented in C
-	
-	by Yangkang Chen, 2022
-	
-	INPUT
-	dn: model  noisy data
-	dipi: inline slope
-	dipx: xline slope
-	r1,r2:    spray radius
-	order:    PWD order
-	eps: regularization (default:0.01);
-	hasmask: if 1, using the provided mask; if 0, using the data itself to determine
-	
-	OUTPUT
-	dout: filtered data 
-	
-	EXAMPLE
-	demos/test_pyseistr_soint3d.py
-	'''
-	
-	from .solvers import solver
-	from .solvers import cgstep
-	from .operators import allpass3_lop
-	import numpy as np
-	
-	nw=order;
-	nj1=njs[0];
-	nj2=njs[1];
-	[n1,n2,n3]=din.shape;
-
-	
-	dipi=np.float32(dipi).flatten(order='F');
-	dipx=np.float32(dipx).flatten(order='F');
-	mask=np.float32(mask).flatten(order='F');
-	din=np.float32(din).flatten(order='F');
-	dout=csoint3d(din,mask,dipi,dipx,n1,n2,n3,nw,nj1,nj2,niter,drift,seed,hasmask,var,verb);
-	dout=dout.reshape(n1,n2,n3,order='F');
-
-
-	
-	
-	return dout
-
-
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/solvers.py` & `pyseistr-win-0.0.1.1/pyseistrw/solvers.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/pyseistrw/somf2d.py` & `pyseistr-win-0.0.1.1/pyseistrw/somf2d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from sofcfun import *
-
 def somf2d(dn,dip,ns,order,eps,option=1):
 	'''
 	somf2d: structure-oriented median filter
 	
 	INPUT:
 	dn: model   noisy data
 	dip: slope (2D array)
@@ -53,55 +51,9 @@
 		else:
 			u[:,:,i2],win_tmp=svmf(u[:,:,i2],ns2,1,2);
 	
 	ds=u[:,ns,:];
 	
 	return ds
 
-def somf2dc(dn,dip,ns,order,eps,option=1,verb=1):
-	'''
-	somf2dc: structure-oriented median filter in C
-	
-	INPUT
-	dn: model   noisy data
-	dip: slope (2D array)
-	ns:       spray radius
-	order:    PWD order
-	eps: regularization (default:0.01);
-	option=1 or 2: (1 for MF; 2 for SVMF)
-	
-	OUTPUT
-	ds:  filtered data
-	 
-	REFERENCES
-	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	
-	EXAMPLE
-	demos/test_pyseistr_somf2d.py
-	'''
-	
-	import numpy as np
-	ns2=2*ns+1;	#spray diameter
-	
-	if dn.ndim==2:
-		[n1,n2]=dn.shape;
-		n3=1;
-	else: #assuming ndim=3;
-		[n1,n2,n3]=dn.shape;
-	
-	dn=np.float32(dn).flatten(order='F');
-	dip=np.float32(dip).flatten(order='F');
-	
-	ds=csomf2d(dn,dip,n1,n2,n3,ns,2*ns+1,option,order,eps,verb);
-	ds=ds.reshape(n1,n2,n3,order='F')
-	
-	if n3==1:	#for 2D problems
-		ds=np.squeeze(ds)
-	return ds
-	
-
-
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/somf3d.py` & `pyseistr-win-0.0.1.1/pyseistrw/somf3d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from sof3dcfun import *
-
 def somf3d(dn,dipi,dipx,r1,r2,eps,order,option=1):
 	'''
 	somf3d: 3D structure-oriented median filter
 	
 	by Yangkang Chen, 2022
 	
 	INPUT
@@ -46,53 +44,7 @@
 			else:
 				u[:,:,i2,i3],win_tmp=svmf(u[:,:,i2,i3],ns2,1,2);
 	
 	ds=u[:,int(nnp/2),:,:];
 
 	return ds
 
-
-def somf3dc(dn,dipi,dipx,r1,r2,eps,order,option=1,verb=1):
-	'''
-	somf3dc: 3D structure-oriented median filter implemented in C
-	
-	by Yangkang Chen, 2022
-	
-	INPUT
-	dn: model  noisy data
-	dipi: inline slope
-	dipx: xline slope
-	r1,r2:    spray radius
-	order:    PWD order
-	eps: regularization (default:0.01);
-	
-	OUTPUT
-	ds: filtered data
-	 
-	REFERENCES
-	Huang et al., 2021, Erratic noise suppression using iterative structure-oriented space-varying median filtering with sparsity constraint, Geophysical Prospecting, 69, 101-121.
-	Chen et al., 2020, Deblending of simultaneous-source data using a structure-oriented space-varying median filter, Geophysical Journal International, 222, 1805–1823.
-	Gan et al., 2016, Separation of simultaneous sources using a structural-oriented median filter in the flattened dimension, Computers & Geosciences, 86, 46-54.
-	Chen, Y., 2015, Deblending using a space-varying median filter, Exploration Geophysics, 46, 332-341.
-	
-	EXAMPLE
-	demos/test_pyseistr_somf3d.py
-	'''
-	import numpy as np
-	nnp=(2*r1+1)*(2*r2+1);
-
-	if dn.ndim==2:
-		[n1,n2]=dn.shape;
-		n3=1;
-	else: #assuming ndim=3;
-		[n1,n2,n3]=dn.shape;
-		
-	dn=np.float32(dn).flatten(order='F');
-	dipi=np.float32(dipi).flatten(order='F');
-	dipx=np.float32(dipx).flatten(order='F');
-	
-	rmf=2*r1*r2+1; #median filter length
-	ds=csomf3d(dn,dipi,dipx,n1,n2,n3,r1,r2,rmf,option,order,eps,verb);
-	ds=ds.reshape([n1,n2,n3],order='F');
-
-	return ds
-
```

### Comparing `pyseistr-win-0.0.1/pyseistrw/synthetics.py` & `pyseistr-win-0.0.1.1/pyseistrw/synthetics.py`

 * *Files identical despite different names*

### Comparing `pyseistr-win-0.0.1/setup.py` & `pyseistr-win-0.0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def read(*names, **kwargs):
     return io.open(
         os.path.join(os.path.dirname(__file__), *names),
         encoding=kwargs.get("encoding", "utf8")).read()
 
 setup(
     name="pyseistr-win",
-    version="0.0.1",
+    version="0.0.1.1",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="A python package for structural denoising and interpolation of multi-channel seismic data",
     long_description=long_description,
     author="pyseistr-win developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyseistr-win",
     packages=['pyseistrw'],
```

