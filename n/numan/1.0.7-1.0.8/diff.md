# Comparing `tmp/numan-1.0.7.tar.gz` & `tmp/numan-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numan-1.0.7.tar", last modified: Mon Jul  3 21:16:44 2023, max compression
+gzip compressed data, was "numan-1.0.8.tar", last modified: Wed Jul  5 18:39:55 2023, max compression
```

## Comparing `numan-1.0.7.tar` & `numan-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 21:16:44.921122 numan-1.0.7/
--rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     2181 2023-07-03 21:16:44.920135 numan-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.7/README.md
--rw-rw-rw-   0        0        0     1314 2023-07-03 21:16:16.000000 numan-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 21:16:44.921122 numan-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 21:16:44.863122 numan-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 21:16:44.888122 numan-1.0.7/src/numan/
--rw-rw-rw-   0        0        0      224 2023-07-03 21:16:23.000000 numan-1.0.7/src/numan/__init__.py
--rw-rw-rw-   0        0        0    44350 2023-07-03 19:08:23.000000 numan-1.0.7/src/numan/analysis.py
--rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.7/src/numan/notifications.py
--rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.7/src/numan/plots.py
--rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.7/src/numan/project.py
--rw-rw-rw-   0        0        0    27184 2023-07-03 21:12:36.000000 numan-1.0.7/src/numan/report.py
--rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.7/src/numan/runner.py
--rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.7/src/numan/utils.py
--rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.7/src/numan/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-03 21:16:44.917120 numan-1.0.7/src/numan.egg-info/
--rw-rw-rw-   0        0        0     2181 2023-07-03 21:16:44.000000 numan-1.0.7/src/numan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-07-03 21:16:44.000000 numan-1.0.7/src/numan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 21:16:44.000000 numan-1.0.7/src/numan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-03 21:16:44.000000 numan-1.0.7/src/numan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-03 21:16:44.000000 numan-1.0.7/src/numan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 21:16:44.919121 numan-1.0.7/tests/
--rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.7/tests/test_plots.py
--rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.596357 numan-1.0.8/
+-rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     2181 2023-07-05 18:39:55.594345 numan-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.8/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-05 18:38:51.000000 numan-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 18:39:55.597357 numan-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.472558 numan-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.557557 numan-1.0.8/src/numan/
+-rw-rw-rw-   0        0        0      224 2023-07-05 18:39:03.000000 numan-1.0.8/src/numan/__init__.py
+-rw-rw-rw-   0        0        0    45479 2023-07-05 18:23:16.000000 numan-1.0.8/src/numan/analysis.py
+-rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.8/src/numan/notifications.py
+-rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.8/src/numan/plots.py
+-rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.8/src/numan/project.py
+-rw-rw-rw-   0        0        0    27184 2023-07-03 21:12:36.000000 numan-1.0.8/src/numan/report.py
+-rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.8/src/numan/runner.py
+-rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.8/src/numan/utils.py
+-rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.8/src/numan/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.581563 numan-1.0.8/src/numan.egg-info/
+-rw-rw-rw-   0        0        0     2181 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.591596 numan-1.0.8/tests/
+-rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.8/tests/test_plots.py
+-rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.8/tests/test_utils.py
```

### Comparing `numan-1.0.7/LICENSE.md` & `numan-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/PKG-INFO` & `numan-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.7
+Version: 1.0.8
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.7/README.md` & `numan-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/pyproject.toml` & `numan-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numan"
-version = "1.0.7"
+version = "1.0.8"
 description='numerosity analysis package'
 readme = "README.md"
 authors = [{ name = "Anna Nadtochiy", email = "nadtochi@usc.edu" }]
 license = { file = "LICENSE" }
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
@@ -34,15 +34,15 @@
 [project.optional-dependencies]
 dev = ["bumpver"]
 
 [project.urls] # Read The Docs will also go in here
 Homepage = "https://github.com/LemonJust/numan"
 
 [tool.bumpver]
-current_version = "1.0.7"
+current_version = "1.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `numan-1.0.7/src/numan/analysis.py` & `numan-1.0.8/src/numan/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,37 +204,53 @@
 
         self.traces_type = traces_type
         self.fps = fps
 
     def change_fs(self, fps):
         self.fps = fps
 
-    def as_dff(self, window_size):
+    def as_dff(self, method="step", window_size=None, step_size=None, baseline_volumes=None):
         """
         Returns dff of the design_matrix, the beginning of the proper measurement and the end
         ( such measurement that used the whole window for definition of baseline )
+
+        method : "step" or "sliding" - how to calculate the baseline
+            ( step - one value for the whole window, sliding - a value for each time point )
+        window_size : int, size of the window in volumes, used for baseline calculation if method = "sliding"
+        step_size : int, step size in volumes, used for baseline calculation if method = "step"
+        baseline_volumes : list of ints, volumes to use for baseline calculation if method = "step"
         """
         assert self.traces_type == "raw", f"Can't apply dff: " \
-                                          f"the signals have already been processed, these are {self.traces_type} signals"
-        dff, start, end = get_dff(self.traces, window_size)
+                                          f"the signals have already been processed, " \
+                                          f"these are {self.traces_type} signals"
+        if method == "sliding":
+            assert window_size is not None, "window_size should be provided for sliding baseline calculation"
+            dff, start, end = get_dff(self.traces, window_size)
+        elif method == "step":
+            assert step_size is not None, "step_size should be provided for step baseline calculation"
+            assert baseline_volumes is not None, "baseline_volumes should be provided for step baseline calculation"
+            dff, baseline = get_dff_in_steps(self.traces, step_size, baseline_volumes)
+        else:
+            raise AssertionError("method should be 'sliding' or 'step'")
 
         return Signals(dff, traces_type="dff")
 
     def hp_filter(self, cutoff):
         """
         Returns high-pass filtered signals from the design_matrix
         """
         assert self.traces_type == "raw", f"Can't apply dff: " \
                                           f"the signals have already been processed, these are {self.traces_type} signals"
+        import scipy.signal as signal
 
         def butter_highpass(cutoff, fps, order=5):
             # calculate the numerator and denominator coefficient vectors of the filter
             nyq = 0.5 * fps
             normal_cutoff = cutoff / nyq
-            b, a = signal.butter(order, normal_cutoff, btype="high", analog=False)
+            b, a = signal.butter(order, normal_cutoff, btype="high", analog=False, output='ba')
             return b, a
 
         def butter_highpass_filter(data, cutoff, fps, order=5):
             # return the filtered signal
             b, a = butter_highpass(cutoff, fps, order=order)
             y = signal.filtfilt(b, a, data, axis=0)
             return y
@@ -681,15 +697,15 @@
     """
     Collection of methods to perform preprocessing of the raw data in experiment.
     """
 
     def __init__(self, experiment):
         self.experiment = experiment
 
-    def remove_offset(self, save_dir, batch_size, volumes = None, offset_img=None, offset_file=None, verbose=False):
+    def remove_offset(self, save_dir, batch_size, volumes=None, offset_img=None, offset_file=None, verbose=False):
         """
         Denoises the raw movie by subtracting the offset image.
         The offset image can be prepared using coscmos package.
         Will only process full volumes.
         """
         assert offset_img is not None or offset_file is not None, \
             "Either offset_img or offset_file should be provided"
@@ -698,15 +714,15 @@
         if offset_img is None:
             offset_img = imread(offset_file)
 
         # Split the volumes into chunks of the defined size that will be loaded into RAM at once
         # if volumes are not provided, will use all the full volumes
         # if volumes are provided, will only process the requested volumes
         chunks = self.experiment.batch_volumes(batch_size, volumes=volumes, full_only=True)
-        
+
         if verbose:
             tot_volumes = 0
             n_requested_volumes = self.experiment.n_full_volumes
             if volumes is not None:
                 n_requested_volumes = len(volumes)
 
         for ichunk, chunk in enumerate(chunks):
@@ -726,17 +742,17 @@
                     data.astype(np.int16), shape=(nt, z, y, x),
                     metadata={'axes': 'TZYX'}, imagej=True)
 
             if verbose:
                 tot_volumes = tot_volumes + nt
                 print(f"written volumes : {tot_volumes}, out of {n_requested_volumes} full volumes")
 
-    def drift_correct_naive(self, save_dir, batch_size, spacing_xyz, template = 0, 
-                            registration_type = "Rigid", volumes = None, verbose=False, 
-                            ants_kwargs = {}):
+    def drift_correct_naive(self, save_dir, batch_size, spacing_xyz, template=0,
+                            registration_type="Rigid", volumes=None, verbose=False,
+                            ants_kwargs={}):
         """
         Performs drift correction using ANTs library for registration. 
         template can be an int (a frame to register to), or a 3D numpy array.
         If template is not provided, the first volume will be used as a template.
         if volumes is not None, then only the volumes in the list will be registered.
         For more info, see ANTs documentation: https://antspy.readthedocs.io/en/latest/registration.html
 
@@ -752,108 +768,111 @@
                 mask and moving_mask can be provided as paths to the masks, they will be converted to ants images.
                 Note: (see https://stackoverflow.com/questions/334655/passing-a-dictionary-to-a-function-as-keyword-parameters)
                  1. ants.registration can have parameters that are not included in the dictionary, just specify what you want, the rest will be default. 
                  2. You can not override an ants.registration function parameter that is already in the dictionary, 
                  so don't try to include keywords fixed, moving, type_of_transform, verbose and outprefix in the dictionary.
                  3. The dictionary can not have values that aren't in the ants.registration function.
         """
-        def _register(moving_image, fixed_image, spacing, registration_type, outprefix = None):
+
+        def _register(moving_image, fixed_image, spacing, registration_type, outprefix=None):
 
             # if fixed image in not ants image, convert it
             if not isinstance(fixed_image, ants.core.ants_image.ANTsImage):
                 print("Converting fixed image to ants image")
-                fixed_image = ants.from_numpy(np.transpose(fixed_image.astype(float), axes=[2,1,0]), 
-                                    spacing=spacing) # spacing in xyz order
-                
-            moving_image = ants.from_numpy(np.transpose(moving_image.astype(float), axes=[2,1,0]), 
-                                spacing=spacing)
-            
+                fixed_image = ants.from_numpy(np.transpose(fixed_image.astype(float), axes=[2, 1, 0]),
+                                              spacing=spacing)  # spacing in xyz order
+
+            moving_image = ants.from_numpy(np.transpose(moving_image.astype(float), axes=[2, 1, 0]),
+                                           spacing=spacing)
+
             # run the registration and save verbose to file
             rr = ants.registration(
-                                    fixed=fixed_image,
-                                    moving=moving_image,
-                                    type_of_transform=registration_type, 
-                                    verbose  = False,
-                                    outprefix = outprefix,
-                                    **ants_kwargs
-                                )
-            return rr['warpedmovout'].numpy().astype(np.int16).transpose((2,1,0))
-        
-        def _register_batch(batch, template, spacing, registration_type, outprefix = None):
+                fixed=fixed_image,
+                moving=moving_image,
+                type_of_transform=registration_type,
+                verbose=False,
+                outprefix=outprefix,
+                **ants_kwargs
+            )
+            return rr['warpedmovout'].numpy().astype(np.int16).transpose((2, 1, 0))
+
+        def _register_batch(batch, template, spacing, registration_type, outprefix=None):
             corrected = []
             for volume in batch:
                 # load the volume
                 volume_img = self.experiment.load_volumes([volume], verbose=False)[0]
                 # register
-                volume_img = _register(volume_img, template, spacing, registration_type, 
-                                       outprefix = outprefix)
+                volume_img = _register(volume_img, template, spacing, registration_type,
+                                       outprefix=outprefix)
                 corrected.append(volume_img)
             corrected = np.array(corrected)
             return corrected
 
         # prepare list of volumes to register
         n_full_volumes = self.experiment.n_full_volumes
         if volumes is not None:
             volumes = np.array(volumes)
-            assert volumes.max() < n_full_volumes,\
-                  f"Some volumes are outside of the experiment with {n_full_volumes} full volumes" 
+            assert volumes.max() < n_full_volumes, \
+                f"Some volumes are outside of the experiment with {n_full_volumes} full volumes"
             assert volumes.min() >= 0, "volumes must be positive integers"
             n_reguested_volumes = len(volumes)
         else:
             volumes = np.arange(n_full_volumes)
             n_reguested_volumes = n_full_volumes
 
         # if template is not an array, get template volume
         if isinstance(template, int):
             assert template < n_full_volumes, f"Template frame {template} is outside of the experiment with {n_full_volumes} full volumes"
             assert template >= 0, "Template frame must be a positive integer"
             template = self.experiment.load_volumes([template], verbose=False)[0]
         # turn template into ants image
-        template = ants.from_numpy(np.transpose(template.astype(float), axes=[2,1,0]), 
-                                    spacing=spacing_xyz) # spacing in xyz order
-        
+        template = ants.from_numpy(np.transpose(template.astype(float), axes=[2, 1, 0]),
+                                   spacing=spacing_xyz)  # spacing in xyz order
+
         # if mask and moving_mask are in ants_kwargs, convert them to ants images
         # and if they are string or pthlib.Path, load them as numpy arrays first
         if 'mask' in ants_kwargs:
             if isinstance(ants_kwargs['mask'], str) or isinstance(ants_kwargs['mask'], Path):
-                ants_kwargs['mask'] = ants.from_numpy(np.transpose(imread(ants_kwargs['mask']).astype(float), axes=[2,1,0]), 
-                                    spacing=spacing_xyz)
+                ants_kwargs['mask'] = ants.from_numpy(
+                    np.transpose(imread(ants_kwargs['mask']).astype(float), axes=[2, 1, 0]),
+                    spacing=spacing_xyz)
             elif isinstance(ants_kwargs['mask'], np.ndarray):
-                ants_kwargs['mask'] = ants.from_numpy(np.transpose(ants_kwargs['mask'].astype(float), axes=[2,1,0]), 
-                                    spacing=spacing_xyz)
+                ants_kwargs['mask'] = ants.from_numpy(np.transpose(ants_kwargs['mask'].astype(float), axes=[2, 1, 0]),
+                                                      spacing=spacing_xyz)
 
         if 'moving_mask' in ants_kwargs:
             if isinstance(ants_kwargs['moving_mask'], str) or isinstance(ants_kwargs['moving_mask'], Path):
-                ants_kwargs['moving_mask'] = ants.from_numpy(np.transpose(imread(ants_kwargs['moving_mask']).astype(float), axes=[2,1,0]), 
-                                    spacing=spacing_xyz)
+                ants_kwargs['moving_mask'] = ants.from_numpy(
+                    np.transpose(imread(ants_kwargs['moving_mask']).astype(float), axes=[2, 1, 0]),
+                    spacing=spacing_xyz)
             elif isinstance(ants_kwargs['moving_mask'], np.ndarray):
-                ants_kwargs['moving_mask'] = ants.from_numpy(np.transpose(ants_kwargs['moving_mask'].astype(float), axes=[2,1,0]), 
-                                    spacing=spacing_xyz)
-        
+                ants_kwargs['moving_mask'] = ants.from_numpy(
+                    np.transpose(ants_kwargs['moving_mask'].astype(float), axes=[2, 1, 0]),
+                    spacing=spacing_xyz)
+
         # load in batches and process volume by volume
-        chunks = self.experiment.batch_volumes(batch_size, volumes= volumes, full_only=True)
+        chunks = self.experiment.batch_volumes(batch_size, volumes=volumes, full_only=True)
         # create a directory for the transforms
         os.makedirs(f'{save_dir}/transforms', exist_ok=True)
 
         tot_volumes = 0
         for ichunk, chunk in enumerate(chunks):
             # register the chunk
             outprefix = f'{save_dir}/transforms/volume_{chunk[0]:04d}'
             corrected = _register_batch(chunk, template, spacing_xyz, registration_type,
-                                        outprefix = outprefix)
+                                        outprefix=outprefix)
             # save 
             nt, z, y, x = corrected.shape
             imwrite(f'{save_dir}/drift_corrected_movie_{ichunk:04d}.tif',
                     corrected.astype(np.int16), shape=(nt, z, y, x),
                     metadata={'axes': 'TZYX'}, imagej=True)
             if verbose:
                 tot_volumes = tot_volumes + nt
                 print(f"written volumes : {tot_volumes}, out of {n_reguested_volumes} requested volumes")
 
-
     def batch_dff_sliding_window(self, save_dir, batch_size, window_size, blur_sigma=None, verbose=False):
         """
         Creates 3D dff movie from raw 3D movie using sliding window. Will only use full_volumes,
         so the number of frames in the resulting movie can be smaller than in the original.
 
         :param blur_sigma: If not None, will apply gaussian blur in 3D with sigma = blur_sigma.
                          Can be int - then the same sigma in all 3 directions is applied,
@@ -914,15 +933,15 @@
             if verbose:
                 print(f"written frames : {chunk[start_tp]} - {chunk[end_tp - 1]}, out of {n_volumes}")
             # exit cycle the first chunk you saw the end of the experiment
             if chunk[-1] == (n_volumes - 1):
                 break
 
     def calculate_dff(self, save_dir, batch_size, step_size, baseline_volumes,
-                      resolution_xyz = [1, 1, 1], blur_sigma=None, 
+                      resolution_xyz=[1, 1, 1], blur_sigma=None,
                       verbose=False, save_baseline=False):
         """
         Creates 3D dff movie from raw 3D movie by processing movie in steps. Will only use full_volumes,
         so the number of frames in the resulting movie can be smaller than in the original.
 
         Args:
             blur_sigma (Union(int, list)): If not None, will apply gaussian blur in 3D with sigma = blur_sigma.
@@ -937,26 +956,26 @@
         """
         # TODO : make the size & digit estimation
         # TODO : write resolution into metadata
 
         assert batch_size % step_size == 0, "batch_size must be multiple of step_size"
 
         if save_baseline:
-            #create directory for baseline
+            # create directory for baseline
             os.makedirs(f'{save_dir}/baseline', exist_ok=True)
 
         # will only use full volumes
         volume_list = self.experiment.list_volumes()
         volume_list = volume_list[volume_list >= 0]
         n_volumes = len(volume_list)
 
         # will multiply dff image by this value for better visualisation later
         SCALE = 1000
 
-        #create chunks
+        # create chunks
         chunks = self.experiment.batch_volumes(batch_size, volumes=volume_list, full_only=True)
 
         for ich, chunk in enumerate(tqdm(chunks, disable=verbose)):
 
             data = self.experiment.load_volumes(chunk, verbose=False)
             # add 1 to all pixels to aviod division by zero
             data = data + 1
@@ -977,21 +996,24 @@
             min_value = dff_img.min()
             max_value = dff_img.max()
             if max_value * SCALE > 32767 or min_value * SCALE < -32768:
                 warnings.warn(f"Scaled DFF values outside the int16 range for scale = {SCALE},"
                               f" min: {min_value}, max: {max_value}")
             # write dff image
             imwrite(f'{save_dir}/dff_movie_{ich:04d}.tif', (dff_img * SCALE).astype(np.int16), shape=(t, z, y, x),
-                    resolution=(1./resolution_xyz[0], 1./resolution_xyz[1]), metadata={'spacing': resolution_xyz[2], 'unit': 'um','axes': 'TZYX'}, 
+                    resolution=(1. / resolution_xyz[0], 1. / resolution_xyz[1]),
+                    metadata={'spacing': resolution_xyz[2], 'unit': 'um', 'axes': 'TZYX'},
                     imagej=True)
             if save_baseline:
                 # print(f"Baseline shape{baseline_img.shape}")
                 # write baseline image
-                imwrite(f'{save_dir}/baseline/baseline_movie_{ich:04d}.tif', baseline_img.astype(np.int16), shape=(t, z, y, x),
-                        resolution=(1./resolution_xyz[0], 1./resolution_xyz[1]), metadata={'spacing': resolution_xyz[2], 'unit': 'um','axes': 'TZYX'}, 
+                imwrite(f'{save_dir}/baseline/baseline_movie_{ich:04d}.tif', baseline_img.astype(np.int16),
+                        shape=(t, z, y, x),
+                        resolution=(1. / resolution_xyz[0], 1. / resolution_xyz[1]),
+                        metadata={'spacing': resolution_xyz[2], 'unit': 'um', 'axes': 'TZYX'},
                         imagej=True)
 
             if verbose:
                 print(f"written frames : {chunk[0]} - {chunk[- 1]}, out of {n_volumes}")
             # exit cycle the first chunk you saw the end of the experiment
             if chunk[-1] == (n_volumes - 1):
                 break
```

### Comparing `numan-1.0.7/src/numan/notifications.py` & `numan-1.0.8/src/numan/notifications.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/plots.py` & `numan-1.0.8/src/numan/plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/project.py` & `numan-1.0.8/src/numan/project.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/report.py` & `numan-1.0.8/src/numan/report.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/runner.py` & `numan-1.0.8/src/numan/runner.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/utils.py` & `numan-1.0.8/src/numan/utils.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan/visualization.py` & `numan-1.0.8/src/numan/visualization.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/src/numan.egg-info/PKG-INFO` & `numan-1.0.8/src/numan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.7
+Version: 1.0.8
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.7/tests/test_plots.py` & `numan-1.0.8/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.7/tests/test_utils.py` & `numan-1.0.8/tests/test_utils.py`

 * *Files identical despite different names*

