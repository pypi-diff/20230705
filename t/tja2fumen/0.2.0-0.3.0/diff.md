# Comparing `tmp/tja2fumen-0.2.0.tar.gz` & `tmp/tja2fumen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.2.0.tar", last modified: Sat Jul  1 21:44:13 2023, max compression
+gzip compressed data, was "tja2fumen-0.3.0.tar", last modified: Wed Jul  5 20:10:18 2023, max compression
```

## Comparing `tja2fumen-0.2.0.tar` & `tja2fumen-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/
--rw-rw-rw-   0        0        0     1083 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/README.md
--rw-rw-rw-   0        0        0      897 2023-07-01 21:43:57.000000 tja2fumen-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.267272 tja2fumen-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.282905 tja2fumen-0.2.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     1597 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    15602 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    18892 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3308 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2905 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.282905 tja2fumen-0.2.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-05 20:10:07.000000 tja2fumen-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.470891 tja2fumen-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.486514 tja2fumen-0.3.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1825 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    15536 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19843 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.502142 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
+-rw-rw-rw-   0        0        0     3308 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2905 2023-07-05 20:09:12.000000 tja2fumen-0.3.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:10:18.486514 tja2fumen-0.3.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 20:10:18.000000 tja2fumen-0.3.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.2.0/LICENSE.txt` & `tja2fumen-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/PKG-INFO` & `tja2fumen-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.2.0/README.md` & `tja2fumen-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/pyproject.toml` & `tja2fumen-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.2.0"
+version = "0.3.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.2.0/src/tja2fumen/__init__.py` & `tja2fumen-0.3.0/src/tja2fumen/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,20 +29,25 @@
     # Convert TJA data to fumen data
     parsedSongsTJA = parseTJA(fnameTJA)
     parsedSongsFumen = {course: convertTJAToFumen(tjaData)
                         for course, tjaData in parsedSongsTJA.items()}
 
     # Generate output filenames
     baseName = os.path.splitext(fnameTJA)[0]
-    outputFilenames = [baseName + f"_{COURSE_IDS[course]}.bin" if len(parsedSongsTJA) > 1
-                       else baseName + ".bin"
-                       for course in parsedSongsFumen.keys()]
-
-    # Write fumen data to files
-    for fumenData, outputName in zip(parsedSongsFumen.values(), outputFilenames):
+    outputFilenames = []
+    for courseName, fumenData in parsedSongsFumen.items():
+        if len(parsedSongsTJA) == 1:
+            outputName = f"{baseName}.bin"
+        else:
+            splitName = courseName.split("P")  # e.g. 'OniP2' -> ['Oni', '2'], 'Oni' -> ['Oni']
+            outputName = f"{baseName}_{COURSE_IDS[splitName[0]]}"
+            if len(splitName) == 2:
+                outputName += f"_{splitName[1]}"  # Add "_1" or "_2" if P1/P2 chart
+            outputName += ".bin"
+        outputFilenames.append(outputName)
         writeFumen(outputName, fumenData)
 
     if return_vars:
         return parsedSongsTJA, parsedSongsFumen, outputFilenames
 
 
 # NB: This entry point is necessary for the Pyinstaller executable
```

### Comparing `tja2fumen-0.2.0/src/tja2fumen/constants.py` & `tja2fumen-0.3.0/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/converters.py` & `tja2fumen-0.3.0/src/tja2fumen/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,27 +133,25 @@
         currentDrumroll = None
         courseBalloons = tja['metadata']['balloon'].copy()
         for idx_m, measureTJA in enumerate(branch):
             measureFumen = tjaConverted['measures'][idx_m]
 
             # Check to see if the measure contains a branching condition
             if measureTJA['branchStart']:
-                measureFumen['branchStart'] = measureTJA['branchStart']
-            if measureFumen['branchStart']:
-                if measureFumen['branchStart'][0] == 'p':
+                if measureTJA['branchStart'][0] == 'p':
                     if currentBranch == 'normal':
                         idx_b1, idx_b2 = 0, 1
                     elif currentBranch == 'advanced':
                         idx_b1, idx_b2 = 2, 3
                     elif currentBranch == 'master':
                         idx_b1, idx_b2 = 4, 5
-                    measureFumen['branchInfo'][idx_b1] = int(total_notes_branch * measureFumen['branchStart'][1] * 20)
-                    measureFumen['branchInfo'][idx_b2] = int(total_notes_branch * measureFumen['branchStart'][2] * 20)
+                    measureFumen['branchInfo'][idx_b1] = int(total_notes_branch * measureTJA['branchStart'][1] * 20)
+                    measureFumen['branchInfo'][idx_b2] = int(total_notes_branch * measureTJA['branchStart'][2] * 20)
                 elif measureTJA['branchStart'][0] == 'r':
-                    pass
+                    measureFumen['branchInfo'] = measureTJA['branchStart'][1:] * 3
                 total_notes_branch = 0
             total_notes_branch += note_counter_branch
 
             # Compute the duration of the measure
             measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
             measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
             measureRatio = 1.0 if measureTJA['subdivisions'] == 0.0 else (measureLength / measureTJA['subdivisions'])
```

### Comparing `tja2fumen-0.2.0/src/tja2fumen/parsers.py` & `tja2fumen-0.3.0/src/tja2fumen/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+from copy import deepcopy
 
 from tja2fumen.utils import readStruct, getBool, shortHex
 from tja2fumen.constants import NORMALIZE_COURSE, TJA_NOTE_TYPES, branchNames, noteTypes
 
 
 ########################################################################################################################
 # TJA-parsing functions ( Original source: https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js)
@@ -23,14 +24,15 @@
 
     return courses
 
 
 def getCourseData(lines):
     courses = {}
     currentCourse = ''
+    currentCourseCached = ''
     songBPM = 0
     songOffset = 0
 
     for line in lines:
         # Case 1: Header metadata
         match_header = re.match(r"^([A-Z]+):(.*)", line)
         if match_header:
@@ -42,14 +44,15 @@
                 songBPM = value
             elif nameUpper == 'OFFSET':
                 songOffset = value
 
             # Course-specific header fields
             elif nameUpper == 'COURSE':
                 currentCourse = NORMALIZE_COURSE[value]
+                currentCourseCached = currentCourse
                 if currentCourse not in courses.keys():
                     courses[currentCourse] = {
                         'metadata': {'course': currentCourse, 'bpm': songBPM, 'offset': songOffset, 'level': 0,
                                      'balloon': [], 'scoreInit': 0, 'scoreDiff': 0},
                         'data': [],
                     }
             elif nameUpper == 'LEVEL':
@@ -58,159 +61,153 @@
                 courses[currentCourse]['metadata']['scoreInit'] = int(value) if value else 0
             elif nameUpper == 'SCOREDIFF':
                 courses[currentCourse]['metadata']['scoreDiff'] = int(value) if value else 0
             elif nameUpper == 'BALLOON':
                 if value:
                     balloons = [int(v) for v in value.split(",") if v]
                     courses[currentCourse]['metadata']['balloon'] = balloons
-            # STYLE is a P1/P2 command, which we don't support yet, so normally this would be a
-            # NotImplemetedError. However, TakoTako outputs `STYLE:SINGLE` when converting Ura
-            # charts, so throwing an error here would prevent Ura charts from being converted.
-            # See: https://github.com/vivaria/tja2fumen/issues/15#issuecomment-1575341088
             elif nameUpper == 'STYLE':
-                pass
+                # Reset the course name to remove "P1/P2" that may have been added by a previous STYLE:DOUBLE chart
+                if value == 'Single':
+                    currentCourse = currentCourseCached
             else:
                 pass  # Ignore other header fields such as 'TITLE', 'SUBTITLE', 'WAVE', etc.
 
         # Case 2: Commands and note data (to be further processed course-by-course later on)
         elif not re.match(r"//.*", line):  # Exclude comment-only lines ('//')
             match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
             match_notes = re.match(r"^(([0-9]|A|B|C|F|G)*,?).*$", line)
             if match_command:
                 nameUpper = match_command.group(1).upper()
                 value = match_command.group(2).strip() if match_command.group(2) else ''
+                # For STYLE:Double, #START P1/P2 indicates the start of a new chart
+                # But, we want multiplayer charts to inherit the metadata from the course as a whole, so we deepcopy
+                if nameUpper == "START" and value in ["P1", "P2"]:                   
+                    currentCourse = currentCourseCached + value
+                    courses[currentCourse] = deepcopy(courses[currentCourseCached])
+                    courses[currentCourse]['data'] = list()  # Keep the metadata, but reset the note data
+                    value = ''  # Once we've made the new course, we can reset this to a normal #START command
             elif match_notes:
                 nameUpper = 'NOTES'
                 value = match_notes.group(1)
             courses[currentCourse]['data'].append({"name": nameUpper, "value": value})
+            
+    # If a course has no song data, then this is likely because the course has "STYLE: Double" but no "STYLE: Single".
+    # To fix this, we copy over the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
+    for courseName, course in courses.items():
+        if not course['data']:
+            if courseName+"P1" in courses.keys():
+                courses[courseName] = deepcopy(courses[courseName+"P1"])
 
     return courses
 
 
 def parseCourseMeasures(lines):
     # Check if the course has branches or not
     hasBranches = True if [l for l in lines if l['name'] == 'BRANCHSTART'] else False
-    if hasBranches:
-        currentBranch = 'all'
-        targetBranch = 'all'
-    else:
-        currentBranch = 'normal'
-        targetBranch = 'normal'
+    currentBranch = 'all' if hasBranches else 'normal'
     flagLevelhold = False
 
     # Process course lines
-    branches = {'normal': [], 'advanced': [], 'master': []}
-    measureNotes = ''
-    measureEvents = []
+    idx_m = 0
+    idx_m_branchstart = 0
+    emptyMeasure = {'data': '', 'events': []}
+    branches = {'normal': [deepcopy(emptyMeasure)], 'advanced': [deepcopy(emptyMeasure)], 'master': [deepcopy(emptyMeasure)]}
     for line in lines:
         # 1. Parse measure notes
         if line['name'] == 'NOTES':
             notes = line['value']
-            # If measure has ended, then append the measure and start anew
+            # If measure has ended, then add notes to the current measure, then start a new one by incrementing idx_m
             if notes.endswith(','):
-                measureNotes += notes[0:-1]
-                measureCurrent = {
-                    "data": measureNotes,
-                    "events": measureEvents,
-                }
-                if currentBranch == 'all':
-                    for branch in branches.keys():
-                        branches[branch].append(measureCurrent)
-                else:
-                    branches[currentBranch].append(measureCurrent)
-                measureNotes = ''
-                measureEvents = []
-            # Otherwise, keep tracking measureNotes
+                for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
+                    branches[branch][idx_m]['data'] += notes[0:-1]
+                    branches[branch].append(deepcopy(emptyMeasure))
+                idx_m += 1
+            # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
-                measureNotes += notes
+                for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
+                    branches[branch][idx_m]['data'] += notes
 
-        # 2. Parse commands
-        else:
-            # Measure commands
+        # 2. Parse measure commands that produce an "event"
+        elif line['name'] in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF',
+                              'SCROLL', 'BPMCHANGE', 'MEASURE', 'BRANCHSTART']:
+            # Get position of the event
+            for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
+                pos = len(branches[branch][idx_m]['data'])
+
+            # Parse event type
             if line['name'] == 'GOGOSTART':
-                measureEvents.append({"name": 'gogo', "position": len(measureNotes), "value": '1'})
+                currentEvent = {"name": 'gogo', "position": pos, "value": '1'}
             elif line['name'] == 'GOGOEND':
-                measureEvents.append({"name": 'gogo', "position": len(measureNotes), "value": '0'})
+                currentEvent = {"name": 'gogo', "position": pos, "value": '0'}
             elif line['name'] == 'BARLINEON':
-                measureEvents.append({"name": 'barline', "position": len(measureNotes), "value": '1'})
+                currentEvent = {"name": 'barline', "position": pos, "value": '1'}
             elif line['name'] == 'BARLINEOFF':
-                measureEvents.append({"name": 'barline', "position": len(measureNotes), "value": '0'})
+                currentEvent = {"name": 'barline', "position": pos, "value": '0'}
             elif line['name'] == 'SCROLL':
-                measureEvents.append({"name": 'scroll', "position": len(measureNotes), "value": float(line['value'])})
+                currentEvent = {"name": 'scroll', "position": pos, "value": float(line['value'])}
             elif line['name'] == 'BPMCHANGE':
-                measureEvents.append({"name": 'bpm', "position": len(measureNotes), "value": float(line['value'])})
+                currentEvent = {"name": 'bpm', "position": pos, "value": float(line['value'])}
             elif line['name'] == 'MEASURE':
-                measureEvents.append({"name": 'measure', "position": len(measureNotes), "value": line['value']})
+                currentEvent = {"name": 'measure', "position": pos, "value": line['value']}
+            elif line["name"] == 'BRANCHSTART':
+                if flagLevelhold:
+                    continue
+                currentBranch = 'all'  # Ensure that the #BRANCHSTART command is present for all branches
+                values = line['value'].split(',')
+                if values[0] == 'r':  # r = drumRoll
+                    values[1] = int(values[1])  # # of drumrolls
+                    values[2] = int(values[2])  # # of drumrolls
+                elif values[0] == 'p':  # p = Percentage
+                    values[1] = float(values[1]) / 100  # %
+                    values[2] = float(values[2]) / 100  # %
+                currentEvent = {"name": 'branchStart', "position": pos, "value": values}
+                idx_m_branchstart = idx_m  # Preserve the index of the BRANCHSTART command to re-use for each branch
 
-            # Branch commands
-            elif line["name"] == 'START' or line['name'] == 'END':
-                if hasBranches:
-                    currentBranch = 'all'
-                    targetBranch = 'all'
-                else:
-                    currentBranch = 'normal'
-                    targetBranch = 'normal'
+            # Append event to the current measure's events
+            for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
+                branches[branch][idx_m]['events'].append(currentEvent)
+
+        # 3. Parse commands that don't create an event (e.g. simply changing the current branch)
+        else:
+            if line["name"] == 'START' or line['name'] == 'END':
+                currentBranch = 'all' if hasBranches else 'normal'
                 flagLevelhold = False
             elif line['name'] == 'LEVELHOLD':
                 flagLevelhold = True
             elif line["name"] == 'N':
                 currentBranch = 'normal'
+                idx_m = idx_m_branchstart
             elif line["name"] == 'E':
                 currentBranch = 'advanced'
+                idx_m = idx_m_branchstart
             elif line["name"] == 'M':
                 currentBranch = 'master'
+                idx_m = idx_m_branchstart
             elif line["name"] == 'BRANCHEND':
-                currentBranch = targetBranch
-            elif line["name"] == 'BRANCHSTART':
-                if flagLevelhold:
-                    continue
-                values = line['value'].split(',')
-                if values[0] == 'r':
-                    if len(values) >= 3:
-                        targetBranch = 'master'
-                    elif len(values) == 2:
-                        targetBranch = 'advanced'
-                    else:
-                        targetBranch = 'normal'
-                elif values[0] == 'p':  # p = percentage
-                    values[1] = float(values[1]) / 100  # %
-                    values[2] = float(values[2]) / 100  # %
-                    measureEvents.append({"name": 'branchStart', "position": len(measureNotes), "value": values})
-                    if len(values) >= 3 and float(values[2]) <= 100:
-                        targetBranch = 'master'
-                    elif len(values) >= 2 and float(values[1]) <= 100:
-                        targetBranch = 'advanced'
-                    else:
-                        targetBranch = 'normal'
+                currentBranch = 'all'
 
             # Ignored commands
             elif line['name'] == 'LYRIC':
                 pass
             elif line['name'] == 'NEXTSONG':
                 pass
 
             # Not implemented commands
             elif line['name'] == 'SECTION':
-                pass  # TODO: Implement
+                pass  # This seems to be inconsequential, but I'm not 100% sure. Need to test more branching fumens.
             elif line['name'] == 'DELAY':
                 raise NotImplementedError
             else:
                 raise NotImplementedError
 
-    # If there is measure data (i.e. the file doesn't end on a "measure end" symbol ','), append whatever is left
-    if measureNotes:
-        branches[currentBranch].append({
-            "data": measureNotes,
-            "events": measureEvents,
-        })
-    # Otherwise, if the file ends on a measure event (e.g. #GOGOEND), append any remaining events
-    elif measureEvents:
-        for event in measureEvents:
-            event['position'] = len(branches[len(branches) - 1]['data'])
-            branches[currentBranch][len(branches[currentBranch]) - 1]['events'].append(event)
+    # Delete the last measure in the branch if no notes or events were added to it (due to preallocating empty measures)
+    for branch in branches.values():
+        if not branch[-1]['data'] and not branch[-1]['events']:
+            del branch[-1]
 
     # Merge measure data and measure events in chronological order
     for branchName, branch in branches.items():
         for measure in branch:
             notes = [{'pos': i, 'type': 'note', 'value': TJA_NOTE_TYPES[note]}
                      for i, note in enumerate(measure['data']) if note != '0']
             events = [{'pos': e['position'], 'type': e['name'], 'value': e['value']}
```

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.3.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/utils.py` & `tja2fumen-0.3.0/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen/writers.py` & `tja2fumen-0.3.0/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.2.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.3.0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.2.0/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.3.0/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

