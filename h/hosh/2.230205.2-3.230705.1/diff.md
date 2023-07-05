# Comparing `tmp/hosh-2.230205.2.tar.gz` & `tmp/hosh-3.230705.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosh-2.230205.2.tar", max compression
+gzip compressed data, was "hosh-3.230705.1.tar", max compression
```

## Comparing `hosh-2.230205.2.tar` & `hosh-3.230705.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-2.230205.2/LICENSE
--rw-r--r--   0        0        0     9697 2023-02-05 21:54:51.186998 hosh-2.230205.2/README.md
--rw-r--r--   0        0        0      728 2023-02-05 21:54:52.599017 hosh-2.230205.2/pyproject.toml
--rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-2.230205.2/src/hosh/__init__.py
--rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-2.230205.2/src/hosh/_internals_appearance.py
--rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-2.230205.2/src/hosh/config.py
--rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/groups.py
--rw-r--r--   0        0        0    30399 2023-02-05 21:48:38.821663 hosh-2.230205.2/src/hosh/hosh_.py
--rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-2.230205.2/src/hosh/misc/__init__.py
--rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-2.230205.2/src/hosh/misc/colors.py
--rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/core.py
--rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/__init__.py
--rw-r--r--   0        0        0     9083 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/base.py
--rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/base777.py
--rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-2.230205.2/src/hosh/misc/exception.py
--rw-r--r--   0        0        0     1517 2022-12-31 19:32:46.000000 hosh-2.230205.2/src/hosh/misc/helper.py
--rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-2.230205.2/src/hosh/misc/identity.py
--rw-r--r--   0        0        0     4503 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/math.py
--rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/root.py
--rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-2.230205.2/src/hosh/theme.py
--rw-r--r--   0        0        0    10713 1970-01-01 00:00:00.000000 hosh-2.230205.2/setup.py
--rw-r--r--   0        0        0    10416 1970-01-01 00:00:00.000000 hosh-2.230205.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-3.230705.1/LICENSE
+-rw-r--r--   0        0        0     9771 2023-07-05 21:21:04.153737 hosh-3.230705.1/README.md
+-rw-r--r--   0        0        0      776 2023-07-05 21:21:10.973739 hosh-3.230705.1/pyproject.toml
+-rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-3.230705.1/src/hosh/__init__.py
+-rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-3.230705.1/src/hosh/_internals_appearance.py
+-rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-3.230705.1/src/hosh/config.py
+-rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/groups.py
+-rw-r--r--   0        0        0    39941 2023-07-05 21:11:26.169527 hosh-3.230705.1/src/hosh/hosh_.py
+-rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-3.230705.1/src/hosh/misc/__init__.py
+-rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-3.230705.1/src/hosh/misc/colors.py
+-rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/core.py
+-rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/encoding/__init__.py
+-rw-r--r--   0        0        0     9099 2023-04-17 16:49:34.360852 hosh-3.230705.1/src/hosh/misc/encoding/base.py
+-rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/encoding/base777.py
+-rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-3.230705.1/src/hosh/misc/exception.py
+-rw-r--r--   0        0        0     1559 2023-04-22 00:24:44.334832 hosh-3.230705.1/src/hosh/misc/helper.py
+-rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-3.230705.1/src/hosh/misc/identity.py
+-rw-r--r--   0        0        0     4988 2023-05-04 17:05:47.757107 hosh-3.230705.1/src/hosh/misc/math.py
+-rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/root.py
+-rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-3.230705.1/src/hosh/theme.py
+-rw-r--r--   0        0        0    10787 1970-01-01 00:00:00.000000 hosh-3.230705.1/setup.py
+-rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 hosh-3.230705.1/PKG-INFO
```

### Comparing `hosh-2.230205.2/LICENSE` & `hosh-3.230705.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/README.md` & `hosh-3.230705.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)
 <a href="https://pypi.org/project/hosh">
 <img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
-
+[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)
 
 # hosh - Identification based on group theory
 [Website](https://hosh.page) |
 [Latest Release](https://pypi.org/project/hosh) |
 [Current Code](https://github.com/davips/hosh) |
 [API Documentation](https://davips.github.io/hosh)
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg) [![codecov]
 (https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://
 codecov.io/gh/davips/hosh) [pypi] ![Python version](https://img.shields.io/
-badge/python-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://
-doi.org/10.5281/zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-
-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [!
-[API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
+badge/python-â¥3.8-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
+License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/
+zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
+b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
+documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hosh) [![Manual](https://img.shields.io/badge/manual-
-handcrafted-a030a0.svg)](https://hosh.page) # hosh - Identification based on
-group theory [Website](https://hosh.page) | [Latest Release](https://pypi.org/
-project/hosh) | [Current Code](https://github.com/davips/hosh) | [API
-Documentation](https://davips.github.io/hosh) This [Python library](https://
-pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a
-reference implementation for the UT*.4 specification presented [here](https://
-arxiv.org/abs/2109.06028). A previous version, containing extra group theory
-content, is available in the package [GaROUPa](https://pypi.org/project/
-garoupa). Please see the [website](https://hosh.page) for more detailed usage
-information. We adopt a novel paradigm to universally unique identification
-(UUID), making identifiers deterministic and predictable, even before an object
-is generated by a (possibly costly) process. Here, data versioning and
-composition of processing steps are directly mapped as simple operations over
-identifiers. We call each of the latter a `Hosh`, i.e., an identifier is an
-_**o**perable **h**a**sh**_. A first implementation of the remaining ideas from
-the [paper](https://arxiv.org/abs/2109.06028) is provided in this [cacheable
-lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh`
-and serves as an advanced usage example.
+handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh) # hosh -
+Identification based on group theory [Website](https://hosh.page) | [Latest
+Release](https://pypi.org/project/hosh) | [Current Code](https://github.com/
+davips/hosh) | [API Documentation](https://davips.github.io/hosh) This [Python
+library](https://pypi.org/project/hosh) / [code](https://github.com/davips/
+hosh) provides a reference implementation for the UT*.4 specification presented
+[here](https://arxiv.org/abs/2109.06028). A previous version, containing extra
+group theory content, is available in the package [GaROUPa](https://pypi.org/
+project/garoupa). Please see the [website](https://hosh.page) for more detailed
+usage information. We adopt a novel paradigm to universally unique
+identification (UUID), making identifiers deterministic and predictable, even
+before an object is generated by a (possibly costly) process. Here, data
+versioning and composition of processing steps are directly mapped as simple
+operations over identifiers. We call each of the latter a `Hosh`, i.e., an
+identifier is an _**o**perable **h**a**sh**_. A first implementation of the
+remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided
+in this [cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which
+depends on `hosh` and serves as an advanced usage example.
 A second (entirely rewritten) version is available in the package [idict]
 (https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/
 project/hoshmap). The most recent rewritten version of a hosh-based dict (and
 the most robust, recommended, one) is available in the package [hdict](https://
 pypi.org/project/hdict). ## Overview A product of identifiers produces a new
 identifier as shown below, where sequences of bytes (`b"..."`) are passed to
 simulate binary objects to be hashed. ![img.png](https://
```

### Comparing `hosh-2.230205.2/pyproject.toml` & `hosh-3.230705.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "hosh"
-version = "2.230205.2"
+version = "3.230705.1"
 description = "Predictable Operable HaSH-based identifiers"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "hosh", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-wheel = "^0.37.0"
-blake3 = "^0.2.0"
-colored = "1.4.2"
+wheel = "^0.40.0"
+blake3 = "^0.3.3"
+colored = "1.4.2" # Newer minor version has breaking changes.
 ansi2html = "^1.6.0"
 bs4 = "^0.0.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pdoc3 = "^0.10.0"
-autoreadme = "^0.2102.20"
-pytest = "^6.2.5"
-pytest-cov = "^2.12.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 ipython = "^7.27.0"
 black = "^21.9b0"
 flake8 = "^4.0.1"
+autoreadme = "^0.2302.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 # 
 # [[tool.poetry.source]]
 # name = "dvpypi"
```

### Comparing `hosh-2.230205.2/src/hosh/__init__.py` & `hosh-3.230705.1/src/hosh/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/_internals_appearance.py` & `hosh-3.230705.1/src/hosh/_internals_appearance.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/config.py` & `hosh-3.230705.1/src/hosh/config.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/groups.py` & `hosh-3.230705.1/src/hosh/groups.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/hosh_.py` & `hosh-3.230705.1/src/hosh/hosh_.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 #  You should have received a copy of the GNU General Public License
 #  along with hosh.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and unethical regarding the effort and
 #  time spent here.
-import operator
 from functools import reduce
+from operator import mul, add
 from sys import maxsize
 from typing import Union
 
-from hosh.theme import HTML, ANSI, BW
 from hosh.config import GLOBAL
 from hosh.groups import UT40_4, groups
 from hosh.misc.colors import ansi2html, id2ansi, id2rgb
 from hosh.misc.core import cells_id_fromblob, cells_fromid, id_fromcells
 from hosh.misc.encoding.base777 import b777enc
 from hosh.misc.exception import (
     WrongContent,
     DanglingEtype,
     CellValueTooHigh,
     WrongIdentifier,
     ElementTooHigh,
     WrongVersion,
 )
 from hosh.misc.math import cellsmul, cellsinv, cells2int, int2cells, cellspow, cellsroot
+from hosh.theme import HTML, ANSI, BW
 
 
 class Hosh:
     """
     Operable hash.
 
     Generate a Hosh object from a binary content or a list of 6 ints.
@@ -90,17 +90,17 @@
     >>> print(ø * "7ysdf98ysdf98ysdf98ysdfysdf98ysdasddsa32" * "6gdsf76dfqwe123de8gaf87gaf87gaf87agdfa78")
     94UrdYKjCGQWdd5P.W4xvFJgc9hZpIHlhytqHkaa
     >>> h = ø.u * b"sdff"
     >>> print(h)
     f_9e1a267c8_____________________________
     >>> x.id, (+x).id  # Making an ordered x.
     ('ZN_60eec3e6c7b68087329e16b581401a6bb2b1f', '6BDj3b7Mmj7n-6B8XYaP3akO7400s9FlG4AtcHTp')
-    >>> -x * y != y * -x
+    >>> +x * y != y * +x
     True
-    >>> --x == x
+    >>> ++x == x
     True
     >>> x ** y == +(+x * +y)  # a ** b is a shortcut for +(+a * +b)
     True
     >>> x ** y != y ** x
     True
     >>> (x ** b"1") * (y ** b"2") != (x ** b"2") * (y ** b"1")
     True
@@ -126,19 +126,20 @@
     """
 
     _n, _id, _ansi_light, _ansi_dark = None, None, None, None
     _sansi_light, _sansi_dark, _sid, _etype, _rgb_light, _rgb_dark = None, None, None, None, None, None
 
     _etype_inducer, _bits, _ø = None, None, None
     _rev = None
+    components_cache_size = 100
 
     def __init__(self, content, etype="default:ordered", version=UT40_4):
         self.version = version
         self.p, self.p4, self.p6, self.digits, self.bytes, _, _, _, _, _, _ = version
-        self._composition_nolast = {}
+        self._composition_memo = {}
         if isinstance(content, list):
             if etype != "default:ordered":
                 raise DanglingEtype(f"Cannot set etype={etype} when providing cells ({content}).")
             if max(content) >= self.p:
                 raise CellValueTooHigh(f"A cell value exceeds the limit for the group: {max(content)} >= {self.p}")
             self.cells = content
         elif isinstance(content, bytes):
@@ -174,27 +175,94 @@
             from hosh import Identity
 
             self._ø = Identity(version=self.version, etype_inducer=self.etype)
         return self._ø
 
     @property
     def rev(self):
-        """Element with the reversed indentifier
+        """
+        Reversed element (warning: this is not the inverse element)
+
+        Element with the internal cells reversed.
+        This operation is its own inverse.
+
+        This is useful wherever a unary operation is needed.
+        For instance, a function can be represented as a value by its original identifier,
+        and can be represented as (an applied) function by its reversed element identifier.
+
+        Not all hoshes are digest-reversible, i.e., at the digit level, due to the intrinsic mismatch between base 64 (i.e., a power of two) representation and the group (prime) order.
+        Therefore, we must resort to reversing the cells.
+        As an exception, unordered elements do have (most) digits reversed as it has only one internal cell.
+
+        Probabilistically irrelevant corner cases:
+            The presence of empty cells (i.e., with zero value) might cause migration from one etype to another.
+            The presence of duplicate cells (i.e., with the same value) might make the hosh reverse to itself.
+            See examples below.
 
         Usage:
 
-        >>> from hosh import Hosh
+        >>> from hosh import Hosh, groups
         >>> h = Hosh.fromid("J5.uRTue8X4r1xu.JFkPbURVVGvTRPSFLncXdyzj").rev
         >>> h.id
-        'jzydXcnLFSPRTvGVVRUbPkFJ.ux1r4X8euTRu.5J'
-        >>> "".join(reversed(h.id))
-        'J5.uRTue8X4r1xu.JFkPbURVVGvTRPSFLncXdyzj'
+        'lUz6uu1ZBCJf342R7-qKOOqWJgaf3TDHx2M.CWGT'
+        >>> h.rev.rev == h
+        True
+        >>> h = Hosh.fromid("ab_cabcdefabcdefabcdefabcdefabcdefabcdef")
+        >>> h.rev.id
+        'Hh_c7201818f76878562c52010943fe4f2a7f3b2'
+        >>> h = Hosh.fromid("2_dbe78441d_____________________________")
+        >>> h.rev.id
+        '2_dbd14487e_____________________________'
+
+        >>> # Limits of subgroup Z.
+        >>> Hosh.fromid(groups[40].firstp).id,  Hosh.fromid(groups[40].lastp).id
+        ('0_100000000_____________________________', 'f_8afffffff_____________________________')
+        >>> Hosh.fromid(groups[40].firstp).rev.id,  Hosh.fromid(groups[40].lastp).rev.id
+        ('0_100000000_____________________________', 'f_8afffffff_____________________________')
+
+        >>> # Limits of subgroup H.
+        >>> Hosh.fromid(groups[40].firstp4).id, Hosh.fromid(groups[40].lastp4).id
+        ('00_1000000000000000000000000000000000000', '.._87c2a630003eec7dffff561b0000004aeffff')
+        >>> Hosh.fromid(groups[40].firstp4).rev.id, Hosh.fromid(groups[40].lastp4).rev.id
+        ('00_9ed100000015ffffffff00000000000000000', '.._87c2a630003eec7dffff561b0000004aeffff')
+        >>> Hosh.fromid(groups[40].firstp4).cells, Hosh.fromid(groups[40].lastp4).cells
+        ([0, 0, 0, 0, 1, 0], [0, 0, 1099511627688, 1099511627688, 1099511627688, 1099511627688])
+        >>> Hosh.fromid(groups[40].firstp4).rev.cells, Hosh.fromid(groups[40].lastp4).rev.cells
+        ([0, 0, 0, 1, 0, 0], [0, 0, 1099511627688, 1099511627688, 1099511627688, 1099511627688])
+
+        >>> # Limits of group G.
+        >>> Hosh.fromid(groups[40].firstp6).id, Hosh.fromid(groups[40].lastp6).id
+        ('1000000000000000000000000000000000000000', 'g-8KOjCQREq2Vz8VTc30gLMd..vvX6000ov.....')
+        >>> Hosh.fromid(groups[40].firstp6).rev.id, Hosh.fromid(groups[40].lastp6).rev.id
+        ('00_1000000000000000000000000000000000000', 'g-8KOjCQREq2Vz8VTc30gLMd..vvX6000ov.....')
+        >>> Hosh.fromid(groups[40].firstp6).cells, Hosh.fromid(groups[40].lastp6).cells
+        ([0, 1, 0, 0, 0, 0], [1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688])
+        >>> Hosh.fromid(groups[40].firstp6).rev.cells, Hosh.fromid(groups[40].lastp6).rev.cells
+        ([0, 0, 0, 0, 1, 0], [1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688])
+
+        >>> # Near limits of group G.
+        >>> Hosh.fromn(groups[40].p4+1).id, Hosh.fromn(groups[40].p6 - 2).id
+        ('2000000000000000000000000000000000000000', 'f-8KOjCQREq2Vz8VTc30gLMd..vvX6000ov.....')
+        >>> Hosh.fromn(groups[40].p4+1).rev.id, Hosh.fromn(groups[40].p6 - 2).rev.id
+        ('ihdwjXvMdIj40gZQq-..5Ai0000j-....3000000', '7XoPrombpt9-UXQnse30Cgud..fcZ6000kv.....')
+        >>> Hosh.fromn(groups[40].p4+1).cells, Hosh.fromn(groups[40].p6 - 2).cells
+        ([0, 1, 0, 0, 0, 1], [1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627687])
+        >>> Hosh.fromn(groups[40].p4+1).rev.cells, Hosh.fromn(groups[40].p6 - 2).rev.cells
+        ([1, 0, 0, 0, 1, 0], [1099511627687, 1099511627688, 1099511627688, 1099511627688, 1099511627688, 1099511627688])
         """
         if self._rev is None:
-            self._rev = Hosh.fromid("".join(reversed(self.id)))
+            id = self.id
+            if self.etype == "ordered":
+                self._rev = Hosh(list(reversed(self.cells)))
+            elif self.etype == "hybrid":
+                self._rev = Hosh(self.cells[:2] + list(reversed(self.cells[2:])))
+            elif self.etype == "unordered":
+                self._rev = Hosh.fromid(id[:4] + "".join(reversed(id[4:11])) + "_____________________________")
+            else:  # pragma: no cover
+                raise Exception(f"Unexpected condition. element type: {self.etype}")
         return self._rev
 
     @property
     def etype(self):
         """
         Type of this element
 
@@ -445,20 +513,14 @@
         elif GLOBAL["format"] == HTML:
             return self.shtml if GLOBAL["short"] else self.html
         elif callable(GLOBAL["format"]):  # pragma: no cover
             return GLOBAL["format"](self)
         else:  # pragma: no cover
             raise Exception(f"Unknown format: {GLOBAL['format']}")
 
-    # @property
-    # def bits(self):
-    #     if self._bits is None:
-    #         self._bits = bin(self.n)[2:].rjust(256, "0")
-    #     return self._bits
-
     def __xor__(self, other: int):
         if other == 1:
             return self
         return Hosh(cellspow(self.cells, other, self.p), version=self.version)
 
     def __mul__(self, other: Union["Hosh", str, bytes, int]):
         if (other := self.convert(other)) is NotImplemented:  # pragma: no cover
@@ -527,38 +589,21 @@
     def __floordiv__(self, other):
         """Lift"""
         if (other := self.convert(other)) is NotImplemented:  # pragma: no cover
             return NotImplemented
         return +(+self / +other)
 
     def __neg__(self):
-        """Change disposition of element-matrix cells in a way that even hybrid ids will not commute.
-        ps. This differs from +hosh because it creates a lower element.
-
-        Switch positions of cells a2 and a4. This operation is it own inverse.
-
-        Cells are represented as a list in the format: [a5, a4, a3, a2, a1, a0]
-        Cells are represented as a matrix in the format:
-        1 a4 a1 a0
-        0  1 a2 a3
-        0  0  1 a5
-        0  0  0  1
-
-        """
-        cells = self.cells.copy()
-        cells[3] = cells[1]
-        cells[1] = self.cells[3]
-        return Hosh(cells, version=self.version)
+        return Hosh(cellsinv(self.cells, self.p, additive=True), version=self.version)
 
     def __pos__(self):
         """Change disposition of element-matrix cells in a way that even hybrid ids will not commute.
-        ps. This differs from -hosh because it creates a higher element.
-        For this reason it is adopted in __floordiv__
+        ps. Semantics of +hosh are completely unrelated from -hosh as -hosh creates the inverse additive element.
 
-        Switch positions of cells a2 and a5. This operation is it own inverse.
+        Switch positions of cells a2 and a5. This operation is its own inverse.
 
         Cells are represented as a list in the format: [a5, a4, a3, a2, a1, a0]
         Cells are represented as a matrix in the format:
         1 a4 a1 a0
         0  1 a2 a3
         0  0  1 a5
         0  0  0  1
@@ -688,153 +733,287 @@
         True
         True
         True
         True
         """
         if k == 1:
             return self
-        return Hosh(cellsroot(self.cells, k, self.p))
+        return Hosh(cellsroot(self.cells, k, self.p), version=self.version)
+
+    def power_component(self, i, n):
+        """Elements corresponding to `n` components of "multiplicative decomposition" such that
+        `x  =  x1 * x2 * x3 * ... * xn  =  x * x² * x³ * ... * x^n`
 
-    def multiplicative_component(self, i, n):
-        """Elements within 'n' components of "multiplicative" decomposition
+        Not very useful as the resulting elements commute among themselves.
+        This happens because they are all powers of x, making up just a sequence of `x`s .
 
-        Resulting elements commute among themselves.
+        Parameters
+        ==========
+        i
+            Desired component index
+        n
+            Desired total number of components
+
+        Returns
+        =======
+            Hosh (component)
 
         >>> a = Hosh(b"a")
-        >>> a.multiplicative_component(0, 1) == a
+        >>> a.power_component(0, 1) == a
         True
-        >>> a.multiplicative_component(0, 2) * a.multiplicative_component(1, 2) == a
+        >>> a.power_component(0, 2) * a.power_component(1, 2) == a
         True
-        >>> a.multiplicative_component(0, 3) * a.multiplicative_component(1, 3) * a.multiplicative_component(2, 3) == a
+        >>> a.power_component(0, 3) * a.power_component(1, 3) * a.power_component(2, 3) == a
         True
-        >>> a.multiplicative_component(2, 3) * a.multiplicative_component(1, 3) * a.multiplicative_component(0, 3) == a
+        >>> a.power_component(2, 3) * a.power_component(1, 3) * a.power_component(0, 3) == a
         True
         """
         if i >= n:  # pragma: no cover
             raise Exception(f"Hosh component should be defined by 'index' ({i}) < '#components' ({n})")
         if n == 1:
             return self
         exp = n * (n + 1) // 2
         r = self.root(exp)
         return r ^ (i + 1)
 
-    def additive_decomposition(self, n):
+    def bad_additive_components(self, n):
         """
-        Return the 'n' additive components for 'x' such that 'x = c1+c2+...+cn'
+        Return the `n` additive components for `x` such that `x = x1 + x2 + ... + xn`
 
-        Remaining values are adjusted in 'cn'.
+        `xn` fills the gap left by the other components remainder.
+        We do not recommend this "decomposition" as it always generates different ids for the same subvalue.
+        For instance,
+            if a list `[value1, value2, value3]` induces ids `a`, `b`, and `any`,
+             another list `[value1, value2, ...]` necessarily induces `c` and `d` as first two ids such that `a != c` and `b != d`.
+
+        Parameters
+        ==========
+        n
+            Desired total number of components
+
+        Returns
+        =======
+            Generator of hoshes
 
         >>> from functools import reduce
         >>> import operator
-        >>> reduce(operator.add, Hosh(b"x").additive_decomposition(5)) == Hosh(b"x")
+        >>> reduce(operator.add, Hosh(b"x").bad_additive_components(5)) == Hosh(b"x")
         True
         """
         den = n * (n + 1) // 2
         p = self.p
 
         def fac(x):
             parc, rem = divmod(x + p, den)
             lst = [i * parc for i in range(1, n + 1)]
             lst[-1] += rem
             return [l % p for l in lst]
 
-        return (Hosh(list(x)) for x in zip(*(fac(c) for c in self.cells)))
+        return (Hosh(list(x), version=self.version) for x in zip(*(fac(c) for c in self.cells)))
 
-    def additive_component(self, i, n):
+    def bad_additive_component(self, i, n):
         """
-        Return the 'i'-th component of the additive decomposition of current hosh
+        Return the `i`-th additive component for `x` such that `x = x1 + x2 + ... + xn`
 
-        Remaining values are adjusted in the last component.
+        See `bad_additive_components` for more details.
 
         >>> from functools import reduce
         >>> import operator
-        >>> list(Hosh(b"x").additive_decomposition(2))[0] == Hosh(b"x").additive_component(0, 2)
+        >>> list(Hosh(b"x").bad_additive_components(2))[0] == Hosh(b"x").bad_additive_component(0, 2)
         True
-        >>> list(Hosh(b"x").additive_decomposition(2))[1] == Hosh(b"x").additive_component(1, 2)
+        >>> list(Hosh(b"x").bad_additive_components(2))[1] == Hosh(b"x").bad_additive_component(1, 2)
         True
-        >>> list(Hosh(b"x").additive_decomposition(3))[0] == Hosh(b"x").additive_component(0, 3)
+        >>> list(Hosh(b"x").bad_additive_components(3))[0] == Hosh(b"x").bad_additive_component(0, 3)
         True
-        >>> list(Hosh(b"x").additive_decomposition(3))[1] == Hosh(b"x").additive_component(1, 3)
+        >>> list(Hosh(b"x").bad_additive_components(3))[1] == Hosh(b"x").bad_additive_component(1, 3)
         True
-        >>> list(Hosh(b"x").additive_decomposition(3))[2] == Hosh(b"x").additive_component(2, 3)
+        >>> list(Hosh(b"x").bad_additive_components(3))[2] == Hosh(b"x").bad_additive_component(2, 3)
         True
-        >>> list(Hosh(b"x").additive_decomposition(5))[0] == Hosh(b"x").additive_component(0, 5)
+        >>> list(Hosh(b"x").bad_additive_components(5))[0] == Hosh(b"x").bad_additive_component(0, 5)
         True
-        >>> list(Hosh(b"x").additive_decomposition(5))[1] == Hosh(b"x").additive_component(1, 5)
+        >>> list(Hosh(b"x").bad_additive_components(5))[1] == Hosh(b"x").bad_additive_component(1, 5)
         True
-        >>> list(Hosh(b"x").additive_decomposition(5))[2] == Hosh(b"x").additive_component(2, 5)
+        >>> list(Hosh(b"x").bad_additive_components(5))[2] == Hosh(b"x").bad_additive_component(2, 5)
         True
-        >>> list(Hosh(b"x").additive_decomposition(5))[4] == Hosh(b"x").additive_component(4, 5)
+        >>> list(Hosh(b"x").bad_additive_components(5))[4] == Hosh(b"x").bad_additive_component(4, 5)
         True
-        >>> list(Hosh(b"x").additive_decomposition(7))[0] == Hosh(b"x").additive_component(0, 7)
+        >>> list(Hosh(b"x").bad_additive_components(7))[0] == Hosh(b"x").bad_additive_component(0, 7)
         True
-        >>> list(Hosh(b"x").additive_decomposition(7))[1] == Hosh(b"x").additive_component(1, 7)
+        >>> list(Hosh(b"x").bad_additive_components(7))[1] == Hosh(b"x").bad_additive_component(1, 7)
         True
-        >>> list(Hosh(b"x").additive_decomposition(7))[2] == Hosh(b"x").additive_component(2, 7)
+        >>> list(Hosh(b"x").bad_additive_components(7))[2] == Hosh(b"x").bad_additive_component(2, 7)
         True
-        >>> list(Hosh(b"x").additive_decomposition(7))[4] == Hosh(b"x").additive_component(4, 7)
+        >>> list(Hosh(b"x").bad_additive_components(7))[4] == Hosh(b"x").bad_additive_component(4, 7)
         True
         """
         den = n * (n + 1) // 2
         p = self.p
         i += 1
         toggle = 1 if i == n else 0
 
         def fac(x):
             parc, rem = divmod(x + p, den)
             return (i * parc + toggle * rem) % p
 
-        return Hosh(list(fac(c) for c in self.cells))
+        return Hosh(list(fac(c) for c in self.cells), version=self.version)
 
-    def __getitem__(self, item):
-        """
-        Multiplicative decomposition based on values extracted from id+index
+    def components(self, start, stop, n, additive=False):
+        r"""
+        Pseudo"decomposition" based on the hosh of the current id concatenated as bytes to a given component index
+
+        Perform a multiplicative decomposition by default.
 
         Syntax:
-            Hosh(b"blob")[:n]           # Takes all 'n' components.
-            Hosh(b"blob")[index:n]      # Takes a single component out of 'n'.
+            Hosh(b"blob").components(i, m, n)   # Takes a slice of elements.
+            Hosh(b"blob")[i:m, n]               # Takes a slice of elements.
+            Hosh(b"blob")[i, n]                 # Takes element `i` out of `n` components.
+            Hosh(b"blob")[:n, n]                # All `n` elements.
+        Warning:
+            Hosh(b"blob")[-1]                   # Reverse element. Not to be confused with inverse element.
+
 
-        Use arbitrarily internally defined elements based on current id:
-        id+"-_1", id+"-2", ..., id+"-n"
+        The components are arbitrarily internally defined group elements based on current id as hashed bytes:
+        Hosh(id+"-1"), Hosh(id+"-2"), ..., Hosh(id+"-n")
 
-        The last element makes the multiplication x1*x2*...*xn match x:
+        The last element (xn) is the exception as it makes the product x1 * x2 * ... * xn match x:
         x1      = id+"-1" * x
          ...
         xn-1    = id+"-n-1" * x
         xn      = (id+"-1" * x * ... * id+"-n-1")-¹
+
+        Parameters
+        ==========
+        start
+            Start of a slice
+        stop
+            Stop of a slice
+        n
+            Desired total number of components
+        additive
+            Set up an additive decomposition
+
+        Returns
+        =======
+            List if hoshes
+
+        >>> from hosh import Hosh
         >>> a = Hosh(b"a")
-        >>> a[0:1] == a
+        >>> a[-1].rev == a
         True
-        >>> a[:1] == [a]
+        >>> a[0, 1][0] == a
         True
-        >>> a[:3][0] * a[:3][1] * a[:3][2] == a
+        >>> a[0:, 1][0] == a
         True
-        >>> a[0:3] * a[1:3] * a[2:3] == a
+        >>> a[:1, 1][0] == a
         True
+        >>> a[0:1, 1][0] == a
+        True
+        >>> from operator import mul
+        >>> reduce(mul, a[:, 3]) == a
+        True
+        >>> [x.id for x in a[:, 3]]
+        ['Bd6Axil5pFSp15HUBz8eCujvu3gBsEk6XMpRsMNo', '32MloLPcivDbbPMCJn1RBY31aNZ6z-Dqnt4vQhot', 'la3xnZmlhn3lFBAnvWw-UWAvK.2hk-QqUNFYAs3e']
+        >>> a[:, 3][0] * a[:, 3][1] * a[:, 3][2] == a
+        True
+        >>> a[0, 3] * a[1, 3] * a[2, 3] == a
+        True
+        >>> a.id
+        'cIXBKPediDiOKabeZ6SthD04rnzaquNXaAEhSud4'
+        >>> from operator import add, mul
+        >>> from functools import reduce
+        >>> print("\n".join(x.id for x in a.components(0, 7, 7)))
+        Bd6Axil5pFSp15HUBz8eCujvu3gBsEk6XMpRsMNo
+        32MloLPcivDbbPMCJn1RBY31aNZ6z-Dqnt4vQhot
+        Y2JlyuF8.KJc0DvvcIivLA5uLYloF7HN9ovO14Sq
+        6.F-NB-G4vBXs7evbBImex9x3foNi85Ca7wDb1c3
+        tZmUsjVcZAGTajUOzsSNrr7a7BQVNSiA6xaiPEYf
+        iCLMdAlduXvUtK1.awng0D0YP49kV8Cit7OLXyab
+        BA6UvITsIN822llT9eErc1R0rmf.ARbc0adwEbWk
+        >>> reduce(mul, a.components(0, 2, 7)) * reduce(mul, a.components(2, 3, 7)) * reduce(mul, a.components(3, 7, 7)) == a
+        True
+        >>> reduce(mul, a.components(0, 7, 7)) == a
+        True
+
+        >>> print("\n".join(x.id for x in a.components(0, 7, 7, additive=True)))
+        Bd6Axil5pFSp15HUBz8eCujvu3gBsEk6XMpRsMNo
+        32MloLPcivDbbPMCJn1RBY31aNZ6z-Dqnt4vQhot
+        Y2JlyuF8.KJc0DvvcIivLA5uLYloF7HN9ovO14Sq
+        6.F-NB-G4vBXs7evbBImex9x3foNi85Ca7wDb1c3
+        tZmUsjVcZAGTajUOzsSNrr7a7BQVNSiA6xaiPEYf
+        iCLMdAlduXvUtK1.awng0D0YP49kV8Cit7OLXyab
+        7jJmsfrPpa2CeeYCAiByF3HW2J9.ARbc0adwEbWk
+        >>> reduce(add, a.components(0, 2, 7, additive=True)) + reduce(add, a.components(2, 3, 7, additive=True)) + reduce(add, a.components(3, 7, 7, additive=True)) == a
+        True
+        >>> reduce(add, a.components(0, 7, 7, additive=True)) == a
+        True
+        """
+        if stop > n:  # pragma: no cover
+            raise Exception(f"Wrong value:   stop=`{stop}`  >=  n=`{n}`")
+        acc = self.ø
+        operator = add if additive else mul
+        for i in range(0, stop):
+            if stop == n and i == stop - 1:
+                break
+            if (t := (i, n, additive)) not in self._composition_memo:
+                self._composition_memo[t] = Hosh(f"{self.id}-{i}".encode(), version=self.version)
+                if len(self._composition_memo) > self.components_cache_size:  # pragma: no cover
+                    first = next(iter(self._composition_memo))
+                    del self._composition_memo[first]
+            h = self._composition_memo[t]
+            acc = operator(acc, h)
+            if i >= start:
+                yield h
+        if stop == n:
+            inv = Hosh(cellsinv(acc.cells, self.p, additive), version=self.version)
+            last = operator(inv, self)
+            yield last
+
+    def __getitem__(self, item: Union[int, tuple]):
+        """
+        Reverse element:    Hosh(b"blob")[-1]
+        """
+        if item == -1:
+            return self.rev
+        if not isinstance(item, tuple) or len(item) != 2:  # pragma: no cover
+            raise Exception("Wrong syntax, tuple or `-1` expected: hosh[-1] or hosh[i, n] or hosh[l:m, n]")
+        slc, n = item
+        if n <= 0:  # pragma: no cover
+            raise Exception(f"Wrong value: n={n}  <=  0")
 
-        """
-        if not isinstance(item, slice) or item.step is not None or (n := item.stop) is None:  # pragma: no cover
-            raise Exception("Wrong syntax, expected: hosh[:n] or hosh[index:n]")
-        if (index := item.start) is not None:
-            if index >= n or index < 0:  # pragma: no cover
-                raise Exception(f"Wrong values: i ({index}) >= n ({n}) (or negative)")
+        if isinstance(idx := slc, int):
+            if idx < n - 1:
+                return Hosh(f"{self.id}-{idx}".encode())
             if n == 1:
-                return self
-            if index < n - 1:
-                return Hosh(f"{self.id}-{index}".encode())
-            return ~self.composition_nolast(n) * self
+                return [self]
+            if idx == n - 1:
+                return list(self.components(0, n, n))[idx]
+            raise Exception(f"Wrong value: i={slc}  >  n={n}")  # pragma: no cover
+
+        if not isinstance(slc, slice) or slc.step is not None:  # pragma: no cover
+            raise Exception(f"Wrong syntax. Simple slice or index expected as first tuple item, not `{slc}`: hosh[i, n] or hosh[l:m, n]")
+
+        if (start := slc.start) is None:
+            start = 0
+        if (stop := slc.stop) is None:
+            stop = n
+
+        if start > n or start < 0:  # pragma: no cover
+            raise Exception(f"Wrong values, expected: 0  <=  i={start}  <=  n={n}")
         if n == 1:
             return [self]
-        if n <= 0:  # pragma: no cover
-            raise Exception(f"Wrong value: n ({n}) <= 0")
-        lst = [Hosh(f"{self.id}-{i}".encode()) for i in range(n - 1)]
-        lst.append(~reduce(operator.mul, lst) * self)
-        return lst
-
-    def composition_nolast(self, n):
-        if n not in self._composition_nolast:
-            if len(self._composition_nolast) > 5:  # pragma: no cover
-                first = next(iter(self._composition_nolast))
-                del self._composition_nolast[first]
-            gen = (Hosh(f"{self.id}-{i}".encode()) for i in range(n - 1))
-            self._composition_nolast[n] = reduce(operator.mul, gen)
-        return self._composition_nolast[n]
+        return list(self.components(start, stop, n))
+
+    @property
+    def bits(self):
+        """
+        >>> from hosh import Hosh, groups
+        >>> Hosh(b"asd").bits
+        '000110111101001001111010010101011100011010000011101010100000000001101101111101100111110100001011001001111001110110101101100110000000011111000110100100110011110010101110100011111101100010010111100111010101010011001110000001000100001101001111'
+        >>> bits = Hosh.fromn(groups[40].p6 - 1).bits  # Max number.
+        >>> bits
+        '111111111111111111111111111111011111011000000000000000000000000110111011011111101111111111111111001101110000101001110100000000000011001100111000100101011110111011111001000010011000001000000100101101100110010011110110001000101011101110110000'
+        >>> int(bits, 2) == groups[40].p6 - 1
+        True
+        """
+        if self._bits is None:
+            self._bits = '{:b}'.format(self.n).rjust(self.digits * 6, "0")
+        return self._bits
```

### Comparing `hosh-2.230205.2/src/hosh/misc/__init__.py` & `hosh-3.230705.1/src/hosh/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/colors.py` & `hosh-3.230705.1/src/hosh/misc/colors.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/core.py` & `hosh-3.230705.1/src/hosh/misc/core.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/__init__.py` & `hosh-3.230705.1/src/hosh/misc/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/base.py` & `hosh-3.230705.1/src/hosh/misc/encoding/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     ... except Exception as e:
     ...     print(e)
     Invalid position for '_' in id 32t42t4_tr32t32t23t32t32t432t42t4_tr32t32t23t32t32t432t42t4_tr32
     >>> try:
     ...     id2n("3212t32t432t32t422t32t23t32t32t432t432t32t23t32.................", p)
     ... except Exception as e:
     ...     print(e)
-    Ordered id (3212t32t432t32t422t32t23t32t32t432t432t32t23t32.................) with n 39402006196394479212279040100136092515698659329147013992262201319596801387366846232950291543016464135950927013148147 outside allowed range for its kind: [115792089237316193942174975457431254695161196299352022581048345476735855814001;39402006196394478456139629384141450683325994812909116356652328479007639701989040511471346632255226219324457074810248].
+    Ordered id (3212t32t432t32t422t32t23t32t32t432t432t32t23t32.................) with n 39402006196394479212279040100136092515698659329147013992262201319596801387366846232950291543016464135950927013148147 outside allowed range for its element type: [115792089237316193942174975457431254695161196299352022581048345476735855814001;39402006196394478456139629384141450683325994812909116356652328479007639701989040511471346632255226219324457074810248].
 
     Parameters
     ----------
     id
     p
 
     Returns
@@ -164,15 +164,15 @@
         if n == 0:
             return 0
         n += p ** 4 - 1
         kind, lower, upper = "Ordered", p ** 4, p ** 6 - 1
     else:  # pragma: no cover
         raise Exception(f"Invalid position for '_' in id {id}")
     if not lower <= n <= upper:  # pragma: no cover
-        raise Exception(f"{kind} id ({id}) with n {n} outside allowed range for its kind: [{lower};{upper}].")
+        raise Exception(f"{kind} id ({id}) with n {n} outside allowed range for its element type: [{lower};{upper}].")
     return n
 
 
 def n2id(num, digits, p):
     """
     Usage:
```

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/base777.py` & `hosh-3.230705.1/src/hosh/misc/encoding/base777.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/exception.py` & `hosh-3.230705.1/src/hosh/misc/exception.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/helper.py` & `hosh-3.230705.1/src/hosh/misc/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     """Internal use only.
 
     Not to be directly instantiated."""
 
     version: str
 
     def __call__(self, blob, etype="ordered"):
-        return Hosh(blob, etype, self.version)
+        return Hosh(blob, etype=etype, version=self.version)
 
     def u(self, blob):
-        return Hosh(blob, "unordered", self.version)
+        return Hosh(blob, etype="unordered", version=self.version)
 
     def h(self, blob):
-        return Hosh(blob, "hybrid", self.version)
+        return Hosh(blob, etype="hybrid", version=self.version)
 
     fromid = Hosh.fromid
     fromn = Hosh.fromn
```

### Comparing `hosh-2.230205.2/src/hosh/misc/identity.py` & `hosh-3.230705.1/src/hosh/misc/identity.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/math.py` & `hosh-3.230705.1/src/hosh/misc/math.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,42 +123,54 @@
         (a[2] + b[2] + a[3] * b[0]) % mod,
         (a[3] + b[3]) % mod,
         (a[4] + b[4] + a[1] * b[3]) % mod,
         (a[5] + b[5] + a[1] * b[2] + a[4] * b[0]) % mod,
     ]
 
 
-def cellsinv(m, mod):
+def cellsinv(m, mod, additive=False):
     """
     Inverse of unitriangular matrix modulo 'mod'
 
     'm' given as a list in the format: [a5, a4, a3, a2, a1, a0]
 
     1 a4 a1 a0
     0  1 a2 a3
     0  0  1 a5
     0  0  0  1
 
     Based on https://groupprops.subwiki.org/wiki/Unitriangular_matrix_group:UT(4,p)
 
+    >>> from hosh.misc.math import cellsinv
     >>> e = [42821,772431,428543,443530,42121,7213]
-    >>> cellsinv(cellsinv(e, 4294967291), 4294967291)==e
+    >>> cellsinv(cellsinv(e, 4294967291), 4294967291) == e
     True
 
+    >>> cellsinv(cellsinv(e, 4294967291, additive=True), 4294967291, additive=True) == e
+    True
+
+    >>> e = [1,2,3,4,5,6]
+    >>> cellsinv(e, 7, additive=True)
+    [6, 5, 4, 3, 2, 1]
+
     Parameters
     ----------
     m
         List with six values
     mod
         Large prime number
+    additive
+        Whether to calculate additive inverse or not (multiplicative)
 
     Returns
     -------
         The list that corresponds to the inverse element
     """
+    if additive:
+        return [(mod - m[0]) % mod, (mod - m[1]) % mod, (mod - m[2]) % mod, (mod - m[3]) % mod, (mod - m[4]) % mod, (mod - m[5]) % mod]
     return [
         -m[0] % mod,
         -m[1] % mod,
         (m[3] * m[0] - m[2]) % mod,
         -m[3] % mod,
         (m[1] * m[3] - m[4]) % mod,
         (m[1] * m[2] + m[4] * m[0] - m[1] * m[3] * m[0] - m[5]) % mod,
```

### Comparing `hosh-2.230205.2/src/hosh/misc/root.py` & `hosh-3.230705.1/src/hosh/misc/root.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/theme.py` & `hosh-3.230705.1/src/hosh/theme.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/setup.py` & `hosh-3.230705.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 ['hosh', 'hosh.misc', 'hosh.misc.encoding']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ansi2html>=1.6.0,<2.0.0',
- 'blake3>=0.2.0,<0.3.0',
+ 'blake3>=0.3.3,<0.4.0',
  'bs4>=0.0.1,<0.0.2',
  'colored==1.4.2',
- 'wheel>=0.37.0,<0.38.0']
+ 'wheel>=0.40.0,<0.41.0']
 
 setup_kwargs = {
     'name': 'hosh',
-    'version': '2.230205.2',
+    'version': '3.230705.1',
     'description': 'Predictable Operable HaSH-based identifiers',
-    'long_description': '![test](https://github.com/davips/hosh/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)\n<a href="https://pypi.org/project/hosh">\n<img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n\n\n# hosh - Identification based on group theory\n[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https://davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).\nA previous version, containing extra group theory content, is available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA first implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh` and serves as an advanced usage example.\n<br>\nA second (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/project/hoshmap).\nThe most recent rewritten version of a hosh-based dict (and the most robust, recommended, one) is available in the package [hdict](https://pypi.org/project/hdict).\n\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/hosh) \nand [GitHub repository](https://github.com/davips/hosh), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/hosh/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/hosh).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install hosh\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/hosh\ncd hosh\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom hosh import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n\n## Performance\nComputation time for the simple operations performed by `hosh` can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_6.png)\nThe package [hoshrust](https://pypi.org/project/hoshrust) was a faster implementation of an earlier version of `hosh`.\nAs the performance of the current `hosh` seems already very high (only ~2x slower than if it was implemented in native code in like _rust_), \nwe don\'t have plans for a new \'rust\' implementation in the near future.\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
+    'long_description': '![test](https://github.com/davips/hosh/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)\n<a href="https://pypi.org/project/hosh">\n<img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)\n\n# hosh - Identification based on group theory\n[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https://davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).\nA previous version, containing extra group theory content, is available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA first implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh` and serves as an advanced usage example.\n<br>\nA second (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/project/hoshmap).\nThe most recent rewritten version of a hosh-based dict (and the most robust, recommended, one) is available in the package [hdict](https://pypi.org/project/hdict).\n\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/hosh) \nand [GitHub repository](https://github.com/davips/hosh), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/hosh/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/hosh).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install hosh\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/hosh\ncd hosh\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom hosh import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n\n## Performance\nComputation time for the simple operations performed by `hosh` can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_6.png)\nThe package [hoshrust](https://pypi.org/project/hoshrust) was a faster implementation of an earlier version of `hosh`.\nAs the performance of the current `hosh` seems already very high (only ~2x slower than if it was implemented in native code in like _rust_), \nwe don\'t have plans for a new \'rust\' implementation in the near future.\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hosh', 'hosh.misc', 'hosh.misc.encoding'] package_data =
 \ {'': ['*']} install_requires = \ ['ansi2html>=1.6.0,<2.0.0',
-'blake3>=0.2.0,<0.3.0', 'bs4>=0.0.1,<0.0.2', 'colored==1.4.2',
-'wheel>=0.37.0,<0.38.0'] setup_kwargs = { 'name': 'hosh', 'version':
-'2.230205.2', 'description': 'Predictable Operable HaSH-based identifiers',
+'blake3>=0.3.3,<0.4.0', 'bs4>=0.0.1,<0.0.2', 'colored==1.4.2',
+'wheel>=0.40.0,<0.41.0'] setup_kwargs = { 'name': 'hosh', 'version':
+'3.230705.1', 'description': 'Predictable Operable HaSH-based identifiers',
 'long_description': '![test](https://github.com/davips/hosh/workflows/test/
 badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/
 badge.svg)](https://codecov.io/gh/davips/hosh)\n\n[pypi]\n\n![Python version]
-(https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL
-v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
+(https://img.shields.io/badge/python-â¥3.8-blue.svg)\n[![license: GPL v3]
+(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/
 zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https:/
 /img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
 arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
 API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual]
 (https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://
-hosh.page)\n\n\n# hosh - Identification based on group theory\n[Website](https:
-//hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current
-Code](https://github.com/davips/hosh) |\n[API Documentation](https://
-davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh)
-/ [code](https://github.com/davips/hosh) provides a reference implementation
-for the UT*.4 specification presented [here](https://arxiv.org/abs/
-2109.06028).\nA previous version, containing extra group theory content, is
+hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hosh)](https://
+pepy.tech/project/hosh)\n\n# hosh - Identification based on group theory\n
+[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh)
+|\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https:
+//davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/
+hosh) / [code](https://github.com/davips/hosh) provides a reference
+implementation for the UT*.4 specification presented [here](https://arxiv.org/
+abs/2109.06028).\nA previous version, containing extra group theory content, is
 available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease
 see the [website](https://hosh.page) for more detailed usage information.\n\nWe
 adopt a novel paradigm to universally unique identification (UUID), making
 identifiers deterministic and predictable, \neven before an object is generated
 by a (possibly costly) process. \nHere, data versioning and composition of
 processing steps are directly mapped as simple operations over identifiers.\nWe
 call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable
```

### Comparing `hosh-2.230205.2/PKG-INFO` & `hosh-3.230705.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: hosh
-Version: 2.230205.2
+Version: 3.230705.1
 Summary: Predictable Operable HaSH-based identifiers
 License: GPL
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansi2html (>=1.6.0,<2.0.0)
-Requires-Dist: blake3 (>=0.2.0,<0.3.0)
+Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: colored (==1.4.2)
-Requires-Dist: wheel (>=0.37.0,<0.38.0)
+Requires-Dist: wheel (>=0.40.0,<0.41.0)
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)
 <a href="https://pypi.org/project/hosh">
 <img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
-
+[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)
 
 # hosh - Identification based on group theory
 [Website](https://hosh.page) |
 [Latest Release](https://pypi.org/project/hosh) |
 [Current Code](https://github.com/davips/hosh) |
 [API Documentation](https://davips.github.io/hosh)
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: hosh Version: 2.230205.2 Summary: Predictable
+Metadata-Version: 2.1 Name: hosh Version: 3.230705.1 Summary: Predictable
 Operable HaSH-based identifiers License: GPL Author: davips Author-email:
 dpsabc@gmail.com Requires-Python: >=3.8 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: ansi2html
-(>=1.6.0,<2.0.0) Requires-Dist: blake3 (>=0.2.0,<0.3.0) Requires-Dist: bs4
+(>=1.6.0,<2.0.0) Requires-Dist: blake3 (>=0.3.3,<0.4.0) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: colored (==1.4.2) Requires-Dist: wheel
-(>=0.37.0,<0.38.0) Description-Content-Type: text/markdown ![test](https://
+(>=0.40.0,<0.41.0) Description-Content-Type: text/markdown ![test](https://
 github.com/davips/hosh/workflows/test/badge.svg) [![codecov](https://
 codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/
 davips/hosh) [pypi] ![Python version](https://img.shields.io/badge/python-
-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
-License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
+â¥3.8-blue.svg) [![license: GPL v3](https://img.shields.io/badge/License-
+GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
 zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/
 zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
 b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
 documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hosh) [![Manual](https://img.shields.io/badge/manual-
-handcrafted-a030a0.svg)](https://hosh.page) # hosh - Identification based on
-group theory [Website](https://hosh.page) | [Latest Release](https://pypi.org/
-project/hosh) | [Current Code](https://github.com/davips/hosh) | [API
-Documentation](https://davips.github.io/hosh) This [Python library](https://
-pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a
-reference implementation for the UT*.4 specification presented [here](https://
-arxiv.org/abs/2109.06028). A previous version, containing extra group theory
-content, is available in the package [GaROUPa](https://pypi.org/project/
-garoupa). Please see the [website](https://hosh.page) for more detailed usage
-information. We adopt a novel paradigm to universally unique identification
-(UUID), making identifiers deterministic and predictable, even before an object
-is generated by a (possibly costly) process. Here, data versioning and
-composition of processing steps are directly mapped as simple operations over
-identifiers. We call each of the latter a `Hosh`, i.e., an identifier is an
-_**o**perable **h**a**sh**_. A first implementation of the remaining ideas from
-the [paper](https://arxiv.org/abs/2109.06028) is provided in this [cacheable
-lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh`
-and serves as an advanced usage example.
+handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh) # hosh -
+Identification based on group theory [Website](https://hosh.page) | [Latest
+Release](https://pypi.org/project/hosh) | [Current Code](https://github.com/
+davips/hosh) | [API Documentation](https://davips.github.io/hosh) This [Python
+library](https://pypi.org/project/hosh) / [code](https://github.com/davips/
+hosh) provides a reference implementation for the UT*.4 specification presented
+[here](https://arxiv.org/abs/2109.06028). A previous version, containing extra
+group theory content, is available in the package [GaROUPa](https://pypi.org/
+project/garoupa). Please see the [website](https://hosh.page) for more detailed
+usage information. We adopt a novel paradigm to universally unique
+identification (UUID), making identifiers deterministic and predictable, even
+before an object is generated by a (possibly costly) process. Here, data
+versioning and composition of processing steps are directly mapped as simple
+operations over identifiers. We call each of the latter a `Hosh`, i.e., an
+identifier is an _**o**perable **h**a**sh**_. A first implementation of the
+remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided
+in this [cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which
+depends on `hosh` and serves as an advanced usage example.
 A second (entirely rewritten) version is available in the package [idict]
 (https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/
 project/hoshmap). The most recent rewritten version of a hosh-based dict (and
 the most robust, recommended, one) is available in the package [hdict](https://
 pypi.org/project/hdict). ## Overview A product of identifiers produces a new
 identifier as shown below, where sequences of bytes (`b"..."`) are passed to
 simulate binary objects to be hashed. ![img.png](https://
```

