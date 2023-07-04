# Comparing `tmp/relative_dose_1d-0.1.3.tar.gz` & `tmp/relative_dose_1d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.1.3.tar", last modified: Tue May  9 23:47:06 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.4.tar", last modified: Tue Jul  4 23:44:27 2023, max compression
```

## Comparing `relative_dose_1d-0.1.3.tar` & `relative_dose_1d-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4105 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-09 23:44:23.000000 relative_dose_1d-0.1.3/README.md
--rw-rw-rw-   0        0        0     1414 2023-05-08 22:29:08.000000 relative_dose_1d-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.813105 relative_dose_1d-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.864545 relative_dose_1d-0.1.3/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     9352 2023-05-03 01:27:57.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0     9133 2023-05-08 22:22:38.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.904500 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     4105 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.349592 relative_dose_1d-0.1.4/
+-rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4190 2023-07-04 23:44:27.344602 relative_dose_1d-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3092 2023-07-04 23:43:45.000000 relative_dose_1d-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1414 2023-07-04 23:42:21.000000 relative_dose_1d-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:44:27.349592 relative_dose_1d-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.257785 relative_dose_1d-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.293686 relative_dose_1d-0.1.4/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     9352 2023-05-03 01:27:57.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/__init__.py
+-rw-rw-rw-   0        0        0    10542 2023-07-04 23:35:01.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.335081 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     4190 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.1.3/LICENSE` & `relative_dose_1d-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.3/PKG-INFO` & `relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative_dose_1d
-Version: 0.1.3
+Name: relative-dose-1d
+Version: 0.1.4
 Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -17,22 +17,22 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # relative_dose_1d
 
-Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Python package to read 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
 ## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
 
 ## Format specifications
-The data should be in M ​​rows by 2 columns, corresponding to positions and
+Data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
 * File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
@@ -88,7 +88,10 @@
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
+
+Jul-2023 Version 0.1.4
+  * A new function to create a an array with physical positions.
```

### Comparing `relative_dose_1d-0.1.3/README.md` & `relative_dose_1d-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # relative_dose_1d
 
-Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Python package to read 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
 ## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
 
 ## Format specifications
-The data should be in M ​​rows by 2 columns, corresponding to positions and
+Data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
 * File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
@@ -66,8 +66,11 @@
 May-2023 Version 0.1.0
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
-  * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
+  * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
+
+Jul-2023 Version 0.1.4
+  * A new function to create a an array with physical positions.
```

### Comparing `relative_dose_1d-0.1.3/pyproject.toml` & `relative_dose_1d-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `relative_dose_1d-0.1.3/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.4/src/relative_dose_1d/GUI.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.3/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.4/src/relative_dose_1d/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -189,14 +189,69 @@
     if delta != None:
         data_array[:,0] = data_array[:,0] + float(delta)
         
     
     return data_array
 
 
+def build_from_array_and_step(array, step):
+    """Create a new array with the same length but an additional axis. The first column represents the 
+    physical positions of the given values. The second column is a copy of the given array. 
+    The positions are builded with evenly step spacing starting from zero.
+
+    Parameters
+    ----------
+
+    array : ndarrya,
+        Numpy 1D array with the profile values
+
+    resolution : float,
+        The spacing between samples
+
+    Returns
+    -------
+
+    array, ndarray
+        A new array with shape (M,2), where M is the shape of array.
+
+    Examples
+    --------
+
+    >>> y = np.array([2,4,6,8,10])
+    >>> A = build_from_array_and_step(y, 0.5)
+    [ 
+    [0.0, 2] 
+    [0.5, 4]         
+    [1.0, 6]
+    [1.5, 8]
+    [2.0, 10]]
+
+    >>> y = np.arange(6)
+    >>> B = build_from_array_and_step(y, 3)
+    [
+    [0, 0]
+    [3, 1]
+    [6, 2]
+    [9, 3]
+    [12, 4]]
+
+    """
+
+    num = array.shape[0]
+    start = 0
+    stop = (num - 1) * step
+
+    positions = np.linspace(start, stop, num = num, endpoint = True)
+    profile = np.zeros((num, 2))
+    profile[:,0] = positions
+    profile[:,1] = array
+
+    return profile
+    
+
 def gamma_1D(ref, eval, dose_t = 3, dist_t = 2, dose_tresh = 0, interpol = 1):
     '''
     1-dimensional gamma index calculation.
     Dose profiles have to be normalized (0-100%).
 
     Parameters
     ----------
@@ -276,18 +331,26 @@
     gamma_percent = float(less_than_1)/total_points*100
 
     return gamma, gamma_percent
 
 
 if __name__ == '__main__':
 
+    y = np.array([2,4,6,8,10])
+    A = build_from_array_and_step(y, 0.5)
+    print(A)
+
+    y = np.arange(10)
+    B = build_from_array_and_step(y, 3)
+    print(B)
+
     """Test files"""
     #file_name = './test_data/test_ptw.mcc'
     #file_name = './test_data/test_varian.data'
-    file_name = './test_data/test_txt.txt'
+    #file_name = './test_data/test_txt.txt'
 
-    file_name_eval = "./test_data/X06 OPEN 10X10 PDD WAT 221214 13'13'42.mcc"
+    #file_name_eval = "./test_data/X06 OPEN 10X10 PDD WAT 221214 13'13'42.mcc"
     
-    data_ref = get_data(file_name, start_word =  'Field 1')
-    data_eval = get_data(file_name_eval)
-    g, gp = gamma_1D(data_ref, data_eval)
-    print(gp)
+    #data_ref = get_data(file_name, start_word =  'Field 1')
+    #data_eval = get_data(file_name_eval)
+    #g, gp = gamma_1D(data_ref, data_eval)
+    #print(gp)
```

### Comparing `relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative-dose-1d
-Version: 0.1.3
+Name: relative_dose_1d
+Version: 0.1.4
 Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -17,22 +17,22 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # relative_dose_1d
 
-Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Python package to read 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
 ## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
 
 ## Format specifications
-The data should be in M ​​rows by 2 columns, corresponding to positions and
+Data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
 * File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
@@ -88,7 +88,10 @@
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
+
+Jul-2023 Version 0.1.4
+  * A new function to create a an array with physical positions.
```

