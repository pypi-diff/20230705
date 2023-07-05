# Comparing `tmp/pqinput-0.0.406.tar.gz` & `tmp/pqinput-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.406.tar", last modified: Wed Jul  5 08:31:15 2023, max compression
+gzip compressed data, was "pqinput-0.0.5.tar", last modified: Mon Jul  3 16:40:09 2023, max compression
```

## Comparing `pqinput-0.0.406.tar` & `pqinput-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-05 08:31:15.106921 pqinput-0.0.406/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.406/LICENSE.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-07-05 08:31:15.106921 pqinput-0.0.406/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.406/README.md
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-05 08:31:15.106921 pqinput-0.0.406/pqinput/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.406/pqinput/__init__.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     8712 2023-07-04 11:39:11.000000 pqinput-0.0.406/pqinput/drawPES.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)    15674 2023-07-04 11:57:23.000000 pqinput-0.0.406/pqinput/inpxml.py
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-05 08:31:15.106921 pqinput-0.0.406/pqinput.egg-info/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-07-05 08:31:15.000000 pqinput-0.0.406/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      226 2023-07-05 08:31:15.000000 pqinput-0.0.406/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-05 08:31:15.000000 pqinput-0.0.406/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-07-05 08:31:15.000000 pqinput-0.0.406/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      542 2023-07-05 08:24:40.000000 pqinput-0.0.406/pyproject.toml
--rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-05 08:31:15.106921 pqinput-0.0.406/setup.cfg
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      653 2023-07-05 08:24:54.000000 pqinput-0.0.406/setup.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.5/LICENSE.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.408741 pqinput-0.0.5/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.5/README.md
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      134 2023-05-03 12:56:50.000000 pqinput-0.0.5/pqinput/__init__ (conflicted copy 2023-05-03 145650).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.5/pqinput/__init__.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     8672 2023-05-11 13:17:09.000000 pqinput-0.0.5/pqinput/drawPES.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    12777 2023-05-03 14:39:36.000000 pqinput-0.0.5/pqinput/inpxml (conflicted copy 2023-05-03 163936).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    15598 2023-07-03 16:30:51.000000 pqinput-0.0.5/pqinput/inpxml.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput.egg-info/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      336 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      540 2023-07-03 16:39:30.000000 pqinput-0.0.5/pyproject.toml
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-03 16:40:09.408741 pqinput-0.0.5/setup.cfg
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      651 2023-07-03 16:39:40.000000 pqinput-0.0.5/setup.py
```

### Comparing `pqinput-0.0.406/LICENSE.txt` & `pqinput-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.406/PKG-INFO` & `pqinput-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.406
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.406/README.md` & `pqinput-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.406/pqinput/drawPES.py` & `pqinput-0.0.5/pqinput/drawPES.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     except:
         c = color
     c = np.array(colorsys.rgb_to_hls(*mc.to_rgb(c)))
     return colorsys.hls_to_rgb(c[0],1-amount * (1-c[1]),c[2])
 
 def plotPES(inxstc, savename=None, SIunits=True, yrange=None, xrange=None, 
 legend=None, showfig=None, showWF=True, offset_overlap=0.5, sizex=12/2.54, sizey=8/2.54,
-title=None, offsetlabel=None, drawpure=True): # inx structure
+title=None, offsetlabel=None): # inx structure
     
     
     fig, ax = plt.subplots(layout='constrained', figsize=(sizex, sizey))
     plt.rcParams.update({'font.size': 10})
     
     cmap = plt.get_cmap("tab10")
     potmin = 0
@@ -93,15 +93,15 @@
                 dim = meta['dim'][0]
                 x = np.linspace(dim.xmin, dim.xmax, dim.size)
                 
             '''PES plotting, if there is a offset (photon energy) the line is dashed'''
             ################# main plot #################
             ax.plot(x, Pot*(HEeV if SIunits else 1), 
                     color=(cmap(j) if not offset else lighter(cmap(j),.5) ), 
-                    linestyle=('-' if not offset else ' ' if not drawpure else '--') ,
+                    linestyle=('-' if not offset else '--') ,
             # label=(re.findall('([\d]+)', element.tag)[0] if not offset else '_nolegend_') )
             label=(element.get('label') if not offset else '_nolegend_') )
     
             '''If the state PES has a photonic contribution'''
             if offset: 
                 homega = float(offset)*HEeV/sec2au*f2En
```

### Comparing `pqinput-0.0.406/pqinput/inpxml.py` & `pqinput-0.0.5/pqinput/inpxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,31 +266,30 @@
                     # if 'heir' in  mel.keys():
                     #     for ind in range(len(mel['heir'])):
                     #         branch.append( self.dict2ope(mel['heir'][ind])) 
         self._hamiltonian = Hel            
         
     # %% 
     ''' Propagator '''
-    def propagation(self, name, hamilt_params, attrib=None):
+    def propagation(self, name, hamilt_params):
         """ Method for the wavefunction propagation. Return a etree.SubElement of previous defined program.
         
         Args:
             name (string) name of the propagation method:
-                *GSPO, Cheby, *SIL, Arnoldi (*not defined yet)
+                *GSPO, Cheby, *SIL, *Arnoldi (*not defined yet)
             hamilt_params (dict) parameters dictionary for the required Cheby hamiltonian
             _format: {'type':hamiltonian type, 'Matrix_elems':[mij, ]} 
             _type in ('Sum', 'Multistate', )
             _matrix elements for multistate, see hamilt_elem() function for format
             
         """
-        # Propagator
-        if name in ['Cheby', 'Arnoldi']:# requires hamiltonian
+        # Chebychev propagator
+        if name == 'Cheby':# requires hamiltonian
             # create the propagator subelement of the program
-            self._propagation = et.SubElement(self._program, 'propagator', name=name,
-                                              attrib=attrib)
+            self._propagation = et.SubElement(self._program, 'propagator', name=name)
             self.def_hamiltonian(hamilt_params)
             # define hamiltonian 
             self._wavefunction.set('states', str(self.states))
             # change wavefunction states based on hamiltonian matrix
         else:
             raise SyntaxError('Propagator type not defined.')
         # others propagators
```

### Comparing `pqinput-0.0.406/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.5/pqinput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.406
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.406/pyproject.toml` & `pqinput-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.406"
+version = "0.0.5"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.406/setup.py` & `pqinput-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.406",
+    version = "0.0.5",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

