# Comparing `tmp/psychopy-phidgets-0.1.2.tar.gz` & `tmp/psychopy-phidgets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy-phidgets-0.1.2.tar", last modified: Sat Jan  7 23:29:50 2023, max compression
+gzip compressed data, was "dist\psychopy-phidgets-0.2.1.tar", last modified: Wed Jul  5 21:03:16 2023, max compression
```

## Comparing `psychopy-phidgets-0.1.2.tar` & `psychopy-phidgets-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.242199 psychopy-phidgets-0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-01-07 04:09:42.000000 psychopy-phidgets-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      211 2023-01-07 05:12:31.000000 psychopy-phidgets-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      482 2023-01-07 23:29:50.242199 psychopy-phidgets-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-01-07 04:23:08.000000 psychopy-phidgets-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.215270 psychopy-phidgets-0.1.2/psychopy_phidgets/
--rw-rw-rw-   0        0        0        0 2023-01-07 05:09:44.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.206296 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.206296 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.228297 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/
--rw-rw-rw-   0        0        0        0 2023-01-07 06:01:44.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.231229 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/classic/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/classic/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/classic/phidgets@2x.png
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.234219 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/dark/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/dark/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/dark/phidgets@2x.png
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.237211 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/light/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/light/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/light/phidgets@2x.png
--rw-rw-rw-   0        0        0     6408 2023-01-07 22:01:06.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/phidgets.py
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.240203 psychopy-phidgets-0.1.2/psychopy_phidgets/hardware/
--rw-rw-rw-   0        0        0        0 2023-01-07 04:57:59.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/hardware/__init__.py
--rw-rw-rw-   0        0        0     2726 2023-01-07 21:32:46.000000 psychopy-phidgets-0.1.2/psychopy_phidgets/hardware/phidgets.py
-drwxrwxrwx   0        0        0        0 2023-01-07 23:29:50.225243 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/
--rw-rw-rw-   0        0        0      482 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      242 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-07 04:39:59.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-07 23:29:50.000000 psychopy-phidgets-0.1.2/psychopy_phidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-07 23:29:50.243196 psychopy-phidgets-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-01-07 23:29:26.000000 psychopy-phidgets-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-07 04:09:42.000000 psychopy-phidgets-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      211 2023-01-07 05:12:31.000000 psychopy-phidgets-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      482 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-01-07 04:23:08.000000 psychopy-phidgets-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.130927 psychopy-phidgets-0.2.1/psychopy_phidgets/
+-rw-rw-rw-   0        0        0      101 2023-07-05 20:38:09.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.138906 psychopy-phidgets-0.2.1/psychopy_phidgets/component/
+-rw-rw-rw-   0        0        0        0 2023-01-07 06:01:44.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/component/__init__.py
+-rw-rw-rw-   0        0        0     6423 2023-07-05 20:54:04.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/component/phidgets.py
+-rw-rw-rw-   0        0        0     2726 2023-01-07 21:32:46.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/phidgets.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.137909 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      184 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-01-07 04:39:59.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2023-07-05 20:58:16.000000 psychopy-phidgets-0.2.1/setup.py
```

### Comparing `psychopy-phidgets-0.1.2/LICENSE` & `psychopy-phidgets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.1.2/psychopy_phidgets/experiment/components/phidgets/phidgets.py` & `psychopy-phidgets-0.2.1/psychopy_phidgets/component/phidgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             startType=startType, startVal=startVal,
             stopType=stopType, stopVal=stopVal,
             startEstim=startEstim, durationEstim=durationEstim)
 
         self.type = 'PhidgetRelay'
         self.url = 'https://www.psychopy.org/builder/components/phidget.html'
 
-        self.exp.requireImport(importName='phidgets',
+        self.exp.requireImport(importName='PhidgetOutputComponent',
                                importFrom='psychopy.hardware')
 
         # Order in which the user-settable parameters will be displayed
         # in the component's properties window.
         self.order += ['syncToScreen',  # Basic tab
                         'channelList', 'serialNumber', 'reversedRelay', # Hardware tab
                       ]
@@ -79,16 +79,16 @@
         self.params['syncToScreen'] = Param(
             syncToScreen, valType='bool', inputType="bool", categ='Basic',
             allowedVals=[True, False],
             hint=_translate('Sync relay events to the screen refresh'),
             label=_localized['syncToScreen'])
 
     def writeRunOnceInitCode(self, buff):
-        code = ('# Initialize relays\n'
-                '%(name)s = phidgets.PhidgetOutputComponent(channelList = %(channelList)s, '
+        code = ('# Initialize relays LALALALAL\n'
+                '%(name)s = PhidgetOutputComponent(channelList = %(channelList)s, '
                                                            'serialNumber = %(serialNumber)s, '
                                                            'reversedRelay = %(reversedRelay)s)\n'
                 % self.params )
         buff.writeOnceIndentedLines(code)
 
     def writeRoutineStartCode(self, buff):
         """Write the code that will be called at the start of the routine.
```

### Comparing `psychopy-phidgets-0.1.2/psychopy_phidgets/hardware/phidgets.py` & `psychopy-phidgets-0.2.1/psychopy_phidgets/phidgets.py`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.1.2/setup.py` & `psychopy-phidgets-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(name='psychopy-phidgets',
-    version='0.1.2',
+    version='0.2.1',
     description='Psychopy plugin providing support for Phidgets',
     long_description='',
     url='https://github.com/maqadri/psychopy-phidgets',
     author='Muhammad A. J. Qadri',
     author_email='mqadri@holycross.edu',
     license='GPL3',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3'
     ],
     keywords='psychopy phidgets',
     packages=['psychopy_phidgets',
-              'psychopy_phidgets.hardware',
-              'psychopy_phidgets.experiment.components.phidgets',
-              'psychopy_phidgets.experiment.components.phidgets.light',
-              'psychopy_phidgets.experiment.components.phidgets.dark',
-              'psychopy_phidgets.experiment.components.phidgets.classic'],
+              'psychopy_phidgets.component',
+              'psychopy_phidgets.component.light',
+              'psychopy_phidgets.component.dark',
+              'psychopy_phidgets.component.classic'],
     install_requires=['psychopy'],
     include_package_data=True,
     entry_points={
-        'psychopy.hardware': ['PhidgetOutputComponent = psychopy_phidgets.hardware.phidgets:PhidgetOutputComponent'],
-        'psychopy.experiment.components': ['PhidgetRelayComponent = psychopy_phidgets.experiment.components.phidgets.phidgets:PhidgetRelayComponent']
+        'psychopy.hardware': ['PhidgetOutputComponent = psychopy_phidgets:PhidgetOutputComponent'],
+        'psychopy.experiment.components': ['PhidgetRelayComponent = psychopy_phidgets:PhidgetRelayComponent']
     },
     zip_safe=False)
```

