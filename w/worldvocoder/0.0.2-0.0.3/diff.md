# Comparing `tmp/worldvocoder-0.0.2.tar.gz` & `tmp/worldvocoder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worldvocoder-0.0.2.tar", last modified: Fri Jun  9 18:46:51 2023, max compression
+gzip compressed data, was "worldvocoder-0.0.3.tar", last modified: Wed Jul  5 15:36:15 2023, max compression
```

## Comparing `worldvocoder-0.0.2.tar` & `worldvocoder-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-09 18:46:51.706388 worldvocoder-0.0.2/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.2/LICENSE.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-06-09 18:46:51.706432 worldvocoder-0.0.2/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)     2514 2023-06-08 22:48:56.000000 worldvocoder-0.0.2/README.md
--rw-r--r--   0 julianvanasse   (501) staff       (20)      443 2023-06-09 18:46:44.000000 worldvocoder-0.0.2/pyproject.toml
--rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-06-09 18:46:51.706651 worldvocoder-0.0.2/setup.cfg
--rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.2/setup.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-09 18:46:51.705755 worldvocoder-0.0.2/worldvocoder/
--rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.2/worldvocoder/__init__.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.2/worldvocoder/cheaptrick.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    12049 2023-06-07 18:37:53.000000 worldvocoder-0.0.2/worldvocoder/d4c.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    11051 2023-06-07 20:00:18.000000 worldvocoder-0.0.2/worldvocoder/d4cRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.2/worldvocoder/dio.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.2/worldvocoder/get_seeds_signals.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    27292 2023-06-07 19:34:25.000000 worldvocoder-0.0.2/worldvocoder/harvest.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.2/worldvocoder/main.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.2/worldvocoder/stonemask.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.2/worldvocoder/swipe.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    10737 2023-05-27 21:20:51.000000 worldvocoder-0.0.2/worldvocoder/synthesis.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.2/worldvocoder/synthesisRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     9535 2023-05-27 21:20:51.000000 worldvocoder-0.0.2/worldvocoder/synthesis_a.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-09 18:46:51.706212 worldvocoder-0.0.2/worldvocoder.egg-info/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-06-09 18:46:51.000000 worldvocoder-0.0.2/worldvocoder.egg-info/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)      532 2023-06-09 18:46:51.000000 worldvocoder-0.0.2/worldvocoder.egg-info/SOURCES.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-06-09 18:46:51.000000 worldvocoder-0.0.2/worldvocoder.egg-info/dependency_links.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-06-09 18:46:51.000000 worldvocoder-0.0.2/worldvocoder.egg-info/top_level.txt
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 15:36:15.408381 worldvocoder-0.0.3/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.3/LICENSE.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-05 15:36:15.408448 worldvocoder-0.0.3/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     2514 2023-06-08 22:48:56.000000 worldvocoder-0.0.3/README.md
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      443 2023-07-05 15:36:08.000000 worldvocoder-0.0.3/pyproject.toml
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-07-05 15:36:15.408708 worldvocoder-0.0.3/setup.cfg
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.3/setup.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 15:36:15.407644 worldvocoder-0.0.3/worldvocoder/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.3/worldvocoder/__init__.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.3/worldvocoder/cheaptrick.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    12049 2023-06-07 18:37:53.000000 worldvocoder-0.0.3/worldvocoder/d4c.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    11051 2023-06-07 20:00:18.000000 worldvocoder-0.0.3/worldvocoder/d4cRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.3/worldvocoder/dio.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.3/worldvocoder/get_seeds_signals.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    27292 2023-06-07 19:34:25.000000 worldvocoder-0.0.3/worldvocoder/harvest.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.3/worldvocoder/main.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.3/worldvocoder/stonemask.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.3/worldvocoder/swipe.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    10742 2023-07-05 15:21:43.000000 worldvocoder-0.0.3/worldvocoder/synthesis.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.3/worldvocoder/synthesisRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     9540 2023-07-05 15:22:41.000000 worldvocoder-0.0.3/worldvocoder/synthesis_a.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 15:36:15.408281 worldvocoder-0.0.3/worldvocoder.egg-info/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-05 15:36:15.000000 worldvocoder-0.0.3/worldvocoder.egg-info/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      532 2023-07-05 15:36:15.000000 worldvocoder-0.0.3/worldvocoder.egg-info/SOURCES.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-07-05 15:36:15.000000 worldvocoder-0.0.3/worldvocoder.egg-info/dependency_links.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-07-05 15:36:15.000000 worldvocoder-0.0.3/worldvocoder.egg-info/top_level.txt
```

### Comparing `worldvocoder-0.0.2/LICENSE.txt` & `worldvocoder-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/PKG-INFO` & `worldvocoder-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of WORLD vocoder.
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
 Author-email: Julian <julian.vanasse@gmail.com>
 Project-URL: Homepage, https://github.com/javanasse/worldvocoder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `worldvocoder-0.0.2/README.md` & `worldvocoder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/setup.cfg` & `worldvocoder-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/cheaptrick.py` & `worldvocoder-0.0.3/worldvocoder/cheaptrick.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/d4c.py` & `worldvocoder-0.0.3/worldvocoder/d4c.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/d4cRequiem.py` & `worldvocoder-0.0.3/worldvocoder/d4cRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/dio.py` & `worldvocoder-0.0.3/worldvocoder/dio.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/get_seeds_signals.py` & `worldvocoder-0.0.3/worldvocoder/get_seeds_signals.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/harvest.py` & `worldvocoder-0.0.3/worldvocoder/harvest.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/main.py` & `worldvocoder-0.0.3/worldvocoder/main.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/stonemask.py` & `worldvocoder-0.0.3/worldvocoder/stonemask.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/swipe.py` & `worldvocoder-0.0.3/worldvocoder/swipe.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/synthesis.py` & `worldvocoder-0.0.3/worldvocoder/synthesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     temporal_position_index = interp1d(temporal_positions, np.arange(1, len(temporal_positions) + 1),
                                        fill_value='extrapolate')(pulse_locations)
     temporal_position_index = np.maximum(1, np.minimum(len(temporal_positions), temporal_position_index))
     
     amplitude_aperiodic = source_object['aperiodicity'] ** 2
     amplitude_periodic = np.maximum(0.001, (1 - amplitude_aperiodic))
 
-    dc_remover_base = signal.hanning(fft_size + 2)[1:-1]
+    dc_remover_base = signal.windows.hann(fft_size + 2)[1:-1]
     dc_remover_base = dc_remover_base / np.sum(dc_remover_base)
     coefficient = 2.0 * np.pi * fs / fft_size
     
     for i in range(len(pulse_locations_index)):
         spectrum_slice, periodic_slice, aperiodic_slice = \
             get_spectral_parameters(temporal_positions, temporal_position_index[i],
                                     spectrogram, amplitude_periodic, amplitude_aperiodic, pulse_locations[i])
```

### Comparing `worldvocoder-0.0.2/worldvocoder/synthesisRequiem.py` & `worldvocoder-0.0.3/worldvocoder/synthesisRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.2/worldvocoder/synthesis_a.py` & `worldvocoder-0.0.3/worldvocoder/synthesis_a.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             tmp_cepstrum = np.fft.fft(np.log(np.abs(periodic_spectrum)) / 2).real
             tmp_complex_cepstrum[latter_index.astype(int) - 1] = tmp_cepstrum[latter_index.astype(int) - 1] * 2
             tmp_complex_cepstrum[0] = tmp_cepstrum[0]
 
             #  TODO: possible speed up via rfft?
 
             response = np.fft.fftshift(np.fft.ifft(np.exp(np.fft.ifft(tmp_complex_cepstrum))).real)
-            dc_remover = signal.hanning(len(response) + 2)[1:-1]
+            dc_remover = signal.windows.hann(len(response) + 2)[1:-1]
             dc_remover = dc_remover / np.sum(dc_remover)
             dc_remover = dc_remover * -np.sum(response)
             response += dc_remover
             y[output_buffer_index.astype(int) - 1] += response * np.sqrt(max(1, noise_size))
             tmp_aperiodic_spectrum = spectrum_slice * aperiodic_slice
         else:
             tmp_aperiodic_spectrum = spectrum_slice
```

### Comparing `worldvocoder-0.0.2/worldvocoder.egg-info/PKG-INFO` & `worldvocoder-0.0.3/worldvocoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of WORLD vocoder.
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
 Author-email: Julian <julian.vanasse@gmail.com>
 Project-URL: Homepage, https://github.com/javanasse/worldvocoder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `worldvocoder-0.0.2/worldvocoder.egg-info/SOURCES.txt` & `worldvocoder-0.0.3/worldvocoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

