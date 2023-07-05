# Comparing `tmp/np_nwb-0.1.1.tar.gz` & `tmp/np_nwb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_nwb-0.1.1.tar", last modified: Sat Jun  3 02:21:59 2023, max compression
+gzip compressed data, was "np_nwb-0.1.2.tar", last modified: Wed Jul  5 20:05:34 2023, max compression
```

## Comparing `np_nwb-0.1.1.tar` & `np_nwb-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 02:21:59.754120 np_nwb-0.1.1/
--rw-rw-rw-   0        0        0     3115 2023-06-03 02:21:59.753118 np_nwb-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2722 2023-06-03 01:48:55.000000 np_nwb-0.1.1/README.md
--rw-rw-rw-   0        0        0      782 2023-06-03 02:21:46.000000 np_nwb-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 02:21:59.754120 np_nwb-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 02:21:59.682783 np_nwb-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 02:21:59.698907 np_nwb-0.1.1/src/np_nwb/
--rw-rw-rw-   0        0        0        0 2023-06-02 21:15:02.000000 np_nwb-0.1.1/src/np_nwb/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-02 21:15:30.000000 np_nwb-0.1.1/src/np_nwb/dynamic_routing_dev.py
-drwxrwxrwx   0        0        0        0 2023-06-03 02:21:59.750118 np_nwb-0.1.1/src/np_nwb/init_with_metadata/
--rw-rw-rw-   0        0        0      201 2023-06-03 02:09:37.000000 np_nwb-0.1.1/src/np_nwb/init_with_metadata/__init__.py
--rw-rw-rw-   0        0        0      142 2023-06-03 02:09:26.000000 np_nwb-0.1.1/src/np_nwb/init_with_metadata/__main__.py
--rw-rw-rw-   0        0        0     3025 2023-06-03 02:16:35.000000 np_nwb-0.1.1/src/np_nwb/init_with_metadata/from_np_session.py
--rw-rw-rw-   0        0        0      890 2023-06-03 01:48:24.000000 np_nwb-0.1.1/src/np_nwb/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 02:21:59.731995 np_nwb-0.1.1/src/np_nwb.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-06-03 02:21:59.000000 np_nwb-0.1.1/src/np_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-06-03 02:21:59.000000 np_nwb-0.1.1/src/np_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 02:21:59.000000 np_nwb-0.1.1/src/np_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-03 02:21:59.000000 np_nwb-0.1.1/src/np_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 02:21:59.000000 np_nwb-0.1.1/src/np_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.176058 np_nwb-0.1.2/
+-rw-rw-rw-   0        0        0     2356 2023-07-05 20:05:34.175058 np_nwb-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-06-27 18:22:47.000000 np_nwb-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1786 2023-07-05 20:05:19.000000 np_nwb-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:05:34.177057 np_nwb-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.027058 np_nwb-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.052055 np_nwb-0.1.2/src/np_nwb/
+-rw-rw-rw-   0        0        0       84 2023-07-04 21:03:07.000000 np_nwb-0.1.2/src/np_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.103057 np_nwb-0.1.2/src/np_nwb/database/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:14:08.000000 np_nwb-0.1.2/src/np_nwb/database/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-07-04 22:02:17.000000 np_nwb-0.1.2/src/np_nwb/database/base.py
+-rw-rw-rw-   0        0        0     7577 2023-07-04 21:54:33.000000 np_nwb-0.1.2/src/np_nwb/database/json_db.py
+-rw-rw-rw-   0        0        0     9500 2023-07-04 21:39:49.000000 np_nwb-0.1.2/src/np_nwb/database/validated.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.109058 np_nwb-0.1.2/src/np_nwb/dynamic_routing/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:14:08.000000 np_nwb-0.1.2/src/np_nwb/dynamic_routing/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-06-08 22:26:50.000000 np_nwb-0.1.2/src/np_nwb/dynamic_routing/licks.py
+-rw-rw-rw-   0        0        0     7226 2023-07-01 17:26:44.000000 np_nwb-0.1.2/src/np_nwb/dynamic_routing/running.py
+-rw-rw-rw-   0        0        0      854 2023-06-08 03:14:33.000000 np_nwb-0.1.2/src/np_nwb/dynamic_routing/utils.py
+-rw-rw-rw-   0        0        0    12411 2023-06-23 04:29:41.000000 np_nwb-0.1.2/src/np_nwb/ephys_utils.py
+-rw-rw-rw-   0        0        0      608 2023-06-07 21:40:33.000000 np_nwb-0.1.2/src/np_nwb/interfaces.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.114058 np_nwb-0.1.2/src/np_nwb/metadata/
+-rw-rw-rw-   0        0        0      202 2023-06-07 21:40:33.000000 np_nwb-0.1.2/src/np_nwb/metadata/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-06-07 21:40:33.000000 np_nwb-0.1.2/src/np_nwb/metadata/__main__.py
+-rw-rw-rw-   0        0        0     2502 2023-06-07 21:40:34.000000 np_nwb-0.1.2/src/np_nwb/metadata/from_np_session.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.131057 np_nwb-0.1.2/src/np_nwb/scripts/
+-rw-rw-rw-   0        0        0        0 2023-06-07 01:03:10.000000 np_nwb-0.1.2/src/np_nwb/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5732 2023-07-04 20:52:54.000000 np_nwb-0.1.2/src/np_nwb/scripts/generate_dynamic_routing_pilot_ecephys.py
+-rw-rw-rw-   0        0        0     1948 2023-07-02 02:37:06.000000 np_nwb-0.1.2/src/np_nwb/scripts/generate_sound_latencies.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.170058 np_nwb-0.1.2/src/np_nwb/trials/
+-rw-rw-rw-   0        0        0    22571 2023-07-05 17:13:21.000000 np_nwb-0.1.2/src/np_nwb/trials/DRtask.py
+-rw-rw-rw-   0        0        0    11229 2023-07-04 03:22:43.000000 np_nwb-0.1.2/src/np_nwb/trials/RFtrials.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 21:15:02.000000 np_nwb-0.1.2/src/np_nwb/trials/__init__.py
+-rw-rw-rw-   0        0        0     6956 2023-07-04 00:45:40.000000 np_nwb-0.1.2/src/np_nwb/trials/property_dict.py
+-rw-rw-rw-   0        0        0    39807 2023-07-01 20:35:03.000000 np_nwb-0.1.2/src/np_nwb/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.173058 np_nwb-0.1.2/src/np_nwb/videos/
+-rw-rw-rw-   0        0        0        0 2023-06-02 21:15:02.000000 np_nwb-0.1.2/src/np_nwb/videos/__init__.py
+-rw-rw-rw-   0        0        0     2676 2023-06-20 16:28:02.000000 np_nwb-0.1.2/src/np_nwb/videos/videos.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:05:34.085058 np_nwb-0.1.2/src/np_nwb.egg-info/
+-rw-rw-rw-   0        0        0     2356 2023-07-05 20:05:33.000000 np_nwb-0.1.2/src/np_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-07-05 20:05:34.000000 np_nwb-0.1.2/src/np_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:05:33.000000 np_nwb-0.1.2/src/np_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      380 2023-07-05 20:05:33.000000 np_nwb-0.1.2/src/np_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 20:05:33.000000 np_nwb-0.1.2/src/np_nwb.egg-info/top_level.txt
```

### Comparing `np_nwb-0.1.1/PKG-INFO` & `np_nwb-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: np_nwb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
 Author-email: arjunsridhar12345 <arjun.sridhar@alleninstitute.org>, bjhardcastle <ben.hardcastle@alleninstitute.org>, mochic <chrism@alleninstitute.org>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-
-# np_nwb
-Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
+Provides-Extra: db
+Provides-Extra: packaging
+Provides-Extra: offsite
+Provides-Extra: onsite
+Provides-Extra: dev
 
 # np_nwb
 Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
 
 Generating an `.nwb` file will entail:
 - inputting a path to a folder of raw data from a single experiment (`session_folder`)
 - creating an instance of `pynwb.NWBFile` and writing to disk (`nwb_file`)
@@ -21,68 +23,45 @@
   - accept or load an instance of `pynwb.NWBFile` from `nwb_file`
   - recognize the type of experiment contained in `session_folder` 
   - process raw data in `session_folder` accordingly
   - append tables to the `pynwb.NWBFile` instance
   - optionally write to disk
   - return the `pynwb.NWBFile` instance
 
-Each module should therefore provide **a single function or method** which
-implements the following `append()` interface:
+Each module should therefore provide a function implementing the following `append()` interface:
 
 ```python
 import logging
 import pathlib
 import tempfile
 from typing import Optional
 
+import np_tools
 import pynwb
 
 logger = logging.getLogger(__name__)
 
 
 def append(
     session_folder: str | pathlib.Path,
     nwb_file: str | pathlib.Path | pynwb.NWBFile,
     output_file: Optional[str | pathlib.Path] = None,
     ) -> pynwb.NWBFile:
     """Append one or more new components to an `.nwb` file.
 
-    - callable from within a Python process, by accepting & returning instances of `pynwb.  NWBFile` 
+    - callable from within a Python process, by accepting & returning instances of `pynwb.NWBFile` 
     - callable from the command line, in which case all three input arguments are required, with `nwb_file` specified as a path
     """
     session_folder = pathlib.Path(session_folder)
 
     # ... process session_folder
 
     if not isinstance(nwb_file, pynwb.NWBFile):
-        nwb_file = load_nwb_from_disk(nwb_file) 
+        nwb_file = np_tools.load_nwb(nwb_file) 
     
     # ... append new components to nwb_file
 
     if output_file is not None:
-        write_nwb_to_disk(nwb_file, output_file)
+        np_tools.save_nwb(nwb_file, output_file)
     
     return nwb_file
-
-
-def load_nwb_from_disk(
-    nwb_path: str | pathlib.Path,
-    ) -> pynwb.NWBFile:
-    logger.info(f'Loading nwb file at {nwb_path}')
-    with pynwb.NWBHDF5IO(nwb_path, mode='r') as f:
-        return f.read()
-
-
-def write_nwb_to_disk(
-    nwb_file: pynwb.NWBFile, output_path: Optional[str | pathlib.Path] = None
-    ) -> None:
-    if output_path is None:
-        output_path = pathlib.Path(tempfile.mkdtemp()) / f'{nwb_file.session_id}.nwb'
-    
-    nwb_file.set_modified()
-
-    logger.info(f'Writing nwb file `{nwb_file.session_id!r}` to {output_path}')
-    with pynwb.NWBHDF5IO(output_path, mode='w') as f:
-        f.write(nwb_file, cache_spec=True)
-    logger.debug(f'Writing complete for nwb file `{nwb_file.session_id!r}`')
-  
 ```
```

### Comparing `np_nwb-0.1.1/README.md` & `np_nwb-0.1.2/src/np_nwb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,20 @@
-# np_nwb
-Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
+Metadata-Version: 2.1
+Name: np-nwb
+Version: 0.1.2
+Summary: Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
+Author-email: arjunsridhar12345 <arjun.sridhar@alleninstitute.org>, bjhardcastle <ben.hardcastle@alleninstitute.org>, mochic <chrism@alleninstitute.org>
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: db
+Provides-Extra: packaging
+Provides-Extra: offsite
+Provides-Extra: onsite
+Provides-Extra: dev
 
 # np_nwb
 Tools for quickly generating `.nwb` files from non-standard Mindscope Neuropixels experiments.
 
 Generating an `.nwb` file will entail:
 - inputting a path to a folder of raw data from a single experiment (`session_folder`)
 - creating an instance of `pynwb.NWBFile` and writing to disk (`nwb_file`)
@@ -12,68 +23,45 @@
   - accept or load an instance of `pynwb.NWBFile` from `nwb_file`
   - recognize the type of experiment contained in `session_folder` 
   - process raw data in `session_folder` accordingly
   - append tables to the `pynwb.NWBFile` instance
   - optionally write to disk
   - return the `pynwb.NWBFile` instance
 
-Each module should therefore provide **a single function or method** which
-implements the following `append()` interface:
+Each module should therefore provide a function implementing the following `append()` interface:
 
 ```python
 import logging
 import pathlib
 import tempfile
 from typing import Optional
 
+import np_tools
 import pynwb
 
 logger = logging.getLogger(__name__)
 
 
 def append(
     session_folder: str | pathlib.Path,
     nwb_file: str | pathlib.Path | pynwb.NWBFile,
     output_file: Optional[str | pathlib.Path] = None,
     ) -> pynwb.NWBFile:
     """Append one or more new components to an `.nwb` file.
 
-    - callable from within a Python process, by accepting & returning instances of `pynwb.  NWBFile` 
+    - callable from within a Python process, by accepting & returning instances of `pynwb.NWBFile` 
     - callable from the command line, in which case all three input arguments are required, with `nwb_file` specified as a path
     """
     session_folder = pathlib.Path(session_folder)
 
     # ... process session_folder
 
     if not isinstance(nwb_file, pynwb.NWBFile):
-        nwb_file = load_nwb_from_disk(nwb_file) 
+        nwb_file = np_tools.load_nwb(nwb_file) 
     
     # ... append new components to nwb_file
 
     if output_file is not None:
-        write_nwb_to_disk(nwb_file, output_file)
+        np_tools.save_nwb(nwb_file, output_file)
     
     return nwb_file
-
-
-def load_nwb_from_disk(
-    nwb_path: str | pathlib.Path,
-    ) -> pynwb.NWBFile:
-    logger.info(f'Loading nwb file at {nwb_path}')
-    with pynwb.NWBHDF5IO(nwb_path, mode='r') as f:
-        return f.read()
-
-
-def write_nwb_to_disk(
-    nwb_file: pynwb.NWBFile, output_path: Optional[str | pathlib.Path] = None
-    ) -> None:
-    if output_path is None:
-        output_path = pathlib.Path(tempfile.mkdtemp()) / f'{nwb_file.session_id}.nwb'
-    
-    nwb_file.set_modified()
-
-    logger.info(f'Writing nwb file `{nwb_file.session_id!r}` to {output_path}')
-    with pynwb.NWBHDF5IO(output_path, mode='w') as f:
-        f.write(nwb_file, cache_spec=True)
-    logger.debug(f'Writing complete for nwb file `{nwb_file.session_id!r}`')
-  
 ```
```

