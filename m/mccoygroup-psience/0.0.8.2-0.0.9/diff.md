# Comparing `tmp/mccoygroup-psience-0.0.8.2.tar.gz` & `tmp/mccoygroup-psience-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-psience-0.0.8.2.tar", last modified: Tue Mar 28 19:48:00 2023, max compression
+gzip compressed data, was "mccoygroup-psience-0.0.9.tar", last modified: Wed Jul  5 17:52:07 2023, max compression
```

## Comparing `mccoygroup-psience-0.0.8.2.tar` & `mccoygroup-psience-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.538741 mccoygroup-psience-0.0.8.2/Psience/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.538741 mccoygroup-psience-0.0.8.2/Psience/AIMD/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AIMD/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AIMD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.538741 mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    41487 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/AnalyticModelConstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/Helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.542741 mccoygroup-psience-0.0.8.2/Psience/BasisReps/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/Bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/ClassicalBases.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23059 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/HarmonicOscillator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/Operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/Representations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateIndexers.py
--rw-r--r--   0 runner    (1001) docker     (123)   172965 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateSpaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/BasisReps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.542741 mccoygroup-psience-0.0.8.2/Psience/DGB/
--rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DGB/DGB.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DGB/Wavefunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DGB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.542741 mccoygroup-psience-0.0.8.2/Psience/DVR/
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/BaseDVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/ColbertMiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/DVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/DirectProduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/FiniteBasisDVR.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/DVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.542741 mccoygroup-psience-0.0.8.2/Psience/Data/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Data/KEData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.542741 mccoygroup-psience-0.0.8.2/Psience/Data/PsiDatasets/
--rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Data/PsiDatasets/KEData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Data/PsiDatasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Data/Surfaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/Psience/Molecools/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/CoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/MolecularFunctionExpansion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55226 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/Molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/MoleculeInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/Transformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/Vibrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Molecools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/Psience/Spectra/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Spectra/BaseSpectrum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/Psience/VPT2/
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Analyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Common.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/DegeneracySpecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49289 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    85785 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    98497 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Solver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   128546 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Terms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3670 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VPT2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/Psience/VSCF/
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VSCF/VSCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/VSCF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/Psience/Wavefun/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Wavefun/DirectProduct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Wavefun/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/Wavefun/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/Psience/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-03-28 19:47:49.000000 mccoygroup-psience-0.0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-28 19:48:00.000000 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-28 19:48:00.000000 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:48:00.000000 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 19:48:00.000000 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 19:48:00.000000 mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 19:48:00.546742 mccoygroup-psience-0.0.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-03-28 19:47:50.000000 mccoygroup-psience-0.0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/AIMD/
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AIMD/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AIMD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/AnalyticModels/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticModelConstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/Helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/BasisReps/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/ClassicalBases.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30348 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/HarmonicOscillator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateIndexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   184429 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateSpaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/DGB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76300 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/DGB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/Wavefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/DVR/
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/BaseDVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/ColbertMiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/DVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/DirectProduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/FiniteBasisDVR.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/KEData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/KEData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/Surfaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Molecools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/CoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/MolecularFunctionExpansion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55296 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/MoleculeInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Transformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Vibrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Spectra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Spectra/BaseSpectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/VPT2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Analyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/DegeneracySpecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49293 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86022 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99465 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Solver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   128543 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Terms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/VSCF/
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VSCF/VSCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VSCF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Wavefun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/DirectProduct.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/setup.py
```

### Comparing `mccoygroup-psience-0.0.8.2/LICENSE.txt` & `mccoygroup-psience-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/PKG-INFO` & `mccoygroup-psience-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.8.2
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/AIMD/Simulator.py` & `mccoygroup-psience-0.0.9/Psience/AIMD/Simulator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py` & `mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/AnalyticModelConstructors.py` & `mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticModelConstructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,14 +548,35 @@
         def _broadcast_tree(self, shape, expr_list):
             if not isinstance(expr_list, (np.ndarray,) + AnalyticModelBase.numeric_types):
                 return [self._broadcast_tree(shape, l) for l in expr_list]
             elif isinstance(expr_list, np.ndarray):
                 return expr_list
             else:
                 return np.full(shape, expr_list)
+
+        def _array_call(self, grid, core):
+            vals = core(*grid)
+            # broadcast appropriately
+            if not isinstance(vals, np.ndarray):
+                if isinstance(vals, AnalyticModelBase.numeric_types):
+                    vals = np.full(grid.shape[1:], vals)
+                else:
+                    vals = np.array(self._broadcast_tree(grid.shape[1:], vals))
+                    for _ in range(grid.ndim - 1):
+                        vals = np.moveaxis(vals, -1, 0)
+            return vals
+        def _rec_call(self, grid, core, depth=0, rec_counter=None):
+            if callable(core):
+                if rec_counter is not None:
+                    rec_counter[0] = depth
+                return self._array_call(grid, core)
+            else:
+                if rec_counter is None:
+                    rec_counter = [-1]
+                return [self._rec_call(grid, c, depth=depth+1, rec_counter=rec_counter) for c in core]
         def __call__(self, grid, vector=None, **kwargs):
             core = self.lam
             ndim = self.ndim
             grid = np.asanyarray(grid)
             if grid.ndim == 1:
                 vals = core(*grid)
                 if not isinstance(vals, AnalyticModelBase.numeric_types):
@@ -563,29 +584,50 @@
                 return vals
 
             if vector is None:
                 vector = grid.shape[-1] == ndim and grid.shape[0] != ndim
             if vector:
                 grid = np.moveaxis(grid, -1, 0) #grid.transpose(np.roll(np.arange(grid.ndim), 1))
 
-            vals = core(*grid)
-            # broadcast appropriately
-            if not isinstance(vals, np.ndarray):
-                if isinstance(vals, AnalyticModelBase.numeric_types):
-                    vals = np.full(grid.shape[1:], vals)
-                else:
-                    vals = np.array(self._broadcast_tree(grid.shape[1:], vals))
-                    for _ in range(grid.ndim - 1):
-                        vals = np.moveaxis(vals, -1, 0)
-            return vals
+            rec_counter = [0] # ugly hack to track the number of recursions done over lists
+            base = self._rec_call(grid, core, rec_counter=rec_counter)
+            res = np.asanyarray(base)
+            if not isinstance(base, np.ndarray):
+                # raise Exception(
+                #     res.shape,
+                #
+                # )
+                # print(
+                #     np.roll(np.arange(res.ndim), -rec_counter[0]),
+                #     rec_counter[0]
+                # )
+                res = res.transpose(
+                    np.roll(np.arange(res.ndim), -rec_counter[0])
+                )
+
+            return res
+
         def __repr__(self):
             return "{}({})".format(
                 type(self).__name__,
                 self.expr
             )
+
+        @classmethod
+        def _lambdiy(cls, vars, expr):
+            if isinstance(expr, sym.Expr):
+                core = sym.lambdify(vars, expr)
+                return core
+            else:
+                return [cls._lambdiy(vars, e) for e in expr]
+        @classmethod
+        def lambdify(cls, vars, expr, ndim):
+            core = cls._lambdiy(vars, expr)
+            return cls(expr, core, ndim)
+
     def wrap_function(self, expr, transform_coordinates=True, mode=None):
         coord_vec = self.coords
         ndim = len(coord_vec)
         if isinstance(expr, AnalyticModelBase.numeric_types):
             if isinstance(expr, np.ndarray):
                 val = expr
             else:
@@ -594,18 +636,16 @@
 
         if transform_coordinates and self.rotation is not None:
             coord_vec, new_coords = self._get_rotated_coordinates()
             # subtract off equilibrium values since we have a rotation...
             shift_subs = [(s, s+self.vals[s]) for s in self.coords if s in self.vals]
             expr = expr.subs(shift_subs)
             expr = expr.subs([(old, new) for old,new in zip(self.coords, new_coords)])
-        core = sym.lambdify(coord_vec, expr)
-
 
-        return self.SympyExpr(expr, core, ndim)
+        return self.SympyExpr.lambdify(coord_vec, expr, ndim)
 
     def expand_potential(self, order, lambdify=True, evaluate=True, contract=True):
         potential_expansions = self.v(order, evaluate=evaluate)
         coord_vec = self.coords
         if contract:
             pots = []
             for i, d in enumerate(potential_expansions):
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/AnalyticModels/Helpers.py` & `mccoygroup-psience-0.0.9/Psience/AnalyticModels/Helpers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/Bases.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/Bases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/ClassicalBases.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/ClassicalBases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/HarmonicOscillator.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/HarmonicOscillator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 Provides representations based on starting from a harmonic oscillator basis
 """
 
 __all__ = [
     "HarmonicOscillatorBasis",
-    "HarmonicOscillatorProductBasis"
+    "HarmonicOscillatorProductBasis",
+    "HarmonicOscillatorMatrixGenerator",
+    "HarmonicOscillatorRaisingLoweringPolyTerms"
 ]
 
 import scipy.sparse as sp, numpy as np, functools, itertools
+import scipy.signal
 
 from .Bases import *
 from .Operators import Operator, ContractedOperator
 from .StateSpaces import BraKetSpace
 
 from McUtils.Data import WavefunctionData
 from McUtils.Scaffolding import MaxSizeCache
 import McUtils.Numputils as nput
+from McUtils.Combinatorics import StirlingS1, Binomial
+from McUtils.Zachary import DensePolynomial
 
 class HarmonicOscillatorBasis(RepresentationBasis):
     """
     Provides a concrete implementation of RepresentationBasis using the H.O.
     Need to make it handle units a bit better.
     Currently 1D, need to make multidimensional in the future.
     """
@@ -235,14 +240,483 @@
 
     def __repr__(self):
         return "HOBasis(dim={})".format(len(self.dimensions))
         #     ",".join(str(x) for x in self.dimensions)
         # )
 
 default_cache_size = 128
+
+
+class HarmonicOscillatorRaisingLoweringPolyTerms:
+    """
+    The polynomial induced by _a_ raising operations and _b_ lowering ops
+    """
+    _stirlings = None
+    _binomials = None
+
+    @classmethod
+    def get_poly_coeffs(cls, a, b, shift=0):
+        if b > a:
+            shift = a - b + shift
+            a, b = b, a
+        prefactor = cls.binom(a + b, a)
+        coeffs = prefactor * cls.get_reduced_raising_lowering_coeffs(a, b)
+        if shift != 0:
+            coeffs = DensePolynomial._compute_shifted_coeffs(coeffs, shift)
+        return coeffs
+
+    @classmethod
+    def get_sqrt_remainder_coeffs(cls, delta, k):
+        # provides rising or falling coeffs with a starting shift
+        # by essentially only providing rising coeffs but
+        # shifting appropriately
+        d = min(abs(delta), abs(k))
+        if delta == 0:
+            return 1
+        elif delta < 0:
+            # we're falling towards zero from above, so we shift our starting point
+            # and swap the ordering so we can use a rising fac instead
+            k = k + d
+        # because of the asymmetry of falling and rising
+        # we shift our starting point
+        k = k + 1
+        if k == 0:
+            return np.array([ np.abs(cls.s1(d, j)) for j in range(0, d + 1) ])
+        else:
+            return np.array([
+                sum(
+                    cls.binom(j, l) * np.abs(cls.s1(d, j)) * (k**(j-l))
+                    for j in range(l, d+1)
+                )
+                for l in range(0, d+1)
+            ])
+
+    @classmethod
+    def s1(cls, i, j):
+        if cls._stirlings is None or cls._stirlings.shape[0] <= i or cls._stirlings.shape[0] <= j:
+            cls._stirlings = StirlingS1(2 ** int(np.ceil(np.log2(max([64, i, j])))))
+        return cls._stirlings[i, j]
+
+    @classmethod
+    def binom(cls, i, j):
+        if cls._binomials is None or cls._binomials.shape[0] <= i or cls._binomials.shape[0] <= j:
+            cls._binomials = Binomial(2 ** int(np.ceil(np.log2(max([64, i, j])))))
+        return cls._binomials[i, j]
+
+    @classmethod
+    def get_reduced_raising_lowering_coeffs(cls, a, b):
+        return np.array([
+            sum(
+                (cls.s1(b - w, j) * cls.binom(a, w) * cls.binom(b, w) * np.math.factorial(w) / (2 ** w))
+                for w in range(0, b - j + 1)
+            )
+            for j in range(0, b + 1)
+        ])
+
+
+class HarmonicOscillatorMatrixGenerator:
+    """
+    1D evaluator for terms looking like `x`, `p`, `q`, etc.
+    All of the overall `(-i)^N` info is in the `ProdOp` class that's expected to hold this.
+    Only maintains phase info & calculates elements.
+    """
+
+    state_cache_size = default_cache_size
+    default_evaluator_mode = 'poly'
+    def __init__(self, terms, mode=None):
+        self.terms = tuple(terms)
+        self.N = len(terms)
+        self.generators = {}
+        if mode is None:
+            mode = self.default_evaluator_mode
+        self.mode = mode
+        if mode == 'poly':
+            self.p_pos = None
+        else:
+            p_pos = []
+            for i, o in enumerate(terms):
+                if o == "p":
+                    p_pos.append(i)
+            self.p_pos = tuple(p_pos)
+        self._state_group_cache = MaxSizeCache(self.state_cache_size)
+
+    def __repr__(self):
+        return "{}({})".format(
+            type(self).__name__,
+            ", ".join(self.terms)
+        )
+
+    _eval_cache_size = default_cache_size
+    _evaluators = None
+    @classmethod
+    def clear_cache(cls):
+        cls._evaluators = MaxSizeCache(cls._eval_cache_size)
+    @classmethod
+    def set_cache_size(cls, new_size):
+        cls._eval_cache_size = new_size
+        cls._evaluators = cls._evaluators[:new_size]
+    @classmethod
+    def load_cached(cls, terms):
+        if cls._evaluators is None:
+            cls.clear_cache() # lol
+        if terms in cls._evaluators:
+            eval = cls._evaluators[terms]
+        else:
+            eval = cls(terms)
+            cls._evaluators[terms] = eval
+
+        return eval
+
+    @property
+    def selection_rules(self):
+        return list(range(-self.N, self.N+1, 2))
+
+    def __call__(self, states):
+        return self.evaluate_state_terms(states)
+        # return self.evaluate_state_terms(states)
+
+    def state_pair_hash(self, states):
+        # we use a hash to avoid recomputing harmonic terms
+        # whether or not this is the best hash is certainly up for debate
+        h1 = states[0]
+        h1.flags.writeable = False
+        h2 = states[1]
+        h2.flags.writeable = False
+        # raise Exception(h1.data, h2.data)
+        return (hash(h1.data.tobytes()), hash(h2.data.tobytes()))
+        # return (len(states[0]), np.max(states[0]), np.min(states[0]), np.max(states[1]), np.min(states[1]),)
+
+    def pull_state_groups(self, states):
+
+        deltas = states[1] - states[0]
+        groups, _ = nput.group_by(np.arange(len(states[1])), deltas)
+        # delta_vals = np.unique(deltas)
+        # delta_sels = [np.where(deltas == a) for a in delta_vals]
+        # delta_sels = []
+        # reminds = np.arange(len(deltas))
+        # for a in delta_vals:
+        #     woop = np.where(deltas[reminds] == a)
+        #     reminds = np.setdiff1d(reminds, woop[0])
+        #     delta_sels.append(woop)
+        return groups
+
+    def evaluate_state_terms(self, states, mode=None):
+        """
+        Evaluates terms coming from different state excitations.
+        Doesn't do any pre-filtering, since that's expected to be in the caller.
+
+        :param states:
+        :type states:
+        :return:
+        :rtype:
+        """
+
+        if mode is None:
+            mode = self.mode
+
+        h = self.state_pair_hash(states)
+        # might fuck things up from a memory perspective...
+        if h not in self._state_group_cache:
+            (delta_vals, delta_sels) = self.pull_state_groups(states)
+
+            biggo = np.zeros(states[0].shape)
+            for a, s in zip(delta_vals, delta_sels):
+                gen = self.load_generator(a, mode=mode)
+                biggo[s] = gen(states[0][s])
+
+            self._state_group_cache[h] = biggo
+
+        return self._state_group_cache[h]
+
+    def load_generator(self, a, mode=None):
+        # print(a)
+        if a not in self.generators:
+            if mode == 'poly':
+                gen = self.poly_term_generator(self.terms, a)
+            else:
+                gen = self.rho_term_generator(a, self.N, self.p_pos)
+            self.generators[a] = gen
+        else:
+            gen = self.generators[a]
+        return gen
+
+    @classmethod
+    def _enumerate_path(self, steps, cumsteps, delta): # we assume the parity is fine, cumsteps just an optimization
+        if len(steps) == 1:
+            a = (steps[0]+delta)//2
+            b = (steps[0]-delta)//2
+            return [[[a, b]]]
+        else:
+            s = steps[0]
+            sT = cumsteps[0]
+            min_a = max(0, (delta + (s-sT))//2)
+            max_a = min(s, (delta + (s+sT))//2)
+            paths = []
+            for a in range(min_a, max_a+1):
+                b = s - a
+                d = delta - (a - b)
+                subpaths = [p + [[a, b]] for p in self._enumerate_path(steps[1:], cumsteps[1:], d)]
+                paths.extend(subpaths)
+            return paths
+
+    @classmethod
+    def get_paths(cls, sizes, change):
+        cumsums = np.flip(np.cumsum(np.flip(sizes)))
+        # print("===", delta, "===")
+        return cls._enumerate_path(sizes, cumsums[1:], change)
+
+    @classmethod
+    def _build_xp_blocks(self, terms):
+        parities = []
+        sizes = []
+        cur_parity = (-1 if terms[0] == 'p' else 1)
+        s = 0
+        for t in terms:
+            new_parity = (-1 if t == 'p' else 1)
+            if new_parity != cur_parity:
+                parities.append(cur_parity)
+                cur_parity = new_parity
+                sizes.append(s)
+                s = 1
+            else:
+                s += 1
+        else:
+            parities.append(cur_parity)
+            sizes.append(s)
+        return np.array(sizes), np.array(parities)
+
+    @classmethod
+    def get_path_poly(cls, path, parities=None):
+        poly_contrib = None
+        k = 0
+        # print(">>>", path, parities)
+        if parities is None:
+            parities = [1]*len(path)
+
+        total_parity = 1
+        for (a, b), p in zip(reversed(path), parities):
+            total_parity *= p ** b
+            coeffs = HarmonicOscillatorRaisingLoweringPolyTerms.get_poly_coeffs(a, b, k)
+            # print(f" p({a},{b})({k})>", coeffs)
+            if poly_contrib is None:
+                poly_contrib = coeffs
+            else:
+                poly_contrib = scipy.signal.convolve(poly_contrib, coeffs)
+
+            d = a - b
+            if d != 0:
+                dir_change = np.sign(d) == -np.sign(k)  # avoid the zero case
+                if dir_change:
+                    sqrt_contrib = HarmonicOscillatorRaisingLoweringPolyTerms.get_sqrt_remainder_coeffs(d, k)
+                    # print(f" s({a},{b})({k})>", sqrt_contrib)
+                    poly_contrib = scipy.signal.convolve(poly_contrib, sqrt_contrib)
+            k = k + d
+            # print("..>", poly_contrib)
+        # print("+->", total_parity)
+        poly_contrib *= total_parity
+        # print(" > ", poly_contrib)
+
+        return poly_contrib
+
+    _size_blocks_cache = MaxSizeCache()
+    @classmethod
+    def _get_poly_coeffs(cls, terms, delta):
+
+        if (delta % 2) != len(terms) % 2:
+            return 0
+        if abs(delta) > len(terms):
+            return 0
+        # we know we need to change by delta
+        # over
+        if terms not in cls._size_blocks_cache:
+            cls._size_blocks_cache[terms] = cls._build_xp_blocks(terms)
+        sizes, parities = cls._size_blocks_cache[terms]
+        # total_parity = (-1)**(np.count_nonzero(parities-1)//2)
+        poly = None
+        cumsums = np.flip(np.cumsum(np.flip(sizes)))
+        # print("===", delta, "===")
+        for path in cls._enumerate_path(sizes, cumsums[1:], delta):
+            poly_contrib = cls.get_path_poly(path, parities=parities)
+
+            if poly is None:
+                poly = poly_contrib
+            else:
+                if len(poly) < len(poly_contrib):
+                    poly = np.pad(poly, [0, len(poly_contrib)-len(poly)])
+                elif len(poly_contrib) < len(poly):
+                    poly_contrib = np.pad(poly_contrib, [0, len(poly)-len(poly_contrib)])
+                poly = poly + poly_contrib
+
+        return poly / np.sqrt(2)**len(terms)
+
+    @classmethod
+    def get_poly_coeffs(cls, terms, delta, shift=0):
+        coeffs = cls._get_poly_coeffs(terms, delta)
+        if shift != 0:
+            coeffs = DensePolynomial._compute_shifted_coeffs(coeffs, shift=shift)
+        return coeffs
+
+    @classmethod
+    def poly_term_generator(cls, terms, delta, shift=0):
+        coeffs = cls.get_poly_coeffs(terms, delta, shift=shift)
+        if not isinstance(coeffs, np.ndarray) and coeffs == 0:
+            return lambda n: np.zeros(n.shape)
+        else:
+            orders = np.arange(len(coeffs))[:, np.newaxis]
+            dstart = delta+1 if delta < 0 else 1
+            dend = 1 if delta < 0 else delta + 1
+            if shift != 0:
+                return lambda n: np.dot(
+                    coeffs,
+                    np.power(n[np.newaxis, :], orders)
+                ) * np.sqrt(np.prod([n + i + shift for i in range(dstart, dend)], axis=0))
+            else:
+                return lambda n: np.dot(
+                    coeffs,
+                    np.power(n[np.newaxis, :], orders)
+                ) * np.sqrt(np.prod([n + i for i in range(dstart, dend)], axis=0))
+
+    _partitions_cache = MaxSizeCache()
+    @staticmethod
+    def _unique_permutations(elements):
+        """
+        From StackOverflow, an efficient enough
+        method to get unique permutations
+        :param perms:
+        :type perms:
+        :return:
+        :rtype:
+        """
+
+        class unique_element:
+            def __init__(self, value, occurrences):
+                self.value = value
+                self.occurrences = occurrences
+
+        def perm_unique_helper(listunique, result_list, d):
+            if d < 0:
+                yield tuple(result_list)
+            else:
+                for i in listunique:
+                    if i.occurrences > 0:
+                        result_list[d] = i.value
+                        i.occurrences -= 1
+                        for g in perm_unique_helper(listunique, result_list, d - 1):
+                            yield g
+                        i.occurrences += 1
+
+        if not hasattr(elements, 'count'):
+            elements = list(elements)
+        eset = set(elements)
+        listunique = [unique_element(i, elements.count(i)) for i in eset]
+        u = len(elements)
+        return list(sorted(list(perm_unique_helper(listunique, [0] * u, u - 1)), reverse=True))
+
+    @classmethod
+    def rho_term_generator(cls, a, N, sel):
+        """
+        Returns a function to be called on a quantum number to get the coefficient associated with exciting that mode by `a` quanta over
+        `N` steps w/ phase info coming from where the momenta-terms are.
+
+        :param a:
+        :type a:
+        :param N:
+        :type N:
+        :param i_phase:
+        :type i_phase:
+        :param is_complex:
+        :type is_complex:
+        :param sel:
+        :type sel:
+        :return:
+        :rtype:
+        """
+
+        if abs(a) > N or (N - a) % 2 != 0:
+            def terms(ni):
+                if isinstance(ni, (int, np.integer)):
+                    return 0
+                else:
+                    return np.zeros(ni.shape)
+            return terms
+
+        if a < 0:
+            up_steps = (N - abs(a)) // 2
+            down_steps = (N + abs(a)) // 2
+        else:
+            down_steps = (N - abs(a)) // 2
+            up_steps = (N + abs(a)) // 2
+
+        # this can be sped up considerably by using cleverer integer partitioning stuff and whatno
+        #TODO: use properer unique permutations code...
+        partitions = np.array(cls._unique_permutations(
+            [-1] * down_steps
+            + [1] * up_steps
+        ))
+        # np.unique(
+        #     np.array(list(
+        #         itertools.permutations(
+        #             [-1] * down_steps
+        #             + [1] * up_steps
+        #         )
+        #     )),
+        #     axis=0
+        # )
+
+        # print(a, down_steps, up_steps, partitions)
+        # determine the 'phase' of each 'path'
+        phases = np.prod(partitions[:, sel], axis=1) / np.sqrt(2) ** N
+        # print("   > p", sel, phases)
+        # then compute the 'paths' themselves
+        unitized = np.abs(np.sign(partitions - 1))
+        paths = np.cumsum(partitions, axis=1) + unitized
+
+        def terms(ni, phases=phases, paths=paths):
+            return cls.rho(phases, paths, ni)
+
+        return terms
+
+    @classmethod
+    def rho(cls, phases, paths, ni):
+        """
+
+        :param phases:
+        :type phases:
+        :param paths:
+        :type paths:
+        :param ni:
+        :type ni:
+        :return:
+        :rtype:
+        """
+        # finally define a function that will apply the the "path" to a quantum number and add everything up
+        mult = not isinstance(ni, (int, np.integer))
+        if mult:
+            # print("   ??", ni)
+            ni = np.asanyarray(ni)
+            # we need to make the broadcasting work
+            # requires basically that we copy the shape from ni to the beginning for phases and paths
+            # so basically we figure out how many (1) we need to insert at the end of paths
+            # and add a (1) to the start of ni
+            nidim = ni.ndim
+            for i in range(nidim):
+                # phases = np.expand_dims(phases, axis=-1)
+                paths = np.expand_dims(paths, axis=-1)
+            ni = np.expand_dims(ni, 0)
+
+        path_displacements = paths + ni
+        path_displacements[path_displacements < 0] = 0
+        path_terms = np.sqrt(np.prod(path_displacements, axis=1))
+
+        # return np.sum(phases * path_terms, axis=0)
+        if mult:
+            return np.dot(phases, path_terms)
+        else:
+            return phases * path_terms
+
 class HarmonicProductOperatorTermEvaluator:
     """
     A simple class that can be used to directly evaluate any operator built as a product of `p` and `x` terms.
     Automatically dispatches to provide different permutations.
     """
 
     def __init__(self, terms):
@@ -267,15 +741,15 @@
         if self.is_complex:
             raise ValueError("For simplicity, complex-valued operators not supported right now")
 
     _operator_cache = None
     _operator_cache_size = default_cache_size
     @classmethod
     def clear_cache(cls):
-        cls.TermEvaluator1D.clear_cache()
+        HarmonicOscillatorMatrixGenerator.clear_cache()
         cls._operator_cache = MaxSizeCache(cls._operator_cache_size)
     @classmethod
     def set_cache_size(cls, new_size):
         cls._eval_cache_size = new_size
         cls._operator_cache = cls.get_operator_cache()[:new_size]
     @classmethod
     def get_operator_cache(cls):
@@ -314,15 +788,15 @@
 
         term_spec = tuple(tuple(t) for t in ind_map.values())
 
         cache = self.get_operator_cache()
         if term_spec in cache:
             prop = cache[term_spec]
         else:
-            terms_1D = [self.TermEvaluator1D.load_cached(terms) for terms in term_spec]
+            terms_1D = [HarmonicOscillatorMatrixGenerator.load_cached(terms) for terms in term_spec]
             uinds = list(ind_map.keys())
             prop = self.ProdOp(terms_1D, uinds, self.i_phase, self.is_complex)
             cache[term_spec] = prop
 
         return prop
     @property
     def diag(self):
@@ -394,263 +868,9 @@
         def __call__(self, states):
             return self.eval_states(states)
 
         @property
         def selection_rules(self):
             return [o.selection_rules for o in self.ops]
 
-    class TermEvaluator1D:
-        """
-        1D evaluator for terms looking like `x`, `p`, `q`, etc.
-        All of the overall `(-i)^N` info is in the `ProdOp` class that's expected to hold this.
-        Only maintains phase info & calculates elements.
-        """
-
-
-        state_cache_size = default_cache_size
-        def __init__(self, terms):
-            self.terms = terms
-            self.N = len(terms)
-            self.generators = {}
-            p_pos = []
-            for i, o in enumerate(terms):
-                if o == "p":
-                    p_pos.append(i)
-            self.p_pos = tuple(p_pos)
-            self._state_group_cache = MaxSizeCache(self.state_cache_size)
-
-        def __repr__(self):
-            return "{}({})".format(
-                type(self).__name__,
-                ", ".join(self.terms)
-            )
-
-        _eval_cache_size = default_cache_size
-        _evaluators = None
-        @classmethod
-        def clear_cache(cls):
-            cls._evaluators = MaxSizeCache(cls._eval_cache_size)
-        @classmethod
-        def set_cache_size(cls, new_size):
-            cls._eval_cache_size = new_size
-            cls._evaluators = cls._evaluators[:new_size]
-        @classmethod
-        def load_cached(cls, terms):
-            if cls._evaluators is None:
-                cls.clear_cache() # lol
-            if terms in cls._evaluators:
-                eval = cls._evaluators[terms]
-            else:
-                eval = cls(terms)
-                cls._evaluators[terms] = eval
-
-            return eval
-
-        @property
-        def selection_rules(self):
-            return list(range(-self.N, self.N+1, 2))
-
-        def __call__(self, states):
-            return self.evaluate_state_terms(states)
-
-        def state_pair_hash(self, states):
-            # we use a hash to avoid recomputing harmonic terms
-            # whether or not this is the best hash is certainly up for debate
-            h1 = states[0]
-            h1.flags.writeable = False
-            h2 = states[1]
-            h2.flags.writeable = False
-            # raise Exception(h1.data, h2.data)
-            return (hash(h1.data.tobytes()), hash(h2.data.tobytes()))
-            # return (len(states[0]), np.max(states[0]), np.min(states[0]), np.max(states[1]), np.min(states[1]),)
-
-        def pull_state_groups(self, states):
-
-            deltas = states[1] - states[0]
-            groups, _ = nput.group_by(np.arange(len(states[1])), deltas)
-            # delta_vals = np.unique(deltas)
-            # delta_sels = [np.where(deltas == a) for a in delta_vals]
-            # delta_sels = []
-            # reminds = np.arange(len(deltas))
-            # for a in delta_vals:
-            #     woop = np.where(deltas[reminds] == a)
-            #     reminds = np.setdiff1d(reminds, woop[0])
-            #     delta_sels.append(woop)
-            return groups
-
-        def evaluate_state_terms(self, states):
-            """
-            Evaluates terms coming from different state excitations.
-            Doesn't do any pre-filtering, since that's expected to be in the caller.
-
-            :param states:
-            :type states:
-            :return:
-            :rtype:
-            """
-
-            h = self.state_pair_hash(states)
-            # might fuck things up from a memory perspective...
-            if h not in self._state_group_cache:
-                (delta_vals, delta_sels) = self.pull_state_groups(states)
-
-                biggo = np.zeros(states[0].shape)
-                for a, s in zip(delta_vals, delta_sels):
-                    gen = self.load_generator(a)
-                    og = states[0][s]
-                    vals, inv = np.unique(og, return_inverse=True)
-                    biggo[s] = gen(vals)[inv]
-
-                self._state_group_cache[h] = biggo
-
-            return self._state_group_cache[h]
-
-
-        def load_generator(self, a):
-            # print(a)
-            if a not in self.generators:
-                gen = self.rho_term_generator(a, self.N, self.p_pos)
-                self.generators[a] = gen
-            else:
-                gen = self.generators[a]
-            return gen
-
-        _partitions_cache = MaxSizeCache()
-        @staticmethod
-        def _unique_permutations(elements):
-            """
-            From StackOverflow, an efficient enough
-            method to get unique permutations
-            :param perms:
-            :type perms:
-            :return:
-            :rtype:
-            """
-
-            class unique_element:
-                def __init__(self, value, occurrences):
-                    self.value = value
-                    self.occurrences = occurrences
-
-            def perm_unique_helper(listunique, result_list, d):
-                if d < 0:
-                    yield tuple(result_list)
-                else:
-                    for i in listunique:
-                        if i.occurrences > 0:
-                            result_list[d] = i.value
-                            i.occurrences -= 1
-                            for g in perm_unique_helper(listunique, result_list, d - 1):
-                                yield g
-                            i.occurrences += 1
-
-            if not hasattr(elements, 'count'):
-                elements = list(elements)
-            eset = set(elements)
-            listunique = [unique_element(i, elements.count(i)) for i in eset]
-            u = len(elements)
-            return list(sorted(list(perm_unique_helper(listunique, [0] * u, u - 1)), reverse=True))
-
-        @classmethod
-        def rho_term_generator(cls, a, N, sel):
-            """
-            Returns a function to be called on a quantum number to get the coefficient associated with exciting that mode by `a` quanta over
-            `N` steps w/ phase info coming from where the momenta-terms are.
-
-            :param a:
-            :type a:
-            :param N:
-            :type N:
-            :param i_phase:
-            :type i_phase:
-            :param is_complex:
-            :type is_complex:
-            :param sel:
-            :type sel:
-            :return:
-            :rtype:
-            """
-
-            if abs(a) > N or (N - a) % 2 != 0:
-                def terms(ni):
-                    if isinstance(ni, (int, np.integer)):
-                        return 0
-                    else:
-                        return np.zeros(ni.shape)
-                return terms
-
-            if a < 0:
-                up_steps = (N - abs(a)) // 2
-                down_steps = (N + abs(a)) // 2
-            else:
-                down_steps = (N - abs(a)) // 2
-                up_steps = (N + abs(a)) // 2
-
-            # this can be sped up considerably by using cleverer integer partitioning stuff and whatno
-            #TODO: use properer unique permutations code...
-            partitions = np.array(cls._unique_permutations(
-                [-1] * down_steps
-                + [1] * up_steps
-            ))
-            # np.unique(
-            #     np.array(list(
-            #         itertools.permutations(
-            #             [-1] * down_steps
-            #             + [1] * up_steps
-            #         )
-            #     )),
-            #     axis=0
-            # )
-
-            # print(a, down_steps, up_steps, partitions)
-            # determine the 'phase' of each 'path'
-            phases = np.prod(partitions[:, sel], axis=1) / np.sqrt(2) ** N
-            # print("   > p", sel, phases)
-            # then compute the 'paths' themselves
-            unitized = np.abs(np.sign(partitions - 1))
-            paths = np.cumsum(partitions, axis=1) + unitized
-
-            def terms(ni, phases=phases, paths=paths):
-                return cls.rho(phases, paths, ni)
-
-            return terms
-
-        @classmethod
-        def rho(cls, phases, paths, ni):
-            """
-
-            :param phases:
-            :type phases:
-            :param paths:
-            :type paths:
-            :param ni:
-            :type ni:
-            :return:
-            :rtype:
-            """
-            # finally define a function that will apply the the "path" to a quantum number and add everything up
-            mult = not isinstance(ni, (int, np.integer))
-            if mult:
-                # print("   ??", ni)
-                ni = np.asanyarray(ni)
-                # we need to make the broadcasting work
-                # requires basically that we copy the shape from ni to the beginning for phases and paths
-                # so basically we figure out how many (1) we need to insert at the end of paths
-                # and add a (1) to the start of ni
-                nidim = ni.ndim
-                for i in range(nidim):
-                    # phases = np.expand_dims(phases, axis=-1)
-                    paths = np.expand_dims(paths, axis=-1)
-                ni = np.expand_dims(ni, 0)
-
-            path_displacements = paths + ni
-            path_displacements[path_displacements < 0] = 0
-            path_terms = np.sqrt(np.prod(path_displacements, axis=1))
-
-            # return np.sum(phases * path_terms, axis=0)
-            if mult:
-                return np.dot(phases, path_terms)
-            else:
-                return phases * path_terms
-
     def __repr__(self):
         return "{}({})".format("HOTermEvaluator", ", ".join(str(t) for t in self.terms))
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/Operators.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/Operators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/Representations.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/Representations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateFilters.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/StateFilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
     def from_property_rules(cls,
                             initial_space,
                             target_space,
                             perturbation_rules,
                             property_rules,
                             order=2,
                             postfilters=None
+                            , **opts
                             ):
         """
         :param initial_space:
         :type initial_space:
         :param target_space:
         :type target_space:
         :param perturbation_rules:
@@ -339,15 +340,16 @@
         :rtype:
         """
         int_rules = cls._create_prop_rules_tree(
             initial_space,
             target_space,
             perturbation_rules,
             property_rules,
-            order=order
+            order=order,
+            **opts
         )
 
         if isinstance(initial_space, BasisStateSpace):
             basis = initial_space.basis
             ndim = initial_space.ndim
         else:
             from .HarmonicOscillator import HarmonicOscillatorProductBasis
@@ -420,15 +422,16 @@
     def _create_prop_rules_tree(cls,
                                 initial_space,
                                 target_space,
                                 perturbation_rules,
                                 property_rules,
                                 order=2,
                                 eliminate_negatives=True,
-                                subspace=True
+                                subspace=True,
+                                check_subspaces=True
                                 ):
 
         # we really want to do this one at a time for every initial quanta
         # and target quanta pair
 
         init_nquanta, init_places = cls._build_nquanta_trees(initial_space, perturbation_rules, order)
         targ_nquanta, targ_places = cls._build_nquanta_trees(target_space, perturbation_rules, order)
@@ -495,21 +498,24 @@
                 for ord,rules in full_rules.items()
             }
 
         if isinstance(target_space, BasisStateSpace):
             target_space = target_space.excitations
         space_counts = dict(zip(*np.unique(np.sum(target_space, axis=1), return_counts=True)))
         quants = list(space_counts.keys())
-        is_subspace = {
-            k:space_counts[k] < v
-            for k,v in zip(
-                quants,
-                BasisStateSpace.num_states_with_quanta(quants, len(target_space[0]))
-            )
-        }
+        if check_subspaces:
+            is_subspace = {
+                k:space_counts[k] < v
+                for k,v in zip(
+                    quants,
+                    BasisStateSpace.num_states_with_quanta(quants, len(target_space[0]))
+                )
+            }
+        else:
+            is_subspace = {}
 
         tree_ordering = list(sorted(full_rules.keys()))
         tree_groups = [[full_rules[x] for x in tree_ordering if x[0] == i+1] for i in range(order)]
         new_rules = {
             k:cls._prune_transition_tree(
                 tree_groups[k[0]-1][:k[1]],
                 t,
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateIndexers.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/StateIndexers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/StateSpaces.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/StateSpaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Provides a relatively haphazard set of simple classes to keep track of state information.
 By providing a single interface here, we can avoid recomputing information over and over.
 """
+import itertools
 
 import numpy as np, itertools as ip, enum, scipy.sparse as sp
 import abc
 
 from McUtils.Numputils import SparseArray
 import McUtils.Numputils as nput, McUtils.Misc as mcmisc
 from McUtils.Parallelizers import Parallelizer, SerialNonParallelizer
@@ -2215,15 +2216,15 @@
                                                           )
 
 class SelectionRuleStateSpace(BasisMultiStateSpace):
     """
     A `BasisMultiStateSpace` subclass that is only built from applying selection rules to an initial space
     This really should have been called `TransformedStateSpace` but I am dumb
     """
-    def __init__(self, init_space, excitations, selection_rules=None, ignore_shapes=False):
+    def __init__(self, init_space, excitations, selection_rules=None, ignore_shapes=False, changes=None):
         """
         :param init_space:
         :type init_space:
         :param excitations:
         :type excitations:
         :param selection_rules:
         :type selection_rules:
@@ -2238,14 +2239,17 @@
             excitations = new_exc
         if not ignore_shapes and len(init_space) != len(excitations):
             raise ValueError("index space {} doesn't work with excitations {}".format(init_space, excitations))
         if not init_space.is_unique():
             raise ValueError("index space {} contains duplicate elements")
         self._base_space = init_space
         self.sel_rules = selection_rules
+        self.changes = changes
+        # if changes is not None:
+        #     raise Exception(...)
         super().__init__(excitations)
 
     def to_state(self, serializer=None):
         return {
             'base_space':self._base_space,
             'spaces':[{'indices':x._indices, 'excitations':x._excitations} for x in self.spaces.flatten()],
             'selection_rules':self.sel_rules
@@ -2315,14 +2319,17 @@
         Takes the intersection of each held space and the specified states
         :param states:
         :type states:
         :return:
         :rtype:
         """
 
+        if self.changes is not None:
+            raise NotImplementedError("need to handle state change tracking")
+
 
         # if self.spaces.ndim == 1:
         new_spaces = [
                 s.take_states(states,
                                     track_excitations=track_excitations,
                                     track_indices=track_indices
                                     ) for s in self.spaces.flat
@@ -2340,14 +2347,18 @@
         Takes the intersection of each held space and the specified states
         :param states:
         :type states:
         :return:
         :rtype:
         """
 
+
+        if self.changes is not None:
+            raise NotImplementedError("need to handle state change tracking")
+
         def take_inter(space, states=states):
             try:
                 return space.take_subspace(states)
             except:
                 raise ValueError(space, len(self.spaces[0]), self.spaces[0], self.spaces.shape)
 
         new_spaces = [s.take_subspace(states) for s in self.spaces.flat]
@@ -2367,14 +2378,17 @@
         Takes the subdimensions from each space
         :param inds:
         :type inds:
         :return:
         :rtype:
         """
 
+        if self.changes is not None:
+            raise NotImplementedError("need to work in changes")
+
         def take(space, inds=inds):
             return space.take_subdimensions(inds)
 
         new_spaces = [take(s) for s in self.spaces.flat]
         ret_spaces = np.full(len(new_spaces), None, dtype=object)
         for i, s in enumerate(new_spaces):
             ret_spaces[i] = s
@@ -2391,14 +2405,17 @@
         Takes the intersection of each held space and the specified states
         :param states:
         :type states:
         :return:
         :rtype:
         """
 
+        if self.changes is not None:
+            raise NotImplementedError("need to handle state change tracking")
+
         def take_inter(space, states=states):
             try:
                 return space.drop_states(states)
             except:
                 raise ValueError(space, len(self.spaces[0]), self.spaces[0], self.spaces.shape)
 
         if self.spaces.ndim == 1:
@@ -2412,14 +2429,18 @@
         Takes the intersection of each held space and the specified states
         :param states:
         :type states:
         :return:
         :rtype:
         """
 
+
+        if self.changes is not None:
+            raise NotImplementedError("need to handle state change tracking")
+
         def take_inter(space, states=inds):
             try:
                 return space.drop_subspace(states)
             except:
                 raise ValueError(space, len(self.spaces[0]), self.spaces[0], self.spaces.shape)
 
         if self.spaces.ndim == 1:
@@ -2433,14 +2454,17 @@
         Takes the subdimensions from each space
         :param inds:
         :type inds:
         :return:
         :rtype:
         """
 
+        if self.changes is not None:
+            raise NotImplementedError("need to work in changes")
+
         def take(space, inds=inds):
             return space.drop_subdimension(inds)
         new_spaces = np.apply_along_axis(take, -1, self.spaces)
         return type(self)(self._base_space.drop_subdimension(inds), new_spaces)
 
     def get_representation_indices(self,
                                    other=None,
@@ -2515,15 +2539,14 @@
         # upairs = pairs[np.sort(upos), ...]
         # raise Exception(len(upos), len(pairs), len(inds_l), len(upairs))
 
         if return_filter:
             return upairs, filter
         else:
             return upairs
-
     def filter_representation_inds(self, ind_pairs, q_changes):
         """
         Filters representation indices by the allowed #quantum changes.
         Not sure I'll even need this, if `get_representation_indices` is tight enough.
 
         :param ind_pairs:
         :type ind_pairs:
@@ -2545,14 +2568,35 @@
         good_doggo = np.full((len(diffs),), False, dtype=bool)
         for q in q_changes:
             good_doggo = np.logical_or(good_doggo, diffs == q)
 
         new_stuff = np.array([d[good_doggo] for d in ind_pairs])
         return new_stuff
 
+    def get_representation_brakets(self,
+                                   freqs=None,
+                                   freq_threshold=None,
+                                   other=None,
+                                   selection_rules=None,
+                                   filter=None,
+                                   return_filter=False
+                                   ):
+        brakets = super().get_representation_brakets(
+            freqs=freqs,
+            freq_threshold=freq_threshold,
+            other=other,
+            selection_rules=selection_rules,
+            filter=filter,
+            return_filter=return_filter
+        )
+        if self.changes is not None:
+            flat_changes = np.concatenate(self.changes, axis=0)
+            brakets.changes = flat_changes
+        return brakets
+
     @classmethod
     def _from_permutations(cls, space, permutations, filter_space, selection_rules):
         """
         Applies a set of permutations to an initial space and returns a new state space.
 
         :param space:
         :type space:
@@ -2671,51 +2715,85 @@
     def _apply_rules_recursive(cls, space, permutations, filter_space, selection_rules, iterations=1):
         new = cls._from_permutations(space, permutations, filter_space, selection_rules)
         if iterations > 1:
             for n, s in enumerate(new):
                 new[n] = cls._apply_rules_recursive(s,  permutations, filter_space, selection_rules, iterations=iterations-1)
         return new
 
+    track_change_positions=True
     @classmethod
     def _get_direct_product_spaces(cls, selection_rules, symm_grp, filter_space, logger, full_basis=None, exc=None, parallelizer=None):
 
         # selection_rules, symm_grp, filter_space = parallelizer.broadcast([selection_rules, symm_grp, filter_space])
         exc = parallelizer.scatter(exc)
 
         # parallelizer.print('block size: {s} {p}'.format(
         #     s=exc.shape, p=parallelizer
         # ))
 
         if filter_space is None:
-            new_exc, new_inds = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
-                                                                          full_basis=full_basis,
-                                                                          return_indices=True, split_results=True,
-                                                                          logger=logger
-                                                                          )
+            res = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
+                                                            full_basis=full_basis,
+                                                            return_indices=True,
+                                                            split_results=True,
+                                                            return_change_positions=cls.track_change_positions,
+                                                            logger=logger
+                                                            )
+            if cls.track_change_positions:
+                new_exc, new_inds, changes = res
+            else:
+                changes = None
+                new_exc, new_inds = res
+
+            # print("="*50)
+            # if new_exc is None:
+            #     new_exc = [symm_grp.from_indices(i) for i in new_inds]
+            # for e,n,c in zip(exc, new_exc, changes):
+            #     print(e)
+            #     print(n)
+            #     print(c)
+            #     print("-"*10)
 
             # raise Exception(new_exc, selection_rules)
             filter = None
         else:
             if isinstance(filter_space, BasisStateSpace):
                 filter_space = (filter_space.excitations, filter_space.indices)
 
-            new_exc, new_inds, filter = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
-                                                                                  full_basis=full_basis,
-                                                                                  filter_perms=filter_space,
-                                                                                  return_filter=True,
-                                                                                  return_indices=True,
-                                                                                  split_results=True,
-                                                                                  logger=logger
-                                                                                  )
+
+            res = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
+                                                            full_basis=full_basis,
+                                                            filter_perms=filter_space,
+                                                            return_filter=True,
+                                                            return_indices=True,
+                                                            return_change_positions=cls.track_change_positions,
+                                                            split_results=True,
+                                                            logger=logger
+                                                            )
+            if cls.track_change_positions:
+                new_exc, new_inds, changes, filter = res
+            else:
+                changes = None
+                new_exc, new_inds, filter = res
+
+            # new_exc, new_inds, changes, filter = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
+            #                                                                       full_basis=full_basis,
+            #                                                                       filter_perms=filter_space,
+            #                                                                       return_filter=True,
+            #                                                                       return_indices=True,
+            #                                                                        return_change_positions=True,
+            #                                                                       split_results=True,
+            #                                                                       logger=logger
+            #                                                                       )
 
         new_exc = parallelizer.gather(new_exc)
         new_inds = parallelizer.gather(new_inds)
 
         if parallelizer.on_main:
-            return new_exc, new_inds, filter
+            return new_exc, new_inds, changes, filter
 
     direct_sum_chunk_size = int(1e4) # so I can mess with this as I debug
     @classmethod
     def from_rules(cls, space, selection_rules, target_dimensions=None, filter_space=None, iterations=1, method='new',
                    parallelizer=None, chunk_size=None,
                    logger=None, track_excitations=True, track_indices=True, full_basis=None
                    ):
@@ -2753,14 +2831,17 @@
         else:
             if iterations > 1:
                 raise NotImplementedError(
                     "things have changed and higher iterations aren't currently supported but could be supported in the future by being smart with the selection rules"
                 )
 
             if target_dimensions is not None:
+                if cls.track_change_positions:
+                    raise NotImplementedError("positions tracking and using target dimensions not currently supported")
+
                 if filter_space is not None:
                     raise NotImplementedError(
                         "simultaneously filtering and using target_dimensions not currently supported"
                     )
 
                 if not track_excitations:
                     raise NotImplementedError(
@@ -2769,21 +2850,21 @@
 
                 exc = space.excitations
                 exc = exc[:, target_dimensions]
 
                 symm_grp = SymmetricGroupGenerator(exc.shape[-1])
 
                 new_exc = symm_grp.take_permutation_rule_direct_sum(exc, selection_rules,
-                                                                                      filter_perms=None,
-                                                                                      return_filter=False,
-                                                                                      full_basis=full_basis,
-                                                                                      return_indices=False,
-                                                                                      split_results=True,
-                                                                                      logger=logger
-                                                                                      )
+                                                                    filter_perms=None,
+                                                                    return_filter=False,
+                                                                    full_basis=full_basis,
+                                                                    return_indices=False,
+                                                                    split_results=True,
+                                                                    logger=logger
+                                                                    )
 
                 new = np.full(len(space), None, dtype=object)
                 for n,e in enumerate(new_exc):  # same size as input permutations
                     real_exc = np.broadcast_to(space.excitations[n], (len(e), space.excitations.shape[-1])).copy()
                     real_exc[:, target_dimensions] = e
                     new_space = BasisStateSpace(space.basis, real_exc, mode=BasisStateSpace.StateSpaceSpec.Excitations,
                                                 full_basis=full_basis
@@ -2812,23 +2893,25 @@
 
                 with par:
                     if chunk_size is None:
                         chunk_size = cls.direct_sum_chunk_size
                     if len(exc) > chunk_size:
                         new_exc = []
                         new_inds = []
+                        new_changes = []
                         filter = filter_space
                         num_chunks = len(exc) // chunk_size
                         chunks = np.array_split(exc, num_chunks, axis=0)
                         for chunk in chunks:
-                            new_exc_chunk, new_inds_chunk, filter = par.run(cls._get_direct_product_spaces,
+                            new_exc_chunk, new_inds_chunk, new_changes_chunk, filter = par.run(cls._get_direct_product_spaces,
                                                                             selection_rules, symm_grp, filter, logger, full_basis,
                                                                             main_kwargs={'exc':chunk},
                                                                             comm = list(range(len(chunk))) if len(chunk) < (1 + par.nprocs) else None
                                                                             )
+
                             if new_exc_chunk is not None:
                                 if new_exc_chunk[0] is None:
                                     if not isinstance(new_inds_chunk[0], np.ndarray):
                                         # means we got too blocky of a shape out of the parallelizer
                                         new_inds_chunk = sum(new_inds_chunk, [])
                                     new_exc_chunk = [None] * len(new_inds_chunk)
                                 elif not isinstance(new_exc_chunk[0], np.ndarray):
@@ -2836,19 +2919,28 @@
                                     new_exc_chunk = sum(new_exc_chunk, [])
                                     new_inds_chunk = sum(new_inds_chunk, [])
                             else:
                                 if not isinstance(new_inds_chunk[0], np.ndarray):
                                     # means we got too blocky of a shape out of the parallelizer
                                     new_inds_chunk = sum(new_inds_chunk, [])
                                 new_exc_chunk = [None] * len(new_inds_chunk)
+
+                            if new_changes_chunk is not None and new_changes_chunk[0] is not None:
+                                if not isinstance(new_changes_chunk[0], np.ndarray):
+                                    # means we got too blocky of a shape out of the parallelizer
+                                    new_changes_chunk = sum(new_changes_chunk, [])
                             new_exc.extend(new_exc_chunk)
                             new_inds.extend(new_inds_chunk)
+                            if new_changes_chunk is not None and new_changes_chunk[0] is not None:
+                                new_changes.extend(new_changes_chunk)
+                            else:
+                                new_changes = None
 
                     else:
-                        new_exc, new_inds, filter = par.run(cls._get_direct_product_spaces,
+                        new_exc, new_inds, new_changes, filter = par.run(cls._get_direct_product_spaces,
                                                             selection_rules, symm_grp, filter_space, logger, full_basis,
                                                             main_kwargs={'exc':exc},
                                                             comm=list(range(len(exc))) if len(exc) < (1 + par.nprocs) else None
                                                             )
                         if new_exc is not None:
                             if new_exc[0] is None:
                                 if not isinstance(new_inds[0], np.ndarray):
@@ -2863,19 +2955,26 @@
                             if len(new_inds) > 0:
                                 if not isinstance(new_inds[0], np.ndarray):
                                     # means we got too blocky of a shape out of the parallelizer
                                     new_inds = sum(new_inds, [])
                                 new_exc = [None] * len(new_inds)
                             else:
                                 new_exc = []
+                        if new_changes is not None and new_changes[0] is not None:
+                            if not isinstance(new_changes[0], np.ndarray):
+                                # means we got too blocky of a shape out of the parallelizer
+                                new_changes = sum(new_changes, [])
 
                 new = []
-                for e,i in zip(new_exc, new_inds): # looping over input excitations
+                new_chng = [] if new_changes is not None else None
+                for n,(e,i) in enumerate(zip(new_exc, new_inds)): # looping over input excitations
                     # make stuff unique...kinda just because?
                     i, _, inds = nput.unique(i, return_index=True)
+                    if new_chng is not None:
+                        new_chng.append(new_changes[n][inds,])
                     if track_excitations:
                         e = e[inds,]
                         new_space = BasisStateSpace(space.basis, e, mode=BasisStateSpace.StateSpaceSpec.Excitations,
                                                     full_basis=full_basis
                                                     )
                         new_space.indexer = np.arange(len(i))
                         new_space._uexc_indexer = new_space.indexer
@@ -2892,18 +2991,24 @@
 
                     new.append(new_space)
                 new = np.array(new, dtype=object)
 
             if len(new) == 0:
                 return None
 
+            # raise Exception(
+            #     space.excitations,
+            #     new[0].excitations,
+            #     new_chng[0]
+            # )
+
             if filter_space is None:
-                return cls(space, new, selection_rules)
+                return cls(space, new, selection_rules, changes=new_chng)
             else:
-                return cls(space, new, selection_rules), filter
+                return cls(space, new, selection_rules, changes=new_chng), filter
 
     @classmethod
     def _filter_transitions(cls, space:BasisStateSpace, excitations:"Iterable[BasisStateSpace]", excluded_transitions):
         excluded_transitions = np.asanyarray(excluded_transitions)
         if len(excluded_transitions) == 0:
             return excitations
         new = np.empty(len(space), dtype=object)
@@ -3005,15 +3110,16 @@
             else:
                 vals[bad_vals] = -1
         else:
             vals = np.full_like(vals, -1)
 
         return vals
 
-    def union(self, other,
+    def union(self,
+              other,
               handle_subspaces=True,
               track_excitations=True,
               track_indices=True
               ):
         """
         Returns a merged version of self and other, adding
         any states in other to self and merging where they intersect
@@ -3041,14 +3147,15 @@
             ))
 
         excitation_mode = (
             track_excitations
             and self.representative_space.has_excitations
             and other.representative_space.has_excitations
         )
+        # we determine which initial states are new between self and other
         if excitation_mode: # special case I guess?
             self_exc = self.representative_space.excitations
             other_exc = other.representative_space.excitations
 
             other_exclusions, sortings, union_sorting = nput.difference(
                 other_exc, self_exc
                 # sortings=(other.representative_space._exc_indexer, self.representative_space._exc_indexer)
@@ -3071,25 +3178,36 @@
             )
             other.representative_space._indexer, self.representative_space._indexer = sortings
             where_inds, _ = nput.find(other_inds, other_exclusions,
                                       sorting=other.representative_space._indexer
                                       )
             where_inds = np.sort(where_inds)
 
-        new_rep = self.representative_space.union(other.representative_space,
-                                                  track_excitations=track_excitations,
-                                                  track_indices=track_indices
-                                                  )#, union_sorting=union_sorting)
+        c1 = self.changes
+        c2 = other.changes
+        if c1 is None and c2 is not None or c2 is None and c1 is not None:
+            raise Exception("selection rule space with tracked changes and without can't be merged")
+
+
+        new_rep = self.representative_space.union(
+            other.representative_space,
+            track_excitations=track_excitations,
+            track_indices=track_indices
+        )#, union_sorting=union_sorting)
         new_spaces = np.concatenate(
             [
                 self.spaces,
                 other.spaces[where_inds,]
             ],
             axis=0
         )
+        if c1 is not None:
+            changes = c1 + [c2[w] for w in where_inds]
+        else:
+            changes = None
         if len(new_rep) != len(new_spaces):
             raise ValueError("Mismatch between union of {} and {} (rep space. len={} and subspaces len={})".format(
                 self, other, len(new_rep), len(new_spaces)
             ))
 
         if handle_subspaces:
             if excitation_mode:
@@ -3103,20 +3221,51 @@
                 _, _, _, other_inc_inds, self_inc_inds = nput.intersection(
                     other_inds, self_inds,
                     sortings=(other.representative_space._indexer, self.representative_space._indexer),
                     return_indices=True,
                     union_sorting=union_sorting
                 )
             for i_new, i_old in zip(self_inc_inds, other_inc_inds):
-                new_spaces[i_new] = new_spaces[i_new].union(other[i_old],
-                                                            track_indices=track_indices,
-                                                            track_excitations=track_excitations
-                                                            )
+                if changes is not None: #TODO: be careful about sorting
+                    ospace = other[i_old]
+                    sspace = self[i_new]
+                    if excitation_mode:
+                        ote = ospace.excitations
+                        ste = sspace.excitations
+                        other_exclusions, subsortings, subunion_sorting = nput.difference(
+                            ote, ste
+                            # sortings=(other.representative_space._exc_indexer, self.representative_space._exc_indexer)
+                        )
+                        ospace._exc_indexer, sspace._exc_indexer = subsortings
+                        where_inds, _ = nput.find(ote, other_exclusions,
+                                                  sorting=ospace._exc_indexer
+                                                  )
+                    else:
+                        oti = ospace.indices
+                        sti = sspace.indices
+                        other_exclusions, subsortings, subunion_sorting = nput.difference(
+                            oti, sti
+                            # sortings=(other.representative_space._exc_indexer, self.representative_space._exc_indexer)
+                        )
+                        ospace._indexer, sspace._indexer = subsortings
+                        where_inds, _ = nput.find(oti, other_exclusions,
+                                                  sorting=ospace._indexer
+                                                  )
+                    if len(where_inds) > 0:
+                        where_inds = np.sort(where_inds)
+                        changes[i_new] = np.concatenate([changes[i_new], c2[where_inds]])
+                    # print(" >", changes[i_new])
+
+                new_spaces[i_new] = new_spaces[i_new].union(
+                    other[i_old],
+                    track_indices=track_indices,
+                    track_excitations=track_excitations
+                )
 
-        return type(self)(new_rep, new_spaces)
+        return type(self)(new_rep, new_spaces, changes=changes)
 
     def intersection(self, other, handle_subspaces=True, use_indices=False,
                      track_excitations=True,
                      track_indices=True
                      ):
         """
         Returns an intersected self and other
@@ -3126,14 +3275,19 @@
         :return:
         :rtype:
         """
 
         if self.representative_space.full_basis is not None:
             track_excitations = False
 
+        c1 = self.changes
+        c2 = other.changes
+        if c1 is None and c2 is not None or c2 is None and c1 is not None:
+            raise Exception("selection rule space with tracked changes and without can't be merged")
+
 
         if not isinstance(other, SelectionRuleStateSpace):
             raise TypeError("intersection with {} only defined over subclasses of {}".format(
                 type(self).__name__,
                 SelectionRuleStateSpace.__name__
             ))
 
@@ -3172,21 +3326,56 @@
                 return_indices=True
             )
             where_inds = np.sort(where_inds)
 
             # _, where_inds, other_where = np.intersect1d(self_inds, other_inds, return_indices=True)
 
         new_spaces = self.spaces[where_inds,]
+        if c1 is not None:
+            changes = [c1[w] for w in where_inds]
+        else:
+            changes = None
         if handle_subspaces:
             for n,i in enumerate(other_where):
+                if changes is not None:
+                    sspace = self[n]
+                    ospace = other[n]
+                    if track_excitations and not use_indices and (
+                            sspace.has_excitations
+                            and ospace.has_excitations
+                    ):  # special case I guess?
+                        self_exc = sspace.excitations
+                        other_exc = ospace.excitations
+
+                        inter_ind, sortings, _, where_inds, _ = nput.intersection(
+                            self_exc, other_exc,
+                            sortings=(sspace._exc_indexer, ospace._exc_indexer),
+                            return_indices=True
+                        )
+
+                        self.representative_space._exc_indexer, ospace._exc_indexer = sortings
+                        where_inds = np.sort(where_inds)
+                    else:
+                        self_inds = sspace.indices
+                        other_inds = ospace.indices
+
+                        inter_ind, _, _, where_inds, _ = nput.intersection(
+                            self_inds, other_inds,
+                            sortings=(sspace.indexer, ospace.indexer),
+                            return_indices=True
+                        )
+                        where_inds = np.sort(where_inds)
+                    changes[n] = changes[n][where_inds,]
+
                 new_spaces[n] = new_spaces[n].intersection(other[n])
 
+
         new_rep = self.representative_space.take_subspace(where_inds)#(other.representative_space)
 
-        return type(self)(new_rep, new_spaces)
+        return type(self)(new_rep, new_spaces, changes=changes)
     def difference(self, other, handle_subspaces=True):
         """
         Returns an diff'ed self and other.
         We get fundamentally different behaviour for `handle_subspaces` than without it.
         If we have it _on_ then differences are computed for each states in the intersection of
           the primary (key) states.
         If we have it off then the difference in the key states is computed and nothing more is
@@ -3209,14 +3398,21 @@
 
         if self.basis != other.basis:
             raise ValueError("can't take a difference of state spaces over different bases ({} and {})".format(
                 self.basis,
                 other.basis
             ))
 
+        c1 = self.changes
+        c2 = other.changes
+        if c1 is None and c2 is not None or c2 is None and c1 is not None:
+            raise Exception("selection rule space with tracked changes and without can't be merged")
+        if c1 is not None:
+            raise NotImplementedError("change tracking for difference not implemented yet")
+
         self_inds = self.representative_space.indices
         other_inds = other.representative_space.indices
 
         if handle_subspaces:
             new_rep = self.representative_space
             inter_rep = self.representative_space.intersection(other.representative_space)
             intersected_inds = inter_rep.indices
@@ -3306,15 +3502,16 @@
     Represents a set of pairs of states that can be fed into a `Representation` or `Operator`
     to efficiently tell it what terms it need to calculate.
     This basically just implements a bunch of stuff for generating a Graph defining
     the connections between states.
     """
     def __init__(self,
                  bra_space,
-                 ket_space
+                 ket_space,
+                 changes=None
                  ):
         """
         :param bra_space:
         :type bra_space: BasisStateSpace
         :param ket_space:
         :type ket_space: BasisStateSpace
         """
@@ -3323,14 +3520,16 @@
         self.ndim = self.bras.ndim
         self._orthogs = None
         self._preind_trie = None
         if len(bra_space) != len(ket_space) or (bra_space.ndim != ket_space.ndim):
             raise ValueError("Bras {} and kets {} have different dimension".format(bra_space, ket_space))
         self._state_pairs = None
         self._state_diffs = None
+        self.changes = changes
+        self._unique_changes = None
 
     @property
     def state_pairs(self):
         if self._state_pairs is None:
             brex = self.bras.excitations
             if brex.dtype.names is not None:
                 brex = nput.uncoerce_dtype(brex, (len(brex), len(brex.dtype.names)), brex.dtype[0])
@@ -3716,14 +3915,15 @@
             """
             Directly computes orthogonality relations
             :param inds:
             :type inds:
             :return:
             :rtype:
             """
+
             orthos = self.tests
             unused = np.delete(np.arange(len(orthos)), inds)
             if subinds is None:
                 cur_inds = np.where(self.tests[unused[0]])[0]
                 unused = unused[1:]
                 for e in unused:
                     cur_inds = cur_inds[self.tests[e, cur_inds]]
@@ -3900,17 +4100,22 @@
         sels = [
             apply_rules(k - b, r) for b, k, r in zip(bra, ket, rules)
         ]
         # then we figure out which states by satisfied all the rules
         return fp.reduce(np.logical_and, sels[1:], sels[0])
 
     def take_subspace(self, sel):
+        if self.changes is not None:
+            changes = self.changes[sel,]
+        else:
+            changes = None
         sub = type(self)(
             self.bras.take_subspace(sel),
-            self.kets.take_subspace(sel)
+            self.kets.take_subspace(sel),
+            changes=changes
         )
         if len(self) > 0:
             sub.state_pairs = (
                 self.state_pairs[0][:, sel],
                 self.state_pairs[1][:, sel]
             )
         return sub
@@ -3922,41 +4127,95 @@
         )
         new.state_pairs = (
             self.state_pairs[0][inds],
             self.state_pairs[1][inds]
         )
         return new
 
+    use_change_indices = True
     def apply_non_orthogonality(self,
                                 inds,
                                 use_aggressive_caching=None,
                                 use_preindex_trie=None,
                                 preindex_trie_depth=None,
-                                assume_unique=False
+                                assume_unique=False,
+                                use_change_indices=None
                                 ):
         """
         Takes the bra-ket pairs that are non-orthogonal under the indices `inds`
 
         :param inds:
         :type inds:
         :param assume_unique:
         :type assume_unique:
         :return:
         :rtype:
         """
-        if use_aggressive_caching is None:
-            use_aggressive_caching = self.aggressive_caching_enabled
-        if use_preindex_trie is None:
-            use_preindex_trie = self.preindex_trie_enabled
-        non_orthog = self.get_non_orthog(inds,
-                                         use_aggressive_caching=use_aggressive_caching,
-                                         assume_unique=assume_unique,
-                                         use_preindex_trie=use_preindex_trie,
-                                         preindex_trie_depth=preindex_trie_depth
-                                         )
+
+        if use_change_indices is None:
+            use_change_indices = self.use_change_indices
+        if use_change_indices and self.changes is not None:
+            if self._unique_changes is None:
+                changes, indices = nput.group_by(np.arange(len(self.changes)), self.changes)[0]
+                self._unique_changes = dict(zip(changes, indices))
+
+            # raise Exception(self._unique_changes)
+
+            inds = np.unique(inds)
+            radix = self.ndim
+            possible_change_ints = np.unique([
+                SymmetricGroupGenerator.changed_index_number(
+                    idx,
+                    radix
+                )
+                for r in range(0, len(inds)+1)
+                for idx in itertools.combinations(inds, r=r)
+            ])
+            non_orthog = np.sort(np.concatenate([
+                self._unique_changes.get(c, np.array([], dtype=int))
+                for c in possible_change_ints
+            ]))
+            # if len(possible_change_ints) == 1:
+            #     non_orthog = np.where(self.changes==possible_change_ints[0])[0]
+            #     # print(">", self.state_pairs[0].T[:5])
+            #     # print(">", self.state_pairs[1].T[:5])
+            #     # print(">", self.changes[:5])
+            #     # raise Exception(...) from None
+            # else:
+            #     mask = np.full(len(self.changes), True, dtype=bool)
+            #     for c in possible_change_ints:
+            #         # print(c)
+            #         mask[mask] = np.logical_and(
+            #             mask[mask],
+            #             self.changes[mask] != c
+            #         )
+            #         # print(mask)
+            #     non_orthog = np.where(np.logical_not(mask))[0]
+            # print(">>>", non_orthog)
+        else:
+        # no = non_orthog
+            if use_aggressive_caching is None:
+                use_aggressive_caching = self.aggressive_caching_enabled
+            if use_preindex_trie is None:
+                use_preindex_trie = self.preindex_trie_enabled
+            non_orthog = self.get_non_orthog(inds,
+                                             use_aggressive_caching=use_aggressive_caching,
+                                             assume_unique=assume_unique,
+                                             use_preindex_trie=use_preindex_trie,
+                                             preindex_trie_depth=preindex_trie_depth
+                                             )
+        # print(" > ", non_orthog_old)
+        # new_issues = np.setdiff1d(non_orthog, non_orthog_old)
+        # if len(new_issues) > 0:
+        #     print(inds)
+        #     print(self.state_pairs[0].T[new_issues[0]])
+        #     print(self.state_pairs[1].T[new_issues[0]])
+        #     print(self.changes[new_issues[0]])
+        #     raise Exception(new_issues)
+
         return self.take_subspace(non_orthog), non_orthog
 
     @staticmethod
     @mcmisc.jit(nopython=True)
     def _get_rule_matches(test_space, rules, M):
         masks = {0: np.arange(len(test_space[0]))}
         inds = []
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/Wavefunctions.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/BasisReps/__init__.py` & `mccoygroup-psience-0.0.9/Psience/BasisReps/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DGB/DGB.py` & `mccoygroup-psience-0.0.9/Psience/DGB/DGB.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np, scipy as sp, itertools, functools
-from McUtils.Zachary import RBFDInterpolator
+
+from McUtils.Zachary import RBFDInterpolator, DensePolynomial
 from McUtils.Scaffolding import Logger
 from McUtils.Data import AtomData, UnitsData
 import McUtils.Numputils as nput
 
 __all__ =  [
     "DGB"
 ]
@@ -76,17 +77,19 @@
                  clustering_radius=-1,
                  min_singular_value=1e-4,
                  num_svd_vectors=None,
                  svd_contrib_cutoff=1e-3,
                  quadrature_degree=4,
                  expansion_degree=None,
                  expansion_type='multicenter',
-                 reference_structure=None
+                 reference_structure=None,
+                 poly_coeffs=None
     ):
         self._S, self._T, self._V = None, None, None
+        self._scaling_S = None
         self.logger = Logger.lookup(logger)
 
         self.potential_function = potential_function
         self.quadrature_degree = quadrature_degree
         self.expansion_degree = expansion_degree
         self.expansion_type = expansion_type
         self.ref = reference_structure
@@ -145,18 +148,23 @@
                 full_good_pos = np.unique(np.where(np.abs(evecs[:, good_loc]) > svd_contrib_cutoff)[0])
                 self.centers = self.centers[full_good_pos]
                 self.alphas = self.alphas[full_good_pos]
                 if self.transformations is not None:
                     self.transformations = [t[full_good_pos] for t in self.transformations]
 
                 self._S = None#self._S[full_good_pos, :][:, full_good_pos]
+                self._scaling_S = None
                 self._T = None#self._T[full_good_pos, :][:, full_good_pos]
 
         self.logger.log_print("Number of centers: {N}", N=len(self.centers))
 
+        if poly_coeffs is not None:
+            poly_coeffs = self.canonicalize_poly_coeffs(poly_coeffs, self.alphas)
+        self._poly_coeffs = poly_coeffs
+
     def canonicalize_transforms(self, tfs):
         if tfs is None:
             return tfs
         if isinstance(tfs, np.ndarray):
             dets = np.linalg.det(tfs)
             if not np.allclose(dets, np.ones(len(dets))):
                 raise ValueError("inverse must be supplied for non-unitary transforms")
@@ -170,34 +178,63 @@
                     for x in tfs
                 )
         ):
             raise ValueError("transforms must have shape {s}".format(
                 s=(len(self.alphas), self.alphas.shape[-1], self.alphas.shape[-1])
             ))
         return tfs
-
     @property
     def transformations(self):
         return self._transforms
     @transformations.setter
     def transformations(self, tf):
         self._transforms = self.canonicalize_transforms(tf)
 
+    def _get_hermite_poly(self, coeff_dict, alphas):
+        ndim = self.centers.shape[-1]
+        # raise Exception(
+        #     np.flip(np.asarray(sp.special.hermite(coeff_dict.get(0, 0), monic=False))) *
+        #         np.sqrt( (2 * alphas[0]) ** np.arange(coeff_dict.get(0, 0) + 1) )
+        # )
+        parts = [
+            np.flip(np.asarray(sp.special.hermite(coeff_dict.get(k, 0), monic=False)))
+            * np.sqrt(
+                (2 * alphas[k] ) ** np.arange(coeff_dict.get(k, 0)+1)
+                / ( 2**(coeff_dict.get(k, 0)) * np.math.factorial(coeff_dict.get(k, 0)) )
+            )
+            for k in range(ndim)
+        ]
+        coeffs = parts[0]
+        for c in parts[1:]:
+            coeffs = np.multiply.outer(coeffs, c)
+        return coeffs
+
+    def canonicalize_poly_coeffs(self, coeffs, alphas):
+        if coeffs is None:
+            return None
+
+        poly_coeffs = [
+            self._get_hermite_poly(c, a) if isinstance(c, dict) else c
+            for c, a in zip(coeffs, alphas)
+        ]
+
+        return poly_coeffs
+
     def optimize_centers(self,
                          centers, alphas,
                          max_condition_number=1e16,
                          initial_custering=.005,
                          cluster_step_size=.005,
-                         max_steps = 50
+                         max_steps=50
                          ):
         raise NotImplementedError("ugh...")
         c, a = centers, alphas
         cr = initial_custering
         centers, alphas = self.initialize_gaussians(c, a, cr)
-        S, T = self.get_ST(centers, alphas)
+        _, S, T = self.get_ST(centers, alphas)
         n = 0
         while np.linalg.cond(S) > max_condition_number and n < max_steps:
             cr += cluster_step_size
             n += 1
             centers, alphas = self.initialize_gaussians(c, a, cr)
             S, T = self.get_ST(centers, alphas)
 
@@ -506,23 +543,23 @@
             opts = {}
 
         return alphas, rots, opts
 
     @property
     def S(self):
         if self._S is None:
-            self._S, self._T = self.get_ST()
+            self._scaling_S, self._S, self._T = self.get_ST()
         return self._S
     @S.setter
     def S(self, smat):
         self._S = smat
     @property
     def T(self):
         if self._T is None:
-            self._S, self._T = self.get_ST()
+            self._scaling_S, self._S, self._T = self.get_ST()
         return self._T
     @T.setter
     def T(self, tmat):
         self._T = tmat
     @property
     def V(self):
         if self._V is None:
@@ -697,14 +734,15 @@
             #     print(new_alphas[0] / self.alphas[0])
             #     print(new_alphas[0] / np.linalg.eigh(sigs[0])[0])
             #     print(new_rots[0])
             #     print(self.transformations[0])
             # raise Exception(...)
 
             if self.inds is not None:
+                # build the inverse covariance in the basis of vibrational coordinates
                 i = np.array(self.inds)
                 d = np.zeros((new_alphas.shape[0], new_alphas.shape[1], new_alphas.shape[1]))
                 diag_inds = (
                     np.arange(new_alphas.shape[0])[:, np.newaxis],
                     i[np.newaxis, :],
                     i[np.newaxis, :]
                 )
@@ -735,144 +773,580 @@
                 'row_sigs': sigs[rows],
                 'col_sigs': sigs[cols],
                 'sum_inverse':sum_sigs
             }
 
         return overlap_data
 
+    def get_base_polynomials(self):
+        base_coeffs = self._poly_coeffs
+        if self.inds is not None:
+            comp = np.setdiff1d(np.arange(self.centers.shape[-1]), self.inds)
+            new_pc = []
+            for c in base_coeffs:
+                if c is not None:
+                    c = c.copy()
+                    for idx in comp:
+                        c = np.moveaxis(c, idx, 0)
+                        c = c[:1].reshape(c.shape[1:])
+                        # c = np.moveaxis(c, 0, idx)
+                new_pc.append(c)
+            base_coeffs = new_pc
+        # raise Exception(self._poly_coeffs[0].shape, base_coeffs[0].shape)
+        base_polys = [
+            DensePolynomial(coeffs) if coeffs is not None else None
+            for coeffs in base_coeffs
+        ]
+        centers = self.centers
+        if self.transformations is not None:
+            tfs, invs = self.transformations
+            if self.inds is not None:
+                tfs = tfs[:, :, self.inds]
+                invs = invs[:, self.inds, :]
+            # raise Exception(invs[0].shape)
+            base_polys = [
+                p.transform(inv) if p is not None else 1
+                for p,inv in zip(base_polys, tfs)
+            ]
+        elif self.inds is not None:
+            centers = centers[..., self.inds]
+        base_polys = [
+                p.shift(-c) if isinstance(p, DensePolynomial) else 1
+                for p,c in zip(base_polys, centers)
+            ]
+        # raise Exception(base_polys[0].coeffs)
+        return base_polys
+
+    def get_kinetic_polynomials(self):
+        # TODO: implement _multipolynomial_ support so that we can handle
+        #       this in a simpler form
+
+        ndim = self.centers.shape[-1]
+        if self.transformations is None and self.inds is not None:
+            ndim = len(self.inds)
+
+        core_polys = self.get_base_polynomials()
+        core_derivs = [ # these will be indexed by columns
+            [poly.deriv(i) if isinstance(poly, DensePolynomial) else 0 for i in range(ndim)]
+            for poly in core_polys
+        ]
+        core_d2s = [
+            [p.deriv(i) if isinstance(p, DensePolynomial) else 0 for i, p in enumerate(poly_list)]
+            for poly_list in core_derivs
+        ]
+
+        if self.transformations is None:
+            centers = self.centers
+            alphas = self.alphas
+            if self.inds is not None:
+                ndim = len(self.inds)
+                centers = centers[:, self.inds]
+                alphas = alphas[:, self.inds]
+            exp_polys = [ # these will be indexed by columns as well
+                DensePolynomial.from_tensors([0, np.zeros(ndim), np.diag(2*a)], shift=-pt, rescale=False)
+                for pt,a in zip(centers, alphas)
+            ]
+        else:
+            sigs = self.get_inverse_covariances()
+            centers = self.centers
+            if self.inds is not None:
+                Lt, L = self.transformations
+                Lt = Lt[:, :, self.inds]
+                L = L[:, self.inds, :]
+                centers = Lt@( L @ centers[:, :, np.newaxis] )
+                centers = centers.reshape(self.centers.shape)
+
+            raise Exception(sigs[2], centers[2])
+
+            exp_polys = [
+                DensePolynomial.from_tensors([0, np.zeros(ndim), sig], shift=-pt)
+                for pt,sig in zip(
+                    centers,
+                    sigs
+                )
+            ]
+        def _d(p, i):
+            if isinstance(p, DensePolynomial):
+                d = p.deriv(i)
+                if isinstance(d, DensePolynomial):
+                    d = d.clip()
+            else:
+                d = p
+            return d
+        exp_derivs = [
+            [-1/2*_d(poly, i) for i in range(ndim)]
+            for poly in exp_polys
+        ]
+ #        raise Exception(exp_derivs[0][1].coeffs)
+ #        """
+ #        [[[-0.24875972 -1.62256994]
+ #  [-1.91803054 -0.        ]]
+ #
+ # [[ 3.58730135 -0.        ]
+ #  [-0.         -0.        ]]]
+ #  """
+        exp_d2s = [
+            [_d(p, i) for i,p in enumerate(poly_list)]
+            for poly_list in exp_derivs
+        ]
+        # raise Exception(
+        #     (
+        #             (exp_derivs[0][0] * exp_derivs[0][0])
+        #             + exp_d2s[0][0].coeffs*exp_d2s[0][0].scaling
+        #     ).coeffs,
+        #     core_polys[0].coeffs
+        # )
+
+        raise Exception(
+            exp_polys[2].coeffs
+        )
+
+        # and now we can construct the polynomials for each center and axis
+        def _k(p, pd1, pd2, ed1, ed2):
+            t = pd2 + 2*pd1 * ed1 + p * ((ed1 * ed1) + ed2)
+            if isinstance(t, DensePolynomial):
+                t = t.clip(threshold=1e-8)
+            return t
+        kinetic_polys = [
+            [
+                _k(p, pd1, pd2, ed1, ed2)
+                for pd1, pd2, ed1, ed2 in zip(pd1s, pd2s, ed1s, ed2s)
+            ]
+            for p, pd1s, pd2s, ed1s, ed2s in zip(
+                core_polys,
+                core_derivs,
+                core_d2s,
+                exp_derivs,
+                exp_d2s
+            )
+        ]
+
+        # raise Exception(
+        #     kinetic_polys[0][0].coeffs,
+        #     kinetic_polys[0][1],
+        #     kinetic_polys[0][2].coefficient_tensors,
+        #     # kinetic_polys[0][0].coeffs,
+        # )
+
+        return core_polys, kinetic_polys
+
+    @classmethod
+    def _unrot_base_ST_components(cls, centers, alphas, masses, inds):
+        if inds is not None:
+            alphas = alphas[:, inds]
+            centers = centers[:, inds]
+            masses = masses[inds]
+
+        aouter = alphas[:, np.newaxis] * alphas[np.newaxis, :]
+        aplus = alphas[:, np.newaxis] + alphas[np.newaxis, :]
+        arat = aouter / aplus
+
+        disps = centers[:, np.newaxis, :] - centers[np.newaxis, :, :]
+
+        # A = outer_tet / np.sqrt(np.pi)
+        B = np.sqrt(aplus)
+        C = arat * np.power(disps, 2)
+
+        return arat, aouter, B, C, masses
+
+    @classmethod
+    def _unrot_base_S(cls, centers, alphas, masses, inds):
+
+        arat, aouter, B, C, masses = cls._unrot_base_ST_components(centers, alphas, masses, inds)
+
+        S_dim = (np.sqrt(2) * np.power(aouter, 1 / 4) / B) * np.exp(-C)
+        S = np.prod(S_dim, axis=-1)
+
+        return S
+
+    @classmethod
+    def _unrot_base_ST(cls, centers, alphas, masses, inds):
+
+        arat, aouter, B, C, masses = cls._unrot_base_ST_components(centers, alphas, masses, inds)
+
+        S_dim = (np.sqrt(2) * np.power(aouter, 1 / 4) / B) * np.exp(-C)
+        T_dim = arat * (1 - 2 * C) / masses[np.newaxis, np.newaxis, :]
+
+        S = np.prod(S_dim, axis=-1)
+        T = S * np.sum(T_dim, axis=-1)
+
+        return S, T
+
+    @classmethod
+    def _rot_base_S_components(cls, rot_data, centers, alphas, inds):
+        row_inds = rot_data['row_inds']
+        col_inds = rot_data['col_inds']
+
+        # alphas = self.alphas
+        # masses = self.masses
+        rotas = rot_data["alphas"]
+        if inds is not None:
+            alphas = alphas[:, inds]
+            rotas = rotas[:, inds]
+
+        ndim = centers.shape[-1]
+        dets = np.prod(rotas, axis=-1)
+        # we prefactor out the 2**ndim
+        rdets = np.prod(alphas[row_inds], axis=-1)
+        cdets = np.prod(alphas[col_inds], axis=-1)  # literally a product of passed in alphas
+
+        L = rot_data['inverse_rotations']  #
+        Lt = rot_data['rotations']
+        if inds is not None:
+            ndim = len(inds)
+            disps = L @ (centers[row_inds] - centers[col_inds])[:, :, np.newaxis]
+            disps = np.reshape(disps, disps.shape[:2])[:, inds]
+            si = L @ rot_data['sum_inverse'] @ Lt
+            si = si[:, inds, :][:, :, inds]
+            C = disps[:, np.newaxis, :] @ si @ disps[:, :, np.newaxis]
+        else:
+            disps = centers[row_inds] - centers[col_inds]
+            C = disps[:, np.newaxis, :] @ rot_data['sum_inverse'] @ disps[:, :, np.newaxis]
+        C = C.reshape(disps.shape[0])
+
+        return alphas, rotas, L, Lt, row_inds, col_inds, ndim, rdets, cdets, dets, C
+
+    @classmethod
+    def _rot_base_S(cls, rot_data, centers, alphas, inds):
+
+        S = np.eye(len(centers))
+        alphas, rotas, L, Lt, row_inds, col_inds, ndim, rdets, cdets, dets, C = \
+            cls._rot_base_S_components(rot_data, centers, alphas, inds)
+
+        S[row_inds, col_inds] = S[col_inds, row_inds] = (
+                2 ** (ndim / 2) * ((rdets * cdets) / (dets ** 2)) ** (1 / 4) * np.exp(-C / 2)
+        )
+        return S
+
+    @classmethod
+    def _rot_base_ST(cls, rot_data, centers, alphas, masses, inds):
+
+        S = np.eye(len(centers))
+        alphas, rotas, L, Lt, row_inds, col_inds, ndim, rdets, cdets, dets, C = \
+            cls._rot_base_S_components(rot_data, centers, alphas, inds)
+
+        S[row_inds, col_inds] = S[col_inds, row_inds] = (
+                2 ** (ndim / 2) * ((rdets * cdets) / (dets ** 2)) ** (1 / 4) * np.exp(-C / 2)
+        )
+
+        T = np.zeros((len(centers), len(centers)))
+
+        rows = rot_data['row_sigs']
+        cols = rot_data['col_sigs']
+
+        idx = col_inds
+        Sj = cols
+
+        zetas = L @ (rot_data['centers'] - centers[idx])[:, :, np.newaxis]
+        zetas = zetas.reshape(rot_data['centers'].shape)
+        if inds is not None:
+            zetas = zetas[:, inds]
+
+        minv = np.diag(1 / masses)
+        Amat = L @ (Sj @ minv @ Sj) @ Lt
+        M = L @ np.broadcast_to(minv[np.newaxis], L.shape) @ Lt
+        # msj = rot_data['rotations']@(Sj@minv)@np.transpose(rot_data['rotations'], (0, 1, 2))
+        # raise Exception(
+        #     np.diagonal(msj, axis1=1, axis2=2),# / self.masses[np.newaxis],
+        #     - 1 / 2 * np.diagonal(Amat, axis1=1, axis2=2) / rot_data['alphas']
+        # )
+        submasses = np.diagonal(M, axis1=1, axis2=2)
+        sminv = np.diagonal(Amat, axis1=1, axis2=2)
+        if inds is not None:
+            submasses = submasses[:, inds]
+            sminv = sminv[:, inds]
+            Amat = Amat[:, inds, :][:, :, inds]
+        # raise Exception(
+        #     submasses,
+        #     sminv,
+        #     np.sum(
+        #         2 * alphas[col_inds] * submasses -
+        #         1 / 2 * sminv / rotas,
+        #         axis=1
+        #     )
+        # )
+        T[row_inds, col_inds] = 1 / 2 * (
+                np.sum(
+                    2 * alphas[idx] * submasses - 1 / 2 * sminv / rotas,
+                    axis=1
+                ) - 1 / 2 * sum(
+            # easier this way than the proper series summation...
+            Amat[..., k, kp] * (
+                4 * zetas[..., k] * zetas[..., kp]  # I discovered I was off by a factor of 4 in the 2D case...
+                    if k != kp else
+                2 * zetas[..., k] ** 2
+            )
+            for k, kp in zip(*np.triu_indices(Amat.shape[-1]))
+        )  # could be a dot but this is fine
+        )
+        T[row_inds, col_inds] *= S[row_inds, col_inds]
+        T[col_inds, row_inds] = T[row_inds, col_inds]
+
+        return S, T
+
+    @classmethod
+    def _rot_poly_ST(cls, rot_data, base_polys, centers, alphas, masses, inds):
+
+        # S = np.eye(len(centers))
+        alphas, rotas, L, Lt, row_inds, col_inds, ndim, rdets, cdets, dets, C = \
+            cls._rot_base_S_components(rot_data, centers, alphas, inds)
+
+        # S[row_inds, col_inds] = S[col_inds, row_inds] = (
+        #         2 ** (ndim / 2) * ((rdets * cdets) / (dets ** 2)) ** (1 / 4) * np.exp(-C / 2)
+        # )
+
+        T = np.zeros((len(centers), len(centers)))
+
+        rows = rot_data['row_sigs']
+        cols = rot_data['col_sigs']
+
+        idx = col_inds
+        Sj = cols
+
+        tf_centers = L @ centers[idx][:, :, np.newaxis]
+        tf_centers = tf_centers[:, :, inds]
+
+        tf_sigs = L @ (Sj @ np.transpose(L, (0, 2, 1)))
+        tf_sigs = tf[:, inds, :][:, :, inds]
+
+        exp_polys = [
+            DensePolynomial.from_tensors([0, np.zeros(ndim), sig]).shift(c)
+            # , shift=-pt)
+            for sig, c in zip(tf_sigs, tf_centers)
+            # for pt, sig in zip(
+            #     centers,
+            #     sigs
+            # )
+        ]
+
+
+
+
+        raise Exception('need to apply indices before floop')
+
+        exp_d1 = [
+            d.der
+        ]
+
+        zetas = L @ (rot_data['centers'] - centers[idx])[:, :, np.newaxis]
+        zetas = zetas.reshape(rot_data['centers'].shape)
+        if inds is not None:
+            zetas = zetas[:, inds]
+
+        minv = np.diag(1 / masses)
+        Amat = L @ (Sj @ minv @ Sj) @ Lt
+        M = L @ np.broadcast_to(minv[np.newaxis], L.shape) @ Lt
+        # msj = rot_data['rotations']@(Sj@minv)@np.transpose(rot_data['rotations'], (0, 1, 2))
+        # raise Exception(
+        #     np.diagonal(msj, axis1=1, axis2=2),# / self.masses[np.newaxis],
+        #     - 1 / 2 * np.diagonal(Amat, axis1=1, axis2=2) / rot_data['alphas']
+        # )
+        submasses = np.diagonal(M, axis1=1, axis2=2)
+        sminv = np.diagonal(Amat, axis1=1, axis2=2)
+        if inds is not None:
+            submasses = submasses[:, inds]
+            sminv = sminv[:, inds]
+            Amat = Amat[:, inds, :][:, :, inds]
+        # raise Exception(
+        #     submasses,
+        #     sminv,
+        #     np.sum(
+        #         2 * alphas[col_inds] * submasses -
+        #         1 / 2 * sminv / rotas,
+        #         axis=1
+        #     )
+        # )
+        T[row_inds, col_inds] = 1 / 2 * (
+                np.sum(
+                    2 * alphas[idx] * submasses - 1 / 2 * sminv / rotas,
+                    axis=1
+                ) - 1 / 2 * sum(
+            # easier this way than the proper series summation...
+            Amat[..., k, kp] * (
+                4 * zetas[..., k] * zetas[..., kp]  # I discovered I was off by a factor of 4 in the 2D case...
+                if k != kp else
+                2 * zetas[..., k] ** 2
+            )
+            for k, kp in zip(*np.triu_indices(Amat.shape[-1]))
+        )  # could be a dot but this is fine
+        )
+        T[row_inds, col_inds] *= S[row_inds, col_inds]
+        T[col_inds, row_inds] = T[row_inds, col_inds]
+
+        return S, T
+
     def get_ST(self, centers=None, alphas=None, transformations=None):
         if centers is None:
             centers = self.centers
         if alphas is None:
             alphas = self.alphas
         if transformations is None:
             transformations = self.transformations
 
         masses = self.masses
         if self.mass_weighted:
             centers = centers * np.sqrt(masses)[np.newaxis]
             masses = np.ones(len(masses))
 
-        if transformations is None:
-            if self.inds is not None:
-                alphas = alphas[:, self.inds]
-                # masses = masses[:, self.inds]
+        if self._poly_coeffs is not None:
 
-            aouter = alphas[:, np.newaxis] * alphas[np.newaxis, :]
-            aplus = alphas[:, np.newaxis] + alphas[np.newaxis, :]
-            arat = aouter / aplus
+            rot_data = self.get_overlap_gaussians()
+            base_polys, ke_polys = self.get_kinetic_polynomials() # polys for each dimension + other stuff
 
-            disps = centers[:, np.newaxis, :] - centers[np.newaxis, :, :]
+            if not isinstance(rot_data, dict):
+                ov_centers, ov_alphas = rot_data
+                rot_data = None
+                row_inds, col_inds = np.triu_indices(len(self.centers))
+            else:
+                ov_centers = rot_data['centers']
+                ov_alphas = rot_data['alphas']
+                row_inds = rot_data['row_inds']
+                col_inds = rot_data['col_inds']
 
-            # A = outer_tet / np.sqrt(np.pi)
-            B = np.sqrt(aplus)
-            C = arat * np.power(disps, 2)
+            if rot_data is None:
+                S = self._unrot_base_S(centers, alphas, masses, self.inds)
+            else:
+                S = self._rot_base_S(rot_data, centers, alphas, self.inds)
 
-            # Base components
-            S_dim = (np.sqrt(2) * np.power(aouter, 1/4) / B) * np.exp(-C)
-            T_dim = arat * (1 - 2*C) / masses[np.newaxis, np.newaxis, :]
+            ndim = self.centers.shape[-1]
+            if rot_data is None and self.inds is not None:
+                ndim = len(self.inds)
 
-            # if self.inds is not None:
-            #     S_dim = S_dim[:, :, self.inds]
-            #     T_dim = T_dim[:, :, self.inds]
+            # raise Exception(S)
 
-            # Combine appropriately
-            S = np.prod(S_dim, axis=-1)
-            T = S * np.sum(T_dim, axis=-1)
-        else:
+            overlap_polys = [
+                base_polys[r] * base_polys[c]
+                for r, c in zip(row_inds, col_inds)
+            ]
+            overlap_polys = [
+                p.shift(c) if isinstance(p, DensePolynomial) else p
+                for p, c in zip(overlap_polys, ov_centers)
+            ]
+            # print(overlap_polys[0].coeffs)
 
-            T = np.zeros((len(self.centers), len(self.centers)))
-            S = np.eye(len(self.centers)) #np.full((len(self.centers), len(self.centers)), 1e10) #pick a crazy value to decouple bad inds
-            # row_inds, col_inds = np.triu_indices(len(self.alphas))
+            subtensors = [
+                p.clip(threshold=1e-8).coefficient_tensors
+                if isinstance(p, DensePolynomial) else None
+                for p in overlap_polys
+            ]
 
-            rot_data = self.get_overlap_gaussians()
-            row_inds = rot_data['row_inds']
-            col_inds = rot_data['col_inds']
+            # raise Exception(subtensors[0])
+            i = 1
+            # raise Exception([
+            #         tt[i]
+            #             if isinstance(tt, list) else
+            #         np.zeros((nd,)*i)
+            #             if i > 0 else
+            #         1
+            #         for tt in subtensors
+            #     ])
+            order = max(tuple(len(tt) for tt in subtensors if tt is not None) + (1,))
+            derivs = [
+                np.array([
+                    tt[i]
+                        if isinstance(tt, list) and i < len(tt) else
+                    np.zeros((ndim,)*i)
+                        if i > 0 else
+                    1
+                        if tt is None else
+                    tt
+                    for tt in subtensors
+                ])
+                for i in range(order)
+            ]
+            # raise Exception(derivs[2][0])
+            #
+            S_extra = self.tensor_expansion_integrate(
+                    len(self.centers),
+                    derivs,
+                    ov_centers,
+                    ov_alphas,
+                    inds=None if rot_data is None else self.inds,
+                    rot_data=rot_data,
+                    expansion_type='multicenter',
+                    logger=None,#self.logger
+                    reweight=False
+                )
 
-            alphas = self.alphas
-            # masses = self.masses
-            rotas = rot_data["alphas"]
-            if self.inds is not None:
-                alphas = alphas[:, self.inds]
-                rotas = rotas[:, self.inds]
+            S_base = S
+            S = S * S_extra
 
-            ndim = centers.shape[-1]
-            dets = np.prod(rotas, axis=-1)
-            rows = rot_data['row_sigs']
-            cols = rot_data['col_sigs']
-            # we prefactor out the 2**ndim
-            rdets = np.prod(alphas[row_inds], axis=-1)
-            cdets = np.prod(alphas[col_inds], axis=-1) # literally a product of passed in alphas
+            if self.transformations is None and self.inds is None:
+                T = np.zeros((len(self.centers), len(self.centers)))
+                idxs = range(ndim) if rot_data is not None else self.inds
+                for coord in idxs:
+
+                    kinetic_polys = [
+                        base_polys[r] * ke_polys[c][coord]
+                        for r, c in zip(row_inds, col_inds)
+                    ]
+                    kinetic_polys = [
+                        p.shift(c).clip(threshold=1e-4) if isinstance(p, DensePolynomial) else p
+                        for p, c in zip(kinetic_polys, ov_centers)
+                    ]
+                    subtensors = [
+                        p.coefficient_tensors if isinstance(p, DensePolynomial) else p
+                        for p in kinetic_polys
+                    ]
 
-            L = rot_data['inverse_rotations'] #
-            Lt = rot_data['rotations']
-            if self.inds is not None:
-                ndim = len(self.inds)
-                disps = L @ (centers[row_inds] - centers[col_inds])[:, :, np.newaxis]
-                disps = np.reshape(disps, disps.shape[:2])[:, self.inds]
-                si = L @ rot_data['sum_inverse'] @ Lt
-                si = si[:, self.inds, :][:, :, self.inds]
-                C = disps[:, np.newaxis, :] @ si @ disps[:, :, np.newaxis]
+                    print("?", coord, subtensors[2])
+
+                    order = max([
+                                    len(tt) for tt in subtensors
+                                    if tt is not None and not isinstance(tt, (int, float, np.integer, np.floating))
+                                ] + [0])
+                    derivs = [
+                        np.array([
+                            tt[i]
+                                if isinstance(tt, list) and i < len(tt) else
+                            np.zeros((ndim,) * i)
+                                if i > 0 else
+                            1
+                                if tt is None else
+                            tt
+                            for tt in subtensors
+                        ]
+                        )
+                        for i in range(order)
+                    ]
+                    if len(derivs) > 0:
+                        contrib = self.tensor_expansion_integrate(
+                            len(self.centers),
+                            derivs,
+                            ov_centers,
+                            ov_alphas,
+                            inds=None if rot_data is None else self.inds,
+                            rot_data=rot_data,
+                            expansion_type='multicenter',
+                            logger=None,#self.logger
+                            reweight=False
+                        ) / self.masses[coord]
+
+                        T = T + contrib
+
+                    # raise Exception(T*S_base)
+
+                T *= -1/2 * S_base
             else:
-                disps = centers[row_inds] - centers[col_inds]
-                C = disps[:, np.newaxis, :]@rot_data['sum_inverse']@disps[:, :, np.newaxis]
-            C = C.reshape(disps.shape[0])
+                T = self._rot_poly_ST(rot_data, base_polys, centers, alphas, masses, self.inds)
 
-            S[row_inds, col_inds] = 2**(ndim/2) * ((rdets*cdets)/(dets**2))**(1/4) * np.exp(-C/2)
 
-            zetas = L @ (rot_data['centers'] - centers[col_inds])[:, :, np.newaxis]
-            zetas = zetas.reshape(rot_data['centers'].shape)
-            if self.inds is not None:
-                zetas = zetas[:, self.inds]
+                raise Exception(...)
 
-            minv = np.diag(1/masses)
-            Sj = cols
-            Amat = L@(Sj@minv@Sj)@Lt
-            M = L@np.broadcast_to(minv[np.newaxis], L.shape)@Lt
-            # msj = rot_data['rotations']@(Sj@minv)@np.transpose(rot_data['rotations'], (0, 1, 2))
-            # raise Exception(
-            #     np.diagonal(msj, axis1=1, axis2=2),# / self.masses[np.newaxis],
-            #     - 1 / 2 * np.diagonal(Amat, axis1=1, axis2=2) / rot_data['alphas']
-            # )
-            submasses = np.diagonal(M, axis1=1, axis2=2)
-            sminv = np.diagonal(Amat, axis1=1, axis2=2)
-            if self.inds is not None:
-                submasses = submasses[:, self.inds]
-                sminv = sminv[:, self.inds]
-                Amat = Amat[:, self.inds, :][:, :, self.inds]
-            # raise Exception(
-            #     submasses,
-            #     sminv,
-            #     np.sum(
-            #         2 * alphas[col_inds] * submasses -
-            #         1 / 2 * sminv / rotas,
-            #         axis=1
-            #     )
-            # )
-            T[row_inds, col_inds] = 1 / 2 * (
-                    np.sum(
-                        2 * alphas[col_inds] * submasses  -
-                         1 / 2 * sminv / rotas,
-                        axis=1
-                    ) - 1/2 * sum(
-                        # easier this way than the proper series summation...
-                        Amat[..., k, kp] * (
-                            4 * zetas[..., k] * zetas[..., kp]  # I discovered I was off by a factor of 4 in the 2D case...
-                                if k != kp else
-                            2 * zetas[..., k] ** 2
-                        )
-                        for k, kp in zip(*np.triu_indices(Amat.shape[-1]))
-                    )  # could be a dot but this is fine
-            )
-            T[row_inds, col_inds] *= S[row_inds, col_inds]
+        else:
 
-            S[col_inds, row_inds] = S[row_inds, col_inds]
-            T[col_inds, row_inds] = T[row_inds, col_inds]
+            if transformations is None:
+                S, T = self._unrot_base_ST(centers, alphas, masses, self.inds)
+            else:
+                rot_data = self.get_overlap_gaussians()
+                S, T = self._rot_base_ST(rot_data, centers, alphas, masses, self.inds)
 
-        return S, T
+            S_base = S
+
+        return S_base, S, T
 
     def quad_integrate(self, function, degree=2):
         """
         Integrate potential over all pairs of Gaussians at once
 
         :param degree:
         :type degree:
@@ -926,15 +1400,15 @@
         term = sum(
             (cls.poch(n, l) * (1/2**(2*l-n) if 2*l > n else 2**(n-2*l)))*(c)**(n-2*l)
             for l in range(0, int(np.floor(n/2)) + 1)
         )
         return term
     @classmethod
     def simple_poly_int(cls, n):
-        return np.prod(np.arange(1, n, 2)) # double factorial/gamma/whatever
+        return np.prod(np.arange(1, n, 2)) / 2**(n/2) # double factorial/gamma/whatever
 
     @staticmethod
     def mass_weighted_eval(function, coords, masses, deriv_order=None, **opts):
             # expects just x and y coordinates for the atoms
             mass_vec = np.asanyarray(masses)
 
             coords = coords / np.sqrt(mass_vec[np.newaxis])
@@ -952,101 +1426,90 @@
                     #     print(weight[0])
                     new_d.append(do / weight)
                 else:
                     new_d.append(do)
             derivs = new_d
             return derivs
 
-    def expansion_integrate(self, function, deriv_order=2, expansion_type=None):
-        if expansion_type is None:
-            expansion_type = self.expansion_type
-
-        if self.transformations is None:
-            centers, alphas = self.get_overlap_gaussians()
-            rot_data = None
-        else:
-            rot_data = self.get_overlap_gaussians()
-            centers = rot_data['centers']
-            alphas = rot_data['alphas']
+    @classmethod
+    def tensor_expansion_integrate(cls,
+                                   npts, derivs, centers, alphas,
+                                   inds=None, rot_data=None, expansion_type='multicenter',
+                                   logger=None, reweight=True
+                                   ):
+        """
+        provides an integral from a polynomial expansion with derivs as an expansion in tensors
 
+        :param npts:
+        :param derivs:
+        :param centers:
+        :param alphas:
+        :param inds:
+        :param rot_data:
+        :param expansion_type:
+        :param logger:
+        :return:
+        """
+        """
+        [[-0.00000000e+00 -0.00000000e+00  2.43978381e+02 -1.34979790e-02]
+ [-0.00000000e+00 -0.00000000e+00  2.43978381e+02 -1.34979790e-02]
+ [ 2.43978381e+02  2.43978381e+02 -0.00000000e+00 -0.00000000e+00]
+ [-1.34979790e-02 -1.34979790e-02 -0.00000000e+00 -0.00000000e+00]]
+ """
         ndim = centers.shape[-1]
-        if expansion_type == 'taylor':
-            self.logger.log_print("expanding as a Taylor series about the minumum energy geometry...")
-            assert self.ref is None #TODO: centers need a displacement
-            zero = np.zeros((1, centers.shape[-1])) if self.ref is None else np.array([self.ref])
-            derivs = function(zero, deriv_order=deriv_order)
-            if isinstance(derivs, np.ndarray): # didn't get the full list so we do the less efficient route
-                derivs = (
-                        [function(zero)] +
-                        [function(zero, deriv_order=d) for d in range(1, deriv_order + 1)]
-                )
-            derivs = [
-                np.broadcast_to(
-                    d[np.newaxis],
-                    alphas.shape + d.squeeze().shape
-                )
-                for d in derivs
-            ]
-        else:
-            deriv_order = deriv_order - (deriv_order % 2) # odd orders don't contribute so why evaluate the derivatives...
-            self.logger.log_print("expanding about {N} points...", N=len(alphas))
-            if self.mass_weighted:
-                derivs = self.mass_weighted_eval(function, centers, self.masses, deriv_order=deriv_order)
-            else:
-                derivs = function(centers, deriv_order=deriv_order)
-                if isinstance(derivs, np.ndarray):  # didn't get the full list so we do the less efficient route'
-                    derivs = [function(centers)] + [
-                        function(centers, deriv_order=d) for d in range(1, deriv_order+1)
-                    ]
-
         if rot_data is not None:
-            rotations = rot_data['inverse_rotations']
+            rotations = rot_data['rotations']
             centers = np.reshape(rotations @ centers[:, :, np.newaxis], centers.shape)
 
-            if self.inds is not None:
-                ndim = len(self.inds)
-                rotations = rotations[:, self.inds, :]
-                alphas = alphas[..., self.inds]
-                centers = centers[..., self.inds]
+            if inds is not None:
+                ndim = len(inds)
+                rotations = rotations[:, :, inds]
+                alphas = alphas[..., inds]
+                centers = centers[..., inds]
 
             # if self.
             new_derivs = []
             # rotations = rotations[:, :, :, np.newaxis] # to test shapes
             for n,d in enumerate(derivs):
+                # print("???", d.shape)
                 for _ in range(n):
                     d = nput.vec_tensordot(
                         d, rotations,
-                        axes=[1, 2],
+                        axes=[1, 1],
                         shared=1
                     )
                 new_derivs.append(d)
             derivs = new_derivs
 
-        elif self.inds is not None:
-            ndim = len(self.inds)
-            alphas = alphas[..., self.inds]
-            centers = centers[..., self.inds]
+        elif inds is not None:
+            ndim = len(inds)
+            if alphas.shape[-1] > ndim:
+                alphas = alphas[..., inds]
+            if centers.shape[-1] > ndim:
+                centers = centers[..., inds]
 
             new_derivs = []
             for n, d in enumerate(derivs):
                 for k in range(n):
-                    d = np.take(d, self.inds, axis=k+1)
+                    d = np.take(d, inds, axis=k+1)
                 new_derivs.append(d)
             derivs = new_derivs
 
-        self.logger.log_print("adding up all derivative contributions...")
+        if logger is not None:
+            logger.log_print("adding up all derivative contributions...")
 
         if rot_data is None:
-            row_inds, col_inds = np.triu_indices(len(self.centers))
+            row_inds, col_inds = np.triu_indices(npts)
         else:
             row_inds = rot_data['row_inds']
             col_inds = rot_data['col_inds']
+
         fdim = derivs[0].ndim - 1
         fshape = derivs[0].shape[1:]
-        pot = np.zeros((len(self.centers), len(self.centers)) + fshape)
+        pot = np.zeros((npts, npts) + fshape)
         caches = [{} for _ in range(ndim)]
         for nd,d in enumerate(derivs): # add up all independent integral contribs...
             # iterate over upper triangle coordinates (we'll add bottom contrib by symmetry)
             inds = itertools.combinations_with_replacement(range(ndim), r=nd) if nd > 0 else [()]
             for idx in inds:
                 count_map = {k: v for k, v in zip(*np.unique(idx, return_counts=True))}
                 if expansion_type != 'taylor' and any(n%2 !=0 for n in count_map.values()):
@@ -1055,17 +1518,17 @@
                 contrib = 1
                 for k in range(ndim): # do each dimension of integral independently
                     n = count_map.get(k, 0)
                     if n not in caches[k]:
                         if expansion_type == 'taylor':
                             raise NotImplementedError("Taylor series in rotated basis not implemented yet")
                         caches[k][n] = (
-                           self.simple_poly_int(n)
+                           cls.simple_poly_int(n)
                              if expansion_type != 'taylor' else
-                           self.polyint_1D(centers[..., k], alphas[..., k], n)
+                           cls.polyint_1D(centers[..., k], alphas[..., k], n)
                         )
                     base_contrib = caches[k][n] / alphas[..., k]**(n/2)
                     for _ in range(fdim):
                         base_contrib = np.expand_dims(base_contrib, -1)
                     if isinstance(contrib, int) and fdim > 0:
                         base_contrib = np.broadcast_to(base_contrib,  alphas.shape[:-1] + fshape)
                     contrib *= base_contrib
@@ -1073,22 +1536,79 @@
                 dcont = d[(slice(None, None, None),) + idx] if len(idx) > 0 else d
                 facterms = np.unique([x for x in itertools.permutations(idx)], axis=0)
                 nfac = len(facterms) # this is like a binomial coeff or something but my sick brain won't work right now...
                 scaling = 2**(len(idx)/2) * np.prod([np.math.factorial(count_map.get(k, 0)) for k in range(ndim)])
                 for _ in range(fdim):
                     scaling = np.expand_dims(scaling, -1)
 
-                contrib *= nfac * dcont / scaling
+                if reweight:
+                    contrib *= nfac * dcont / scaling
+                else:
+                    contrib *= nfac * dcont
 
                 pot[row_inds, col_inds] += contrib
 
         pot[col_inds, row_inds] = pot[row_inds, col_inds]
 
         return pot
 
+    def expansion_integrate(self, function, deriv_order=2, expansion_type=None):
+        if expansion_type is None:
+            expansion_type = self.expansion_type
+
+        if self.transformations is None:
+            centers, alphas = self.get_overlap_gaussians()
+            rot_data = None
+        else:
+            rot_data = self.get_overlap_gaussians()
+            centers = rot_data['centers']
+            alphas = rot_data['alphas']
+
+        if expansion_type == 'taylor':
+            self.logger.log_print("expanding as a Taylor series about the minumum energy geometry...")
+            assert self.ref is None #TODO: centers need a displacement
+            zero = np.zeros((1, centers.shape[-1])) if self.ref is None else np.array([self.ref])
+            derivs = function(zero, deriv_order=deriv_order)
+            if isinstance(derivs, np.ndarray): # didn't get the full list so we do the less efficient route
+                derivs = (
+                        [function(zero)] +
+                        [function(zero, deriv_order=d) for d in range(1, deriv_order + 1)]
+                )
+            derivs = [
+                np.broadcast_to(
+                    d[np.newaxis],
+                    alphas.shape + d.squeeze().shape
+                )
+                for d in derivs
+            ]
+        else:
+            deriv_order = deriv_order - (deriv_order % 2) # odd orders don't contribute so why evaluate the derivatives...
+            self.logger.log_print("expanding about {N} points...", N=len(alphas))
+            if self.mass_weighted:
+                derivs = self.mass_weighted_eval(function, centers, self.masses, deriv_order=deriv_order)
+            else:
+                derivs = function(centers, deriv_order=deriv_order)
+                if isinstance(derivs, np.ndarray):  # didn't get the full list so we do the less efficient route'
+                    derivs = [function(centers)] + [
+                        function(centers, deriv_order=d) for d in range(1, deriv_order+1)
+                    ]
+
+        pot = self.tensor_expansion_integrate(
+            len(self.centers),
+            derivs,
+            centers,
+            alphas,
+            inds=self.inds,
+            rot_data=rot_data,
+            expansion_type=expansion_type,
+            logger=self.logger
+        )
+
+        return pot
+
     def analytic_integrate(self):
         raise NotImplementedError("flooped up")
         centers = [np.array(np.meshgrid(x, x)).T for x in self.centers.T]
         alphas = np.array(np.meshgrid(self.alphas, self.alphas)).T
         # raise Exception(alphas.shape)
         return self.potential_function['analytic_integrals'](
             centers, # ...no
@@ -1136,15 +1656,17 @@
 
         pot_mat = self.evaluate_multiplicative_operator_base(
             function,
             handler=handler,
             expansion_degree=expansion_degree, expansion_type=expansion_type,
             quadrature_degree=quadrature_degree
         )
-        S = self.S
+        if self._scaling_S is None:
+            _ = self.S
+        S = self._scaling_S
         for _ in range(pot_mat.ndim - 2):
             S = np.expand_dims(S, -1)
         return S * pot_mat
 
     def get_V(self, potential_handler=None, expansion_degree=None, expansion_type=None, quadrature_degree=None):
         self.logger.log_print("calculating potential matrix")
         return self.evaluate_multiplicative_operator(
@@ -1198,15 +1720,15 @@
         qsort = np.concatenate([qsub, qrest])
         Qqinv = QL[:, qsort].T  # transforms back to the Q basis
 
         return Q, Qinv, (Qq, Qqinv)
 
     def diagonalize(self, print_debug_info=False, subspace_size=None, min_singular_value=None,
                     eps=5e-4,
-                    mode='stable',
+                    mode='classic',
                     nodeless_ground_state=True
                     ):
 
         if min_singular_value is None:
             min_singular_value = self.min_singular_value
         if min_singular_value is not None:
             self.logger.log_print("solving with min_singular_value={ms}", ms=min_singular_value)
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DGB/Wavefunctions.py` & `mccoygroup-psience-0.0.9/Psience/DGB/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/BaseDVR.py` & `mccoygroup-psience-0.0.9/Psience/DVR/BaseDVR.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,15 @@
         if isinstance(plot_units, str) and plot_units == 'wavenumbers':
             pot = pot * UnitsData.convert("Hartrees", "Wavenumbers")
 
         if zero_shift:
             pot = pot - np.min(pot)
 
         if energy_threshold:
+            pot = pot.copy()
             pot[pot > energy_threshold] = energy_threshold
 
         return plot_class(*mesh, pot.reshape(mesh[0].shape), figure=figure, **opts)
 
 class DVRException(Exception):
     """
     Base exception class for working with DVRs
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/ColbertMiller.py` & `mccoygroup-psience-0.0.9/Psience/DVR/ColbertMiller.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/DVR.py` & `mccoygroup-psience-0.0.9/Psience/DVR/DVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/DirectProduct.py` & `mccoygroup-psience-0.0.9/Psience/DVR/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/Extensions.py` & `mccoygroup-psience-0.0.9/Psience/DVR/Extensions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/FiniteBasisDVR.py` & `mccoygroup-psience-0.0.9/Psience/DVR/FiniteBasisDVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/Wavefunctions.py` & `mccoygroup-psience-0.0.9/Psience/DVR/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/DVR/__init__.py` & `mccoygroup-psience-0.0.9/Psience/DVR/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Data/KEData.py` & `mccoygroup-psience-0.0.9/Psience/Data/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Data/PsiDatasets/KEData.py` & `mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Data/Surfaces.py` & `mccoygroup-psience-0.0.9/Psience/Data/Surfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Data/__init__.py` & `mccoygroup-psience-0.0.9/Psience/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/CoordinateSystems.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/CoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/MolecularFunctionExpansion.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/MolecularFunctionExpansion.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/Molecule.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/Molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,14 +761,15 @@
                     good_coords = np.setdiff1d(np.arange(3 * len(self.masses)), embedding_coords)
                     coords = coords.reshape(coords.shape[:-2] + (3 * len(self.masses),))
                     coords = coords[..., good_coords]
             if deriv_order is None:
                 return func(coords).view(np.ndarray)
 
             terms = func(coords, deriv_order=deriv_order)
+            # raise Exception([t.shape for t in terms], coords.shape)
             if strip_embedding:
                 embedding_coords = self._get_embedding_coords()
                 if embedding_coords is not None:
                     good_coords = np.setdiff1d(np.arange(3 * len(self.masses)), embedding_coords)
 
                     const = terms[0]
                     terms = terms[1:]
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/MoleculeInterface.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/MoleculeInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/Properties.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/Transformations.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/Transformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Molecools/Vibrations.py` & `mccoygroup-psience-0.0.9/Psience/Molecools/Vibrations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Spectra/BaseSpectrum.py` & `mccoygroup-psience-0.0.9/Psience/Spectra/BaseSpectrum.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Analyzer.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Analyzer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Common.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Common.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Corrections.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Corrections.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/DegeneracySpecs.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/DegeneracySpecs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Hamiltonian.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         if mode_selection is not None:
             mode_selection = tuple(mode_selection)
         mode_n = modes.basis.matrix.shape[1] if mode_selection is None else len(mode_selection)
         self.mode_n = mode_n
         if n_quanta is None:
             # This is a basically a historical option. We keep it but there's really no reason.
             n_quanta = 15 # dunno yet how I want to handle this since it should really be defined by the order of state requested...
-        self.n_quanta = np.full((mode_n,), n_quanta) if isinstance(n_quanta, (int, np.int)) else tuple(n_quanta)
+        self.n_quanta = np.full((mode_n,), n_quanta) if isinstance(n_quanta, (int, np.integer)) else tuple(n_quanta)
         self.modes = modes
         self.mode_selection = mode_selection
 
         expansion_options['logger'] = self.logger
         expansion_options['checkpointer'] = self.results if self.results is not None else self.checkpointer
         expansion_options['parallelizer'] = self.parallelizer
         expansion_params = ParameterManager(expansion_options)
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Runner.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,16 +390,20 @@
         #         self.state_list,
         #         degeneracy_specs
         #     )
         # else:
         #     raise NotImplementedError("don't know what to do with degeneracy spec {}".format(degeneracy_specs))
 
     def filter_generator(self, target_property, order=2, initial_states=None, postfilters=None):
-        def filter(states):
-            return self.get_state_space_filter(states, initial_states=initial_states, target=target_property, order=order, postfilters=postfilters)
+        def filter(states, **opts):
+            return self.get_state_space_filter(states,
+                                               initial_states=initial_states, target=target_property,
+                                               order=order, postfilters=postfilters,
+                                               **opts
+                                               )
         return filter
     def get_filter(self, target_property, order=2, initial_states=None, postfilters=None):
         """
         Obtains a state space filter for the given target property
         using the states we want to get corrections for
 
         :param target_property:
@@ -412,15 +416,15 @@
         return self.get_state_space_filter(self.state_list,
                                            target=target_property,
                                            order=order,
                                            initial_states=initial_states,
                                            postfilters=postfilters
                                            )
     @classmethod
-    def get_state_space_filter(cls, states, initial_states=None, n_modes=None, order=2, target='wavefunctions', postfilters=None):
+    def get_state_space_filter(cls, states, initial_states=None, n_modes=None, order=2, target='wavefunctions', postfilters=None, **opts):
         """
         Gets `state_space_filters` for the input `states` targeting some property
 
         :param states: the input states
         :type states:
         :param n_modes:
         :type n_modes: int
@@ -447,15 +451,16 @@
                 [
                     HarmonicOscillatorProductBasis(n_modes).selection_rules(*["x"]*i) for i in range(3, order+3)
                 ],
                 [
                     HarmonicOscillatorProductBasis(n_modes).selection_rules(*["x"]*i) for i in range(1, order+2)
                 ],
                 order=order,
-                postfilters=postfilters
+                postfilters=postfilters,
+                **opts
             )
         elif target == 'frequencies':
             # return {
             #     (1, 1): ([],),
             #     (2, 0): (None, [[0]])
             # }
             return BasisStateSpaceFilter.from_property_rules(
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Solver.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,14 +427,24 @@
                             shape=(N, N)
                         )
                         end = time.time()
                         logger.log_print("took {t:.3f}s", t=end - start)
                         self.perts[0].clear_cache()
                         self._zo_engs = None
 
+                    # dm = np.abs(
+                    #     self.zero_order_energies[np.newaxis, :] - self.zero_order_energies[:, np.newaxis]
+                    # )
+                    # np.fill_diagonal(dm, 10)
+                    #
+                    # print(np.min(dm))
+                    #
+                    # self._get_Pi0([[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2]])
+                    # raise Exception(...)
+
                     for i, h in enumerate(self.perts[1:]):
                         if n_spaces > i + 1:
                             cs = new_states[i]
                             with logger.block(tag="building {}".format(h)):
                                 start = time.time()
                                 if len(cs) > 0:
                                     #TODO: add a way to avoid calculating terms
@@ -602,16 +612,16 @@
                 raise ValueError("coupled states must be specified for all perturbations (got {}, expected {})".format(
                     len(self._coupled_states),
                     len(self.perts) - 1
                 ))
             elif any(not isinstance(cs, (BasisStateSpace, SelectionRuleStateSpace)) for cs in self._coupled_states):
                 self._coupled_states = [
                     BasisStateSpace(self.states.basis, cs, full_basis=self.full_basis)
-                    if not isinstance(cs, (BasisStateSpace, SelectionRuleStateSpace))
-                    else cs
+                        if not isinstance(cs, (BasisStateSpace, SelectionRuleStateSpace)) else
+                    cs
                     for cs in self._coupled_states
                 ]
 
             with logger.block(tag="precomputing coupled space indices"):
                 # otherwise they get calculated twice
                 start = time.time()
                 for s in self._coupled_states:
@@ -690,15 +700,17 @@
                                       )
             with parallelizer:  # we put an outermost block here to just make sure everything is clean
                 start = time.time()
                 existing_spaces = {self.perts[0]:None}
                 for p,cs in zip(self.perts[1:], self.coupled_states):
                     existing_spaces[p] = ({None:cs}, cs)
                 if self.state_space_filter_generator is not None:
-                    filters = BasisStateSpaceFilter.from_data(new_targets, self.state_space_filter_generator(new_targets))
+                    filters = BasisStateSpaceFilter.from_data(new_targets,
+                                                              self.state_space_filter_generator(new_targets, check_subspaces=False)
+                                                              )
                 else:
                     filters = None
                 new_spaces = self.load_coupled_spaces([new_targets],
                                                       filter_spaces=filters
                                                       )#, spaces=existing_spaces)
                 self.states = self.states.union(new_targets)
 
@@ -1087,15 +1099,17 @@
                     diffs = b.difference(rep_space)
                     # if diffs.full_basis is None:
                     #     raise ValueError(diffs.full_basis, b.full_basis)
                     if len(diffs) > 0:
                         # raise Exception(projections, rep_space, diffs)
                         # we have an initial space we've already transformed, so we
                         # make sure not to recompute that
-                        b_sels = SelectionRuleStateSpace(b, [], ignore_shapes=True)  # just some type fuckery
+                        b_sels = SelectionRuleStateSpace(b, [], ignore_shapes=True, # just some type fuckery
+                                                         changes=[] if SelectionRuleStateSpace.track_change_positions else None
+                                                         )
                         existing = cur.intersection(b_sels, handle_subspaces=False)
                         # and now we do extra transformations where we need to
 
 
                         if len(diffs) > 0:
                             new_new = self._apply_transformation_with_filters(
                                 a, diffs, filter_space,
@@ -1119,15 +1133,17 @@
                         else:
                             new = b.to_single().take_unique()
 
                     else:
                         # means we already calculated everything
                         # so we don't need to worry about this
                         if cur is not None:
-                            b_sels = SelectionRuleStateSpace(b, [], ignore_shapes=True) # just some type fuckery
+                            b_sels = SelectionRuleStateSpace(b, [],
+                                                             changes=[] if SelectionRuleStateSpace.track_change_positions else None,
+                                                             ignore_shapes=True) # just some type fuckery
                             new = cur.intersection(b_sels, handle_subspaces=False)
                             new = new.to_single().take_unique()
                         else:
                             new = None
 
         else:
             raise TypeError("don't know what to do with {} and {}".format(a, b))
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Terms.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Terms.py`

 * *Files 0% similar despite different names*

```diff
@@ -2205,15 +2205,15 @@
             for i,w in enumerate(wat_exprs):
                 try:
                     arr = w.array
                 except TensorDerivativeConverter.TensorExpansionError:
                     raise ValueError("failed to construct U({})".format(i))
                 else:
                     if arr.shape == ():
-                        arr = np.float(arr)
+                        arr = float(arr)
                     wat_terms.append(arr)
             # print(wat_terms)
 
         try:
             self.checkpointer['psuedopotential_terms'] = wat_terms
         except (OSError, KeyError):
             pass
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/Wavefunctions.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VPT2/__init__.py` & `mccoygroup-psience-0.0.9/Psience/VPT2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,8 +54,11 @@
 from .Solver import *; from .Solver import __all__ as exposed
 __all__ += exposed
 from .Corrections import *; from .Corrections import __all__ as exposed
 __all__ += exposed
 from .Wavefunctions import *; from .Wavefunctions import __all__ as exposed
 __all__ += exposed
 from .Terms import *; from .Terms import __all__ as exposed
+__all__ += exposed
+
+from .Analytic import *; from .Analytic import __all__ as exposed
 __all__ += exposed
```

### Comparing `mccoygroup-psience-0.0.8.2/Psience/VSCF/VSCF.py` & `mccoygroup-psience-0.0.9/Psience/VSCF/VSCF.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Wavefun/DirectProduct.py` & `mccoygroup-psience-0.0.9/Psience/Wavefun/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/Wavefun/Wavefunctions.py` & `mccoygroup-psience-0.0.9/Psience/Wavefun/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/Psience/__init__.py` & `mccoygroup-psience-0.0.9/Psience/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/README.md` & `mccoygroup-psience-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/PKG-INFO` & `mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.8.2
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.8.2/mccoygroup_psience.egg-info/SOURCES.txt` & `mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 Psience/Molecools/MoleculeInterface.py
 Psience/Molecools/Properties.py
 Psience/Molecools/Transformations.py
 Psience/Molecools/Vibrations.py
 Psience/Molecools/__init__.py
 Psience/Spectra/BaseSpectrum.py
 Psience/Spectra/__init__.py
+Psience/VPT2/Analytic.py
 Psience/VPT2/Analyzer.py
 Psience/VPT2/Common.py
 Psience/VPT2/Corrections.py
 Psience/VPT2/DegeneracySpecs.py
 Psience/VPT2/Hamiltonian.py
 Psience/VPT2/Runner.py
 Psience/VPT2/Solver.py
```

### Comparing `mccoygroup-psience-0.0.8.2/setup.py` & `mccoygroup-psience-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     packages=find_packages(),
 
     # Optional include package data to ship with your package
     # Customize MANIFEST.in if the general case does not suit your needs
     # Comment out this line to prevent the files from being packaged with your software
     # include_package_data=True
     install_requires=[
-        'mccoygroup-mcutils>=0.1.0.1'
+        'mccoygroup-mcutils>=0.1.1'
     ]
 )
```

