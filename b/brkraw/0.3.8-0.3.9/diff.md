# Comparing `tmp/brkraw-0.3.8.tar.gz` & `tmp/brkraw-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brkraw-0.3.8.tar", last modified: Sat Jul  1 20:57:45 2023, max compression
+gzip compressed data, was "brkraw-0.3.9.tar", last modified: Wed Jul  5 20:14:07 2023, max compression
```

## Comparing `brkraw-0.3.8.tar` & `brkraw-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.393892 brkraw-0.3.8/
--rw-r--r--   0 shlee      (501) staff       (20)    35149 2022-07-29 18:29:38.000000 brkraw-0.3.8/LICENSE
--rw-r--r--   0 shlee      (501) staff       (20)      533 2023-07-01 20:57:45.393664 brkraw-0.3.8/PKG-INFO
--rw-r--r--   0 shlee      (501) staff       (20)     4586 2022-07-29 18:29:38.000000 brkraw-0.3.8/README.md
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.383841 brkraw-0.3.8/brkraw/
--rw-r--r--   0 shlee      (501) staff       (20)      132 2023-07-01 20:54:52.000000 brkraw-0.3.8/brkraw/__init__.py
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.388601 brkraw-0.3.8/brkraw/lib/
--rw-r--r--   0 shlee      (501) staff       (20)       82 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/lib/__init__.py
--rw-r--r--   0 shlee      (501) staff       (20)    28346 2023-07-01 20:53:22.000000 brkraw-0.3.8/brkraw/lib/backup.py
--rw-r--r--   0 shlee      (501) staff       (20)     4010 2023-07-01 20:53:20.000000 brkraw-0.3.8/brkraw/lib/errors.py
--rw-r--r--   0 shlee      (501) staff       (20)    54910 2023-07-01 20:53:24.000000 brkraw-0.3.8/brkraw/lib/loader.py
--rw-r--r--   0 shlee      (501) staff       (20)     7096 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/lib/orient.py
--rw-r--r--   0 shlee      (501) staff       (20)     1622 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/lib/parser.py
--rw-r--r--   0 shlee      (501) staff       (20)    12837 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/lib/pvobj.py
--rw-r--r--   0 shlee      (501) staff       (20)    12647 2023-07-01 20:53:29.000000 brkraw-0.3.8/brkraw/lib/reference.py
--rw-r--r--   0 shlee      (501) staff       (20)    16089 2023-07-01 20:53:26.000000 brkraw-0.3.8/brkraw/lib/utils.py
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.389488 brkraw-0.3.8/brkraw/scripts/
--rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/scripts/__init__.py
--rw-r--r--   0 shlee      (501) staff       (20)     4335 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/scripts/brk_backup.py
--rw-r--r--   0 shlee      (501) staff       (20)    37893 2023-07-01 20:53:27.000000 brkraw-0.3.8/brkraw/scripts/brkraw.py
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.392973 brkraw-0.3.8/brkraw/ui/
--rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/__init__.py
--rw-r--r--   0 shlee      (501) staff       (20)      419 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/config.py
--rw-r--r--   0 shlee      (501) staff       (20)     8011 2023-06-07 15:37:29.000000 brkraw-0.3.8/brkraw/ui/main_win.py
--rw-r--r--   0 shlee      (501) staff       (20)     7777 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/previewer.py
--rw-r--r--   0 shlee      (501) staff       (20)     3684 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/scan_info.py
--rw-r--r--   0 shlee      (501) staff       (20)     3503 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/scan_list.py
--rw-r--r--   0 shlee      (501) staff       (20)     5467 2022-07-29 18:29:38.000000 brkraw-0.3.8/brkraw/ui/subj_info.py
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.385736 brkraw-0.3.8/brkraw.egg-info/
--rw-r--r--   0 shlee      (501) staff       (20)      533 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/PKG-INFO
--rw-r--r--   0 shlee      (501) staff       (20)      674 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/SOURCES.txt
--rw-r--r--   0 shlee      (501) staff       (20)        1 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/dependency_links.txt
--rw-r--r--   0 shlee      (501) staff       (20)       98 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/entry_points.txt
--rw-r--r--   0 shlee      (501) staff       (20)      128 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/requires.txt
--rw-r--r--   0 shlee      (501) staff       (20)       13 2023-07-01 20:57:45.000000 brkraw-0.3.8/brkraw.egg-info/top_level.txt
--rw-r--r--   0 shlee      (501) staff       (20)       38 2023-07-01 20:57:45.393981 brkraw-0.3.8/setup.cfg
--rw-r--r--   0 shlee      (501) staff       (20)     1545 2023-07-01 20:53:36.000000 brkraw-0.3.8/setup.py
-drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-01 20:57:45.393242 brkraw-0.3.8/tests/
--rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.8/tests/__init__.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.230056 brkraw-0.3.9/
+-rw-r--r--   0 shlee      (501) staff       (20)    35149 2022-07-29 18:29:38.000000 brkraw-0.3.9/LICENSE
+-rw-r--r--   0 shlee      (501) staff       (20)      533 2023-07-05 20:14:07.229763 brkraw-0.3.9/PKG-INFO
+-rw-r--r--   0 shlee      (501) staff       (20)     4586 2023-07-01 21:15:56.000000 brkraw-0.3.9/README.md
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.209129 brkraw-0.3.9/brkraw/
+-rw-r--r--   0 shlee      (501) staff       (20)      132 2023-07-05 20:13:27.000000 brkraw-0.3.9/brkraw/__init__.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.220347 brkraw-0.3.9/brkraw/lib/
+-rw-r--r--   0 shlee      (501) staff       (20)       82 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/lib/__init__.py
+-rw-r--r--   0 shlee      (501) staff       (20)    28330 2023-07-05 20:09:02.000000 brkraw-0.3.9/brkraw/lib/backup.py
+-rw-r--r--   0 shlee      (501) staff       (20)     3978 2023-07-05 20:08:31.000000 brkraw-0.3.9/brkraw/lib/errors.py
+-rw-r--r--   0 shlee      (501) staff       (20)    54850 2023-07-05 20:07:32.000000 brkraw-0.3.9/brkraw/lib/loader.py
+-rw-r--r--   0 shlee      (501) staff       (20)     7092 2023-07-05 20:05:58.000000 brkraw-0.3.9/brkraw/lib/orient.py
+-rw-r--r--   0 shlee      (501) staff       (20)     1622 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/lib/parser.py
+-rw-r--r--   0 shlee      (501) staff       (20)    12833 2023-07-05 20:05:46.000000 brkraw-0.3.9/brkraw/lib/pvobj.py
+-rw-r--r--   0 shlee      (501) staff       (20)    12647 2023-07-01 20:53:29.000000 brkraw-0.3.9/brkraw/lib/reference.py
+-rw-r--r--   0 shlee      (501) staff       (20)    15943 2023-07-05 20:05:28.000000 brkraw-0.3.9/brkraw/lib/utils.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.222465 brkraw-0.3.9/brkraw/scripts/
+-rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/scripts/__init__.py
+-rw-r--r--   0 shlee      (501) staff       (20)     4335 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/scripts/brk_backup.py
+-rw-r--r--   0 shlee      (501) staff       (20)    38021 2023-07-05 20:09:30.000000 brkraw-0.3.9/brkraw/scripts/brkraw.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.228581 brkraw-0.3.9/brkraw/ui/
+-rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/__init__.py
+-rw-r--r--   0 shlee      (501) staff       (20)      419 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/config.py
+-rw-r--r--   0 shlee      (501) staff       (20)     8011 2023-06-07 15:37:29.000000 brkraw-0.3.9/brkraw/ui/main_win.py
+-rw-r--r--   0 shlee      (501) staff       (20)     7777 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/previewer.py
+-rw-r--r--   0 shlee      (501) staff       (20)     3684 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/scan_info.py
+-rw-r--r--   0 shlee      (501) staff       (20)     3503 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/scan_list.py
+-rw-r--r--   0 shlee      (501) staff       (20)     5467 2022-07-29 18:29:38.000000 brkraw-0.3.9/brkraw/ui/subj_info.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.211197 brkraw-0.3.9/brkraw.egg-info/
+-rw-r--r--   0 shlee      (501) staff       (20)      533 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/PKG-INFO
+-rw-r--r--   0 shlee      (501) staff       (20)      674 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/SOURCES.txt
+-rw-r--r--   0 shlee      (501) staff       (20)        1 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/dependency_links.txt
+-rw-r--r--   0 shlee      (501) staff       (20)       98 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/entry_points.txt
+-rw-r--r--   0 shlee      (501) staff       (20)      128 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/requires.txt
+-rw-r--r--   0 shlee      (501) staff       (20)       13 2023-07-05 20:14:07.000000 brkraw-0.3.9/brkraw.egg-info/top_level.txt
+-rw-r--r--   0 shlee      (501) staff       (20)       38 2023-07-05 20:14:07.230160 brkraw-0.3.9/setup.cfg
+-rw-r--r--   0 shlee      (501) staff       (20)     1545 2023-07-01 20:53:36.000000 brkraw-0.3.9/setup.py
+drwxr-xr-x   0 shlee      (501) staff       (20)        0 2023-07-05 20:14:07.229377 brkraw-0.3.9/tests/
+-rw-r--r--   0 shlee      (501) staff       (20)        0 2022-07-29 18:29:38.000000 brkraw-0.3.9/tests/__init__.py
```

### Comparing `brkraw-0.3.8/LICENSE` & `brkraw-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/PKG-INFO` & `brkraw-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brkraw
-Version: 0.3.8
+Version: 0.3.9
 Summary: Bruker PvDataset Loader
 Home-page: https://github.com/brkraw/brkraw
 Author: SungHo Lee
 Author-email: shlee@unc.edu
 License: GNLv3
 Keywords: bruker data_handler converter administrator_tool
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `brkraw-0.3.8/README.md` & `brkraw-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![DOI](https://zenodo.org/badge/245546149.svg)](https://zenodo.org/badge/latestdoi/245546149)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/BrkRaw/tutorials/master)
 
 ## BrkRaw: A comprehensive tool to access raw Bruker Biospin MRI data
-#### Version: 0.3.4
+#### Version: 0.3.8
 
 ### Description
 
 The ‘BrkRaw’ is a python module designed to provide a comprehensive tool to access raw data acquired from 
 Bruker Biospin preclinical MRI scanner. This module is also compatible with the zip compressed data 
 to enable use of the archived data directly.  
 The module is comprised of four components, including graphical user interface (GUI), command-line tools,
```

### Comparing `brkraw-0.3.8/brkraw/lib/backup.py` & `brkraw-0.3.9/brkraw/lib/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                              'set_arc')
                 arc = None
                 raw_dname = None
                 raw_path = None
                 garbage = True
                 crashed = True
 
-            if raw_dname is not None:
+            if raw_dname != None:
                 r = self.get_rpath_obj(raw_dname)
             else:
                 r = None
 
             if r is None:
                 raw_dname = os.path.splitext(arc_fname)[0]
                 self.set_raw(raw_dname, raw_dir, removed=True)
@@ -261,15 +261,15 @@
         for b in tqdm.tqdm(list_of_brk, bar_format=_bar_fmt):
             self._cache.set_arc(b, arc_dir=self._apath, raw_dir=self._rpath)
         self._save_pickle()
 
         # update raw dataset information (raw dataset cache will remain even its removed)
         print('\nScanning raw dataset cache...')
         for r in tqdm.tqdm(self.raw_data[:], bar_format=_bar_fmt):
-            if r.path is not None:
+            if r.path != None:
                 if not os.path.exists(os.path.join(self._rpath, r.path)):
                     if not r.removed:
                         r.removed = True
         self._save_pickle()
 
         print('\nReviewing the cached information...')
         for b in tqdm.tqdm(self.arc_data[:], bar_format=_bar_fmt):
@@ -296,15 +296,15 @@
                     r = self.get_rpath_obj(b.path, by_arc=True)
                     if not r.backup:
                         r.backup = True
         self._save_pickle()
 
     def is_same_as_raw(self, filename):
         arc = BrukerLoader(os.path.join(self._apath, filename))
-        if arc.pvobj.path is not None:
+        if arc.pvobj.path != None:
             raw_path = os.path.join(self._rpath, arc.pvobj.path)
             if os.path.exists(raw_path):
                 raw = BrukerLoader(raw_path)
                 return arc.num_recos == raw.num_recos
             else:
                 return None
         else:
@@ -491,15 +491,15 @@
                              crashed=self.get_crashed()[:],
                              duplicated=self.get_duplicated().copy())
             for label, dset in list_data.items():
                 if label == 'duplicated':
                     print('\nStart removing {} archived data...'.format(label.upper()))
                     if len(dset.items()):
                         for raw_dname, arcs in dset.items():
-                            if raw_dname is not None:
+                            if raw_dname != None:
                                 raw_path = os.path.join(self._rpath, raw_dname)
                                 if os.path.exists(raw_path):
                                     r_size, r_unit = get_dirsize(raw_path)
                                     r_size = '{0:.2f} {1}'.format(r_size, r_unit)
                                 else:
                                     r_size = 'Removed'
                                 if len(raw_dname) < 60:
```

### Comparing `brkraw-0.3.8/brkraw/lib/errors.py` & `brkraw-0.3.9/brkraw/lib/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 class FileNotValidError(Error):
     """ Raised when the file is not valid format """
 
     def __init__(self, file_name=None, data_type=None):
         self.file_name = None
         self.data_type = None
 
-        if file_name is not None:
+        if file_name != None:
             self.file_name = os.path.basename(file_name)
             if os.path.isdir(file_name):
                 object_type = 'directory'
             else:
                 object_type = 'file'
-            if data_type is not None:
+            if data_type != None:
                 self.data_type = data_type
                 self.message = "The {} '{}' is not valid {}".format(object_type,
                                                                     self.file_name,
                                                                     self.data_type)
             else:
                 self.message = "The {} '{}' is not valid".format(object_type,
                                                                  self.file_name)
@@ -41,46 +41,46 @@
 
 
 class ArchiveFailedError(Error):
     """ Raised when the archive process is failed [designed for brkraw module] """
     file_name = None
 
     def __init__(self, file_name=None):
-        if file_name is not None:
+        if file_name != None:
             self.file_name = os.path.basename(file_name)
             self.message = "The data '{}' is not archived".format(
                 self.file_name)
         else:
             self.message = "Archive failed to execute"
 
 
 class RemoveFailedError(Error):
     """ Raise when the os.remove process is failed """
     file_name = None
 
     def __init__(self, file_name=None):
-        if file_name is not None:
+        if file_name != None:
             self.file_name = os.path.basename(file_name)
             self.message = "The file '{}' is not removed".format(
                 self.file_name)
         else:
             self.message = "Remove failed to execute"
 
 
 class RenameFailedError(Error):
     """ Raised when the os.rename process is failed (OSError)"""
     file1_name = None
     file2_name = None
 
     def __init__(self, file1_name=None, file2_name=None):
-        if file1_name is not None:
+        if file1_name != None:
             self.file1_name = os.path.basename(file1_name)
-        if file2_name is not None:
+        if file2_name != None:
             self.file2_name = os.path.basename(file2_name)
-        if (self.file1_name is not None) and (self.file2_name is not None):
+        if (self.file1_name != None) and (self.file2_name != None):
             self.message = "Rename failed to execute from:'{}' to:'{}'".format(self.file1_name,
                                                                                self.file2_name)
         else:
             self.message = "Rename failed to execute"
 
 
 class UnexpectedError(Error):
```

### Comparing `brkraw-0.3.8/brkraw/lib/loader.py` & `brkraw-0.3.9/brkraw/lib/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
             if slice_code not in group_id_:
                 pass
             else:
                 slice_axis_ = group_id_.index(slice_code) + 2
                 dataobj_ = np.swapaxes(dataobj_, 2, slice_axis_)
             return dataobj_
 
-        if fg_info['frame_type'] is not None:
+        if fg_info['frame_type'] != None:
             if group_id[0] == 'FG_SLICE':
                 pass
 
             elif group_id[0] == 'FG_ECHO':  # multi-echo
                 if self.is_multi_echo(scan_id, reco_id):
                     # push echo to last axis for BIDS
                     if 'FG_SLICE' not in group_id:
@@ -323,17 +323,17 @@
         """
         from nibabel import Nifti1Image
         visu_pars = self._get_visu_pars(scan_id, reco_id)
         method = self._method[scan_id]
         affine = self._get_affine(visu_pars, method)
 
         data_slp, data_off = self._get_dataslp(visu_pars)
-        if isinstance(data_slp, list) and slope is not None:
+        if isinstance(data_slp, list) and slope != None:
             slope = True
-            if isinstance(data_off, list) and offset is not None:
+            if isinstance(data_off, list) and offset != None:
                 offset = True
 
         imgobj = self.get_dataobj(scan_id, reco_id, slope=slope, offset=offset)
 
         if isinstance(affine, list):
             parser = []
             slice_info = self._get_slice_info(visu_pars)
@@ -355,15 +355,15 @@
             for e in range(imgobj.shape[-1]):
                 imgobj_ = imgobj[..., e]
                 if len(imgobj_.shape) > 4:
                     x, y, z = imgobj_.shape[:3]
                     f = multiply_all(imgobj_.shape[3:])
                     # all converted nifti must be 4D
                     imgobj_ = imgobj_.reshape([x, y, z, f])
-                if crop is not None:
+                if crop != None:
                     if crop[0] is None:
                         niiobj_ = Nifti1Image(imgobj_[..., :crop[1]], affine)
                     elif crop[1] is None:
                         niiobj_ = Nifti1Image(imgobj_[..., crop[0]:], affine)
                     else:
                         niiobj_ = Nifti1Image(imgobj_[..., crop[0]:crop[1]], affine)
                 else:
@@ -373,15 +373,15 @@
             return parser
         else:
             if len(imgobj.shape) > 4:
                 x, y, z = imgobj.shape[:3]
                 f = multiply_all(imgobj.shape[3:])
                 # all converted nifti must be 4D
                 imgobj = imgobj.reshape([x, y, z, f])
-        if crop is not None:
+        if crop != None:
             if crop[0] is None:
                 niiobj = Nifti1Image(imgobj[..., :crop[1]], affine)
             elif crop[1] is None:
                 niiobj = Nifti1Image(imgobj[..., crop[0]:], affine)
             else:
                 niiobj = Nifti1Image(imgobj[..., crop[0]:crop[1]], affine)
         else:
@@ -507,15 +507,15 @@
 
         if metadata is None:
             metadata = COMMON_META_REF.copy()
         for k, v in metadata.items():
             val = meta_get_value(v, acqp, method, visu_pars)
             if k in ['PhaseEncodingDirection', 'SliceEncodingDirection']:
                 # Convert the encoding direction meta data into BIDS format
-                if val is not None:
+                if val != None:
                     if isinstance(val, int):
                         val = encdir_dic[val]
                     else:
                         if isinstance(val, list):
                             if is_all_element_same(val):
                                 val = val[0]
                             else:
@@ -547,15 +547,15 @@
             if isinstance(val, np.ndarray):
                 val = val.tolist()
             json_obj[k] = val
         return json_obj
 
     def save_json(self, scan_id, reco_id, filename, dir='./', metadata=None, condition=None):
         json_obj = self._parse_json(scan_id, reco_id, metadata)
-        if condition is not None:
+        if condition != None:
             code, idx = condition
             if code == 'me':    # multi-echo
                 if 'EchoTime' in json_obj.keys():
                     te = json_obj['EchoTime']
                     if isinstance(te, list):
                         json_obj['EchoTime'] = te[idx]
                     else:
@@ -595,15 +595,15 @@
         pattern_2 = r'(\d{4}-\d{2}-\d{2})[T](\d{2}:\d{2}:\d{2})'
         if re.match(pattern_1, subject_date):
             # start time
             start_time = dt.time(*map(int, re.sub(pattern_1, r'\1', subject_date).split(':')))
             # date
             date = dt.datetime.strptime(re.sub(pattern_1, r'\2', subject_date), '%d %b %Y').date()
             # end time
-            if visu_pars is not None:
+            if visu_pars != None:
                 last_scan_time = get_value(visu_pars, 'VisuAcqDate')
                 last_scan_time = dt.time(*map(int, re.sub(pattern_1, r'\1', last_scan_time).split(':')))
                 acq_time = get_value(visu_pars, 'VisuAcqScanTime') / 1000.0
                 time_delta = dt.timedelta(0, acq_time)
                 scan_time = (dt.datetime.combine(date, last_scan_time) + time_delta).time()
                 return dict(date=date,
                             start_time=start_time,
@@ -612,15 +612,15 @@
             # start time
             # subject_date = get_value(self._subject, 'SUBJECT_date')[0]
             start_time = dt.time(*map(int, re.sub(pattern_2, r'\2', subject_date).split(':')))
             # date
             date = dt.date(*map(int, re.sub(pattern_2, r'\1', subject_date).split('-')))
 
             # end date
-            if visu_pars is not None:
+            if visu_pars != None:
                 scan_time = get_value(visu_pars, 'VisuCreationDate')[0]
                 scan_time = dt.time(*map(int, re.sub(pattern_2, r'\2', scan_time).split(':')))
                 return dict(date=date,
                             start_time=start_time,
                             scan_time=scan_time)
         else:
             raise Exception(ERROR_MESSAGES['NotIntegrated'])
@@ -781,25 +781,25 @@
             else:
                 raise Exception(ERROR_MESSAGES['NotIntegrated'])
             niiobj.header['slice_start'] = 0
             niiobj.header['slice_end'] = num_slices - 1
         else:
             niiobj.header.set_xyzt_units('mm')
         if not slope:
-            if slope is not None:
+            if slope != None:
                 if isinstance(data_slp, list):
                     raise InvalidApproach('Invalid slope size;'
                                           'The vector type scl_slope cannot be set in nifti header.')
                 niiobj.header['scl_slope'] = data_slp
             else:
                 niiobj.header['scl_slope'] = 1
         else:
             niiobj.header['scl_slope'] = 1
         if not offset:
-            if offset is not None:
+            if offset != None:
                 if isinstance(data_off, list):
                     raise InvalidApproach('Invalid offset size;'
                                           'The vector type scl_offset cannot be set in nifti header.')
                 niiobj.header['scl_inter'] = data_off
             else:
                 niiobj.header['scl_inter'] = 0
         else:
@@ -810,15 +810,15 @@
 
     # EPI
     def _get_temp_info(self, visu_pars):
         """return temporal resolution for each volume of image"""
         total_time = get_value(visu_pars, 'VisuAcqScanTime')
         fg_info = self._get_frame_group_info(visu_pars)
         parser = []
-        if fg_info['frame_type'] is not None:
+        if fg_info['frame_type'] != None:
             for id, fg in enumerate(fg_info['group_id']):
                 if not re.search('slice', fg, re.IGNORECASE):
                     parser.append(fg_info['matrix_shape'][id])
         frame_size = multiply_all(parser) if len(parser) > 0 else 1
         if total_time is None:  # derived reco data
             total_time = 0
         return dict(temporal_resol=(total_time / frame_size),
@@ -1000,15 +1000,15 @@
         omatrix_parser  = []
         oorder_parser   = []
         vposition_parser = []
 
         orient_matrix = get_value(visu_pars, 'VisuCoreOrientation').tolist()
         slice_info = self._get_slice_info(visu_pars)
         slice_position = get_value(visu_pars, 'VisuCorePosition')
-        if self._override_position is not None: # add option to override
+        if self._override_position != None: # add option to override
             subj_position = self._override_position
         else:
             subj_position = get_value(visu_pars, 'VisuSubjectPosition')
         gradient_orient = get_value(method, 'PVM_SPackArrGradOrient')
 
         if slice_info['num_slice_packs'] > 1:
             num_ori_mat = len(orient_matrix)
@@ -1058,15 +1058,15 @@
             except:
                 raise Exception(ERROR_MESSAGES['NumSlicePosition'])
 
             omatrix_parser = np.asarray(orient_matrix).reshape([3, 3])
             oorder_parser = get_axis_orient(omatrix_parser)
             vposition_parser = slice_position
 
-        if self._override_type is not None: # add option to override
+        if self._override_type != None: # add option to override
             subj_type = self._override_type
         else:
             subj_type = get_value(visu_pars, 'VisuSubjectType')    
 
         return dict(subject_type = subj_type,
                     subject_position = subj_position,
                     volume_position = vposition_parser,
@@ -1143,15 +1143,15 @@
                 else:
                     if num_temporal_frame > 1:
                         matrix_size.append(num_temporal_frame)
             else:
                 if num_temporal_frame > 1:
                     matrix_size.append(num_temporal_frame)
 
-        if dataobj is not None:
+        if dataobj != None:
             # matrix size inspection
             dataobj_shape = dataobj.shape[0]
             if multiply_all(matrix_size) != dataobj_shape:
                 raise UnexpectedError('Matrix size mismatch with dataobj;'
                                       '{} != {}{}'.format(multiply_all(matrix_size),
                                                           dataobj_shape,
                                                           ISSUE_REPORT))
```

### Comparing `brkraw-0.3.8/brkraw/lib/orient.py` & `brkraw-0.3.9/brkraw/lib/orient.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         x, y, z coordinate for origin of image matrix
     """
     slice_position = cp(slice_position)
     dx, dy, dz = map(lambda x: x.max() - x.min(), slice_position.T)
     max_delta_axis = np.argmax([dx, dy, dz])
     rx, ry, rz = [None, None, None]
 
-    if gradient_orient is not None:
+    if gradient_orient != None:
         zmat = np.zeros(gradient_orient[0].shape)
         for cid, col in enumerate(gradient_orient[0].T):
             yid = np.argmax(abs(col))
             zmat[cid, yid] = np.round(col[yid], decimals=0)
         rx, ry, rz = calc_eulerangle(np.round(zmat.T))
 
     if max_delta_axis == 0:     # sagital
```

### Comparing `brkraw-0.3.8/brkraw/lib/parser.py` & `brkraw-0.3.9/brkraw/lib/parser.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/lib/pvobj.py` & `brkraw-0.3.9/brkraw/lib/pvobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self._method = dict()
         self._acqp = dict()
         self._visu_pars = dict()
         self._reco = dict()
         self._2dseq = dict()
 
     def _update_studyinfo(self):
-        if self._subject is not None:
+        if self._subject != None:
             subject = self._subject
             self.user_account   = subject.headers['OWNER']
             self.subj_id        = get_value(subject, 'SUBJECT_id')
             self.study_id       = get_value(subject, 'SUBJECT_study_nr')
             self.session_id     = get_value(subject, 'SUBJECT_study_name')
             
             # [20210820] Add-paravision 360 related.
```

### Comparing `brkraw-0.3.8/brkraw/lib/reference.py` & `brkraw-0.3.9/brkraw/lib/reference.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/lib/utils.py` & `brkraw-0.3.9/brkraw/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .errors import UnexpectedError
+from .errors import *
 from .reference import *
 import re
 import os
 import numpy as np
 from collections import OrderedDict
 from functools import partial, reduce
 from copy import copy as cp
@@ -26,15 +26,15 @@
     # JCAMP DX parser
     params = OrderedDict()
     param_addresses = list()
 
     for line_num, line in enumerate(stringlist):
         regex_obj = re.match(ptrn_param, line)
         # if line is key=value pair
-        if regex_obj is not None:
+        if regex_obj != None:
             # parse key and value
             key = re.sub(ptrn_param, r'\g<key>', line)
             value = re.sub(ptrn_param, r'\g<value>', line)
             # if key contains $
             if re.match(ptrn_key, key):
                 # classify as parameter
                 params[line_num] = PARAMETER, re.sub(ptrn_key, r'\g<key>', key), value
@@ -101,30 +101,30 @@
                 while len(re.findall(ptrn_braces, data_holder)) != 0:
                     for parsed in re.finditer(ptrn_braces, data_holder):
                         key = 'level_{}'.format(level)
 
                         cont_parser = []
                         for cont in map(str.strip, parsed.group('contents').split(',')):
                             cont = convert_data_to(cont, -1)
-                            if cont is not None:
+                            if cont != None:
                                 cont_parser.append(cont)
                         if key not in parser.keys():
                             parser[key] = []
                         parser[key].append(cont_parser)
                         data_holder = data_holder.replace(parsed.group(0), '')
                     level += 1
                 del level
                 data = parser
             else:
                 if re.match(ptrn_string, data):
                     data = re.sub(ptrn_string, r'\g<string>', data)
                 else:
                     is_array = re.findall(ptrn_array, data)
                     # parse data shape
-                    if shape is not -1:
+                    if shape != -1:
                         shape = re.sub(ptrn_array, r'\g<array>', shape)
                         if ',' in shape:
                             shape = [convert_string_to(c) for c in shape.split(',')]
 
                     if is_array:
                         is_array = [convert_string_to(c) for c in is_array]
                         if any([',' in cell for cell in is_array]):
@@ -187,15 +187,15 @@
                 parser[k] = meta_get_value(v, acqp, method, visu_pars)
             return parser
     elif isinstance(value, list):
         parser = []
         max_index = len(value) - 1
         for i, vi in enumerate(value):
             val = meta_get_value(vi, acqp, method, visu_pars)
-            if val is not None:
+            if val != None:
                 if val == vi:
                     if i == max_index:
                         parser.append(val)
                 else:
                     parser.append(val)
         if len(parser) > 0:
             return parser[0]
@@ -224,35 +224,35 @@
         return True
     else:
         return False
 
 
 def meta_check_where(value, acqp, method, visu_pars):
     val = meta_get_value(value['key'], acqp, method, visu_pars)
-    if val is not None:
+    if val != None:
         if isinstance(value['where'], str):
             if value['where'] not in val:
                 return None
             else:
                 return val.index(value['where'])
         else:
             where = meta_get_value(value['where'], acqp, method, visu_pars)
             return val.index(where)
     else:
         return None
 
 
 def meta_check_index(value, acqp, method, visu_pars):
     val = meta_get_value(value['key'], acqp, method, visu_pars)
-    if val is not None:
+    if val != None:
         if isinstance(value['idx'], int):
             return val[value['idx']]
         else:
             idx = meta_get_value(value['idx'], acqp, method, visu_pars)
-        if idx is not None:
+        if idx != None:
             return val[idx]
         else:
             return None
     else:
         return None
 
 
@@ -331,41 +331,39 @@
 
     unit = int(len(str(file_size)) / 3)
     return convert_unit(file_size, unit), unit_dict[unit]
 
 
 def bids_validation(df, idx, key, val, num_char_allowed, dtype=None):
     import string
-    from shleeh.errors import InvalidValueInField
     col = string.ascii_uppercase[df.columns.tolist().index(key)]
     special_char = re.compile(r'[^0-9a-zA-Z]')
     str_val = str(val)
     loc = 'col,row:[{},{}]'.format(col, idx + 2)
     if len(str_val) > num_char_allowed:
         message = "{} You can't use more than {} characters.".format(loc, num_char_allowed)
         raise InvalidValueInField(message)
     matched = special_char.search(str_val)
-    if matched is not None:
+    if matched != None:
         if ' ' in matched.group():
             message = "{} Empty string is not allowed.".format(loc)
         else:
             message = "{} Special characters are not allowed.".format(loc)
         raise InvalidValueInField(message)
-    if dtype is not None:
+    if dtype != None:
         try:
             dtype(val)
         except:
             message = "{} Invalid data type. Value must be {}.".format(loc, dtype.__name__)
             raise InvalidValueInField(message)
     return True
 
 
 def get_bids_ref_obj(ref_path, row):
     import json
-    from shleeh.errors import InvalidApproach
     if os.path.exists(ref_path) and ref_path.lower().endswith('.json'):
         ref_data = json.load(open(ref_path))
         ref = ref_data['common']
         if row.modality in ['bold', 'cbv', 'epi']:
             if 'func' in ref_data.keys():
                 for k, v in ref_data['func'].items():
                     if k in ref.keys():
```

### Comparing `brkraw-0.3.8/brkraw/scripts/brk_backup.py` & `brkraw-0.3.9/brkraw/scripts/brk_backup.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/scripts/brkraw.py` & `brkraw-0.3.9/brkraw/scripts/brkraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,24 +292,24 @@
             dpath = os.path.join(path, dname)
 
             try:
                 dset = BrukerLoader(dpath)
             except:
                 dset = None
 
-            if dset is not None:
+            if dset != None:
                 if dset.is_pvdataset:
                     pvobj = dset.pvobj
 
                     rawdata = pvobj.path
                     subj_id = pvobj.subj_id
 
                     # make subj_id bids appropriate
                     subj_id = cleanSubjectID(subj_id)
-
+                    
                     sess_id = pvobj.session_id
 
                     # make sess_id bids appropriate
                     sess_id = cleanSessionID(sess_id)
 
                     for scan_id, recos in pvobj.avail_reco_id.items():
                         for reco_id in recos:
@@ -323,23 +323,23 @@
 
                                     item = dict(zip(Headers, [rawdata, subj_id, sess_id, scan_id, reco_id, datatype]))
                                     if datatype == 'fmap':
                                         for m, s, e in [['fieldmap', 0, 1], ['magnitude', 1, 2]]:
                                             item['modality'] = m
                                             item['Start'] = s
                                             item['End'] = e
-                                            df = df.append(item, ignore_index=True)
+                                            df = pd.concat([df, pd.DataFrame([item])], ignore_index=True)
                                     elif datatype == 'dwi':
                                         item['modality'] = 'dwi'
-                                        df = df.append(item, ignore_index=True)
+                                        df = pd.concat([df, pd.DataFrame([item])], ignore_index=True)
                                     elif datatype == 'anat' and re.search('MSME', method, re.IGNORECASE):
                                         item['modality'] = 'MESE'
-                                        df = df.append(item, ignore_index=True)
+                                        df = pd.concat([df, pd.DataFrame([item])], ignore_index=True)
                                     else:
-                                        df = df.append(item, ignore_index=True)
+                                        df = pd.concat([df, pd.DataFrame([item])], ignore_index=True)
         if 'xlsx' in ds_format:
             df.to_excel(output, index=None)
         elif 'csv' in ds_format:
             df.to_csv(output, index=None, sep=',')
         elif 'tsv' in ds_format:
             df.to_csv(output, index=None, sep='\t')
         else:
@@ -486,14 +486,16 @@
         subj_id (str): the orignal subject id.
     Returns:
         str: the replaced subject id.
     """
 
     import warnings
 
+    subj_id = str(subj_id)
+    
     # underscore will mess up bids output
     if '_' in subj_id:
         subj_id = subj_id.replace('_', 'Underscore')
         # warn user that the subject/participantID has a '_' and is replaced with 'Underscore'
         warnings.warn('Participant or subject ID has "_"s, replaced with "Underscore" to make it bids compatiable. You should avoid use "_" in participant/subject ID for BIDS purpose')
 
     # Hyphen will mess up bids output
@@ -717,23 +719,23 @@
     else:
         return False
 
 
 def override_header(pvobj, subjtype, position):
     """override subject position and subject type"""
     import warnings
-    if position is not None:
+    if position != None:
         try:
             pvobj.override_position(position)
         except:
             msg = "Unknown position string [{}]. Please check your input option.".format(position) + \
                   "The position variable can be defiend as <BodyPart>_<Side>," + \
                   "available BodyParts are (Head, Foot, Tail) and sides are (Supine, Prone, Left, Right). (e.g. Head_Supine)"
             raise InvalidApproach(msg)
-    if subjtype is not None:
+    if subjtype != None:
         try:
             pvobj.override_subjtype(subjtype)
         except:
             msg = "Unknown subject type [{}]. Please check your input option.".format(subjtype) + \
                   "available options are (Biped, Quadruped, Phantom, Other, OtherAnimal)"
             raise InvalidApproach(msg)
     return pvobj
```

### Comparing `brkraw-0.3.8/brkraw/ui/main_win.py` & `brkraw-0.3.9/brkraw/ui/main_win.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/ui/previewer.py` & `brkraw-0.3.9/brkraw/ui/previewer.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/ui/scan_info.py` & `brkraw-0.3.9/brkraw/ui/scan_info.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/ui/scan_list.py` & `brkraw-0.3.9/brkraw/ui/scan_list.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw/ui/subj_info.py` & `brkraw-0.3.9/brkraw/ui/subj_info.py`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/brkraw.egg-info/PKG-INFO` & `brkraw-0.3.9/brkraw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brkraw
-Version: 0.3.8
+Version: 0.3.9
 Summary: Bruker PvDataset Loader
 Home-page: https://github.com/brkraw/brkraw
 Author: SungHo Lee
 Author-email: shlee@unc.edu
 License: GNLv3
 Keywords: bruker data_handler converter administrator_tool
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `brkraw-0.3.8/brkraw.egg-info/SOURCES.txt` & `brkraw-0.3.9/brkraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brkraw-0.3.8/setup.py` & `brkraw-0.3.9/setup.py`

 * *Files identical despite different names*

