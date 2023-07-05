# Comparing `tmp/PowDevLif-0.0.3.tar.gz` & `tmp/PowDevLif-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDevLif-0.0.3.tar", last modified: Fri Jun 23 11:03:48 2023, max compression
+gzip compressed data, was "PowDevLif-0.0.4.tar", last modified: Wed Jul  5 08:00:34 2023, max compression
```

## Comparing `PowDevLif-0.0.3.tar` & `PowDevLif-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.3/README.md
--rw-------   0 runner    (1000) runner    (1000)      451 2023-06-23 11:03:40.000000 PowDevLif-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1072 2023-06-23 11:03:35.000000 PowDevLif-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.494956 PowDevLif-0.0.3/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.498957 PowDevLif-0.0.3/src/PowDevLif.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.498957 PowDevLif-0.0.3/src/powdevlif/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/src/powdevlif/function/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/counters.py
--rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/cumul_endommagement.py
--rw-------   0 runner    (1000) runner    (1000)     3275 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/graphs.py
--rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/losses.py
--rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/materials.py
--rw-------   0 runner    (1000) runner    (1000)     2788 2023-06-23 11:03:20.000000 PowDevLif-0.0.3/src/powdevlif/function/matrix.py
--rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/path_reader.py
--rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/poly_somme.py
--rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/temperature.py
--rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/zth_materials.py
--rw-------   0 runner    (1000) runner    (1000)     3221 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/lifetime.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:00:34.784014 PowDevLif-0.0.4/
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-05 08:00:34.784014 PowDevLif-0.0.4/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.4/README.md
+-rw-------   0 runner    (1000) runner    (1000)      451 2023-07-03 15:13:27.000000 PowDevLif-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-05 08:00:34.784014 PowDevLif-0.0.4/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1072 2023-07-03 15:13:22.000000 PowDevLif-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:00:34.776014 PowDevLif-0.0.4/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:00:34.776014 PowDevLif-0.0.4/src/PowDevLif.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-05 08:00:34.000000 PowDevLif-0.0.4/src/PowDevLif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-07-05 08:00:34.000000 PowDevLif-0.0.4/src/PowDevLif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-05 08:00:34.000000 PowDevLif-0.0.4/src/PowDevLif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-05 08:00:34.000000 PowDevLif-0.0.4/src/PowDevLif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-07-05 08:00:34.000000 PowDevLif-0.0.4/src/PowDevLif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:00:34.776014 PowDevLif-0.0.4/src/powdevlif/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:00:34.784014 PowDevLif-0.0.4/src/powdevlif/function/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/counters.py
+-rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/cumul_endommagement.py
+-rw-------   0 runner    (1000) runner    (1000)     3275 2023-06-23 10:54:01.000000 PowDevLif-0.0.4/src/powdevlif/function/graphs.py
+-rw-------   0 runner    (1000) runner    (1000)     3175 2023-07-03 13:39:32.000000 PowDevLif-0.0.4/src/powdevlif/function/losses.py
+-rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/materials.py
+-rw-------   0 runner    (1000) runner    (1000)     2784 2023-07-03 13:54:31.000000 PowDevLif-0.0.4/src/powdevlif/function/matrix.py
+-rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/path_reader.py
+-rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.4/src/powdevlif/function/poly_somme.py
+-rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.4/src/powdevlif/function/temperature.py
+-rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.4/src/powdevlif/function/zth_materials.py
+-rw-------   0 runner    (1000) runner    (1000)     3216 2023-07-03 13:46:39.000000 PowDevLif-0.0.4/src/powdevlif/lifetime.py
```

### Comparing `PowDevLif-0.0.3/LICENSE` & `PowDevLif-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/PKG-INFO` & `PowDevLif-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.3
+Version: 0.0.4
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.3/README.md` & `PowDevLif-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/setup.py` & `PowDevLif-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='PowDevLif',
-    version='0.0.3',
+    version='0.0.4',
     description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)',
     readme='README.md',
     license='MIT',
     author='Garnier Paul, Baudais Briac',
     author_email='paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages('src'),
```

### Comparing `PowDevLif-0.0.3/src/PowDevLif.egg-info/PKG-INFO` & `PowDevLif-0.0.4/src/PowDevLif.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.3
+Version: 0.0.4
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.3/src/PowDevLif.egg-info/SOURCES.txt` & `PowDevLif-0.0.4/src/PowDevLif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/counters.py` & `PowDevLif-0.0.4/src/powdevlif/function/counters.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/cumul_endommagement.py` & `PowDevLif-0.0.4/src/powdevlif/function/cumul_endommagement.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/graphs.py` & `PowDevLif-0.0.4/src/powdevlif/function/graphs.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/losses.py` & `PowDevLif-0.0.4/src/powdevlif/function/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,14 @@
 
         # Calculate IGBT losses
         self.P_T_cond = (1/(2*np.pi) + self.m*self.cosphi/8) * self.Vce0 * np.sqrt(2) * self.i_ref + (1/8 + self.m*self.cosphi/(3*np.pi)) * self.Rce * 2 * self.i_ref**2
         self.P_T_sw = self.f_sw * self.E_sw * np.sqrt(2) / np.pi * self.i_ref / self.Iref_sw * (self.Vdc / self.Vref_sw)**self.kv_igbt
         self.pertes_igbt = self.P_T_cond + self.P_T_sw
 
         # Calculate Diode losses
-        self.P_D_cond = (1/(2*np.pi) + self.m*self.cosphi/8) * self.Vd * np.sqrt(2) * self.i_ref + (1/8 + self.m*self.cosphi/(3*np.pi)) * self.Rd * 2 * self.i_ref**2
+        self.P_D_cond = (1/(2*np.pi) - self.m*self.cosphi/8) * self.Vd * np.sqrt(2) * self.i_ref + (1/8 - self.m*self.cosphi/(3*np.pi)) * self.Rd * 2 * self.i_ref**2
         self.P_D_sw = self.f_sw * self.E_d * np.sqrt(2) / np.pi * (self.i_ref / self.Iref_d)**self.ki_diode * (self.Vdc / self.Vref_d)**self.kv_diode
         self.pertes_diode = self.P_D_cond + self.P_D_sw
 
         # Calculate total losses and their cumulative sum
         self.total_losses = np.asarray((self.pertes_igbt + self.pertes_diode) * self.number_IGBT, dtype=float)
         self.total_losses_cum = np.cumsum(self.total_losses)
```

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/matrix.py` & `PowDevLif-0.0.4/src/powdevlif/function/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 
     matrix_1, mean_bins_1, range_bins_1 = create_quantized_rainflow_matrix(counter_IGBT)
     matrix_2, mean_bins_2, range_bins_2 = create_quantized_rainflow_matrix(counter_diode)
 
     # Create a new figure with two subplots
     fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(12, 6))
     ax = axes[0]
-    im = ax.imshow(matrix_1, cmap='plasma', interpolation='nearest')
+    im = ax.imshow(matrix_1, cmap='gray', interpolation='nearest')
     ax.set_title('IGBT')
     ax.set_xlabel('Delta T')
     ax.set_ylabel('Mean Tj')
     fig.colorbar(im, ax=ax, label='Count')
     ax.set_xticks(np.arange(len(range_bins_1)))
     ax.set_yticks(np.arange(len(mean_bins_1)))
     ax.set_xticklabels([str(int(val)) for val in range_bins_1])
     ax.set_yticklabels([str(int(val)) for val in mean_bins_1])
 
     # Plot the second matrix
     ax = axes[1]
-    im = ax.imshow(matrix_2, cmap='plasma', interpolation='nearest')
+    im = ax.imshow(matrix_2, cmap='gray', interpolation='nearest')
     ax.set_title('Diode')
     ax.set_xlabel('Delta T')
     ax.set_ylabel('Mean Tj')
     fig.colorbar(im, ax=ax, label='Count')
     ax.set_xticks(np.arange(len(range_bins_2)))
     ax.set_yticks(np.arange(len(mean_bins_2)))
     ax.set_xticklabels([str(int(val)) for val in range_bins_2])
```

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/poly_somme.py` & `PowDevLif-0.0.4/src/powdevlif/function/poly_somme.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/temperature.py` & `PowDevLif-0.0.4/src/powdevlif/function/temperature.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/function/zth_materials.py` & `PowDevLif-0.0.4/src/powdevlif/function/zth_materials.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.3/src/powdevlif/lifetime.py` & `PowDevLif-0.0.4/src/powdevlif/lifetime.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   # Display Torque, Speed, Current, Loss through a graph
   # Uncomment this line if you want to show the graphs
   # graph(file,dic,losses,Temp_IGBT,Temp_diode,Temp_case, counter_IGBT, counter_diode)
   
   # Calculate the cumulative damage law
   lifetime_IGBT, lifetime_diode, e_kwh_byhours, efficiency = calculate_damage_cumulation(counter_IGBT, counter_Nf_IGBT, counter_diode, counter_Nf_diode, losses, dic, file)
 
-  results=[["IGBT Cycles",lifetime_IGBT],["Diode Cycles",lifetime_diode],["Efficiency",efficiency],["e_kwh_byhours",e_kwh_byhours]]
+  results=[["IGBT Cycles",round(lifetime_IGBT,1)],["Diode Cycles",round(lifetime_diode,1)],["Efficiency",round(efficiency,1)]]
   
   # Return the calculated lifetimes and other datas
   return (results[0:3]) #add  e_kwh_byhours if you want
 
 def pdl_graphs(variables_file_path):
   """
   This function executes a sequence of calculations related to thermal
```

