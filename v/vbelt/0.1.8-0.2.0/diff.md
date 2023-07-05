# Comparing `tmp/vbelt-0.1.8.tar.gz` & `tmp/vbelt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbelt-0.1.8.tar", last modified: Thu Mar  9 16:21:03 2023, max compression
+gzip compressed data, was "vbelt-0.2.0.tar", last modified: Wed Jul  5 08:35:59 2023, max compression
```

## Comparing `vbelt-0.1.8.tar` & `vbelt-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:21:03.261433 vbelt-0.1.8/
--rw-r--r--   0 theo      (1000) theo      (1000)    35095 2023-02-14 12:56:15.000000 vbelt-0.1.8/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-03-09 16:21:03.261433 vbelt-0.1.8/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)     1200 2023-02-14 12:50:17.000000 vbelt-0.1.8/README.md
--rw-r--r--   0 theo      (1000) theo      (1000)      968 2023-03-09 16:21:03.261433 vbelt-0.1.8/setup.cfg
--rwxr-x---   0 theo      (1000) theo      (1000)       62 2022-09-01 08:01:08.000000 vbelt-0.1.8/setup.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:21:03.261433 vbelt-0.1.8/vbelt/
--rw-r--r--   0 theo      (1000) theo      (1000)      759 2023-02-23 09:54:24.000000 vbelt-0.1.8/vbelt/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     6218 2023-02-14 12:57:55.000000 vbelt-0.1.8/vbelt/charge_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1907 2023-02-14 12:57:07.000000 vbelt-0.1.8/vbelt/forces.py
--rw-rw----   0 theo      (1000) theo      (1000)     9564 2023-02-14 12:57:09.000000 vbelt-0.1.8/vbelt/gencalc.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1407 2023-02-14 12:57:12.000000 vbelt-0.1.8/vbelt/incar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     4641 2023-02-14 12:57:17.000000 vbelt-0.1.8/vbelt/jobtool.py
--rw-r--r--   0 theo      (1000) theo      (1000)     3001 2023-02-14 12:57:18.000000 vbelt-0.1.8/vbelt/misc.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1661 2023-02-23 10:34:40.000000 vbelt-0.1.8/vbelt/outcar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     4238 2023-02-14 12:57:24.000000 vbelt-0.1.8/vbelt/outcar_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)    10528 2023-02-14 12:57:27.000000 vbelt-0.1.8/vbelt/poscar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9902 2023-02-14 12:57:38.000000 vbelt-0.1.8/vbelt/poscartool.py
--rw-r--r--   0 theo      (1000) theo      (1000)     2168 2023-02-14 12:57:40.000000 vbelt-0.1.8/vbelt/potcar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9953 2023-02-14 12:32:28.000000 vbelt-0.1.8/vbelt/script_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9273 2023-02-23 10:34:20.000000 vbelt-0.1.8/vbelt/wrapper.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:21:03.261433 vbelt-0.1.8/vbelt.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      460 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)      301 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/entry_points.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       64 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/requires.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        6 2023-03-09 16:21:03.000000 vbelt-0.1.8/vbelt.egg-info/top_level.txt
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/
+-rw-r--r--   0 theo      (1000) theo      (1000)    35095 2023-02-14 12:56:15.000000 vbelt-0.2.0/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 08:35:59.653610 vbelt-0.2.0/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)     1200 2023-07-05 08:35:00.000000 vbelt-0.2.0/README.md
+-rw-r--r--   0 theo      (1000) theo      (1000)      968 2023-07-05 08:35:59.653610 vbelt-0.2.0/setup.cfg
+-rwxr-xr-x   0 theo      (1000) theo      (1000)       62 2023-07-05 08:28:11.000000 vbelt-0.2.0/setup.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/vbelt/
+-rw-r--r--   0 theo      (1000) theo      (1000)      759 2023-07-05 08:29:28.000000 vbelt-0.2.0/vbelt/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     6257 2023-03-16 14:19:00.000000 vbelt-0.2.0/vbelt/charge_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1907 2023-02-14 12:57:07.000000 vbelt-0.2.0/vbelt/forces.py
+-rw-rw----   0 theo      (1000) theo      (1000)     9652 2023-07-05 08:32:43.000000 vbelt-0.2.0/vbelt/gencalc.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1407 2023-02-14 12:57:12.000000 vbelt-0.2.0/vbelt/incar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     4641 2023-02-14 12:57:17.000000 vbelt-0.2.0/vbelt/jobtool.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3076 2023-03-17 14:30:03.000000 vbelt-0.2.0/vbelt/misc.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1661 2023-02-23 10:34:40.000000 vbelt-0.2.0/vbelt/outcar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     4238 2023-02-14 12:57:24.000000 vbelt-0.2.0/vbelt/outcar_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     9505 2023-07-05 08:14:09.000000 vbelt-0.2.0/vbelt/poscar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    10361 2023-07-05 08:18:21.000000 vbelt-0.2.0/vbelt/poscartool.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     2168 2023-02-14 12:57:40.000000 vbelt-0.2.0/vbelt/potcar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    12579 2023-07-05 08:26:41.000000 vbelt-0.2.0/vbelt/script_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     9611 2023-03-17 14:30:26.000000 vbelt-0.2.0/vbelt/wrapper.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/vbelt.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      460 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)      301 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/entry_points.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       64 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/requires.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        6 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/top_level.txt
```

### Comparing `vbelt-0.1.8/LICENSE` & `vbelt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/PKG-INFO` & `vbelt-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbelt
-Version: 0.1.8
+Version: 0.2.0
 Summary: The VASP user tool belt.
 Home-page: https://git.sr.ht/~lattay/vbelt
 Author: Théo Cavignac
 Author-email: theo.cavignac@gmail.com
 License: GPL License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `vbelt-0.1.8/README.md` & `vbelt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/setup.cfg` & `vbelt-0.2.0/setup.cfg`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 gencalc = 
 	tc-pysh>=0.2.0
 	chevron >= 0.14.0
 	ase >= 3.22
 
 [options.entry_points]
 console_scripts = 
-	chgx=vbelt.wrapper:charge_extract
 	chgsum=vbelt.wrapper:charge_combine
-	ckforces=vbelt.wrapper:check_forces
-	ckend=vbelt.wrapper:check_end
+	chgx=vbelt.wrapper:charge_extract
 	ckconv=vbelt.wrapper:check_conv
-	termdos=vbelt.wrapper:termdos
-	poscartool=vbelt.poscartool:poscartool
+	ckend=vbelt.wrapper:check_end
+	ckforces=vbelt.wrapper:check_forces
 	jobtool=vbelt.jobtool:jobtool
+	poscartool=vbelt.poscartool:poscartool
+	termdos=vbelt.wrapper:termdos
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vbelt-0.1.8/vbelt/__init__.py` & `vbelt-0.2.0/vbelt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from .charge_utils import *
 
 
-__version__ = "0.1.8"
+__version__ = "0.2.0"
```

### Comparing `vbelt-0.1.8/vbelt/charge_utils.py` & `vbelt-0.2.0/vbelt/charge_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         return (1.0 / x) * self
 
     def total_only(self):
         if self.dif_part is None and self.dif_nc_part is None:
             return self
 
-        return Charge(self.tot_chg, self.tot_aug)
+        return Charge(self.poscar, self.tot_chg, self.tot_aug)
 
     @classmethod
     def read_from(cls, file):
         # Keep the poscar part in text form.
         poscar = []
         poscar.extend(islice(file, 6))
         head = next(file)
@@ -139,15 +139,15 @@
             write_channel(file, self.dif_part)
 
     def split(self):
         "Split the Charge object into a spin up and a spin down object."
         if self.dif_part is None:
             raise ValueError("No spin related data available.")
 
-        return 0.5 * (self + self.dif_part), 0.5 * (self - self.dif_part)
+        return 0.5 * (self.total_only() + self.dif_part), 0.5 * (self.total_only() - self.dif_part)
 
 
 def read_channel(file, head=None):
     head_ = head or next(file)
     ngx, ngy, ngz = map(int, head_.split())
     regular_data = read_block(file, (ngx, ngy, ngz))
```

### Comparing `vbelt-0.1.8/vbelt/forces.py` & `vbelt-0.2.0/vbelt/forces.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/gencalc.py` & `vbelt-0.2.0/vbelt/gencalc.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,33 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-import sys
 from shlex import quote
 
 import numpy as np
 
-from pysh import cd, mkdir, cp, in_dir, ensure_abs_path, ls, cat
 
-from ase.build import sort
-from ase.dft.kpoints import monkhorst_pack
-
-import chevron
-
-from . import poscar as ps
 from .misc import electronegativity
 from .jobtool import calc_nband, calc_par
 
 
+try:
+    from pysh import mkdir, cp, in_dir, ensure_abs_path, ls, cat
+    from ase.build import sort
+    from ase.dft.kpoints import monkhorst_pack
+    import chevron
+except ImportError as e:
+    raise ImportError("tc-pysh, ase and chevron are required for gencalc.") from e
+
+
+
 class Batch:
     def __init__(self):
         self.potcars = ""
         self.batch_preset = "medium2"
         self.ncpu = 1
         self.ncpu_per_node = 1
```

### Comparing `vbelt-0.1.8/vbelt/incar.py` & `vbelt-0.2.0/vbelt/incar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/jobtool.py` & `vbelt-0.2.0/vbelt/jobtool.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/misc.py` & `vbelt-0.2.0/vbelt/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from itertools import count
+from time import perf_counter
+from statistics import mean, variance, stdev
 
 
 def factorize(n):
     assert n != 0, "Cannot factorize zero."
 
     while n % 2 == 0:
         n //= 2
```

### Comparing `vbelt-0.1.8/vbelt/outcar.py` & `vbelt-0.2.0/vbelt/outcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/outcar_utils.py` & `vbelt-0.2.0/vbelt/outcar_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/poscar.py` & `vbelt-0.2.0/vbelt/poscar.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,42 +106,30 @@
         d_p = np.sum(dists * weights) / np.sum(weights)
         eps = abs(d_p - old_dp) / old_dp
 
     return len(dists[np.exp(1.0 - (dists / d_p) ** 6) >= tol])
 
 
 def periodic_dist(lattice, p1, p2):
-    return np.min(
-        np.linalg.norm([p1 - p2 - t for t in gen_translat(lattice)], axis=-1), axis=0
-    )
+    d = p1 - p2
 
+    dfrac = np.remainder(d @ np.linalg.inv(lattice) + 0.5, 1.0) - 0.5
 
-def gen_translat(lattice: np.ndarray):
-    """Generate all translations to adjacent cells
-
-    :param lattice: np.ndarray([a, b, c]) first lattice parameter
-    """
-    for d in product((-1, 0, 1), (-1, 0, 1), (-1, 0, 1)):
-        yield np.array(d).dot(lattice)
+    return np.linalg.norm(dfrac @ lattice, axis=-1)
 
 
 def periodic_diff(lattice, p1, p2):
-    dp = p1 - p2
-    d = np.array([dp - t for t in gen_translat(lattice)])  # shape (27, n, 3)
-    norms = np.linalg.norm(d, axis=2)  # shape = (27, n)
-    best_translat = np.argmin(norms, axis=0)  # shape = (n,)
+    d = p1 - p2
 
-    n = d.shape[1]
-    return d[best_translat, list(range(n)), :]
+    dfrac = np.remainder(d @ np.linalg.inv(lattice) + 0.5, 1.0) - 0.5
 
+    return dfrac @ lattice
 
-def get_disp(poscar1, poscar2, atoms=None):
-    poscar1.recenter()
-    poscar2.recenter()
 
+def get_disp(poscar1, poscar2, atoms=None):
     if atoms is None:
         p1 = poscar1.raw
         p2 = poscar2.raw
     else:
         p1 = np.ndarray((len(atoms), 3))
         p2 = np.ndarray((len(atoms), 3))
 
@@ -200,24 +188,29 @@
 
     @classmethod
     def from_cell(cls, cell):
         species = {}
         positions = cell.positions
         accum = 0
         for name, number in zip(cell.atoms_types, cell.nb_atoms):
-            species[name] = positions[accum : accum + number]
+            species[name] = positions[accum: accum + number]
             accum += number
 
         species_names = list(cell.atoms_types)
         params = cell.cell_parameters
 
         return Poscar(params, species, species_names=species_names)
 
     @classmethod
     def from_file(cls, filename, recenter=True):
+        """Read structure from a POSCAR file.
+
+        :param filename: the path to the file to read.
+        :param recenter: (optional, :code:`True`)
+        """
         with open(filename) as f:
             next(f)  # system name
             fac = float(next(f))
             params = fac * np.array(
                 [
                     np.array(l.strip().split(), dtype="float")
                     for _, l in zip(range(3), f)
@@ -228,54 +221,41 @@
             atoms_pop = list(map(int, next(f).strip().split()))
             if len(labels) != len(atoms_pop):
                 raise ValueError(f"{filename} is not a coherent POSCAR file.")
 
             mode = next(f).strip()[0].lower()
 
             species = {}
-            if mode == "d":
-                for spec, n in zip(labels, atoms_pop):
-                    if spec in species:
-                        raise NotImplementedError(
-                            "Repeated non contiguous species block is not suppoerted yet."
+            for spec, n in zip(labels, atoms_pop):
+                if spec in species:
+                    raise NotImplementedError(
+                        "Repeated non contiguous species block is not supported."
+                    )
+                pos = []
+                for _, line in zip(range(n), f):
+                    ls = line.strip()
+                    if not ls:
+                        raise ValueError(
+                            f"{filename} is not a coherent POSCAR file."
                         )
-                    pos = []
-                    for _, line in zip(range(n), f):
-                        ls = line.strip()
-                        if not ls:
-                            raise ValueError(
-                                f"{filename} is not a coherent POSCAR file."
-                            )
-                        x, y, z, *_ = ls.split()
-                        pos.append(np.array([x, y, z], dtype="float").dot(params))
-                    species[spec] = np.array(pos)
-            else:
-                for spec, n in zip(labels, atoms_pop):
-                    if spec in species:
-                        raise NotImplementedError(
-                            "Repeated non contiguous species block is not suppoerted yet."
-                        )
-                    pos = []
-                    for _, line in zip(range(n), f):
-                        ls = line.strip()
-                        if not ls:
-                            raise ValueError(
-                                f"{filename} is not a coherent POSCAR file."
-                            )
-                        x, y, z, *_ = ls.split()
+                    x, y, z, *_ = ls.split()
+                    if mode == "d":
+                        # Fractional coordinates
+                        pos.append(
+                            np.array([x, y, z], dtype="float").dot(params))
+                    else:
+                        # Cartesian coordinates
                         pos.append(np.array([x, y, z], dtype="float"))
-                    species[spec] = np.array(pos)
+                species[spec] = np.array(pos)
 
         p = Poscar(params, species, species_names=labels)
-        if recenter:
-            p.recenter()
         return p
 
     def to_file(self, path="POSCAR", cartesian=True):
-        """Write a POSCAR file
+        """Write a POSCAR file.
 
         The property system_name may be set to change the comment at the top of
         the file.
         :param path: path to the file to write
         :param cartesian: if True, write the file in cartesian representation,
           if False, write in fractional representation
         """
@@ -305,23 +285,17 @@
                 for _name, lst in species:
                     for pos in lst:
                         d_pos = pos.dot(inv_params)
                         out.write("  ".join(f"{x:.8f}" for x in d_pos))
                         out.write("\n")
 
     def recenter(self):
-        for sp, pos in self.species.items():
-            for v in self.cell_parameters:
-                n = np.linalg.norm(v)
-                d = v / n
-
-                proj = pos @ d
-
-                pos -= np.floor_divide(proj / n, 1.0).reshape((-1, 1)) * v.reshape(
-                    (1, 3)
-                )
+        "Ensure all coordinates are between 0 and 1 in fractional representation."
+        pfrac = np.remainder(self.raw @ np.linalg.inv(lattice), 1.0)
+
+        self.raw = np.linalg.norm(pfrac @ lattice, axis=-1)
 
 
 coord_methods = {
     "econ": calc_econ,
     "econ_tol": calc_econ_tol,
 }
```

### Comparing `vbelt-0.1.8/vbelt/poscartool.py` & `vbelt-0.2.0/vbelt/poscartool.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     if opts.dest:
         dest = opts.dest
     else:
         dest = opts.poscar + ".xyz"
 
     poscar = Poscar.from_file(opts.poscar)
+    poscar.recenter()
 
     with error_catch(), open(dest, "w") as f:
         print(len(poscar.raw), file=f)
 
         print(poscar.system_name, file=f)
 
         for sp, pos in poscar.species.items():
@@ -123,45 +124,49 @@
     flag("--raw", help="Just ouput values in A."),
 )
 def dist(opts):
     from .poscar import distance, Poscar
 
     poscar = Poscar.from_file(opts.poscar)
     at1 = parse_spec(poscar, opts.atom1)
+
+    if at1[1] is None:
+        error(f"First atom need to be numbered (ex: {at1[0]}1)")
+
     sp1 = spec(poscar, at1)
 
     if opts.atom2 is None:
         with error_catch():
             dists = [
                 (distance(poscar, at1, (sp, i)), spec(poscar, (sp, i)))
                 for sp, p in poscar.species.items()
                 for i in range(len(p))
+                if sp1 != spec(poscar, (sp, i))
             ]
 
         dists.sort()
 
         if opts.max is not None:
             dists = dists[: opts.max]
 
-        for d, sp in dists:
-            if sp == sp1:
-                continue
+        for i, (d, sp) in enumerate(dists):
             if opts.raw:
                 print(d)
             else:
                 bond = f"{sp1}--{sp}"
                 print(f"{bond:12}: {d: 9.5f} A")
     else:
         (s2, i2) = at2 = parse_spec(poscar, opts.atom2)
 
         if i2 is None:
             with error_catch():
                 dists = [
                     (distance(poscar, at1, (s2, i)), spec(poscar, (s2, i)))
                     for i in range(len(poscar.species[s2]))
+                    if sp1 != spec(poscar, (sp, i))
                 ]
 
             dists.sort()
 
             if opts.max is not None:
                 dists = dists[: opts.max]
 
@@ -185,15 +190,15 @@
 @poscartool.subcmd(
     positional("POSCAR", type=str, help="POSCAR file to observe."),
     positional("ATOM", type=str, help="Investigated atom."),
     positional("SPECIES", type=str, help="Coordinating species."),
     optional("--method", "-m", default="econ", help="Computation method."),
 )
 def coord(opts):
-    """Evalueate a coordination number for a given atom and a coordinating species."""
+    """Evaluate a coordination number for a given atom and a coordinating species."""
     from .poscar import Poscar, coord_methods
 
     poscar = Poscar.from_file(opts.poscar)
     at = parse_spec(poscar, opts.atom)
 
     fn = coord_methods.get(opts.method, None)
 
@@ -218,14 +223,21 @@
     """Compute the displacement between two structures."""
     from .poscar import get_disp, Poscar
     import numpy as np
 
     poscar1 = Poscar.from_file(opts.poscar1)
     poscar2 = Poscar.from_file(opts.poscar2)
 
+    # FIXME normalize the rotation 
+    # We need to normalize the positions if they are not exactly in the same representation.
+    # That is, we need to be sure that the same cell is represented in both case.
+
+    print(poscar1.cell_parameters)
+    print(poscar2.cell_parameters)
+
     if opts.ref is not None:
         with error_catch():
             sp, i = parse_spec(poscar1, opts.ref)
 
         offset = poscar1.species[sp][i] - poscar2.species[sp][i]
 
         poscar1.raw = poscar1.raw - offset.reshape((1, 3))
```

### Comparing `vbelt-0.1.8/vbelt/potcar.py` & `vbelt-0.2.0/vbelt/potcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.1.8/vbelt/script_utils.py` & `vbelt-0.2.0/vbelt/script_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 compatible with setuptools, as well as package entrypoint. The idea is to write
 the bulk of the script in a function that is decorated with the specification
 of its CLI interface. The function simply takes the Namespace object with the
 parameters already parsed.
 
 Here is a usage example of the module:
 .. code-block:: python
+
     # my_package/cli.py
     from .script_utils import MultiCmd, script, positional, flag
 
     # Single command entry point:
     @script(
         positional("FOO", help="the first parameter."),
         flag("--bar", "-b", help="enable barring the foo."),
@@ -54,14 +55,15 @@
 You can then call `treat_foo` and `treat_baz` with no argument or with
 `sys.argv` in you `__name__ == "__main__"` section. Alternatively, they are
 both valid callable entrypoint to set in your setup.py/setup.cfg.
 
 Here is a short example of a corresponding setup.cfg:
 
 .. code-block:: cfg
+
     [metadata]
     name = my_package
     author = Your name
     author_email = your.address@email.net
     description = A short description
 
     [options]
@@ -102,26 +104,28 @@
     POSSIBILITY OF SUCH DAMAGE.
 """
 import sys
 import os
 from argparse import ArgumentParser
 from contextlib import contextmanager
 from functools import wraps
+from statistics import mean, stdev, variance
+from time import perf_counter
+
+
+_debug = os.environ.get("DEBUG", False) in {"1", "yes", "true"}
 
 
 def _default_post(ret):
     if isinstance(ret, int):
         return ret
     else:
         return 0
 
 
-_debug = os.environ.get("DEBUG", False) in {"1", "yes", "true"}
-
-
 class MultiCmd:
     """A CLI with several subcommands.
 
     Build an entrypoint with several subcommands.
     Register subcommands with MultiCmd.subcmd.
     Call the instance (or its run method) to run the script.
     """
@@ -145,32 +149,41 @@
 
     def post(self, f):
         "Register a function to be called on the return value of the command at the end."
         assert callable(f), "post applies to functions"
         self._post = f
         return f
 
-    def __call__(self, *args):
-        return self.run(*args)
+    def __call__(self, argv=None):
+        return self.run(argv=argv)
 
-    def subcmd(self, *args):
+    def subcmd(self, *args, name=None):
         """Register a new subcommand.
 
         See script.
         """
 
         def decorator(f):
-            parser = self.sub_parsers.add_parser(f.__name__, help=f.__doc__)
+            parser = self.sub_parsers.add_parser(name or f.__name__, help=f.__doc__)
 
             for param in args:
                 param(parser)
 
             parser.set_defaults(handler=f)
 
-            return f
+            @wraps(f)
+            def wrapper(argv=None):
+                if argv is None:
+                    opts = parser.parse_args()
+                else:
+                    opts = parser.parse_args(argv)
+
+                return f(opts)
+
+            return wrapper
 
         return decorator
 
     def run(self, argv=None):
         """Execute the script (calling the instance redirect here).
 
         You can explicitly pass a list of string parameters instead of using
@@ -226,29 +239,29 @@
 def error(msg):
     "Write msg to stderr and exit with -1 return code."
     print(msg, file=sys.stderr)
     exit(-1)
 
 
 @contextmanager
-def error_catch():
+def error_catch(prefix="Error: "):
     """Catch all errors, print them and exit with -1 return code.
 
     Context manager to provide cleaner errors when building a script around a
     function that can raise.
     If the environment variable DEBUG is set to "yes", this does nothing in
     order to let the exception crash the program and show the traceback.
     """
     if _debug:
         yield
     else:
         try:
             yield
         except Exception as e:
-            error(str(e))
+            error(prefix + str(e))
 
 
 def flag(*names, **kwargs):
     """Add a flag dashed parameter that always.
 
     You can provide as many aliases as you want but they must all start with a
     dash.
@@ -321,14 +334,107 @@
     start with a dash.
     kwargs are passed to ArgumentParser.add_argument.
     """
     assert all(
         n.startswith("-") for n in names
     ), "Either use a single non-dash name or only dash names."
 
+    assert kwargs.get("type", str) == str or "default" in kwargs, "You should provide a default value."
+
     def add(parser):
         parser.add_argument(
             *names,
             **kwargs,
         )
 
     return add
+
+
+class PerfCounterCollec:
+    """A collection of perfomance counter.
+
+    A simple facility to time sections of a program.
+
+    Example:
+
+        pc = PerfCounterCollec()
+
+        with pc.foo:
+            # do some stuff
+
+        with pc.bar:
+            # do other stuff
+
+        print(pc.summary())
+
+        # foo: 0.65344 s
+        # bar: 1.32645 s
+    """
+
+    def __init__(self, format="{name}: {c.total:.05f} s"):
+        self.counters = {}
+        self.fmt = format
+
+    def __getattr__(self, name):
+        return self.counters.setdefault(name, PerfCounter())
+
+    def collect(self):
+        for name, counter in self.counters.items():
+            yield (name, counter)
+
+    def summary(self, format=None):
+        lines = []
+
+        if format is None:
+            fmt = self.fmt
+        else:
+            fmt = format
+
+        for name, counter in self.counters.items():
+            lines.append(fmt.format(name=name, c=counter))
+
+        return "\n".join(lines)
+
+
+class PerfCounter:
+    """An individual counter
+
+    Use it as a context manager.
+    Each time it is entered, it start a new counter.
+    Each time it is exited, it add the elapsed time of the last counter to the total.
+    You can also access basic statistics (number of slices, mean and standard deviation).
+    """
+
+    def __init__(self):
+        self.slices = []
+        self.opened = []
+
+    def __enter__(self):
+        self.opened.append(perf_counter())
+
+    def __exit__(self, *args):
+        self.slices.append(perf_counter() - self.opened.pop())
+
+    @property
+    def total(self):
+        "Total time spent under this counter."
+        return sum(self.slices)
+
+    @property
+    def slice_number(self):
+        "Number of separate slices added to this counter."
+        return len(self.slices)
+
+    @property
+    def mean(self):
+        "Mean time spent in a single slice."
+        return mean(self.slices)
+
+    @property
+    def stdev(self):
+        "Standard deviation of time spent in a slice."
+        return stdev(self.slices)
+
+    @property
+    def variance(self):
+        "Variance of time spent in a slice."
+        return variance(self.slices)
```

### Comparing `vbelt-0.1.8/vbelt/wrapper.py` & `vbelt-0.2.0/vbelt/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,61 +19,71 @@
 from .script_utils import (
     script,
     error,
     positional,
     flag,
     optional,
     error_catch,
+    PerfCounterCollec,
 )
 
 
 @script(
     positional("CHGCAR", help="file to extract data from"),
     flag("--split", help="split CHGCAR into up and down channels"),
     flag("--spin", help="extract the spin density"),
     flag("--total", help="extract the total density"),
+    flag("--timing", help="show the timing informations"),
 )
 def charge_extract(opts):
     from .charge_utils import Charge
 
-    if opts.chgcar == "-":
-        chg = Charge.from_file(sys.stdin)
-        name = "CHGCAR"
-    else:
-        with open(opts.chgcar) as f:
-            chg = Charge.read_from(f)
-        name = opts.chgcar
+    pc = PerfCounterCollec()
+
+    with pc.reading:
+        if opts.chgcar == "-":
+            chg = Charge.from_file(sys.stdin)
+            name = "CHGCAR"
+        else:
+            with open(opts.chgcar) as f:
+                chg = Charge.read_from(f)
+            name = opts.chgcar
 
-    out_prefix = name
+    out_prefix, ext = os.path.splitext(name)
 
     if opts.split:
         if chg.dif_part is None:
             error("There is no spin data available in the input file.")
 
-        up, down = chg.split()
-        with open(out_prefix + ".up", "w") as f:
+        with pc.processing:
+            up, down = chg.split()
+
+        with pc.writing, open(out_prefix + ".up" + ext, "w") as f:
             up.write_to(f)
 
-        with open(out_prefix + ".down", "w") as f:
+        with pc.writing, open(out_prefix + ".down" + ext, "w") as f:
             down.write_to(f)
 
     elif opts.spin:
         if chg.dif_part is None:
             error("There is no spin data available in the input file.")
 
-        with open(out_prefix + ".spin", "w") as f:
+        with pc.writing, open(out_prefix + ".spin" + ext, "w") as f:
             chg.dif_part.write_to(f)
 
     elif opts.total:
-        with open(out_prefix + ".total", "w") as f:
+        with pc.writing, open(out_prefix + ".total" + ext, "w") as f:
             chg.total_only().write_to(f)
 
     else:
         error("No action required.")
 
+    if opts.timing:
+        print(pc.summary())
+
 
 @script(
     positional("COEF_A", type=float, help="coeficient for the first file"),
     positional("CHGCAR_A", help="first file to extract data from"),
     positional("COEF_B", type=float, help="coeficient for the second file"),
     positional("CHGCAR_B", help="second file to extract data from"),
 )
```

### Comparing `vbelt-0.1.8/vbelt.egg-info/PKG-INFO` & `vbelt-0.2.0/vbelt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbelt
-Version: 0.1.8
+Version: 0.2.0
 Summary: The VASP user tool belt.
 Home-page: https://git.sr.ht/~lattay/vbelt
 Author: Théo Cavignac
 Author-email: theo.cavignac@gmail.com
 License: GPL License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

