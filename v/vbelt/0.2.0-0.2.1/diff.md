# Comparing `tmp/vbelt-0.2.0.tar.gz` & `tmp/vbelt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbelt-0.2.0.tar", last modified: Wed Jul  5 08:35:59 2023, max compression
+gzip compressed data, was "vbelt-0.2.1.tar", last modified: Wed Jul  5 09:48:36 2023, max compression
```

## Comparing `vbelt-0.2.0.tar` & `vbelt-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/
--rw-r--r--   0 theo      (1000) theo      (1000)    35095 2023-02-14 12:56:15.000000 vbelt-0.2.0/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 08:35:59.653610 vbelt-0.2.0/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)     1200 2023-07-05 08:35:00.000000 vbelt-0.2.0/README.md
--rw-r--r--   0 theo      (1000) theo      (1000)      968 2023-07-05 08:35:59.653610 vbelt-0.2.0/setup.cfg
--rwxr-xr-x   0 theo      (1000) theo      (1000)       62 2023-07-05 08:28:11.000000 vbelt-0.2.0/setup.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/vbelt/
--rw-r--r--   0 theo      (1000) theo      (1000)      759 2023-07-05 08:29:28.000000 vbelt-0.2.0/vbelt/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     6257 2023-03-16 14:19:00.000000 vbelt-0.2.0/vbelt/charge_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1907 2023-02-14 12:57:07.000000 vbelt-0.2.0/vbelt/forces.py
--rw-rw----   0 theo      (1000) theo      (1000)     9652 2023-07-05 08:32:43.000000 vbelt-0.2.0/vbelt/gencalc.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1407 2023-02-14 12:57:12.000000 vbelt-0.2.0/vbelt/incar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     4641 2023-02-14 12:57:17.000000 vbelt-0.2.0/vbelt/jobtool.py
--rw-r--r--   0 theo      (1000) theo      (1000)     3076 2023-03-17 14:30:03.000000 vbelt-0.2.0/vbelt/misc.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1661 2023-02-23 10:34:40.000000 vbelt-0.2.0/vbelt/outcar.py
--rw-r--r--   0 theo      (1000) theo      (1000)     4238 2023-02-14 12:57:24.000000 vbelt-0.2.0/vbelt/outcar_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9505 2023-07-05 08:14:09.000000 vbelt-0.2.0/vbelt/poscar.py
--rw-r--r--   0 theo      (1000) theo      (1000)    10361 2023-07-05 08:18:21.000000 vbelt-0.2.0/vbelt/poscartool.py
--rw-r--r--   0 theo      (1000) theo      (1000)     2168 2023-02-14 12:57:40.000000 vbelt-0.2.0/vbelt/potcar.py
--rw-r--r--   0 theo      (1000) theo      (1000)    12579 2023-07-05 08:26:41.000000 vbelt-0.2.0/vbelt/script_utils.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9611 2023-03-17 14:30:26.000000 vbelt-0.2.0/vbelt/wrapper.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 08:35:59.653610 vbelt-0.2.0/vbelt.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      460 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)      301 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/entry_points.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       64 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/requires.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        6 2023-07-05 08:35:59.000000 vbelt-0.2.0/vbelt.egg-info/top_level.txt
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 09:48:36.199952 vbelt-0.2.1/
+-rw-r--r--   0 theo      (1000) theo      (1000)    35095 2023-02-14 12:56:15.000000 vbelt-0.2.1/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 09:48:36.199952 vbelt-0.2.1/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)     1200 2023-07-05 08:35:00.000000 vbelt-0.2.1/README.md
+-rw-r--r--   0 theo      (1000) theo      (1000)      968 2023-07-05 09:48:36.199952 vbelt-0.2.1/setup.cfg
+-rwxr-xr-x   0 theo      (1000) theo      (1000)       62 2023-07-05 08:28:11.000000 vbelt-0.2.1/setup.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 09:48:36.196619 vbelt-0.2.1/vbelt/
+-rw-r--r--   0 theo      (1000) theo      (1000)      759 2023-07-05 09:43:54.000000 vbelt-0.2.1/vbelt/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     6257 2023-03-16 14:19:00.000000 vbelt-0.2.1/vbelt/charge_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1907 2023-02-14 12:57:07.000000 vbelt-0.2.1/vbelt/forces.py
+-rw-rw----   0 theo      (1000) theo      (1000)     8687 2023-07-05 09:15:44.000000 vbelt-0.2.1/vbelt/gencalc.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1407 2023-02-14 12:57:12.000000 vbelt-0.2.1/vbelt/incar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     7300 2023-07-05 09:47:27.000000 vbelt-0.2.1/vbelt/jobtool.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3479 2023-07-05 09:15:27.000000 vbelt-0.2.1/vbelt/misc.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1661 2023-02-23 10:34:40.000000 vbelt-0.2.1/vbelt/outcar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     4238 2023-02-14 12:57:24.000000 vbelt-0.2.1/vbelt/outcar_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     9505 2023-07-05 08:14:09.000000 vbelt-0.2.1/vbelt/poscar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    10361 2023-07-05 08:18:21.000000 vbelt-0.2.1/vbelt/poscartool.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     2168 2023-02-14 12:57:40.000000 vbelt-0.2.1/vbelt/potcar.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    12579 2023-07-05 08:26:41.000000 vbelt-0.2.1/vbelt/script_utils.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     9611 2023-07-05 08:47:22.000000 vbelt-0.2.1/vbelt/wrapper.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-07-05 09:48:36.199952 vbelt-0.2.1/vbelt.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1652 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      460 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)      301 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/entry_points.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       64 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/requires.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        6 2023-07-05 09:48:36.000000 vbelt-0.2.1/vbelt.egg-info/top_level.txt
```

### Comparing `vbelt-0.2.0/LICENSE` & `vbelt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/PKG-INFO` & `vbelt-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbelt
-Version: 0.2.0
+Version: 0.2.1
 Summary: The VASP user tool belt.
 Home-page: https://git.sr.ht/~lattay/vbelt
 Author: Théo Cavignac
 Author-email: theo.cavignac@gmail.com
 License: GPL License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `vbelt-0.2.0/README.md` & `vbelt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/setup.cfg` & `vbelt-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/__init__.py` & `vbelt-0.2.1/vbelt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from .charge_utils import *
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `vbelt-0.2.0/vbelt/charge_utils.py` & `vbelt-0.2.1/vbelt/charge_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/forces.py` & `vbelt-0.2.1/vbelt/forces.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/gencalc.py` & `vbelt-0.2.1/vbelt/gencalc.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from shlex import quote
 
 import numpy as np
 
 
 from .misc import electronegativity
-from .jobtool import calc_nband, calc_par
+from .jobtool import calc_nband, calc_par, make_fer
 
 
 try:
     from pysh import mkdir, cp, in_dir, ensure_abs_path, ls, cat
     from ase.build import sort
     from ase.dft.kpoints import monkhorst_pack
     import chevron
@@ -214,57 +214,14 @@
             return nelect
         else:
             return 2 * valence_shell - nelect
 
     return sum(at_unpaired(at) for at in struct) / 2.0
 
 
-def make_fer(nelect, nband, nkpt, excite):
-    vbm_down = nelect // 2
-    vbm_up = nelect - vbm_down
-
-    print("nelect", nelect)
-    print("vbm_up", vbm_up)
-    print("vbm_down", vbm_down)
-
-    occ_0_up = [1] * vbm_up + [0] * (nband - vbm_up)
-    occ_0_down = [1] * vbm_down + [0] * (nband - vbm_down)
-
-    occ_up, occ_down = excite(occ_0_up, occ_0_down, vbm_up - 1, vbm_down - 1)
-
-    one_k_up = fortran_array(occ_up)
-    one_k_down = fortran_array(occ_down)
-
-    return " ".join(one_k_up for _ in range(nkpt)), " ".join(
-        one_k_down for _ in range(nkpt)
-    )
-
-
-def fortran_array(lst):
-    assert all(isinstance(i, int) for i in lst)
-
-    elems = []
-
-    prev = 0.5
-    acc = 0
-    for e in lst:
-        if e == prev:
-            acc += 1
-        else:
-            if acc:
-                elems.append(f"{acc}*{float(prev):.01f}")
-            prev = e
-            acc = 1
-
-    if acc:
-        elems.append(f"{acc}*{float(prev):.01f}")
-
-    return " ".join(elems)
-
-
 def ask(msg, collection):
     print(msg)
     for i, elem in enumerate(collection, start=1):
         print(f"{i}. {elem}")
 
     res = ""
     while not res.isdecimal() or int(res) < 1 or int(res) > len(collection):
```

### Comparing `vbelt-0.2.0/vbelt/incar.py` & `vbelt-0.2.1/vbelt/incar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/jobtool.py` & `vbelt-0.2.1/vbelt/jobtool.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,31 +24,29 @@
     error,
 )
 
 from .poscar import Poscar
 from .potcar import Potcar, predict_nelect
 from .incar import parse_incar
 from .outcar_utils import get_int
-from .misc import factorize
+from .misc import factorize, fortran_array
 
 
 jobtool = MultiCmd(description=__doc__)
 
 
 @jobtool.subcmd(
     positional("NCPU", type=int, help="Number of cores."),
     positional("PATH", default=".", type=str, help="Computation directory."),
-    optional(
-        "--nkpt",
-        "-k",
-        default="auto",
-        help="Wether NKPT should be read from a previous computation of should be fixed arbitrary.",
-    ),
 )
 def predict_nband(opts):
+    print(_predict_nband_helper(opts)[0])
+
+
+def _predict_nband_helper(opts):
     with error_catch():
         incar = parse_incar(
             os.path.join(opts.path, "INCAR"),
             {
                 "KPAR": {"cast": int, "default": 1},
                 "NCORE": {"cast": int, "default": -1},
                 "ISPIN": {"cast": int, "default": 1},
@@ -70,26 +68,24 @@
     if incar["NCORE"] > 0:
         ncore = incar["NCORE"]
     elif incar["NPAR"] > 0:
         ncore = max((opts.ncpu // incar["KPAR"]) // incar["NPAR"], 1)
     else:
         ncore = 1
 
-    nbands = calc_nband(
+    return calc_nband(
         nions,
         nions,
         nelect,
         incar["KPAR"],
         opts.ncpu,
         ncore,
         incar["ISPIN"],
         noncol=incar["LSORBIT"],
-    )
-
-    print(nbands)
+    ), int(nelect), 
 
 
 @jobtool.subcmd(
     positional("NCPU", type=int, help="Number of cores."),
     positional("NCPU_PER_NODE", type=int, help="Number of core per nodes."),
     positional("PATH", default=".", type=str, help="Computation directory."),
     optional(
@@ -131,14 +127,106 @@
     ncore_sqrt = int_sqrt(ncpu // kpar)
 
     ncore = min(ncore_cpu, ncore_sqrt)
 
     return kpar, ncore
 
 
+@jobtool.subcmd(
+    positional("NCPU", type=int, help="Number of cores."),
+    positional("PATH", default=".", type=str, help="Computation directory."),
+    optional(
+        "--nkpt",
+        "-k",
+        default="auto",
+        help="Wether NKPT should be read from a previous computation of should be fixed arbitrary.",
+    ),
+    optional("--nholes", "-n", default=1, type=int,
+             help="Number of holes to introduce under the electron."),
+    optional("--spin", "-s", default="uu", type=str,
+             help="Spin of the electron."),
+)
+def make_ferwe(opts):
+    """Compute the adapted FERWE and FERDO for a VASP computation.
+
+    It takes into account parallelization, number of cores and nodes etc.
+
+    The spin parameter tells from which channel to take the electron, and in
+    which to put it.
+
+    For example, taking the electron from the up channel, and putting it in the
+    down channel on top of three holes would be done with parameters:
+    `--nholes=3 --spin="ud"`
+
+    """
+    if opts.nkpt == "auto":
+        try:
+            with open(os.path.join(opts.path, "OUTCAR")) as f:
+                nkpt = get_int(f, "NKPTS", after="k-points", expect_equal=True)
+        except FileNotFoundError:
+            error("Could not find a previous OUTCAR.")
+
+        if nkpt is None:
+            error("Could not find the value of NKPTS in OUTCAR.")
+
+    else:
+        nkpt = int(opts.nkpt)
+
+    nband, nelect = _predict_nband_helper(opts)
+
+    if not opts.spin in {"uu", "dd", "ud", "du"}:
+        error("Spin must be 'uu', 'dd', 'ud' or 'du'.")
+
+    from_ = opts.spin[0]
+    to_ = opts.spin[1]
+
+    def excite(occ_up, occ_down, vbm_up, vbm_down):
+        if from_ == "a":
+            occ_up[vbm_up] = 0
+            vbm_up -= 1
+        else:
+            occ_down[vbm_down] = 0
+            vbm_down -= 1
+
+        if to_ == "a":
+            occ_up[vbm_up+opts.nholes+1] = 1
+        else:
+            occ_down[vbm_down+opts.nholes+1] = 1
+
+        return occ_up, occ_down
+
+    ferwe, ferdo = make_fer(nelect, nband, nkpt, excite)
+
+    print("NELECT =", nelect)
+    print("NBAND =", nband)
+
+    print("FERWE =", ferwe)
+    print("FERDO =", ferdo)
+
+
+def make_fer(nelect, nband, nkpt, excite):
+    assert isinstance(nelect, int)
+    assert isinstance(nband, int)
+    assert isinstance(nkpt, int)
+    vbm_down = nelect // 2
+    vbm_up = nelect - vbm_down
+
+    occ_0_up = [1] * vbm_up + [0] * (nband - vbm_up)
+    occ_0_down = [1] * vbm_down + [0] * (nband - vbm_down)
+
+    occ_up, occ_down = excite(occ_0_up, occ_0_down, vbm_up - 1, vbm_down - 1)
+
+    one_k_up = fortran_array(occ_up)
+    one_k_down = fortran_array(occ_down)
+
+    return " ".join(one_k_up for _ in range(nkpt)), " ".join(
+        one_k_down for _ in range(nkpt)
+    )
+
+
 def int_sqrt(n):
     prev = n
 
     for j in range(n, 0, -1):
         if n % j == 0:
             if j**2 == n:
                 return j
```

### Comparing `vbelt-0.2.0/vbelt/outcar.py` & `vbelt-0.2.1/vbelt/outcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/outcar_utils.py` & `vbelt-0.2.1/vbelt/outcar_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/poscar.py` & `vbelt-0.2.1/vbelt/poscar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/poscartool.py` & `vbelt-0.2.1/vbelt/poscartool.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/potcar.py` & `vbelt-0.2.1/vbelt/potcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/script_utils.py` & `vbelt-0.2.1/vbelt/script_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt/wrapper.py` & `vbelt-0.2.1/vbelt/wrapper.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.2.0/vbelt.egg-info/PKG-INFO` & `vbelt-0.2.1/vbelt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbelt
-Version: 0.2.0
+Version: 0.2.1
 Summary: The VASP user tool belt.
 Home-page: https://git.sr.ht/~lattay/vbelt
 Author: Théo Cavignac
 Author-email: theo.cavignac@gmail.com
 License: GPL License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

