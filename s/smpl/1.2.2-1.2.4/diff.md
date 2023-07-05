# Comparing `tmp/smpl-1.2.2.tar.gz` & `tmp/smpl-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpl-1.2.2.tar", max compression
+gzip compressed data, was "smpl-1.2.4.tar", max compression
```

## Comparing `smpl-1.2.2.tar` & `smpl-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-03-21 14:46:00.070523 smpl-1.2.2/LICENSE
--rw-r--r--   0        0        0     3186 2023-03-21 14:46:00.070523 smpl-1.2.2/README.md
--rw-r--r--   0        0        0     1999 2023-03-21 14:46:03.322541 smpl-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      134 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/__init__.py
--rw-r--r--   0        0        0     3857 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/data.py
--rw-r--r--   0        0        0       74 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/debug.py
--rw-r--r--   0        0        0     2088 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/doc.py
--rw-r--r--   0        0        0    10497 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/fit.py
--rw-r--r--   0        0        0     2177 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/functions.py
--rw-r--r--   0        0        0     5161 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/interpolate.py
--rw-r--r--   0        0        0       62 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/io.py
--rw-r--r--   0        0        0     3062 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/latex.py
--rw-r--r--   0        0        0       85 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/parallel.py
--rw-r--r--   0        0        0    26117 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/plot.py
--rw-r--r--   0        0        0     6309 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/plot2d.py
--rw-r--r--   0        0        0     9652 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/stat.py
--rw-r--r--   0        0        0       66 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/util.py
--rw-r--r--   0        0        0     5302 2023-03-21 14:46:00.090523 smpl-1.2.2/smpl/wrap.py
--rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 smpl-1.2.2/setup.py
--rw-r--r--   0        0        0     4294 1970-01-01 00:00:00.000000 smpl-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-05 09:57:40.857050 smpl-1.2.4/LICENSE
+-rw-r--r--   0        0        0     3186 2023-07-05 09:57:40.857050 smpl-1.2.4/README.md
+-rw-r--r--   0        0        0     2040 2023-07-05 09:57:42.725098 smpl-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/__init__.py
+-rw-r--r--   0        0        0     3875 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/data.py
+-rw-r--r--   0        0        0       74 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/debug.py
+-rw-r--r--   0        0        0     2088 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/doc.py
+-rw-r--r--   0        0        0    10570 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/fit.py
+-rw-r--r--   0        0        0     2177 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/functions.py
+-rw-r--r--   0        0        0     5185 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/interpolate.py
+-rw-r--r--   0        0        0       62 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/io.py
+-rw-r--r--   0        0        0     3062 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/latex.py
+-rw-r--r--   0        0        0       85 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/parallel.py
+-rw-r--r--   0        0        0    26417 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/plot.py
+-rw-r--r--   0        0        0     6327 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/plot2d.py
+-rw-r--r--   0        0        0     9652 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/stat.py
+-rw-r--r--   0        0        0       66 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/util.py
+-rw-r--r--   0        0        0     5302 2023-07-05 09:57:40.873050 smpl-1.2.4/smpl/wrap.py
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 smpl-1.2.4/setup.py
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 smpl-1.2.4/PKG-INFO
```

### Comparing `smpl-1.2.2/LICENSE` & `smpl-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/README.md` & `smpl-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/pyproject.toml` & `smpl-1.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "smpl"
-version = "1.2.2"
+version = "1.2.4"
 description = "SiMPLe plotting and fitting"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/smpl"
 
 [tool.poetry.dependencies]
+python = "^3.8"
 smpl_debug     = "^1.0.5"
 smpl_io        = "^1.0.5"
 smpl_doc       = "^1.0.5"
 smpl_util      = "^1.0.5"
-smpl_parallel      = "^1.0.5"
-python = "^3.8"
-uncertainties="*"
-numpy="*"
-matplotlib="*"
-scipy  = ">=1.7.0"
-sympy= "*"
+smpl_parallel  = "^1.0.5"
+uncertainties = "*"
+numpy = "*"
+matplotlib = "*"
+scipy = ">=1.7.0"
+sympy = "*"
 tqdm = "*"
 pandas = ">=1.0.0"
-deprecation ="*"
+deprecation = "*"
 
-iminuit = {version = "<=2.18.0", optional = true} # StopIteration error in >=2.21.0 ?
+iminuit = {version = "*", optional = true} 
 smpl_animation= {version = "*", optional = true}
 
 [tool.poetry.extras]
 opt = ["iminuit"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "*"
+sphinx = "<7.0.0" # https://github.com/readthedocs/sphinx_rtd_theme/issues/1463
 sphinx-rtd-theme = "*"
 sphinxcontrib-napoleon = "*"
 nbsphinx = "*"
 jupyter-sphinx = "*"
 sphinx-autoapi = "*"
 sphinx_autobuild = "*"
 sphinx_math_dollar = "*"
@@ -45,24 +45,24 @@
 myst-parser  = "*"
 toml = "*"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
+pre-commit = ">=2.20,<4.0"
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.5"
 #pytest-line-profiler-apn = {path="/home/apn/git/pytest-line-profiler", develop = true}
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.25.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `smpl-1.2.2/smpl/data.py` & `smpl-1.2.4/smpl/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 }
 
 
 unv = unp.nominal_values
 usd = unp.std_devs
 
 
-@doc.append_str(doc.table(default, init=False))
-@doc.append_str(doc.table({"data_kwargs": ["default", "description"]}, bottom=False))
+@doc.append_str(doc.array_table(default, init=False))
+@doc.append_str(
+    doc.array_table({"data_kwargs": ["default", "description"]}, bottom=False)
+)
 @doc.append_str("\n\n")
 def data_kwargs(kwargs):
     """Set default :func:`data_kwargs` if not set."""
     for k, v in default.items():
         if not k in kwargs:
             kwargs[k] = v[0]
     return kwargs
```

### Comparing `smpl-1.2.2/smpl/doc.py` & `smpl-1.2.4/smpl/doc.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/smpl/fit.py` & `smpl-1.2.4/smpl/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,18 @@
 }
 
 # @doc.insert_str("\tDefault kwargs\n\n\t")
 
 
 @doc.append_doc(data.data_kwargs)
 @doc.append_str("\t")
-@doc.append_str(doc.table(default, init=False))
-@doc.append_str(doc.table({"fit_kwargs": ["default", "description"]}, bottom=False))
+@doc.append_str(doc.array_table(default, init=False))
+@doc.append_str(
+    doc.array_table({"fit_kwargs": ["default", "description"]}, bottom=False)
+)
 @doc.append_str("\n\n")
 def fit_kwargs(kwargs):
     """Set default :func:`fit_kwargs` if not set."""
     kwargs = data.data_kwargs(kwargs)
     for k, v in default.items():
         if not k in kwargs:
             kwargs[k] = v[0]
@@ -104,22 +106,22 @@
     if funcs is None:
         funcs = list(functions.__dict__.values())
     for f in tqdm(funcs, disable=not kwargs["autotqdm"]):
         if callable(f):
             try:
                 ff = fit(datax, datay, f, **kwargs)
                 fy = f(datax, *ff)
-            except (ValueError, LinAlgError) as ve:
+                sum_sq = (
+                    np.sum((fy - datay) ** 2)
+                    + np.sum((fy + usd(fy) - datay) ** 2)
+                    + np.sum((fy - usd(fy) - datay) ** 2)
+                )
+            except (ValueError, LinAlgError, OverflowError) as ve:
                 debug.msg(ve)
                 continue
-            sum_sq = (
-                np.sum((fy - datay) ** 2)
-                + np.sum((fy + usd(fy) - datay) ** 2)
-                + np.sum((fy - usd(fy) - datay) ** 2)
-            )
             if min_sq is None or sum_sq < min_sq:
                 min_sq = sum_sq
                 best_f = f
                 best_ff = ff
     # if not best_f is None:
     #    fit(datax,datay,best_f,**kwargs)
     return best_f, best_ff, lambda x: best_f(x, *best_ff)
@@ -184,34 +186,35 @@
         params = [1 for i in range(N - 1)]
     tmp_params = []
     for i, pi in enumerate(params):
         if not util.has(i + 1, fixed):
             tmp_params += [pi]
     params = tmp_params
     N = len(params)
+    wlambda = wrap.get_lambda(function, kwargs["xvar"])
 
-    def _wrapped_func(*x):
+    def _wrapped_func(x0, *x):
         """
         wrapper for function with fixed parameters applied.
         """
         tmp_x = []
         j = 1
         # print(x)
         for i in range(1, Ntot + 1):
             # print(i," ",j)
             if not util.has(i, fixed):
-                tmp_x += [x[j]]
+                tmp_x += [x[j - 1]]
                 # print(x[j])
                 j = j + 1
             else:
                 tmp_x += [fixed[i]]
 
         # print(Ntot)
         # print(tmp_x)
-        return unv(wrap.get_lambda(function, kwargs["xvar"])(x[0], *tmp_x))
+        return unv(wlambda(x0, *tmp_x))
 
     return _wrapped_func, params, fixed, Ntot
 
 
 def _unwrap_param(fitt, fixed, Ntot):
     rfit = []
     j = 0
@@ -292,15 +295,15 @@
     # fix slice issue from iminuites rewritten __getitem__ by using super
     return unc.correlated_values(m.values, super(Matrix, m.covariance))
 
 
 import warnings
 
 from scipy import optimize
-from scipy.odr.odrpack import ODR, Model, RealData
+from scipy.odr import ODR, Model, RealData
 
 # fittet ein dataset mit gegebenen x und y werten, eine funktion und ggf. anfangswerten und y-Fehler
 # gibt die passenden parameter der funktion, sowie dessen unsicherheiten zurueck
 #
 # https://stackoverflow.com/questionsquestions/14581358/getting-standard-errors-on-fitted-parameters-using-the-optimize-leastsq-method-i#
 # Updated on 4/6/2016
 # User: https://stackoverflow.com/users/1476240/pedro-m-duarte
```

### Comparing `smpl-1.2.2/smpl/functions.py` & `smpl-1.2.4/smpl/functions.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/smpl/interpolate.py` & `smpl-1.2.4/smpl/interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import numpy as np
 import uncertainties as unc
 import uncertainties.unumpy as unp
 from scipy import interpolate as interp
 
 # from smpl import plot as splot
-from smpl import data
-from smpl.doc import append_doc, append_str, table
+from smpl import data, doc
+from smpl.doc import append_doc, append_str
 
 unv = unp.nominal_values
 usd = unp.std_devs
 
 
 def identity(x):
     return x
@@ -41,16 +41,18 @@
 }
 
 # @doc.insert_str("\tDefault kwargs\n\n\t")
 
 
 @append_doc(data.data_kwargs)
 @append_str("\t")
-@append_str(table(default, init=False))
-@append_str(table({"interpolate_kwargs": ["default", "description"]}, bottom=False))
+@append_str(doc.array_table(default, init=False))
+@append_str(
+    doc.array_table({"interpolate_kwargs": ["default", "description"]}, bottom=False)
+)
 def interpolate_kwargs(kwargs):
     """Set default interpolate_kwargs if not set."""
     kwargs = data.data_kwargs(kwargs)
     for k, v in default.items():
         if not k in kwargs:
             kwargs[k] = v[0]
     return kwargs
```

### Comparing `smpl-1.2.2/smpl/latex.py` & `smpl-1.2.4/smpl/latex.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/smpl/plot.py` & `smpl-1.2.4/smpl/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,17 +216,17 @@
     ],
     "alpha": [0.2, "alpha value for the fill_between plot"],
 }
 
 
 @doc.append_doc(ffit.fit_kwargs)
 @doc.append_str("\t")
-@doc.append_str(doc.table(default, init=False))
+@doc.append_str(doc.array_table(default, init=False))
 @doc.append_str(
-    doc.table({"plot_kwargs        ": ["default", "description"]}, bottom=False)
+    doc.array_table({"plot_kwargs        ": ["default", "description"]}, bottom=False)
 )
 @doc.append_str("\n\n")
 def plot_kwargs(kwargs):
     """Set default :func:`plot_kwargs` if not set."""
     kwargs = ffit.fit_kwargs(kwargs)
     for k, v in default.items():
         if not k in kwargs:
@@ -579,26 +579,34 @@
         else:
             (ll,) = plt.plot(
                 x, y, kwargs["fmt"], label=kwargs["label"], color=kwargs["data_color"]
             )
     else:
         if kwargs["fmt"] is None:
             if kwargs["linestyle"] is None:
-                ll, _, _, = plt.errorbar(
+                (
+                    ll,
+                    _,
+                    _,
+                ) = plt.errorbar(
                     x,
                     y,
                     yerr=yerr,
                     xerr=xerr,
                     fmt=" ",
                     capsize=kwargs["capsize"],
                     label=kwargs["label"],
                     color=kwargs["data_color"],
                 )
             else:
-                ll, _, _, = plt.errorbar(
+                (
+                    ll,
+                    _,
+                    _,
+                ) = plt.errorbar(
                     x,
                     y,
                     yerr=yerr,
                     xerr=xerr,
                     fmt=" ",
                     capsize=kwargs["capsize"],
                     label=kwargs["label"],
@@ -627,28 +635,36 @@
                     y + yerr,
                     label=kwargs["label"],
                     alpha=kwargs["alpha"],
                     step="mid",
                     color=ll.get_color(),
                 )
         elif kwargs["fmt"] == "hist":
-            ll, _, _, = plt.errorbar(
+            (
+                ll,
+                _,
+                _,
+            ) = plt.errorbar(
                 x,
                 y,
                 yerr=yerr,
                 xerr=xerr,
                 fmt=" ",
                 capsize=kwargs["capsize"],
                 color="black",
             )
             plt.fill_between(
                 x, y, step="mid", label=kwargs["label"], color=ll.get_color()
             )
         else:
-            ll, _, _, = plt.errorbar(
+            (
+                ll,
+                _,
+                _,
+            ) = plt.errorbar(
                 x,
                 y,
                 yerr=yerr,
                 xerr=xerr,
                 fmt=kwargs["fmt"],
                 capsize=kwargs["capsize"],
                 label=kwargs["label"],
```

### Comparing `smpl-1.2.2/smpl/plot2d.py` & `smpl-1.2.4/smpl/plot2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     ],
     # 'zscale' : [None,"Rescale z values."],
 }
 
 # @doc.insert_str("\tDefault kwargs\n\n\t")
 
 
-@doc.append_str(doc.table(default, init=False))
-@doc.append_str(doc.table({"plot2d_kwargs": ["default", "description"]}, bottom=False))
+@doc.append_str(doc.array_table(default, init=False))
+@doc.append_str(
+    doc.array_table({"plot2d_kwargs": ["default", "description"]}, bottom=False)
+)
 def plot2d_kwargs(kwargs):
     """Set default plot2d_kwargs if not set."""
     for k, v in default.items():
         if not k in kwargs:
             kwargs[k] = v[0]
     return kwargs
```

### Comparing `smpl-1.2.2/smpl/stat.py` & `smpl-1.2.4/smpl/stat.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/smpl/wrap.py` & `smpl-1.2.4/smpl/wrap.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.2/setup.py` & `smpl-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
  'smpl_parallel>=1.0.5,<2.0.0',
  'smpl_util>=1.0.5,<2.0.0',
  'sympy',
  'tqdm',
  'uncertainties']
 
 extras_require = \
-{'opt': ['iminuit<=2.18.0']}
+{'opt': ['iminuit']}
 
 setup_kwargs = {
     'name': 'smpl',
-    'version': '1.2.2',
+    'version': '1.2.4',
     'description': 'SiMPLe plotting and fitting',
     'long_description': '# smpl\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl.svg)\n\n| [Stable][doc stable]        | [Test][doc test]           |\n| ------------- |:-------------:|\n| [![workflow][a s image]][a s link]   | [![test][a t image]][a t link]     |\n| [![Coverage Status][c s i]][c s l]   | [![Coverage Status][c t i]][c t l] |\n| [![Codacy Badge][cc s c i]][cc s c l] | [![Codacy Badge][cc c i]][cc c l]  |\n| [![Codacy Badge][cc s q i]][cc s q l] | [![Codacy Badge][cc q i]][cc q l]  |\n| [![Documentation][rtd s i]][rtd s l] | [![Documentation][rtd t i]][rtd t l]|\n\n## Documentation\n\n-   <https://smpl.readthedocs.io/en/stable/>\n-   <https://apn-pucky.github.io/smpl/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl/index.html\n[doc test]: https://apn-pucky.github.io/smpl/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl.svg\n[pypi link]: https://pypi.org/project/smpl/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl/badge/?version=stable\n[rtd s l]: https://smpl.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl/badge/?version=latest\n[rtd t l]: https://smpl.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/smpl',
```

### Comparing `smpl-1.2.2/PKG-INFO` & `smpl-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: smpl
-Version: 1.2.2
+Version: 1.2.4
 Summary: SiMPLe plotting and fitting
 Home-page: https://github.com/APN-Pucky/smpl
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: opt
 Requires-Dist: deprecation
-Requires-Dist: iminuit (<=2.18.0) ; extra == "opt"
+Requires-Dist: iminuit ; extra == "opt"
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: scipy (>=1.7.0)
 Requires-Dist: smpl_animation
 Requires-Dist: smpl_debug (>=1.0.5,<2.0.0)
 Requires-Dist: smpl_doc (>=1.0.5,<2.0.0)
```

