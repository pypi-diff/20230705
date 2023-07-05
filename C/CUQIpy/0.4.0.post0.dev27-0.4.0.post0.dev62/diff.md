# Comparing `tmp/CUQIpy-0.4.0.post0.dev27.tar.gz` & `tmp/CUQIpy-0.4.0.post0.dev62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-0.4.0.post0.dev27.tar", last modified: Wed Jun 21 20:56:54 2023, max compression
+gzip compressed data, was "CUQIpy-0.4.0.post0.dev62.tar", last modified: Wed Jul  5 21:18:48 2023, max compression
```

## Comparing `CUQIpy-0.4.0.post0.dev27.tar` & `CUQIpy-0.4.0.post0.dev62.tar`

### file list

```diff
@@ -1,111 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.187833 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-21 20:56:54.000000 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 20:56:54.000000 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:56:54.000000 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 20:56:54.000000 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 20:56:54.000000 CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/cuqi/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.187833 CUQIpy-0.4.0.post0.dev27/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_cmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16345 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.191833 CUQIpy-0.4.0.post0.dev27/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.195833 CUQIpy-0.4.0.post0.dev27/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:56:54.199833 CUQIpy-0.4.0.post0.dev27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 20:56:44.000000 CUQIpy-0.4.0.post0.dev27/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.015668 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-07-05 21:18:47.000000 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-05 21:18:48.000000 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:18:47.000000 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 21:18:47.000000 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 21:18:47.000000 CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.015668 CUQIpy-0.4.0.post0.dev62/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.019668 CUQIpy-0.4.0.post0.dev62/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.019668 CUQIpy-0.4.0.post0.dev62/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.019668 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_cmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17951 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33026 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.019668 CUQIpy-0.4.0.post0.dev62/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40141 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.019668 CUQIpy-0.4.0.post0.dev62/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.023668 CUQIpy-0.4.0.post0.dev62/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:48.027668 CUQIpy-0.4.0.post0.dev62/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_MRFs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_distributions_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 21:18:37.000000 CUQIpy-0.4.0.post0.dev62/tests/test_utilities.py
```

### Comparing `CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0.post0.dev27
+Version: 0.4.0.post0.dev62
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,19 +233,19 @@
 from cuqi.data import grains
 from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ LMRF(0, 0.01)
-x = LMRF(location=np.zeros(A.domain_dim),
-                 scale=0.01,
-                 bc_type='neumann',
-                 physical_dim=2)
+# Step 2: Prior, x ~ LMRF(0,0.01)
+x = LMRF(location=0,
+         scale=0.01,
+         bc_type='neumann',
+         geometry = A.domain_geometry)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
 
 # Step 4: Set up Bayesian problem and sample posterior
 BP = BayesianProblem(y, x).set_data(y=y_data)
 samples = BP.sample_posterior(200)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-0.4.0.post0.dev62/CUQIpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,22 +69,25 @@
 cuqi/solver/__init__.py
 cuqi/solver/_solver.py
 cuqi/testproblem/__init__.py
 cuqi/testproblem/_testproblem.py
 cuqi/utilities/__init__.py
 cuqi/utilities/_get_python_variable_name.py
 cuqi/utilities/_utilities.py
+tests/test_MRFs.py
 tests/test_abstract_distribution_density.py
 tests/test_bayesian_inversion.py
 tests/test_density.py
 tests/test_distribution.py
+tests/test_distributions_shape.py
 tests/test_geometry.py
 tests/test_joint_distribution.py
 tests/test_likelihood.py
 tests/test_model.py
 tests/test_pde.py
+tests/test_posterior.py
 tests/test_problem.py
 tests/test_sampler.py
 tests/test_samples.py
 tests/test_solver.py
 tests/test_testproblem.py
 tests/test_utilities.py
```

### Comparing `CUQIpy-0.4.0.post0.dev27/LICENSE` & `CUQIpy-0.4.0.post0.dev62/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/PKG-INFO` & `CUQIpy-0.4.0.post0.dev62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0.post0.dev27
+Version: 0.4.0.post0.dev62
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,19 +233,19 @@
 from cuqi.data import grains
 from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ LMRF(0, 0.01)
-x = LMRF(location=np.zeros(A.domain_dim),
-                 scale=0.01,
-                 bc_type='neumann',
-                 physical_dim=2)
+# Step 2: Prior, x ~ LMRF(0,0.01)
+x = LMRF(location=0,
+         scale=0.01,
+         bc_type='neumann',
+         geometry = A.domain_geometry)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
 
 # Step 4: Set up Bayesian problem and sample posterior
 BP = BayesianProblem(y, x).set_data(y=y_data)
 samples = BP.sample_posterior(200)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/README.md` & `CUQIpy-0.4.0.post0.dev62/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 from cuqi.data import grains
 from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ LMRF(0, 0.01)
-x = LMRF(location=np.zeros(A.domain_dim),
-                 scale=0.01,
-                 bc_type='neumann',
-                 physical_dim=2)
+# Step 2: Prior, x ~ LMRF(0,0.01)
+x = LMRF(location=0,
+         scale=0.01,
+         bc_type='neumann',
+         geometry = A.domain_geometry)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
 
 # Step 4: Set up Bayesian problem and sample posterior
 BP = BayesianProblem(y, x).set_data(y=y_data)
 samples = BP.sample_posterior(200)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/array/_array.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/array/_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from cuqi.geometry import _DefaultGeometry
+from cuqi.geometry import _DefaultGeometry1D
 
 
 class CUQIarray(np.ndarray):
     """
     A class to represent data arrays, subclassed from numpy array, along with geometry and plotting
 
     Parameters
@@ -45,15 +45,15 @@
         # add the new attribute to the created instance
         obj.is_par = is_par
         if (not is_par) and (geometry is None):
             raise ValueError("geometry cannot be none when initializing a CUQIarray as function values (with is_par False).")
         if is_par and (obj.ndim>1):
             raise ValueError("input_array cannot be multidimensional when initializing CUQIarray as parameter (with is_par True).")
         if geometry is None:
-            geometry = _DefaultGeometry(grid=obj.__len__())
+            geometry = _DefaultGeometry1D(grid=obj.__len__())
         obj.geometry = geometry
         # Finally, we must return the newly created object:
         return obj
 
     def __array_finalize__(self, obj):
         # see InfoArray.__array_finalize__ for comments
         if obj is None: return
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/config.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/data/_data.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/data/astronaut.npz` & `CUQIpy-0.4.0.post0.dev62/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/data/camera.npz` & `CUQIpy-0.4.0.post0.dev62/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/data/cat.npz` & `CUQIpy-0.4.0.post0.dev62/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/data/satellite.mat` & `CUQIpy-0.4.0.post0.dev62/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/density/_density.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/diagnostics.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/__init__.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_beta.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_cauchy.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_cmrf.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_lmrf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import numpy as np
-import warnings
-from cuqi.geometry import _DefaultGeometry, Image2D, _get_identity_geometries
-from cuqi.distribution import Distribution
+from cuqi.geometry import _DefaultGeometry1D, Image2D
 from cuqi.operator import FirstOrderFiniteDifference
-from cuqi.geometry import _DefaultGeometry, Image2D, _get_identity_geometries
+from cuqi.distribution import Distribution
+from cuqi.utilities import force_ndarray
 
-class CMRF(Distribution):
-    """Cauchy distribution on the difference between neighboring nodes.
+class LMRF(Distribution):
+    """Laplace distribution on the difference between neighboring nodes.
 
-    For 1D `(physical_dim=1)`, the Cauchy difference distribution assumes that
+    For 1D, the Laplace difference distribution assumes that
 
     .. math::
 
-        x_i-x_{i-1} \sim \mathrm{Cauchy}(0, \gamma),
+        x_i-x_{i-1} \sim \mathrm{Laplace}(0, b),
 
-    where :math:`\gamma` is the scale parameter.
+    where :math:`b` is the scale parameter.
 
-    For 2D `(physical_dim=2)` the differences are defined in both horizontal and vertical directions.
+    For 2D the differences are defined in both horizontal and vertical directions.
 
     It is possible to define boundary conditions using the `bc_type` parameter.
 
     The location parameter is a shift of the :math:`\mathbf{x}`.
 
     Parameters
     ----------
@@ -29,70 +28,69 @@
 
     scale : scalar
         The scale parameter of the distribution.
 
     bc_type : string
         The boundary conditions of the difference operator.
 
-    physical_dim : int
-        The physical dimension of what the distribution represents (can take the values 1 or 2).
-
     Example
     -------
     .. code-block:: python
 
         import cuqi
-        import numpy as np
-        prior = cuqi.distribution.CMRF(location=np.zeros(128), scale=0.1)
+        prior = cuqi.distribution.LMRF(location=0, scale=0.1, geometry=128)
  
     """
-   
-    def __init__(self, location, scale, bc_type="zero", physical_dim=1, **kwargs):
+    def __init__(self, location, scale, bc_type="zero", **kwargs):
         # Init from abstract distribution class
-        super().__init__(**kwargs) 
-        
+        super().__init__(**kwargs)
+
         self.location = location
         self.scale = scale
         self._bc_type = bc_type
+
+        # Ensure geometry has shape
+        if not self.geometry.fun_shape or self.geometry.par_dim == 1:
+            raise ValueError(f"Distribution {self.__class__.__name__} must be initialized with supported geometry (geometry of which the fun_shape is not None) and has parameter dimension greater than 1.")
+
+        # Default physical_dim to geometry's dimension if not provided
+        physical_dim = len(self.geometry.fun_shape)
+
+        # Ensure provided physical dimension is either 1 or 2
+        if physical_dim not in [1, 2]:
+            raise ValueError("Only physical dimension 1 or 2 supported.")
+
         self._physical_dim = physical_dim
 
-        if physical_dim == 2:
+        if self._physical_dim == 2:
             N = int(np.sqrt(self.dim))
             num_nodes = (N, N)
-            if isinstance(self.geometry, _DefaultGeometry):
-                self.geometry = Image2D(num_nodes)
-            print("Warning: 2D CMRF is still experimental. Use at own risk.")
-        elif physical_dim == 1:
+        else: 
             num_nodes = self.dim
-        else:
-            raise ValueError("Only physical dimension 1 or 2 supported.")
 
         self._diff_op = FirstOrderFiniteDifference(num_nodes=num_nodes, bc_type=bc_type)
 
-        # Check if location parameter is non-zero vector (not supported)
-        if callable(location) or np.linalg.norm(location) > 0:
-            raise ValueError("Non-zero location parameter not supported.")
+    @property
+    def location(self):
+        return self._location
+    
+    @location.setter
+    def location(self, value):
+        self._location = force_ndarray(value, flatten=True)
+
+    def pdf(self, x):
+        Dx = self._diff_op @ (x-self.location)  # np.diff(X)
+        return (1/(2*self.scale))**(len(Dx)) * np.exp(-np.linalg.norm(Dx, ord=1, axis=0)/self.scale)
 
     def logpdf(self, x):
         Dx = self._diff_op @ (x-self.location)
-        # g_logpr = (-2*Dx/(Dx**2 + gamma**2)) @ D
-        return -len(Dx)*np.log(np.pi) + sum(np.log(self.scale) - np.log(Dx**2 + self.scale**2))
-    
-    def _gradient(self, val, **kwargs):
-        #Avoid complicated geometries that change the gradient.
-        if not type(self.geometry) in _get_identity_geometries():
-            raise NotImplementedError("Gradient not implemented for distribution {} with geometry {}".format(self,self.geometry))
-
-        if not callable(self.location): # for prior
-            diff = self._diff_op._matrix @ val
-            return (-2*diff/(diff**2+self.scale**2)) @ self._diff_op._matrix
-        else:
-            warnings.warn('Gradient not implemented for {}'.format(type(self.location)))
+        return len(Dx)*(-(np.log(2)+np.log(self.scale))) - np.linalg.norm(Dx, ord=1, axis=0)/self.scale
 
     def _sample(self,N=1,rng=None):
-        raise NotImplementedError("'CMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
+        raise NotImplementedError("'LMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
 
     # def cdf(self, x):   # TODO
-    #     return 1/np.pi * np.atan((x-self.loc)/self.scale)
+    #     return 1/2 + 1/2*np.sign(x-self.loc)*(1-np.exp(-np.linalg.norm(x, ord=1, axis=0)/self.scale))
 
     # def sample(self):   # TODO
-    #     return self.loc + self.scale*np.tan(np.pi*(np.random.rand(self.dim)-1/2))
+    #     p = np.random.rand(self.dim)
+    #     return self.loc - self.scale*np.sign(p-1/2)*np.log(1-2*abs(p-1/2))
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_custom.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_custom.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,28 +37,19 @@
         # Init from abstract distribution class
         super().__init__(**kwargs)
 
         if logpdf_func is not None and not callable(logpdf_func): raise ValueError("logpdf_func should be callable.")
         if sample_func is not None and not callable(sample_func): raise ValueError("sample_func should be callable.")
         if gradient_func is not None and not callable(gradient_func): raise ValueError("grad_func should be callable.")
         
-        self.dim = dim
+        self.geometry = dim # Store dimension by calling setter for geometry (creates default geometry)
         self.logpdf_func = logpdf_func
         self.sample_func = sample_func
         self.gradient_func = gradient_func
 
-
-    @property
-    def dim(self):
-        return self._dim
-
-    @dim.setter
-    def dim(self, value):
-        self._dim = value
-
     def logpdf(self, x):
         if self.logpdf_func is not None:
             return self.logpdf_func(x)
         else:
             raise Exception("logpdf_func is not defined.")
     
     def _gradient(self, x):
@@ -76,14 +67,20 @@
                 out = np.zeros((self.dim,N))
                 for i in range(N):
                     out[:,i] = self.sample_func()
                 return out
         else:
             raise Exception("sample_func is not defined. Sampling can be performed by passing the density to a sampler from the 'sampler' module.")
 
+    @property
+    def _mutable_vars(self):
+        """ Returns the mutable variables of the distribution. """
+        # Currently mutable variables are not supported for user-defined distributions.
+        return []
+
     def get_conditioning_variables(self):
         """ Returns the conditioning variables of the distribution. """
         # Currently conditioning variables are not supported for user-defined distributions.
         return []
 
 ### BENCHMARKS
 class DistributionGallery(UserDefinedDistribution):
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_distribution.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_distribution.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 from copy import copy
 from functools import partial
 from cuqi.density import Density, EvaluatedDensity
 from cuqi.likelihood import Likelihood
 from cuqi.samples import Samples
 from cuqi.array import CUQIarray
-from cuqi.geometry import _DefaultGeometry, Geometry
+from cuqi.geometry import _DefaultGeometry1D, _DefaultGeometry2D, Geometry
 from cuqi.utilities import infer_len, get_writeable_attributes, get_writeable_properties, get_non_default_args, get_indirect_variables
 import numpy as np # To be replaced by cuqi.array_api
 
 # ========== Abstract distribution class ===========
 class Distribution(Density, ABC):
     """ Abstract Base Class for Distributions.
 
@@ -88,48 +88,79 @@
         """
         super().__init__(name=name)
         self.is_symmetric = is_symmetric
         self.geometry = geometry
 
     @property
     def dim(self):
-        """ Return the dimension of the distribution.
-        
-        The dimension is automatically inferred from the mutable variables of the distribution.
-
+        """ Return the dimension of the distribution based on the geometry.
+    
         If the dimension can not be inferred, None is returned.
 
-        Subclassing distributions can choose to overwrite this property if different behavior is desired.
         """
+        return self.geometry.par_dim
 
+    def _infer_dim_of_mutable_variables(self):
+        """ Infer the dimension of the mutable variables of the distribution. """
         # Get all mutable variables
         mutable_vars = self.get_mutable_variables()
 
+        # Check if mutable_vars is empty, no dimension can be inferred
+        if not mutable_vars:
+            return None
+
         # Loop over mutable variables and get range dimension of each and get the maximum
         max_len = max([infer_len(getattr(self, var)) for var in mutable_vars])
 
         return max_len if max_len > 0 else None
 
     @property
     def geometry(self):
-        if self.dim != self._geometry.par_dim:
-            if isinstance(self._geometry,_DefaultGeometry):
-                self.geometry = self.dim
-            else:
-                raise Exception("Distribution Geometry attribute is not consistent with the distribution dimension ('dim')")
+        """ Return the geometry of the distribution.
+
+        The geometry can be automatically inferred from the mutable variables of the distribution.
+
+        """ 
+
+        inferred_dim = self._infer_dim_of_mutable_variables()
+        geometry_dim = self._geometry.par_dim
+
+        is_inferred_multivariate = inferred_dim > 1 if inferred_dim is not None else False
+
+        # Flag indicating whether distribution geometry matches inferred dimension
+        geometry_matches_inferred_dim = (geometry_dim == inferred_dim) if (geometry_dim and inferred_dim) else True
+
+        # If inconsistent geometry dimensions, raise an exception
+        # If scalar inferred dimension, we allow geometry to take precedence
+        if is_inferred_multivariate and not geometry_matches_inferred_dim:
+            raise TypeError(
+                f"Inconsistent distribution geometry attribute {self._geometry} and inferred "
+                f"dimension from distribution variables {inferred_dim}."
+            )
+        
+        # If Geometry dimension is None, update it with the inferred dimension
+        if inferred_dim and self._geometry.par_dim is None: 
+            self.geometry = inferred_dim
+
+        if self._geometry.par_shape is None:
+            raise ValueError(f"{self.__class__.__name__}: Unable to automatically determine geometry of distribution. Please specify a geometry with the geometry keyword")
+
         # Check if dist has a name, if so we provide it to the geometry
         # We do not use self.name to potentially infer it from python stack.
-        if self._name is not None: 
+        if self._name: 
             self._geometry._variable_name = self._name
+            
         return self._geometry
 
     @geometry.setter
     def geometry(self,value):
-        if isinstance(value, (int,np.integer)) or value is None:
-            self._geometry = _DefaultGeometry(grid=value)
+        if isinstance(value, tuple) and len(value) == 2:
+            self._geometry = _DefaultGeometry2D(value)           
+        elif isinstance(value, (int,np.integer)) or value is None:
+            self._geometry = _DefaultGeometry1D(grid=value)
         elif isinstance(value, Geometry):
             self._geometry = value
         else:
             raise TypeError("The attribute 'geometry' should be of type 'int' or 'cuqi.geometry.Geometry', or None.")
 
     def logd(self, *args, **kwargs):
         """  Evaluate the un-normalized log density function of the distribution.
@@ -384,13 +415,17 @@
             ordered_keys.append("_main_parameter") # Last arg is main parameter
             for index, arg in enumerate(args):
                 if index < len(ordered_keys):
                     if ordered_keys[index] in kwargs:
                         raise ValueError(f"{self._condition.__qualname__}: {ordered_keys[index]} passed as both argument and keyword argument.\nArguments follow the listed conditioning variable order: {self.get_conditioning_variables()}")
                     kwargs[ordered_keys[index]] = arg
         return kwargs
+    
+    def _check_geometry_consistency(self):
+        """ Checks that the geometry of the distribution is consistent by calling the geometry property. Should be called at the end of __init__ of subclasses. """
+        self.geometry
 
     def __repr__(self) -> str:
         if self.is_cond is True:
             return "CUQI {}. Conditioning variables {}.".format(self.__class__.__name__,self.get_conditioning_variables())
         else:
             return "CUQI {}.".format(self.__class__.__name__)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gamma.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gaussian.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,16 @@
         elif sqrtcov is not None:
             self._mutable_vars = ['mean', 'sqrtcov']
             self.sqrtcov = sqrtcov
         elif sqrtprec is not None:
             self._mutable_vars = ['mean', 'sqrtprec']
             self.sqrtprec = sqrtprec
 
+        self._check_geometry_consistency()
+
     @property
     def mean(self):
         """ Mean of the distribution """
         return self._mean
 
     @mean.setter
     def mean(self, value):
@@ -231,15 +233,16 @@
 
     @property
     def rank(self):
         return self._rank
 
     @property
     def sqrtprecTimesMean(self):
-        return (self.sqrtprec@self.mean).flatten()
+        mean = np.repeat(self.mean, self.dim) if len(self.mean) == 1 else self.mean
+        return (self.sqrtprec@mean).flatten()
 
     def compute_cov(self):
         """ Computes the covariance matrix regardless of the mutable variables. 
         
         This is useful for smaller scale problems where we may want to use the full covariance matrix.
 
         """
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_gmrf.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_gmrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from scipy.sparse import diags, eye
 from scipy.sparse import linalg as splinalg
 from scipy.linalg import dft
-from cuqi.geometry import _DefaultGeometry, Image2D, _get_identity_geometries
+from cuqi.geometry import _DefaultGeometry1D, Image2D, _get_identity_geometries
 from cuqi.utilities import sparse_cholesky
 from cuqi import config
 from cuqi.operator import PrecisionFiniteDifference
 from cuqi.distribution import Distribution
 
 class GMRF(Distribution):
     """ Gaussian Markov random field (GMRF).
@@ -102,15 +102,15 @@
         self.prec = prec
         self._partition_size = int(len(mean)**(1/physical_dim))
         self._bc_type = bc_type      # boundary conditions
         self._physical_dim = physical_dim
         
         num_nodes = tuple(self._partition_size for _ in range(physical_dim))
         if physical_dim == 2: #TODO. Remove once _DefaultGeometry is implemented for 2D.
-            if isinstance(self.geometry, _DefaultGeometry):
+            if isinstance(self.geometry, _DefaultGeometry1D):
                 self.geometry = Image2D(num_nodes)
 
         self._prec_op = PrecisionFiniteDifference(num_nodes, bc_type=bc_type, order=order) 
         self._diff_op = self._prec_op._diff_op      
                    
         # compute Cholesky and det
         if (bc_type == 'zero'):    # only for PSD matrices
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_joint_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import List
 from copy import copy
 from cuqi.density import Density, EvaluatedDensity
 from cuqi.distribution import Distribution, Posterior
 from cuqi.likelihood import Likelihood
-from cuqi.geometry import Geometry, _DefaultGeometry
+from cuqi.geometry import Geometry, _DefaultGeometry1D
 import numpy as np # for splitting array. Can avoid.
 
 class JointDistribution:
     """ 
     Joint distribution of multiple variables.
 
     Parameters
@@ -275,15 +275,15 @@
 
     @property
     def dim(self):
         return sum(super().dim)
 
     @property
     def geometry(self):
-        return _DefaultGeometry(self.dim)
+        return _DefaultGeometry1D(self.dim)
 
     def logd(self, stacked_input):
         """ Return the un-normalized log density function stacked joint density. """
 
         # Split the stacked input into individual inputs and call superclass
         split_indices = np.cumsum(super().dim)  # list(accumulate(super().dim))
         inputs = np.split(stacked_input, split_indices[:-1])
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_laplace.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_lmrf.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_cmrf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import numpy as np
-from cuqi.geometry import _DefaultGeometry, Image2D
-from cuqi.operator import FirstOrderFiniteDifference
+import warnings
+from cuqi.geometry import _DefaultGeometry1D, Image2D, _get_identity_geometries
 from cuqi.distribution import Distribution
+from cuqi.operator import FirstOrderFiniteDifference
+from cuqi.utilities import force_ndarray
 
-class LMRF(Distribution):
-    """Laplace distribution on the difference between neighboring nodes.
 
-    For 1D `(physical_dim=1)`, the Laplace difference distribution assumes that
+class CMRF(Distribution):
+    """Cauchy distribution on the difference between neighboring nodes.
+
+    For 1D the Cauchy difference distribution assumes that
 
     .. math::
 
-        x_i-x_{i-1} \sim \mathrm{Laplace}(0, b),
+        x_i-x_{i-1} \sim \mathrm{Cauchy}(0, \gamma),
 
-    where :math:`b` is the scale parameter.
+    where :math:`\gamma` is the scale parameter.
 
-    For 2D `(physical_dim=2)` the differences are defined in both horizontal and vertical directions.
+    For 2D the differences are defined in both horizontal and vertical directions.
 
     It is possible to define boundary conditions using the `bc_type` parameter.
 
     The location parameter is a shift of the :math:`\mathbf{x}`.
 
     Parameters
     ----------
@@ -27,62 +30,79 @@
 
     scale : scalar
         The scale parameter of the distribution.
 
     bc_type : string
         The boundary conditions of the difference operator.
 
-    physical_dim : int
-        The physical dimension of what the distribution represents (can take the values 1 or 2).
-
     Example
     -------
     .. code-block:: python
 
         import cuqi
         import numpy as np
-        prior = cuqi.distribution.LMRF(location=np.zeros(128), scale=0.1)
+        prior = cuqi.distribution.CMRF(location=np.zeros(128), scale=0.1)
  
     """
-    def __init__(self, location, scale, bc_type="zero", physical_dim=1, **kwargs):
+   
+    def __init__(self, location, scale, bc_type="zero", **kwargs):
         # Init from abstract distribution class
         super().__init__(**kwargs) 
-
+        
         self.location = location
         self.scale = scale
         self._bc_type = bc_type
+
+        # Ensure geometry has shape
+        if not self.geometry.fun_shape or self.geometry.par_dim == 1:
+            raise ValueError(f"Distribution {self.__class__.__name__} must be initialized with supported geometry (geometry of which the fun_shape is not None) and has parameter dimension greater than 1.")
+
+        # Default physical_dim to geometry's dimension if not provided
+        physical_dim = len(self.geometry.fun_shape)
+
+        # Ensure provided physical dimension is either 1 or 2
+        if physical_dim not in [1, 2]:
+            raise ValueError("Only physical dimension 1 or 2 supported.")
+
         self._physical_dim = physical_dim
 
-        if physical_dim == 2:
+        if self._physical_dim == 2:
             N = int(np.sqrt(self.dim))
             num_nodes = (N, N)
-            if isinstance(self.geometry, _DefaultGeometry):
-                self.geometry = Image2D(num_nodes)
-
-        elif physical_dim == 1:
+        else: 
             num_nodes = self.dim
-        else:
-            raise ValueError("Only physical dimension 1 or 2 supported.")
 
         self._diff_op = FirstOrderFiniteDifference(num_nodes=num_nodes, bc_type=bc_type)
 
-        # Check if location parameter is non-zero vector (not supported)
-        if callable(location) or np.linalg.norm(location) > 0:
-            raise ValueError("Non-zero location parameter not supported.")
-
-    def pdf(self, x):
-        Dx = self._diff_op @ (x-self.location)  # np.diff(X)
-        return (1/(2*self.scale))**(len(Dx)) * np.exp(-np.linalg.norm(Dx, ord=1, axis=0)/self.scale)
+    @property
+    def location(self):
+        return self._location
+    
+    @location.setter
+    def location(self, value):
+        self._location = force_ndarray(value, flatten=True)
+
 
     def logpdf(self, x):
         Dx = self._diff_op @ (x-self.location)
-        return len(Dx)*(-(np.log(2)+np.log(self.scale))) - np.linalg.norm(Dx, ord=1, axis=0)/self.scale
+        # g_logpr = (-2*Dx/(Dx**2 + gamma**2)) @ D
+        return -len(Dx)*np.log(np.pi) + sum(np.log(self.scale) - np.log(Dx**2 + self.scale**2))
+    
+    def _gradient(self, val, **kwargs):
+        #Avoid complicated geometries that change the gradient.
+        if not type(self.geometry) in _get_identity_geometries():
+            raise NotImplementedError("Gradient not implemented for distribution {} with geometry {}".format(self,self.geometry))
+
+        if not callable(self.location): # for prior
+            diff = self._diff_op._matrix @ val
+            return (-2*diff/(diff**2+self.scale**2)) @ self._diff_op._matrix
+        else:
+            warnings.warn('Gradient not implemented for {}'.format(type(self.location)))
 
     def _sample(self,N=1,rng=None):
-        raise NotImplementedError("'LMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
+        raise NotImplementedError("'CMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
 
     # def cdf(self, x):   # TODO
-    #     return 1/2 + 1/2*np.sign(x-self.loc)*(1-np.exp(-np.linalg.norm(x, ord=1, axis=0)/self.scale))
+    #     return 1/np.pi * np.atan((x-self.loc)/self.scale)
 
     # def sample(self):   # TODO
-    #     p = np.random.rand(self.dim)
-    #     return self.loc - self.scale*np.sign(p-1/2)*np.log(1-2*abs(p-1/2))
+    #     return self.loc + self.scale*np.tan(np.pi*(np.random.rand(self.dim)-1/2))
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_lognormal.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_normal.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_posterior.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_posterior.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,39 +37,51 @@
     def geometry(self):
         return self._geometry
 
     @geometry.setter
     def geometry(self, value):
         # Compare model and prior
         if self.model is not None and self.model.domain_geometry != self.prior.geometry:
-            if isinstance(self.prior.geometry,_DefaultGeometry):
+            if isinstance(self.prior.geometry, _DefaultGeometry):
                 pass #We allow default geometry in prior
             else:
                 raise ValueError("Geometry from likelihood (model.domain_geometry) does not match prior geometry")
 
         # Compare value and prior
         if self.model is None and value is not None and value != self.prior.geometry:
-            if isinstance(self.prior.geometry,_DefaultGeometry):
+            if isinstance(self.prior.geometry, _DefaultGeometry):
                 pass #We allow default geometry in prior
             else:
                 raise ValueError("Posterior and prior geometries are inconsistent.")
 
         # Compare model and value
         if self.model is not None and value is not None and value != self.model.domain_geometry:
-            if isinstance(self.model.domain_geometry,_DefaultGeometry):
+            if isinstance(self.model.domain_geometry, _DefaultGeometry):
                 pass #Allow default model geometry
             else:
                 raise ValueError("Set geometry does not match with model geometry.")
-
+            
+        # Compare likelihood and prior
+        if self.likelihood.geometry != self.prior.geometry:
+            if isinstance(self.prior.geometry, _DefaultGeometry):
+                pass #We allow default geometry in prior
+            elif isinstance(self.likelihood.geometry, _DefaultGeometry):
+                pass #We allow default geometry in likelihood
+            else:
+                raise ValueError("Likelihood and prior geometries are inconsistent.")
+        
         # If value is set, its consistant with prior (and prior is consistant with model)
-        # If value is not set, take from model (if exists) or from prior as last resort
-        if value is not None:
+        # Likelihood and prior are consistant.
+        # If value is not set, take from model (if exists) or from likelihood or prior as last resort
+        if value is not None and not isinstance(value, _DefaultGeometry):
             self._geometry = value
-        elif self.model is not None:
+        elif self.model is not None and not isinstance(self.model.domain_geometry, _DefaultGeometry):
             self._geometry = self.model.domain_geometry
+        elif not isinstance(self.likelihood.geometry, _DefaultGeometry):
+            self._geometry = self.likelihood.geometry
         else:
             self._geometry = self.prior.geometry
             
     def logpdf(self, *args, **kwargs):
         """ Returns the logpdf of the posterior distribution"""
         return self.likelihood.logd(*args, **kwargs)+ self.prior.logd(*args, **kwargs)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/distribution/_uniform.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/geometry/__init__.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/geometry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,24 @@
     Continuous,
     Continuous1D,
     Continuous2D,
     Image2D,
     Discrete,
     MappedGeometry,
     _DefaultGeometry,
+    _DefaultGeometry1D,
+    _DefaultGeometry2D,
     KLExpansion,
     KLExpansion_Full,
     CustomKL,
     StepExpansion
 )
 
 
 # TODO: We will remove the use of identity geometries in the future
-_identity_geometries = [_DefaultGeometry, Continuous1D, Continuous2D, Discrete, Image2D]
+_identity_geometries = [_DefaultGeometry1D, _DefaultGeometry2D, Continuous1D, Continuous2D, Discrete, Image2D]
 
 def _get_identity_geometries():
     """Return the geometries that have identity `par2fun` and `fun2par` methods (including those where `par2fun` and `fun2par` perform reshaping of the parameters or the function values array. e.g. the geometry `Image2D`.).
     These geometries do not alter the gradient computations.
     """
     return _identity_geometries
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/geometry/_geometry.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/geometry/_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,22 +592,36 @@
         if self.imap is None:
             raise ValueError("imap is not defined. This is needed for fun2par.")
         return self.geometry.fun2par(self.imap(f))
 
     def __repr__(self) -> str:
         return "{}({})".format(self.__class__.__name__,self.geometry.__repr__())
 
+class _DefaultGeometry(Geometry):
+    """ Default geometry base class. """
+    pass
 
-class _DefaultGeometry(Continuous1D):
+
+class _DefaultGeometry1D(Continuous1D, _DefaultGeometry):
+    """ Default 1D geometry based on Continuous1D. """
     def __init__(self, grid=None, axis_labels=None):
         super().__init__(grid, axis_labels)
 
     def __eq__(self, obj):
         if not isinstance(obj, (self.__class__,Continuous1D)): return False
         return self._all_values_equal(obj)
+    
+class _DefaultGeometry2D(Image2D, _DefaultGeometry):
+    """ Default 2D geometry based on Image2D. """
+    def __init__(self, im_shape=None, visual_only=False):
+        super().__init__(im_shape, visual_only=visual_only)
+
+    def __eq__(self, obj):
+        if not isinstance(obj, (self.__class__,Image2D)): return False
+        return self._all_values_equal(obj)
 
 # class DiscreteField(Discrete):
 #     def __init__(self, grid, cov_func, mean, std, trunc_term=100, axis_labels=['x']):
 #         super().__init__(grid, axis_labels)
 
 #         self.N = len(self.grid)
 #         self.mean = mean
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/likelihood/__init__.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/likelihood/_likelihood.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/likelihood/_likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import Union
 from cuqi.model import Model
-from cuqi.utilities import get_non_default_args
-from cuqi.geometry import _DefaultGeometry
+from cuqi.utilities import get_non_default_args, _get_python_variable_name
+from cuqi.geometry import _DefaultGeometry1D
 from cuqi.density import Density, EvaluatedDensity
 import warnings
 from copy import copy
 
 class Likelihood(Density):
     """Likelihood function defined from a conditional distribution and some observed data.
 
@@ -80,15 +80,15 @@
         """ Return function space shape of likelihood """
         return self.geometry.fun_shape
 
     @property
     def geometry(self):
         """ Return geometry of likelihood """
         if self.model is None:
-            return _DefaultGeometry()
+            return _DefaultGeometry1D()
         if len(self.get_parameter_names()) > 1:
             warnings.warn(
                 f"Likelihood depends on multiple parameters {self.get_parameter_names()}.\n"
                 f"Returned geometry is only with respect to the model parameter {get_non_default_args(self.model)}."
             )
         return self.model.domain_geometry
 
@@ -159,19 +159,32 @@
         Function evaluating the gradient of the log density.
 
     geometry : Geometry
         Geometry of the likelihood.
     
     """
 
-    def __init__(self, dim=None, logpdf_func=None, gradient_func=None, geometry=None):
+    def __init__(self, dim=None, logpdf_func=None, gradient_func=None, geometry=None, name=None):
         self.dim = dim
         self.logpdf_func = logpdf_func
         self.gradient_func = gradient_func
         self.geometry = geometry
+        self._name = name
+
+    @property
+    def model(self):
+        """ Return model of likelihood """
+        return None
+    
+    @property
+    def name(self):
+        """ Return name of likelihood """
+        if self._name is None:
+            self._name = _get_python_variable_name(self)
+        return self._name
 
     @property
     def dim(self):
         """ Return dimension of likelihood """
         return self._dim
 
     @dim.setter
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/model/_model.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/model/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import numpy as np
 from scipy.sparse import csc_matrix
 from scipy.sparse import hstack
 from scipy.linalg import solve
 from cuqi.samples import Samples
 from cuqi.array import CUQIarray
-from cuqi.geometry import Geometry, _DefaultGeometry, _get_identity_geometries
+from cuqi.geometry import Geometry, _DefaultGeometry1D, _DefaultGeometry2D, _get_identity_geometries
 import cuqi
 import matplotlib.pyplot as plt
 from copy import copy
 
 class Model(object):
     """Generic model defined by a forward operator.
 
@@ -110,32 +110,36 @@
             gradient = lambda direction, wrt: direction@jacobian(wrt)
  
         #Store forward func
         self._forward_func = forward
         self._gradient_func = gradient
          
         #Store range_geometry
-        if isinstance(range_geometry, int):
-            self.range_geometry = _DefaultGeometry(grid=range_geometry)
+        if isinstance(range_geometry, tuple) and len(range_geometry) == 2:
+            self.range_geometry = _DefaultGeometry2D(range_geometry)
+        elif isinstance(range_geometry, int):
+            self.range_geometry = _DefaultGeometry1D(grid=range_geometry)
         elif isinstance(range_geometry, Geometry):
             self.range_geometry = range_geometry
         elif range_geometry is None:
             raise AttributeError("The parameter 'range_geometry' is not specified by the user and it connot be inferred from the attribute 'forward'.")
         else:
-            raise TypeError("The parameter 'range_geometry' should be of type 'int' or 'cuqi.geometry.Geometry'.")
+            raise TypeError("The parameter 'range_geometry' should be of type 'int', 2 dimensional 'tuple' or 'cuqi.geometry.Geometry'.")
 
         #Store domain_geometry
-        if isinstance(domain_geometry, int):
-            self.domain_geometry = _DefaultGeometry(grid=domain_geometry)
+        if isinstance(domain_geometry, tuple) and len(domain_geometry) == 2:
+            self.domain_geometry = _DefaultGeometry2D(domain_geometry)
+        elif isinstance(domain_geometry, int):
+            self.domain_geometry = _DefaultGeometry1D(grid=domain_geometry)
         elif isinstance(domain_geometry, Geometry):
             self.domain_geometry = domain_geometry
         elif domain_geometry is None:
             raise AttributeError("The parameter 'domain_geometry' is not specified by the user and it connot be inferred from the attribute 'forward'.")
         else:
-            raise TypeError("The parameter 'domain_geometry' should be of type 'int' or 'cuqi.geometry.Geometry'.")
+            raise TypeError("The parameter 'domain_geometry' should be of type 'int', 2 dimensional 'tuple' or 'cuqi.geometry.Geometry'.")
 
         # Store non_default_args of the forward operator for faster caching when checking for those arguments.
         self._non_default_args = cuqi.utilities.get_non_default_args(self._forward_func)
 
     @property
     def domain_dim(self): 
         return self.domain_geometry.par_dim
@@ -160,15 +164,15 @@
             If False the input is assumed to be function values.
 
         Returns
         -------
         ndarray or cuqi.array.CUQIarray
             The input value represented as a function.
         """
-        if type(x) is CUQIarray and not isinstance(x.geometry, _DefaultGeometry):
+        if type(x) is CUQIarray and not isinstance(x.geometry, _DefaultGeometry1D):
             return x.funvals
         elif is_par:
             return geometry.par2fun(x)
         else:
             return x
 
     def _output2par(self, out, geometry, to_CUQIarray=False):
@@ -450,17 +454,17 @@
         #Check if input is callable
         if callable(adjoint_func) is not True:
             raise TypeError("Adjoint needs to be callable function of some kind")
 
         # Use matrix to derive range_geometry and domain_geometry
         if matrix is not None:
             if range_geometry is None:
-                range_geometry = _DefaultGeometry(grid=matrix.shape[0])
+                range_geometry = _DefaultGeometry1D(grid=matrix.shape[0])
             if domain_geometry is None:
-                domain_geometry = _DefaultGeometry(grid=matrix.shape[1])  
+                domain_geometry = _DefaultGeometry1D(grid=matrix.shape[1])  
 
         #Initialize Model class
         super().__init__(forward_func,range_geometry,domain_geometry)
 
         #Add adjoint
         self._adjoint_func = adjoint_func
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/operator/_operator.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/pde/_pde.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/pde/_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/problem/_problem.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/problem/_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_conjugate.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_conjugate_approx.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_cwmh.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_cwmh.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         super().__init__(target, proposal=proposal, scale=scale,  x0=x0, dim=dim, **kwargs)
         
     @ProposalBasedSampler.proposal.setter 
     def proposal(self, value):
         fail_msg = "Proposal should be either None, cuqi.distribution.Distribution conditioned only on 'location' and 'scale', lambda function, or cuqi.distribution.Normal conditioned only on 'mean' and 'std'"
 
         if value is None:
-            self._proposal = cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale )
+            self._proposal = cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale, geometry=self.dim)
 
         elif isinstance(value, cuqi.distribution.Distribution) and sorted(value.get_conditioning_variables())==['location','scale']:
             self._proposal = value
 
         elif isinstance(value, cuqi.distribution.Normal) and sorted(value.get_conditioning_variables())==['mean','std']:
             self._proposal = value(mean = lambda location:location, std = lambda scale:scale)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_gibbs.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_hmc.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_laplace_approximation.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,17 +126,23 @@
 
         # Pre-computations
         self._model = self.target.likelihood.model   
         self._data = self.target.likelihood.data
         self._m = len(self._data)
         self._L1 = self.target.likelihood.distribution.sqrtprec
 
+        # If prior location is scalar, repeat it to match dimensions
+        if len(self.target.prior.location) == 1:
+            self._priorloc = np.repeat(self.target.prior.location, self.dim)
+        else:
+            self._priorloc = self.target.prior.location
+
         # Initial Laplace approx
         self._L2 = Lk_fun(self.x0)
-        self._L2mu = self._L2@self.target.prior.location
+        self._L2mu = self._L2@self._priorloc
         self._b_tild = np.hstack([self._L1@self._data, self._L2mu]) 
         
         #self.n = len(self.x0)
         
         # Least squares form
         def M(x, flag):
             if flag == 1:
@@ -156,15 +162,15 @@
                      
         # initial state   
         samples[:, 0] = self.x0
         for s in range(N-1):
 
             # Update Laplace approximation
             self._L2 = Lk_fun(samples[:, s])
-            self._L2mu = self._L2@self.target.prior.location
+            self._L2mu = self._L2@self._priorloc
             self._b_tild = np.hstack([self._L1@self._data, self._L2mu]) 
         
             # Sample from approximate posterior
             e = Normal(mean=np.zeros(len(self._b_tild)), std=1).sample(rng=self.rng)
             y = self._b_tild + e # Perturb data
             sim = CGLS(M, y, samples[:, s], self.maxit, self.tol, self._shift)            
             samples[:, s+1], _ = sim.solve()
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_mh.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_pcn.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_rto.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/sampler/_sampler.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/sampler/_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
     @property
     def geometry(self):
         if hasattr(self, 'target') and hasattr(self.target, 'geometry'):
             geom =  self.target.geometry
         else:
-            geom = cuqi.geometry._DefaultGeometry(self.dim)
+            geom = cuqi.geometry._DefaultGeometry1D(self.dim)
         return geom
 
     @property 
     def target(self):
         return self._target 
 
     @target.setter 
@@ -171,8 +171,8 @@
         if hasattr(self, 'target') and hasattr(self.target, 'geometry') and self.target.geometry.par_dim is not None:
             geom2 = self.target.geometry
         if not isinstance(geom1,cuqi.geometry._DefaultGeometry) and geom1 is not None:
             return geom1
         elif not isinstance(geom2,cuqi.geometry._DefaultGeometry) and geom2 is not None: 
             return geom2
         else:
-            return cuqi.geometry._DefaultGeometry(self.dim)
+            return cuqi.geometry._DefaultGeometry1D(self.dim)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/samples/_samples.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/samples/_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from cuqi.diagnostics import Geweke
-from cuqi.geometry import _DefaultGeometry, Continuous2D, Image2D
+from cuqi.geometry import _DefaultGeometry1D, Continuous2D, Image2D
 from cuqi.array import CUQIarray
 from cuqi.utilities import force_ndarray
 from copy import copy
 import arviz # Plotting tool
 
 
 class Samples(object):
@@ -57,15 +57,15 @@
     def Ns(self):
         """Return number of samples"""
         return self.samples.shape[-1]
 
     @property
     def geometry(self):
         if self._geometry is None:
-            self._geometry = _DefaultGeometry(grid=np.prod(self.samples.shape[:-1]))
+            self._geometry = _DefaultGeometry1D(grid=np.prod(self.samples.shape[:-1]))
         return self._geometry
 
     @property
     def is_par(self):
         return self._is_par
     
     @is_par.setter
```

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/solver/_solver.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/testproblem/_testproblem.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/testproblem/_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/cuqi/utilities/_utilities.py` & `CUQIpy-0.4.0.post0.dev62/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/pyproject.toml` & `CUQIpy-0.4.0.post0.dev62/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_abstract_distribution_density.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_abstract_distribution_density.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import cuqi
 import pytest
+import numpy as np
 
+geom = {"geometry": 1}
 
 #TODO. Make tests for all distributions going through their input variables
 @pytest.mark.parametrize("dist, expected",[
-    (cuqi.distribution.Gaussian(), ["mean", "cov"]),
-    (cuqi.distribution.Gaussian(mean=1), ["cov"]),
-    (cuqi.distribution.Gaussian(cov=1), ["mean"]),
-    (cuqi.distribution.Gaussian(mean=lambda m: m, cov=lambda c:c), ["m", "c"]),
-    (cuqi.distribution.Gaussian(mean=1, cov=lambda c:c), ["c"]),
-    (cuqi.distribution.Gaussian(mean=lambda m:m, cov=1), ["m"]),
+    (cuqi.distribution.Gaussian(**geom), ["mean", "cov"]),
+    (cuqi.distribution.Gaussian(mean=1, **geom), ["cov"]),
+    (cuqi.distribution.Gaussian(cov=1, **geom), ["mean"]),
+    (cuqi.distribution.Gaussian(mean=lambda m: m, cov=lambda c:c, **geom), ["m", "c"]),
+    (cuqi.distribution.Gaussian(mean=1, cov=lambda c:c, **geom), ["c"]),
+    (cuqi.distribution.Gaussian(mean=lambda m:m, cov=1, **geom), ["m"]),
 ])
 def test_conditioning_variables(dist, expected):
     assert dist.get_conditioning_variables() == expected
 
 def test_conditioning_through_likelihood(): #TODO. Add more dists to test here!
     """ This checks the flow of likelihood evaluation. In particular it checks:
         1) that the mean @property setter is invoked after model evaluation through function/model.
@@ -35,15 +37,15 @@
     """ This checks if we raise error if 2 args are given for a distribution that has no conditioning variables. """
     x = cuqi.distribution.Gaussian(mean=1, cov=1)
     with pytest.raises(ValueError):
         x(5, 3) #Should expect value-error since no cond vars
 
 def test_conditioning_on_main_parameter():
     """ This checks if we can condition on the main parameter in various ways. """
-    x = cuqi.distribution.Gaussian()
+    x = cuqi.distribution.Gaussian(geometry=1)
 
     # With keywords (name also automatically inferred)
     assert isinstance(x(mean=1, x=5), cuqi.likelihood.Likelihood)
     assert isinstance(x(mean=1, cov=1, x=5), cuqi.density.EvaluatedDensity)
     
     # Now using positional arguments
     assert isinstance(x(1, 1, 5), cuqi.density.EvaluatedDensity)
@@ -58,42 +60,42 @@
     """ This tests that we throw error if we accidentally provide arg and kwarg for same variable. """
     x = cuqi.distribution.Gaussian(mean=1)
     with pytest.raises(ValueError):
         x(1, cov=1) #Should expect value-error since cov is given as arg and kwarg.
 
 def test_conditioning_multiple_args():
     """ This tests if conditional variables are printed correctly if they appear in multiple mutable variables"""
-    dist = cuqi.distribution.Gaussian(mean=lambda x,y: x+y, cov=lambda y,z: y+z)
+    dist = cuqi.distribution.Gaussian(mean=lambda x,y: x+y, cov=lambda y,z: y+z, geometry=1)
     assert dist.get_conditioning_variables() == ["x","y","z"]
 
 def test_conditioning_partial_function():
     """ This tests the partial functions we define if only part of a callable is given. """
-    dist = cuqi.distribution.Gaussian(mean=lambda x,y: x+y, cov=lambda y,z: y+z)
+    dist = cuqi.distribution.Gaussian(mean=lambda x,y: x+y, cov=lambda y,z: y+z, geometry=1)
     dist2 = dist(x=1, y=2)
     assert dist2.get_conditioning_variables() == ["z"]
     assert dist2.mean == 3
     assert cuqi.utilities.get_non_default_args(dist2.cov) == ["z"]
 
 def test_conditioning_keeps_name():
     """ This tests if the name of the distribution is kept when conditioning. """
-    y = cuqi.distribution.Gaussian(lambda x:x)
+    y = cuqi.distribution.Gaussian(lambda x:x, geometry=1)
     
     assert y(x=1, cov=1).name == y.name
     assert y(x=1)(cov=1).name == y.name
     assert y(x=1)(cov=1)().name == y.name
 
     assert y(x=1).name == y.name
     assert y(cov=1).name == y.name
     assert y().name == y.name
 
 def test_conditioning_class_flow():
     """ This tests the class flow of conditioning a conditional distribution in various ways """
 
     # Initial conditional distribution on parameter x and cov.
-    y = cuqi.distribution.Gaussian(lambda x:x)
+    y = cuqi.distribution.Gaussian(lambda x:x, geometry=1)
 
     # Conditioning on x is still conditional on cov
     assert y(x=1).is_cond
 
     # Conditioning on y (name of distribution) should return a likelihood
     assert isinstance(y(y=1), cuqi.likelihood.Likelihood)
 
@@ -114,28 +116,28 @@
 
 def test_logp_conditional():
     """ This tests logp evaluation for conditional distributions """
     # Base example logp value
     true_val = cuqi.distribution.Gaussian(3, 7).logd(13)
 
     # Distribution with no specified parameters
-    x = cuqi.distribution.Gaussian(cov=lambda s:s)
+    x = cuqi.distribution.Gaussian(cov=lambda s:s, geometry=1)
 
     # Test logp evaluates correctly in various cases
     assert x.logd(mean=3, s=7, x=13) == true_val
     assert x(x=13).logd(mean=3, s=7) == true_val
     assert x(x=13, mean=3).logd(s=7) == true_val
     assert x(x=13, mean=3, s=7).logd() == true_val
     assert x(mean=3).logd(s=7, x=13) == true_val
     assert x(mean=3, s=7).logd(x=13) == true_val
     assert x(mean=3, x=13).logd(s=7) == true_val
 
 def test_logd_err_handling():
     """ This tests if logp correctly identifies errors in the input """
-    x = cuqi.distribution.Gaussian(cov=lambda s:s)
+    x = cuqi.distribution.Gaussian(cov=lambda s:s, geometry=1)
 
     # Test that we raise error if we don't provide all parameters
     with pytest.raises(ValueError, match=r"To evaluate the log density all conditioning variables and main"):
         x.logd(x=3)
 
     # Test that we raise error if we provide parameters that are not specified
     with pytest.raises(ValueError, match=r"do not match keyword arguments"):
@@ -164,15 +166,15 @@
     # Test that we raise error if we don't provide all parameters
     with pytest.raises(ValueError, match=r"Missing conditioning variables:"):
         x.sample()
 
 
 def test_cond_positional_and_kwargs():
     """ Test conditioning for both positional and kwargs """
-    x = cuqi.distribution.Gaussian(cov=lambda s:s)
+    x = cuqi.distribution.Gaussian(cov=lambda s:s, geometry=1)
 
     logd = x(mean=3, cov=7).logd(13)
 
     # Conditioning full positional
     assert x(3, 7, 13).value == logd
     assert x(3, 7)(13).value == logd
     assert x(3)(7, 13).value == logd
@@ -190,23 +192,52 @@
     assert x(3, s=7)(13).value == logd
     assert x(mean=3)(7, x=13).value == logd
     assert x(mean=3)(7)(x=13).value == logd
     assert x(mean=3)(7)(13).value == logd
 
 def test_logd_positional_and_kwargs():
     """ Test logd for both positional and kwargs """
-    x = cuqi.distribution.Gaussian(cov=lambda s:s)
+    x = cuqi.distribution.Gaussian(cov=lambda s:s, geometry=1)
 
     logd = x(mean=3, s=7).logd(13)
 
     # logd full kwargs
     assert x.logd(mean=3, s=7, x=13) == logd
 
     # logd full positional
     assert x.logd(3, 7, 13) == logd
 
     # logd partial positional
     assert x.logd(3, s=7, x=13) == logd
     assert x.logd(3, 7, x=13) == logd
 
+def test_dim_geometry_compatibility():
+    """ Test the compatibility of dim and geometry attributes """
+    dist = cuqi.distribution.Gaussian(geometry=(2,2))
+    assert dist.dim == dist.geometry.par_dim
+
+def test_geometry_inference_from_dim():
+    """ Test that the geometry attribute is correctly inferred from dim """
+    dist = cuqi.distribution.Gaussian(geometry=5)
+    assert dist.dim == 5
+    assert dist.geometry.par_dim == 5
+
+def test_geometry_inference_from_variables():
+    """ Test that the geometry attribute is correctly inferred from variables """
+    dist = cuqi.distribution.Gaussian(mean=np.ones(5))
+    assert dist.dim == 5
+    assert dist.geometry.par_dim == 5
+
+def test_geometry_setting():
+    """ Test that geometry attribute can be set and is correctly reflected in dim """
+    dist = cuqi.distribution.Gaussian(geometry=1)
+    dist.geometry = cuqi.geometry.Continuous1D(np.ones(5))
+    assert dist.dim == 5
+    assert dist.geometry.par_dim == 5
+
+def test_dim_geometry_conflict():
+    """ Test that an error is raised when both dim and geometry are specified """
+    with pytest.raises(TypeError, match=r"Inconsistent distribution geometry"):
+        dist = cuqi.distribution.Gaussian(np.zeros(2), geometry=cuqi.geometry.Continuous1D(np.ones(5)))
+
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_bayesian_inversion.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_bayesian_inversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cuqi.density import Density
 
 #All Ns are reduced by a factor of 10 for speed. Best results are obtained by increasing Ns by at least 10 times.
 @pytest.mark.parametrize("TP_type, phantom, prior, Ns", 
                          [
                              (Deconvolution1D, "gauss", Gaussian(np.zeros(128), 0.071**2), 20),
                              (Deconvolution1D, "gauss", GMRF(np.zeros(128), 100, 1, "zero"), 20),
-                             (Deconvolution1D, "square", LMRF(np.zeros(128), 0.005), 100),
+                             (Deconvolution1D, "square", LMRF(0, 0.005, geometry=128), 100),
                              (Deconvolution1D, "square", CMRF(np.zeros(128), 0.01), 50),
                          ])
 def test_TP_BayesianProblem_sample(copy_reference, TP_type, phantom, prior, Ns):
     # SKIP NUTS test if not windows (for now)
     if isinstance(prior, CMRF) and not sys.platform.startswith('win'):
         pytest.skip("NUTS(CMRF) regression test is not implemented for this platform")
 
@@ -86,15 +86,15 @@
             50
         ),
         # Case 2: LMRF with Gamma hyperpriors on both noise and prior precision
         (
             Deconvolution1D,
             "square",
             [
-                LMRF(np.zeros(128), lambda d: 1/d, name="x"),
+                LMRF(0, lambda d: 1/d, geometry=128, name="x"),
                 Gamma(1, 1e-4, name="l"),
                 Gamma(1, 1e-4, name="d")
             ],
             50,
         ),
     ]
 )
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_density.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_density.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 import pytest
 import numpy as np
 
 def test_density_variable_name_detection():
     """Test that the density variable name is detected correctly at different levels of the python stack. """
 
     # Test that the density variable name is detected correctly at current level.
-    x = cuqi.distribution.Gaussian()
+    x = cuqi.distribution.Gaussian(geometry=1)
     assert x.name == 'x'
 
     # Test that variable name is detected correctly 1 level deep.
     def inner_name():
-        y = cuqi.distribution.Gaussian()
+        y = cuqi.distribution.Gaussian(geometry=1)
         assert y.name == 'y'
     inner_name()
 
     # Test variable name is detected correctly at n levels deep.
     class recursive_name:
         def __init__(self, max_recursion=10):
             self.max_recursion = max_recursion
         def __call__(self, current_recursion=0):
             if current_recursion == self.max_recursion:
-                z = cuqi.distribution.Gaussian()
+                z = cuqi.distribution.Gaussian(geometry=1)
                 assert z.name == 'z'
             else:
                 self(current_recursion + 1)
     recursive_name()()
 
 def test_variable_name_accross_frames():
     """ Test variable name can be inferred across multiple stack frames. """
 
-    h = cuqi.distribution.Gaussian() # Name should be 'h'
+    h = cuqi.distribution.Gaussian(geometry=1) # Name should be 'h'
 
     def recursive_return_dist(dist, recursions):
         if recursions == 0:
             assert dist.name == 'h' # h was defined many frames above, and name should be inferred correctly.
         else:
             recursive_return_dist(dist, recursions - 1)
     
     recursive_return_dist(h, 10)
 
 def test_density_name_consistency():
 
-    x = cuqi.distribution.Gaussian()
+    x = cuqi.distribution.Gaussian(geometry=1)
     x2 = x(mean=1)
     x3 = x2(cov=1)
 
     # Names should be the same as the original density.  
     assert x3.name == 'x'
     assert x2.name == 'x' 
     assert x.name == 'x'
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_distribution.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,30 +617,14 @@
     g_FD = posterior.gradient(x_i)
 
     # Assert that the exact and FD gradient are close,
     # but not exactly equal (since we use a different method)
     assert np.allclose(g_exact, g_FD) and np.all(g_exact != g_FD)\
         or (np.all(np.isnan(g_exact)) and np.all(np.isnan(g_FD)))
 
-def test_CMRF_should_not_allow_non_zero_location():
-    """" CMRF should not allow non-zero location. """
-    with pytest.raises(ValueError):
-        cuqi.distribution.CMRF(np.ones(5), 1)
-
-    with pytest.raises(ValueError):
-        cuqi.distribution.CMRF(lambda x: x, 1)
-
-def test_LMRF_should_not_allow_non_zero_location():
-    """" LMRF should not allow non-zero location. """
-    with pytest.raises(ValueError):
-        cuqi.distribution.LMRF(np.ones(5), 1)
-
-    with pytest.raises(ValueError):
-        cuqi.distribution.LMRF(lambda x: x, 1)
-
 def test_Cauchy_against_scipy():
     """ Test Cauchy distribution logpdf, cdf, pdf, gradient """
 
     x = cuqi.distribution.Cauchy(np.random.randn(5), np.abs(np.random.rand(5)))
 
     val = np.random.randn(5)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_geometry.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 def test_Discrete_geometry(variables,expected_variables,expected_shape,expected_dim):
     geom = cuqi.geometry.Discrete(variables)
     assert(geom.variables == expected_variables
            and (geom.par_shape == expected_shape)
 	   and (geom.par_dim == expected_dim))
 
 @pytest.mark.parametrize("geom1,geom2,truth_value",
-                         [(cuqi.geometry._DefaultGeometry(2),cuqi.geometry.Continuous1D(2), True),
+                         [(cuqi.geometry._DefaultGeometry1D(2),cuqi.geometry.Continuous1D(2), True),
 			  (cuqi.geometry.Continuous1D(2),cuqi.geometry.Continuous2D((1,2)), False),
-			  (cuqi.geometry._DefaultGeometry(np.array([0,1])),cuqi.geometry.Continuous1D(2), True),
-			  (cuqi.geometry.Continuous1D(2),cuqi.geometry._DefaultGeometry(3), False),
+			  (cuqi.geometry._DefaultGeometry1D(np.array([0,1])),cuqi.geometry.Continuous1D(2), True),
+			  (cuqi.geometry.Continuous1D(2),cuqi.geometry._DefaultGeometry1D(3), False),
 			  (cuqi.geometry.Discrete(2),cuqi.geometry.Discrete(["v0","v1"]), True),
 			  (cuqi.geometry.Discrete(2),cuqi.geometry.Continuous1D(2), False)])
 def test_geometry_equivalence(geom1,geom2,truth_value):
     assert( (geom1==geom2) == truth_value)
 
 # Make sure plotting does not fail at least
 @pytest.mark.parametrize("is_par,plot_par",	[(True,False),(True,True),(False,False)])
@@ -85,16 +85,16 @@
 						(cuqi.geometry.Continuous1D(1),[np.pi],[2*np.pi]),
 						(cuqi.geometry.Continuous1D(3),[1,2,3],[4,5,6]),
 						])
 def test_geometry_plot(geom,lo_val,hi_val,is_par,plot_par):
 	geom.plot_envelope(lo_val,hi_val,is_par=is_par,plot_par=plot_par)
 
 def test_geometry_variables_generator_default():
-	g1 = cuqi.geometry._DefaultGeometry(5)
-	g2 = cuqi.geometry._DefaultGeometry(5)
+	g1 = cuqi.geometry._DefaultGeometry1D(5)
+	g2 = cuqi.geometry._DefaultGeometry1D(5)
 	g1.variables #Extract variables (they are generated in g1, but not in g2)
 	assert g1==g2 #g2 has no _variables yet, but during check its generated.
 
 def test_geometry_variables_generator_Geometry():
 	g1 = cuqi.geometry.Continuous1D(5)
 	g2 = cuqi.geometry.Continuous1D(5)
 	g1.variables #Extract variables (they are generated in g1, but not in g2)
@@ -384,7 +384,13 @@
 
     signal_proj = geom.par2fun(p)
     assert(len(signal_proj) == N)
 
     # Check that the projection is accurate
     rel_err = np.linalg.norm(signal-signal_proj)/np.linalg.norm(signal)
     assert np.isclose(rel_err, 0.0, atol=1e-5)
+
+def test_DefaultGeometry2D_should_be_image2D():
+    geom2D = cuqi.geometry._DefaultGeometry2D((100, 100))
+
+    assert isinstance(geom2D, cuqi.geometry.Image2D)
+
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_joint_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     Js = J._as_stacked()
 
     # Check the dimension
     assert Js.dim == sum(J.dim)
 
     # Check the geometry
-    assert Js.geometry == cuqi.geometry._DefaultGeometry(Js.dim)
+    assert Js.geometry == cuqi.geometry._DefaultGeometry1D(Js.dim)
 
     # Check you can evaluate the log density function with a single vector
     Js.logd(np.ones(Js.dim))
 
     # Check that you can condition on the stacked distribution
     # and again evaluate as a single vector
     Ps = Js(y=data)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_likelihood.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
     # dim
     assert likelihood.dim == model.domain_dim
 
     # geometry
     assert likelihood.geometry == model.domain_geometry
 
 @pytest.mark.parametrize("dist",[
-    cuqi.distribution.Gaussian(),
-    cuqi.distribution.Gaussian(lambda x: x, lambda s: s),
-    cuqi.distribution.Gaussian(cuqi.model.Model(lambda x: x, 2, 2), lambda s:s)
+    cuqi.distribution.Gaussian(geometry=2),
+    cuqi.distribution.Gaussian(lambda x: x, lambda s: s, geometry=2),
+    cuqi.distribution.Gaussian(cuqi.model.Model(lambda x: x, 2, 2), lambda s:s, geometry=2)
 ])
 @pytest.mark.parametrize("mean, cov, data",[
     (np.zeros(2), np.eye(2), np.ones(2)),
-    (np.zeros(3), np.eye(3), np.random.rand(3)),
+    (np.ones(2), 0.1*np.eye(2), np.random.rand(2)),
 ])
 def test_likelihood_conditioning(dist, mean, cov, data):
     """ Test conditioning on parameters of likelihood for Gaussian """
 
     # Create likelihood
     likelihood = dist.to_likelihood(data)
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_model.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_pde.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_problem.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_sampler.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
     # Set up proposals
     #proposal1 = cuqi.distribution.Normal(np.zeros(n),1 )
     #proposal2 = cuqi.distribution.Normal(np.zeros(n),2 )
     #def proposal1(x, sigma): return np.random.normal(x, sigma)
     #def proposal2(x, sigma): return np.random.normal(x, 2*sigma)
 
-    proposal1 =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale )
-    proposal2 =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:2*scale )
+    proposal1 =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale, geometry=n)
+    proposal2 =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:2*scale, geometry=n)
 
 
     # Set up sampler
     MCMC1 = cuqi.sampler.CWMH(target, proposal1, scale, x0)
     MCMC2 = cuqi.sampler.CWMH(target, proposal2, scale, x0)
 
     # Switch proposal
@@ -57,15 +57,15 @@
     R = np.array([[1, -0.7], [-0.7, 1]])
     cov = np.diag(std) @ (R @ np.diag(std))
     def target(x): return cuqi.distribution.Gaussian(mean,cov).pdf(x)
 
     # Define proposal
     # def proposal(x, sigma): return np.random.normal(x, sigma)
     #proposal = cuqi.distribution.Normal(np.zeros(len(mean)),1 )
-    proposal =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale )
+    proposal =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale, geometry=2)
 
     # Set up sampler
     MCMC = cuqi.sampler.CWMH(target, proposal, 0.05, np.array([0,0]))
 
     # Compare with previously computed results
     np.allclose(MCMC.sample(5,1).samples,np.array([[ 0.18158052,  0.17641957,  0.21447146,  0.23666462,  0.23666462],[-0.02885603, -0.00832611, -0.00224236,  0.01444136,  0.01444136]]))
 
@@ -140,15 +140,15 @@
     x0 = 0.5*np.ones(n)
 
     # Set up target
     target = cuqi.distribution.CMRF(np.zeros(n), 0.5, 'neumann')
     target.geometry = cuqi.geometry.Continuous2D((1,2))
 
     # Set up proposals
-    proposal =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale )
+    proposal =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale, geometry=n)
 
     # Set up sampler
     MCMC_sampler = cuqi.sampler.CWMH(target, proposal, scale, x0)
     samples = MCMC_sampler.sample(10,2)
 
     assert(MCMC_sampler.geometry == target.geometry and\
            MCMC_sampler.geometry == samples.geometry)
@@ -226,14 +226,36 @@
     Nb = 200   # burn-in
 
     # Sampling
     s_RTO = cuqi.sampler.Linear_RTO(target).sample_adapt(Ns,Nb)
 
     assert np.allclose(s_RTO.shape,(P.dim,Ns))
 
+def test_sampler_scalar_mean_Gaussian_Linear_RTO():
+
+    model = np.eye(2) # Identity model
+
+    P = cuqi.distribution.Gaussian(0, 1, geometry=2)
+    L = cuqi.distribution.Gaussian(model,np.array([[1,0.5],[0.5,3]]))
+
+    # Data
+    data = np.array([5,6])
+
+    # Posterior
+    target = (data, model, L.sqrtprec, P.mean, P.sqrtprec)
+
+    # Parameters
+    Ns = 200   # number of samples
+    Nb = 20   # burn-in
+
+    # Sampling
+    s_RTO = cuqi.sampler.Linear_RTO(target).sample_adapt(Ns,Nb)
+
+    assert np.allclose(s_RTO.shape,(P.dim,Ns))
+
 
 def test_ULA_UserDefinedDistribution():
     expected_samples = \
         np.array([[0.1, 0.11763052, 0.12740614],
                   [1.1, 1.10399157, 1.1263901 ]])
     np.random.seed(0)
     # Parameters
@@ -354,15 +376,15 @@
 
 @pytest.mark.parametrize("prior, sample_method, expected", [
     (Gaussian(np.zeros(128), 0.1), "_sampleMapCholesky", np.arange(10)), # Direct (no burn-in, no initial guess)
     (Gaussian(np.zeros(128), 0.1), "_sampleLinearRTO", np.arange(1,12)), # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_sampleNUTS", np.arange(1,12)),      # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_samplepCN", np.arange(1,12)),       # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_sampleCWMH", np.arange(1,12)),      # 20% burn-in + initial guess
-    (LMRF(np.zeros(128), 0.1),"_sampleUGLA", np.arange(1,12)),   # 20% burn-in + initial guess
+    (LMRF(0, 0.1, geometry=128),"_sampleUGLA", np.arange(1,12)),   # 20% burn-in + initial guess
     ])
 def test_TP_callback(prior, sample_method, expected):
     """ Test that the callback function is called with the correct sample index by comparing to the expected output.
     
     This tests the pipeline from testproblem all the way to the sampler.
     """
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_samples.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         # is done correctly.
         assert not np.allclose(parameters.samples, funvals.samples) and\
             np.allclose(parameters.samples, val)
 
 def test_cuqiarray_default_geometry():
     """ Test that CUQIarray creates a default geometry when no geometry is passed"""
     v = cuqi.array.CUQIarray([0,1,2,3,4,5,6,7,8])
-    assert type(v.geometry) is cuqi.geometry._geometry._DefaultGeometry
+    assert type(v.geometry) is cuqi.geometry._geometry._DefaultGeometry1D
 
 def test_cuqiarray_multidim():
     X = np.array([[1, 2], [3,4]])
     with pytest.raises(Exception) as e:
         C = cuqi.array.CUQIarray(X)
     assert "input_array cannot be multidimensional when initializing CUQIarray as parameter (with is_par True)." in str(e.value) # this message
     assert e.type == ValueError
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_solver.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_testproblem.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_testproblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     assert np.linalg.norm(model.forward(true_image, is_par=False)) == approx(4.580752014966276)
     assert np.linalg.norm(model.forward(np.ones(model.domain_dim))) == approx(9.37456136258068)
 
 #Deconv 2D tests
 #TODO. Add tests for custom PSF
 @pytest.mark.parametrize("prior",[
     (cuqi.distribution.Gaussian(np.zeros(128**2), 1, name="x")),
-    #(cuqi.distribution.LMRF(np.zeros(128**2), 1, "zeros")),
+    #(cuqi.distribution.LMRF(0, 1, "zeros", geometry=128**2)),
     #(cuqi.distribution.CMRF(np.zeros(128**2), 1, "zeros")),
 ])
 def test_Deconvolution2D_Sampling_prior(prior): 
     tp = cuqi.testproblem.Deconvolution2D(prior=prior)
     tp.prior.geometry = tp.model.domain_geometry
     tp.sample_posterior(10) # Tests that sampling at least runs withour error.
     #TODO. Make into regression tests + other samplers. Move some tests to BayesianProblem
```

### Comparing `CUQIpy-0.4.0.post0.dev27/tests/test_utilities.py` & `CUQIpy-0.4.0.post0.dev62/tests/test_utilities.py`

 * *Files identical despite different names*

