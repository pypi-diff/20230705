# Comparing `tmp/sphractal-0.7.0.tar.gz` & `tmp/sphractal-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.7.0.tar", max compression
+gzip compressed data, was "sphractal-0.7.1.tar", max compression
```

## Comparing `sphractal-0.7.0.tar` & `sphractal-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-04 16:13:08.575564 sphractal-0.7.0/LICENSE
--rw-r--r--   0        0        0     4015 2023-07-04 16:13:08.575564 sphractal-0.7.0/README.md
--rw-r--r--   0        0        0     2056 2023-07-04 16:13:49.076139 sphractal-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-04 16:13:49.076139 sphractal-0.7.0/setup.py
--rw-r--r--   0        0        0     1406 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/__init__.py
--rw-r--r--   0        0        0    22696 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4302 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8953 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-07-04 16:13:08.635565 sphractal-0.7.0/tests/fixtures.py
--rw-r--r--   0        0        0    17688 2023-07-04 16:13:08.635565 sphractal-0.7.0/tests/test_sphractal.py
--rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sphractal-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-05 01:38:59.307865 sphractal-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4015 2023-07-05 01:38:59.307865 sphractal-0.7.1/README.md
+-rw-r--r--   0        0        0     2056 2023-07-05 01:39:39.072186 sphractal-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-05 01:39:39.072186 sphractal-0.7.1/setup.py
+-rw-r--r--   0        0        0     1429 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    23019 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4384 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      278 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8749 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11513 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94032 2023-07-05 01:38:59.363866 sphractal-0.7.1/tests/fixtures.py
+-rw-r--r--   0        0        0    17618 2023-07-05 01:38:59.363866 sphractal-0.7.1/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sphractal-0.7.1/PKG-INFO
```

### Comparing `sphractal-0.7.0/LICENSE` & `sphractal-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.0/README.md` & `sphractal-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.0/pyproject.toml` & `sphractal-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.7.0"
+version = "0.7.1"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.7.0/setup.py` & `sphractal-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.7.0/src/sphractal/__init__.py` & `sphractal-0.7.1/src/sphractal/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Code snippets in docstrings are indicated by three greater-than signs::
 
   >>> x = 42
   >>> x = x + 1
 
 Use the built-in ``help`` function to view a function's docstring::
 
+  >>> import sphractal
   >>> help(sphractal.runBoxCnt)
   ... # docstring: +SKIP
 
 Utilities
 ---------
 test (To be implemented)
     Run Sphractal tests.
```

### Comparing `sphractal-0.7.0/src/sphractal/boxCnt.py` & `sphractal-0.7.1/src/sphractal/boxCnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,27 +70,27 @@
         Number of boxes that cover the surface of interest, as represented by the voxels in the 3D binary image.
 
     Examples
     --------
     >>> eles, rads, xyzs, _, minxyz, maxxyz = readXYZ('example.xyz')
     >>> neighs, _ = findNN(rads, xyzs, minxyz, maxxyz, 2.5)
     >>> surfs = findSurf(xyzs, neighs, 'alphaShape', 5.0)
-    >>> scales, counts = genSurfPoints(eles, rads, surfs, xyzs, neighs, 'example')
+    >>> scalesPC, countsPC = genSurfPoints(eles, rads, surfs, xyzs, neighs, 'example')
 
     Notes
     -----
     The 3D binary image resolution (gridNum) is restricted by RAM size available, the relationship is illustrated below:
     -  1024 ->    2 GB (laptops -> typically 8 GB)
     -  2048 ->   16 GB (HPC nodes with GPUs like NCI Gadi gpuvolta queue -> max 32 GB/node)
     -  4096 ->  128 GB
     -  8192 -> 1024 GB (HPC node with huge memories like NCI Gadi megamem queue -> max 2990 GB/node)
     - 16384 -> 8192 GB
     Further details about maximum grid size and memory estimation could be found in 'test.cpp' documented by the authors 
-    (https://www.ugr.es/~demiras/fbc/). As a reference, when 8192 grids are used, allocation of memory took 25 min; while 
-    the CPU algorithm runs for 18 min.
+    (https://www.ugr.es/~demiras/fbc/). As a reference, when 8192 grids are used, allocation of memory took 25 min;
+    while the CPU algorithm runs for 18 min.
     """
     if verbose:
         print(f"  Approximating the surface with {numPoint} point clouds for each atom...")
     if not isdir(writeFileDir):
         mkdir(writeFileDir)
 
     genSurfPoints(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
@@ -153,25 +153,26 @@
         Number of boxes that cover the exact spherical surface of interest.
     
     Examples
     --------
     >>> eles, rads, xyzs, _, minxyz, maxxyz = readXYZ('example.xyz')
     >>> neighs, _ = findNN(rads, xyzs, minxyz, maxxyz, 1.2)
     >>> surfs = findSurf(xyzs, neighs, 'alphaShape', 2.0)
-    >>> scales, counts = getSphereBoxCnts(eles, rads, surfs, xyzs, neighs, 100, (0.2, 1), minxyz, 'example')
+    >>> scalesES, countsES = getSphereBoxCnts(eles, rads, surfs, xyzs, neighs, 100, (0.2, 1), minxyz, 'example')
     """
     atomsIdxs = atomsSurfIdxs if rmInSurf else findTargetAtoms(atomsNeighIdxs)
     numCPUs = cpu_count()
     boxLenScanMaxWorkers = ceil(numCPUs * numBoxLenSample / len(atomsIdxs))
     boxLenConc = False if boxLenScanMaxWorkers < 2 else True
     atomScanMaxWorkers = numCPUs - boxLenScanMaxWorkers if boxLenConc else numCPUs
 
     if verbose:
         print(f"  Representing the surface by treating each atom as exact spheres...")
-        print(f"  Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over atoms, the rest over box lengths...")
+        print(f"  Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over atoms, "
+              f"the rest over box lengths...")
         print(f"    (1/eps)    (# bulk)    (# surf)")
     if writeBox:
         if not isdir(writeFileDir):
             mkdir(writeFileDir)
 
     overallBoxLen = maxRange + MIN_VAL_FROM_BOUND * 2
     allLensSurfBoxs, allLensBulkBoxs, allLensSurfCnts, allLensBulkCnts = [], [], [], []
@@ -193,15 +194,16 @@
             allLensSurfCnts.append(len(allAtomsSurfBoxs))
 
         scales.append(log10(magnFac / overallBoxLen))
         scanBoxLens.append(scanBoxLen)
 
     if boxLenConc:
         with Pool(max_workers=boxLenScanMaxWorkers) as pool:
-            for scanAllAtomsResult in pool.map(scanAllAtoms, scanAllAtomsInps, chunksize=ceil(numBoxLenSample / boxLenScanMaxWorkers)):
+            for scanAllAtomsResult in pool.map(scanAllAtoms, scanAllAtomsInps,
+                                               chunksize=ceil(numBoxLenSample / boxLenScanMaxWorkers)):
                 allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
                 allLensSurfBoxs.append(allAtomsSurfBoxs)
                 allLensBulkBoxs.append(allAtomsBulkBoxs)
                 allLensSurfCnts.append(len(allAtomsSurfBoxs))
     counts = [log10(sCnt) if sCnt != 0 else np.nan for sCnt in allLensSurfCnts]
 
     if writeBox:
@@ -252,58 +254,67 @@
         Confidence interval of the box-counting dimension of the point clouds surface.
     """
     if visReg:
         plt.rc('font', family='sans-serif')
         plt.rc('xtick', labelsize='x-small')
         plt.rc('ytick', labelsize='x-small')
         params = PLT_PARAMS[figType]
-        figsize, dpi, fontsize, labelsize, legendsize, linewidth, markersize = params['figsize'], params['dpi'], params['fontsize'], params['labelsize'], params['legendsize'], params['linewidth'], params['markersize']
+        figSize, dpi, fontSize, labelSize = params['figSize'], params['dpi'], params['fontSize'], params['labelSize']
+        legendSize, lineWidth, markerSize = params['legendSize'], params['lineWidth'], params['markerSize']
+    else:
+        figSize = dpi = fontSize = labelSize = legendSize = lineWidth = markerSize = None
 
     # Remove invalid entries in the box counts data collected
     while np.nan in counts:
         nanIdx = counts.index(np.nan)
         del counts[nanIdx]
         del scales[nanIdx]
 
     if abs(confLvl) > 100:
-        warn(f"Confidence level out of range, confidence intervals are unreliable! 'confLvl' should be within [0, 100) instead of {confLvl}")
+        warn(f"Confidence level out of range, confidence intervals are unreliable! 'confLvl' should be within [0, 100) "
+             f"instead of {confLvl}")
     alphaCI = 1 - confLvl/100
 
     firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scales), True
-    r2score, boxCntDim, slopeCI, r2scorePrev, boxCntDimPrev, slopeCIPrev = 0.0, 0.0, np.array((np.inf, np.inf)), 0.0, 0.0, np.array((np.inf, np.inf))
+    r2score, boxCntDim, slopeCI = 0.0, 0.0, np.array((np.inf, np.inf))
+    r2scorePrev, boxCntDimPrev, slopeCIPrev = 0.0, 0.0, np.array((np.inf, np.inf))
     while len(scales[firstPointIdx:lastPointIdx]) > minSampleNum:
 
         x, y = scales[firstPointIdx:lastPointIdx], counts[firstPointIdx:lastPointIdx]
         regModel = OLS(endog=y, exog=add_constant(x)).fit()
         r2score, boxCntDim, slopeCI = regModel.rsquared, regModel.params[1], regModel.conf_int(alpha=alphaCI)[1]
         yPred = regModel.predict()  # Returns ndarray, allowing subtraction later
 
         if visReg:
             plt.close()
-            fig = plt.figure(figsize=figsize, dpi=dpi)
+            fig = plt.figure(figsize=figSize, dpi=dpi)
             ax = fig.add_subplot(1, 1, 1)
-            handleScatter = ax.scatter(x, y, marker='o', s=markersize, c='r', alpha=1, edgecolors='k', linewidths=1.2, zorder=3)
+            handleScatter = ax.scatter(x, y, marker='o', s=markerSize, c='r', alpha=1, edgecolors='k', linewidths=1.2,
+                                       zorder=3)
             handleBestFit = ax.plot(x, yPred, linestyle='-', linewidth=1., color='k', label='OLS')
             ax.grid(linestyle='dotted')
 
             # Compute confidence bands
             predOLS = regModel.get_prediction()
-            lowCIvals, upCIvals = predOLS.summary_frame()['mean_ci_lower'], predOLS.summary_frame()['mean_ci_upper']
-            handleConfBand = ax.plot(x, upCIvals, linestyle='--', linewidth=linewidth, color='b')
-            ax.plot(x, lowCIvals, linestyle='--', linewidth=linewidth, color='b')
-            ax.fill_between(x, upCIvals, lowCIvals, alpha=0.2)
+            lowCIs, upCIs = predOLS.summary_frame()['mean_ci_lower'], predOLS.summary_frame()['mean_ci_upper']
+            handleConfBand = ax.plot(x, upCIs, linestyle='--', linewidth=lineWidth, color='b')
+            ax.plot(x, lowCIs, linestyle='--', linewidth=lineWidth, color='b')
+            ax.fill_between(x, upCIs, lowCIs, alpha=0.2)
 
-            ax.set_xlabel(r'log$(1/\epsilon)$', fontsize=labelsize)
-            ax.set_ylabel(r'log$(N)$', fontsize=labelsize)
+            ax.set_xlabel(r'log$(1/\epsilon)$', fontsize=labelSize)
+            ax.set_ylabel(r'log$(N)$', fontsize=labelSize)
             ax.yaxis.set_major_formatter(FormatStrFormatter('% 1.1f'))
+            # ax.set_title('', fontsize=fontSize)
             ax.legend(handles=(handleScatter, handleBestFit[0], handleConfBand[0]), 
-                      labels=('Actual box counts', fr"Best fit line ($R^2$: {r2score:.3f})", f"{confLvl}% confidence bands"), 
-                      title=fr"$D_{{box}}$: {boxCntDim:.3f} [{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]", title_fontsize=legendsize, 
-                      fontsize=legendsize)
-            #plt.tight_layout()
+                      labels=('Actual box counts', fr"Best fit line ($R^2$: {r2score:.3f})",
+                              f"{confLvl}% confidence bands"),
+                      title=fr"$D_{{box}}$: {boxCntDim:.3f} [{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]",
+                      title_fontsize=legendSize,
+                      fontsize=legendSize)
+            # plt.tight_layout()
 
         # Removal of next point (beware of weird behaviour in middle range)
         # lstSqErrs = np.subtract(y, yPred) ** 2
         # if len(y) % 2 == 0:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2:].sum()
         # else:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2 + 1:].sum()
```

### Comparing `sphractal-0.7.0/src/sphractal/constants.py` & `sphractal-0.7.1/src/sphractal/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,11 +35,13 @@
     'Hf': 1.59, 'Ta': 1.46, 'W': 1.39, 'Re': 1.37, 'Os': 1.35, 'Ir': 1.355, 'Pt': 1.385, 'Au': 1.44, 'Hg': 1.51,
     'Tl': 1.70, 'Pb': defRad, 'Bi': defRad, 'Po': defRad, 'At': defRad, 'Rn': defRad, 'Fr': defRad, 'Ra': defRad,
     'Ac': defRad, 'Th': 1.79, 'Pa': 1.63, 'U': 1.56, 'Np': 1.55, 'Pu': 1.59, 'Am': 1.73, 'Cm': 1.74, 'Bk': 1.70,
     'Cf': 1.86, 'Es': 1.86, 'Fm': defRad, 'Md': defRad, 'No': defRad, 'Lr': defRad, 'Rf': defRad, 'Db': defRad,
     'Sg': defRad, 'Bh': defRad, 'Hs': defRad, 'Mt': defRad, 'Ds': defRad, 'Rg': defRad, 'Cn': defRad, 'Nh': defRad,
     'Fl': defRad, 'Mc': defRad, 'Lv': defRad, 'Ts': defRad, 'Og': defRad
 }
-PLT_PARAMS = {'article': {'figsize': (3.5, 2.5), 'dpi': 300, 'fontsize': 'medium', 'labelsize': 'small', 'legendsize': 'x-small', 'linewidth': 0.5, 'markersize': 24}, 
-        'poster': {'figsize': (4.5, 3.5), 'dpi': 600, 'fontsize': 'x-large', 'labelsize': 'large', 'legendsize': 'medium', 'linewidth': 1.0, 'markersize': 48}, 
-        'ppt': {'figsize': (4, 3), 'dpi': 144, 'fontsize': 'large', 'labelsize': 'medium', 'legendsize': 'small', 'linewidth': 1.0, 'markersize': 36}}
-
+PLT_PARAMS = {'article': {'figSize': (3.5, 2.5), 'dpi': 300, 'fontSize': 'medium', 'labelSize': 'small',
+                          'legendSize': 'x-small', 'lineWidth': 0.5, 'markerSize': 24},
+              'poster': {'figSize': (4.5, 3.5), 'dpi': 600, 'fontSize': 'x-large', 'labelSize': 'large',
+                         'legendSize': 'medium', 'lineWidth': 1.0, 'markerSize': 48},
+              'ppt': {'figSize': (4, 3), 'dpi': 144, 'fontSize': 'large', 'labelSize': 'medium', 'legendSize': 'small',
+                      'lineWidth': 1.0, 'markerSize': 36}}
```

### Comparing `sphractal-0.7.0/src/sphractal/data/example.xyz` & `sphractal-0.7.1/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.0/src/sphractal/surfPointClouds.py` & `sphractal-0.7.1/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.0/src/sphractal/utils.py` & `sphractal-0.7.1/src/sphractal/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             val = atomsXYZ[row, col]
             minVal, maxVal = min(minVal, val), max(maxVal, val)
         minXYZ[col], maxXYZ[col] = minVal, maxVal
     return max(maxXYZ - minXYZ), minXYZ, maxXYZ
 
 
 # @annotate('readXYZ', color='cyan')
+# noinspection GrazieInspection
 def readXYZ(filePath, radType='atomic'):
     """Parse an xyz or a lmp file."""
     radDict = ATOMIC_RAD_DICT if radType == 'atomic' else METALLIC_RAD_DICT
     atomsEle, atomsRad, atomsXYZ = [], [], []
     numLinesSkip = 9 if '.lmp' in filePath else 2
     with open(filePath, 'r') as f:
         for (i, line) in enumerate(f):
```

### Comparing `sphractal-0.7.0/tests/fixtures.py` & `sphractal-0.7.1/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1348,20 +1348,20 @@
                      [659, 660, 664, 665, 666, 668, 669, -1, -1, -1, -1, -1],
                      [659, 635, 663, 664, 646, 666, 667, 649, 650, -1, -1, -1],
                      [660, 661, 664, 667, -1, -1, -1, -1, -1, -1, -1, -1]])
 
 
 @fixture
 def egAtomsSurfIdxs():
-    return np.array([  0,   1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  11,  12,
-                      16,  17,  19,  20,  21,  22,  23,  24,  26,  27,  28,  29,  30,
-                      31,  32,  33,  34,  35,  36,  37,  41,  42,  44,  45,  46,  47,
-                      48,  49,  61,  62,  64,  65,  66,  67,  68,  69,  76,  79,  80,
-                      81,  82,  83,  84,  85,  87,  88,  89,  90,  91,  92,  93,  94,
-                      95,  96,  97,  98, 102, 103, 105, 106, 107, 108, 109, 110, 122,
+    return np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12,
+                     16, 17, 19, 20, 21, 22, 23, 24, 26, 27, 28, 29, 30,
+                     31, 32, 33, 34, 35, 36, 37, 41, 42, 44, 45, 46, 47,
+                     48, 49, 61, 62, 64, 65, 66, 67, 68, 69, 76, 79, 80,
+                     81, 82, 83, 84, 85, 87, 88, 89, 90, 91, 92, 93, 94,
+                     95, 96, 97, 98, 102, 103, 105, 106, 107, 108, 109, 110, 122,
                      123, 125, 126, 127, 128, 129, 130, 150, 151, 153, 154, 155, 156,
                      157, 158, 173, 176, 177, 178, 179, 180, 181, 182, 189, 192, 193,
                      194, 195, 196, 197, 198, 200, 201, 202, 203, 204, 205, 206, 207,
                      208, 209, 210, 211, 215, 216, 218, 219, 220, 221, 222, 223, 235,
                      236, 238, 239, 240, 241, 242, 243, 263, 264, 266, 267, 268, 269,
                      270, 271, 299, 300, 302, 303, 304, 305, 306, 307, 330, 333, 334,
                      335, 336, 337, 338, 339, 354, 357, 358, 359, 360, 361, 362, 363,
@@ -1378,22 +1378,22 @@
                      638, 639, 640, 641, 642, 645, 648, 649, 650, 651, 652, 653, 654,
                      655, 656, 657, 658, 660, 661, 662, 663, 664, 665, 666, 667, 668,
                      669])
 
 
 @fixture
 def egTargetAtomIdxs():
-    return np.array([  0,   1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  11,  12,
-                      13,  14,  15,  16,  17,  18,  19,  20,  21,  22,  23,  24,  25,
-                      26,  27,  28,  29,  30,  31,  32,  33,  34,  35,  36,  37,  38,
-                      39,  40,  41,  42,  43,  44,  45,  46,  47,  48,  49,  50,  51,
-                      52,  53,  54,  55,  56,  57,  58,  59,  60,  61,  62,  63,  64,
-                      65,  66,  67,  68,  69,  70,  71,  72,  73,  74,  75,  76,  77,
-                      78,  79,  80,  81,  82,  83,  84,  85,  86,  87,  88,  89,  90,
-                      91,  92,  93,  94,  95,  96,  97,  98,  99, 100, 101, 102, 103,
+    return np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12,
+                     13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25,
+                     26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38,
+                     39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51,
+                     52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64,
+                     65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77,
+                     78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90,
+                     91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103,
                      104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116,
                      117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128, 129,
                      130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142,
                      143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155,
                      156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168,
                      169, 170, 171, 172, 173, 174, 175, 176, 177, 178, 179, 180, 181,
                      182, 183, 184, 185, 186, 187, 188, 189, 190, 191, 192, 193, 194,
@@ -1430,9 +1430,7 @@
                      585, 586, 587, 588, 589, 590, 591, 592, 593, 594, 595, 596, 597,
                      598, 599, 600, 601, 602, 603, 604, 605, 606, 607, 608, 609, 610,
                      611, 612, 613, 614, 615, 616, 617, 618, 619, 620, 621, 622, 623,
                      624, 625, 626, 627, 628, 629, 630, 631, 632, 633, 634, 635, 636,
                      637, 638, 639, 640, 641, 642, 643, 644, 645, 646, 647, 648, 649,
                      650, 651, 652, 653, 654, 655, 656, 657, 658, 659, 660, 661, 662,
                      663, 664, 665, 666, 667, 668, 669])
-
-
```

### Comparing `sphractal-0.7.0/tests/test_sphractal.py` & `sphractal-0.7.1/tests/test_sphractal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from math import dist
-from os import environ
+# from os import environ
 from os.path import exists, isdir, isfile
 from shutil import rmtree
 
 from pytest import approx, mark
 
 from fixtures import fixture, np, egAtomsXYZ, egAtomsNeighIdxs, egAtomsSurfIdxs, egTargetAtomIdxs
 from sphractal.datasets import getExampleDataPath
-from sphractal.utils import estDuration, getMinMaxXYZ, readXYZ, findNN, findSurf, calcDist, closestSurfAtoms, oppositeInnerAtoms
+from sphractal.utils import estDuration, getMinMaxXYZ, readXYZ, findNN, findSurf, calcDist, closestSurfAtoms, \
+    oppositeInnerAtoms
 from sphractal.surfPointClouds import fibonacciSphere, pointsOnAtom, pointsToVoxels
 from sphractal.surfExact import getNearFarCoord, scanBox, writeBoxCoords, findTargetAtoms
 from sphractal.boxCnt import getVoxelBoxCnts, getSphereBoxCnts, findSlope, runBoxCnt
 
 
 EG_XYZ_ATOM_NUM = 670
 ATOM_RAD = 1.69
 MAX_RANGE = 36.58499999999998
 
 
 @fixture
 def egMinMaxXYZ():
-    return np.array([404.065, 404.065, 404.065]), np.array([440.65, 440.65, 440.65]) 
+    return np.array([404.065, 404.065, 404.065]), np.array([440.65, 440.65, 440.65])
 
 
 @fixture
 def egAtomsEle():
     return np.array(['Pd']*EG_XYZ_ATOM_NUM, dtype='U2')
 
 
@@ -42,19 +43,14 @@
 @fixture
 def egSphereBoxCnts():
     return ([-0.23688234, -0.16309612, -0.10004438, -0.03477764,  0.03932408, 0.10260591,  0.17060299,  0.24023892,  0.30488175,  0.37314659],
             [3.20194306, 3.32139128, 3.5171959 , 3.68142216, 3.80522891, 3.9531796 , 4.09272064, 4.27207379, 4.38937875, 4.52953301])
 
 
 @fixture
-def egBoxCnts(egVoxelBoxCnts, egSphereBoxCnts):
-    return 
-
-
-@fixture
 def egVoxelBoxCntDims():
     return 0.99646974, 2.11889159, np.array((1.94381059, 2.29397261))
 
 
 @fixture
 def egSphereBoxCntDims():
     return 0.99660096, 2.24426950, np.array((2.11334077, 2.37519824))
@@ -159,17 +155,17 @@
 #def test_oppositeInnerAtoms(pointXYZ, atom1XYZ, atomNeighIdxs, isOppExp, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs):
 #    """Unit test of oppositeInnerAtoms(). (To be implemented)"""
 #    isOppAct = oppositeInnerAtoms(pointXYZ, atom1XYZ, atomNeighIdxs, 
 #                                  egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs)
 #    assert isOppAct == isOppExp, 'Incorrect results'
 
 
-@mark.parametrize('numPoint, sphereRad, xyzsExp', 
-    [(3, 1.0, np.array([[0., 1., 0.], [-0.73736888, 0., -0.67549029], [0., -1., 0.]])), 
-     (5, 1.5, np.array([[0., 1.5, 0.], [-0.95787027, 0.75, -0.87748763], [0.13113859, 0., 1.49425656], [0.79038527, -0.75, -1.03091762], [-0., -1.5, 0.]])), 
+@mark.parametrize('numPoint, sphereRad, xyzsExp',
+    [(3, 1.0, np.array([[0., 1., 0.], [-0.73736888, 0., -0.67549029], [0., -1., 0.]])),
+     (5, 1.5, np.array([[0., 1.5, 0.], [-0.95787027, 0.75, -0.87748763], [0.13113859, 0., 1.49425656], [0.79038527, -0.75, -1.03091762], [-0., -1.5, 0.]])),
      (2, 100, np.array([[0., 100., 0.], [-0., -100., -0.]]))])
 def test_fibonacciSphere(numPoint, sphereRad, xyzsExp):
     """Unit test of fibonacciSphere()."""
     xyzsAct = fibonacciSphere(numPoint, sphereRad)
     assert isinstance(xyzsAct, np.ndarray), 'Incorrect output data type'
     assert xyzsAct == approx(xyzsExp), 'Incorrect surface point coordinates'
 
@@ -280,15 +276,15 @@
     assert isfile('./tests/boxCntOutputs/boxCoords/example_boxCoords.xyz'), 'example_boxCoords.xyz is not a file'
     if isdir('./tests/boxCntOutputs'):
         rmtree('./tests/boxCntOutputs')
 
 
 #def test_runBoxCnt(egVoxelBoxCntDims, egSphereBoxCntDims):
 #    """Unit and regression test of runBoxCnt() (To be uncommented when compiled C++ code could be shipped together)."""
-#    assert isfile(os.environ['FASTBC_EXE']), 'Executable not found at FASTBC_EXE'
+#    assert isfile(environ['FASTBC_EXE']), 'Executable not found at FASTBC_EXE'
 #    boxCntDimsAct = runBoxCnt(getExampleDataPath(), writeFileDir='tests/boxCntOutputs')
 #    assert boxCntDimsAct[:2] == approx(egVoxelBoxCntDims[:2]), 'Incorrect R2 and D_Box for point clouds representation'
 #    assert boxCntDimsAct[2] == approx(egVoxelBoxCntDims[2]), 'Incorrect confidence interval for point clouds representation'
 #    assert boxCntDimsAct[-3:-1] == approx(egSphereBoxCntDims[:2]), 'Incorrect R2 and D_Box for exact surface representation'
 #    assert boxCntDimsAct[-1] == approx(egSphereBoxCntDims[2]), 'Incorrect confidence interval for exact surface representation'
 #    if isdir('./tests/boxCntOutputs'):
 #        rmtree('./tests/boxCntOutputs')
```

### Comparing `sphractal-0.7.0/PKG-INFO` & `sphractal-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

