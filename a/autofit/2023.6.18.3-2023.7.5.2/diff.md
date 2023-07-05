# Comparing `tmp/autofit-2023.6.18.3.tar.gz` & `tmp/autofit-2023.7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofit-2023.6.18.3.tar", last modified: Sun Jun 18 22:19:01 2023, max compression
+gzip compressed data, was "autofit-2023.7.5.2.tar", last modified: Wed Jul  5 14:50:39 2023, max compression
```

## Comparing `autofit-2023.6.18.3.tar` & `autofit-2023.7.5.2.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.216183 autofit-2023.6.18.3/autofit/
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8944 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/aggregator/search_output.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/non_linear/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/GridSearch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/mcmc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/nest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/non_linear/optimize.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/Exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/Gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/GaussianKurtosis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/MultiLevelGaussians.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/prior.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/priors/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/config/visualize/plots_search.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/aggregator/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/migration/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/session_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/migration/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.220183 autofit-2023.6.18.3/autofit/database/model/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/model/prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/database/query/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/junction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/database/query/query/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/query/query/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/database/sqlalchemy_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/example/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/example/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/declarative/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/declarative/factor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/factor/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/declarative/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/ep_mean_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/factor_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/expectation_propagation/visualise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.224183 autofit-2023.6.18.3/autofit/graphical/factor_graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/jacobians.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/factor_graphs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/graphical/laplace/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/laplace/optimiser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18909 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/mean_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/graphical/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/interpolator/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/interpolator/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/mock/mock_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/model_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.228184 autofit-2023.6.18.3/autofit/mapper/prior/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/log_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/tuple_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior/width_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/mapper/prior_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63313 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/attribute_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/prior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/recursion.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/prior_model/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mapper/variable_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.232184 autofit-2023.6.18.3/autofit/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/composed_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/messages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38933 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/abstract_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/free_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/model_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/analysis/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/grid/simple_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.236184 autofit-2023.6.18.3/autofit/non_linear/mcmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/abstract_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/auto_correlations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/zeus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/mock/mock_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/nest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/abstract_nest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.240184 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/abstract_optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/globe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/parallel/sneaky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.244184 autofit-2023.6.18.3/autofit/non_linear/paths/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/paths/sub_directory_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/non_linear/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/samples/stored.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/non_linear/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/plot/samples_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/text/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/samples_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/text/text_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.248185 autofit-2023.6.18.3/autofit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/add_notebook_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/update_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/autofit/tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/autofit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-18 22:19:01.000000 autofit-2023.6.18.3/autofit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/add_notebook_quotes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/aggregate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/update_identifiers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/scripts/update_identifiers_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 22:19:01.252185 autofit-2023.6.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-18 22:18:52.000000 autofit-2023.6.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/CITATIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/aggregator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8944 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/aggregator/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/aggregator/search_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/config/non_linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/non_linear/GridSearch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/non_linear/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/non_linear/mcmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/non_linear/nest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/non_linear/optimize.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/notation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/config/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/Exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/Gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/GaussianKurtosis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/MultiLevelGaussians.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/prior.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/profiles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/priors/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/config/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/visualize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/visualize/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/config/visualize/plots_search.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.201546 autofit-2023.7.5.2/autofit/database/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/aggregator/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/database/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/migration/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/migration/session_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/migration/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/database/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/model/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/model/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/model/prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/database/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/junction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/database/query/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/query/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/query/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/query/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/query/query/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/database/sqlalchemy_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/example/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/example/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/example/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/graphical/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/graphical/declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.205546 autofit-2023.7.5.2/autofit/graphical/declarative/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/factor/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/factor/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/factor/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/factor/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/declarative/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.209546 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/ep_mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/factor_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/expectation_propagation/visualise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.209546 autofit-2023.7.5.2/autofit/graphical/factor_graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/jacobians.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/factor_graphs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.209546 autofit-2023.7.5.2/autofit/graphical/laplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/laplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/laplace/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/laplace/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/laplace/optimiser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18909 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/graphical/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.209546 autofit-2023.7.5.2/autofit/interpolator/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/interpolator/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.213547 autofit-2023.7.5.2/autofit/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.213547 autofit-2023.7.5.2/autofit/mapper/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/mock/mock_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/model_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/model_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.213547 autofit-2023.7.5.2/autofit/mapper/prior/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.213547 autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/log_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/tuple_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior/width_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.213547 autofit-2023.7.5.2/autofit/mapper/prior_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63414 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/attribute_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/prior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/recursion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/prior_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mapper/variable_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/composed_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/messages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/non_linear/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38933 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/abstract_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/non_linear/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/free_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/model_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/analysis/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/non_linear/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/result_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/grid/simple_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.217547 autofit-2023.7.5.2/autofit/non_linear/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/abstract_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/auto_correlations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/zeus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mock/mock_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mock/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mock/mock_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/mock/mock_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/nest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/abstract_nest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/abstract_optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/optimize/drawer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/drawer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/drawer/drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/drawer/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.221547 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/globe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.225547 autofit-2023.7.5.2/autofit/non_linear/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/parallel/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/parallel/sneaky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.225547 autofit-2023.7.5.2/autofit/non_linear/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/paths/sub_directory_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.225547 autofit-2023.7.5.2/autofit/non_linear/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/samples/stored.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/non_linear/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.225547 autofit-2023.7.5.2/autofit/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/plot/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/plot/samples_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/autofit/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/text/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/text/samples_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/text/text_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/autofit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/tools/add_notebook_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/tools/namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/tools/update_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/autofit/tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/autofit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-07-05 14:50:39.000000 autofit-2023.7.5.2/autofit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/scripts/add_notebook_quotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/scripts/aggregate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/scripts/update_identifiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/scripts/update_identifiers_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 14:50:39.229547 autofit-2023.7.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-05 14:50:29.000000 autofit-2023.7.5.2/setup.py
```

### Comparing `autofit-2023.6.18.3/CITATIONS.rst` & `autofit-2023.7.5.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/LICENSE` & `autofit-2023.7.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/PKG-INFO` & `autofit-2023.7.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofit
-Version: 2023.6.18.3
+Version: 2023.7.5.2
 Summary: Classy Probabilistic Programming
 Home-page: https://github.com/rhayes777/PyAutoFit
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autofit-2023.6.18.3/README.rst` & `autofit-2023.7.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/__init__.py` & `autofit-2023.7.5.2/autofit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,9 +110,9 @@
 @register(abc.ABCMeta)
 def save_abc(pickler, obj):
     pickle._Pickler.save_type(pickler, obj)
 
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.18.3"
+__version__ = "2023.7.5.2"
```

### Comparing `autofit-2023.6.18.3/autofit/aggregator/aggregator.py` & `autofit-2023.7.5.2/autofit/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/aggregator/predicate.py` & `autofit-2023.7.5.2/autofit/aggregator/predicate.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/aggregator/search_output.py` & `autofit-2023.7.5.2/autofit/aggregator/search_output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/README.rst` & `autofit-2023.7.5.2/autofit/config/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/general.yaml` & `autofit-2023.7.5.2/autofit/config/general.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/non_linear/mcmc.yaml` & `autofit-2023.7.5.2/autofit/config/non_linear/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/non_linear/nest.yaml` & `autofit-2023.7.5.2/autofit/config/non_linear/nest.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/non_linear/optimize.yaml` & `autofit-2023.7.5.2/autofit/config/non_linear/optimize.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/notation.yaml` & `autofit-2023.7.5.2/autofit/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/Gaussian.yaml` & `autofit-2023.7.5.2/autofit/config/priors/Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/GaussianKurtosis.yaml` & `autofit-2023.7.5.2/autofit/config/priors/GaussianKurtosis.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/README.rst` & `autofit-2023.7.5.2/autofit/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/model.yaml` & `autofit-2023.7.5.2/autofit/config/priors/model.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/profiles.yaml` & `autofit-2023.7.5.2/autofit/config/priors/profiles.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/priors/template.yaml` & `autofit-2023.7.5.2/autofit/config/priors/template.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/config/visualize/plots_search.yaml` & `autofit-2023.7.5.2/autofit/config/visualize/plots_search.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/__init__.py` & `autofit-2023.7.5.2/autofit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/aggregator/aggregator.py` & `autofit-2023.7.5.2/autofit/database/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/aggregator/scrape.py` & `autofit-2023.7.5.2/autofit/database/aggregator/scrape.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/migration/migration.py` & `autofit-2023.7.5.2/autofit/database/migration/migration.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/migration/session_wrapper.py` & `autofit-2023.7.5.2/autofit/database/migration/session_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/model/fit.py` & `autofit-2023.7.5.2/autofit/database/model/fit.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/model/instance.py` & `autofit-2023.7.5.2/autofit/database/model/instance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/model/model.py` & `autofit-2023.7.5.2/autofit/database/model/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/model/prior.py` & `autofit-2023.7.5.2/autofit/database/model/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/condition.py` & `autofit-2023.7.5.2/autofit/database/query/condition.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/junction.py` & `autofit-2023.7.5.2/autofit/database/query/junction.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/query/abstract.py` & `autofit-2023.7.5.2/autofit/database/query/query/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/query/attribute.py` & `autofit-2023.7.5.2/autofit/database/query/query/attribute.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/query/info.py` & `autofit-2023.7.5.2/autofit/database/query/query/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/query/query/named.py` & `autofit-2023.7.5.2/autofit/database/query/query/named.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/database/sqlalchemy_.py` & `autofit-2023.7.5.2/autofit/database/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/example/analysis.py` & `autofit-2023.7.5.2/autofit/example/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/example/model.py` & `autofit-2023.7.5.2/autofit/example/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/example/util.py` & `autofit-2023.7.5.2/autofit/example/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/exc.py` & `autofit-2023.7.5.2/autofit/exc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/fixtures.py` & `autofit-2023.7.5.2/autofit/fixtures.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/__init__.py` & `autofit-2023.7.5.2/autofit/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/abstract.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/collection.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/factor/abstract.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/factor/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/factor/analysis.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/factor/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,58 @@
 from autofit.mapper.model import ModelInstance
 from autofit.mapper.prior_model.prior_model import AbstractPriorModel
 from autofit.non_linear.analysis import Analysis
 from autofit.non_linear.paths.abstract import AbstractPaths
 from .abstract import AbstractModelFactor
 
 
+class FactorCallable:
+    def __init__(
+        self,
+        prior_model: AbstractPriorModel,
+        analysis: Analysis,
+    ):
+        self.prior_model = prior_model
+        self.analysis = analysis
+
+    def __call__(self, **kwargs: np.ndarray) -> float:
+        """
+        Returns an instance of the prior model and evaluates it, forming
+        a factor.
+
+        Parameters
+        ----------
+        kwargs
+            Arguments with names that are unique for each prior.
+
+        Returns
+        -------
+        Calculated likelihood
+        """
+        arguments = dict()
+        for name_, array in kwargs.items():
+            prior_id = int(name_.split("_")[1])
+            prior = self.prior_model.prior_with_id(prior_id)
+            arguments[prior] = array
+        # noinspection PyTypeChecker
+        instance = self.prior_model.instance_for_arguments(arguments)
+        return self.analysis.log_likelihood_function(instance)
+
+
 class AnalysisFactor(AbstractModelFactor):
     @property
     def prior_model(self):
         return self._prior_model
 
     def __init__(
-            self,
-            prior_model: AbstractPriorModel,
-            analysis: Analysis,
-            optimiser: Optional[AbstractFactorOptimiser] = None,
-            name=None
+        self,
+        prior_model: AbstractPriorModel,
+        analysis: Analysis,
+        optimiser: Optional[AbstractFactorOptimiser] = None,
+        name=None,
     ):
         """
         A factor in the graph that actually computes the likelihood of a model
         given values for each variable that model contains
 
         Parameters
         ----------
@@ -36,83 +69,42 @@
         optimiser
             A custom optimiser that will be used to fit this factor specifically
             instead of the default optimiser
         """
         self.label = prior_model.label
         self.analysis = analysis
 
-        def _factor(
-                **kwargs: np.ndarray
-        ) -> float:
-            """
-            Returns an instance of the prior model and evaluates it, forming
-            a factor.
-
-            Parameters
-            ----------
-            kwargs
-                Arguments with names that are unique for each prior.
-
-            Returns
-            -------
-            Calculated likelihood
-            """
-            arguments = dict()
-            for name_, array in kwargs.items():
-                prior_id = int(name_.split("_")[1])
-                prior = prior_model.prior_with_id(
-                    prior_id
-                )
-                arguments[prior] = array
-            instance = prior_model.instance_for_arguments(
-                arguments
-            )
-            return analysis.log_likelihood_function(
-                instance
-            )
-
-        prior_variable_dict = {
-            prior.name: prior
-            for prior
-            in prior_model.priors
-        }
+        prior_variable_dict = {prior.name: prior for prior in prior_model.priors}
 
         super().__init__(
             prior_model=prior_model,
-            factor=_factor,
+            factor=FactorCallable(
+                prior_model=prior_model,
+                analysis=analysis,
+            ),
             optimiser=optimiser,
             prior_variable_dict=prior_variable_dict,
-            name=name
+            name=name,
         )
 
     def __getstate__(self):
         return self.__dict__
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
     def __getattr__(self, item):
         return getattr(self.prior_model, item)
 
-    def name_for_variable(
-            self,
-            variable
-    ):
-        path = ".".join(
-            self.prior_model.path_for_prior(
-                variable
-            )
-        )
+    def name_for_variable(self, variable):
+        path = ".".join(self.prior_model.path_for_prior(variable))
         return f"{self.name}.{path}"
 
     def visualize(
-            self,
-            paths: AbstractPaths,
-            instance: ModelInstance,
-            during_analysis: bool
+        self, paths: AbstractPaths, instance: ModelInstance, during_analysis: bool
     ):
         """
         Visualise the instances provided using each factor.
 
         Instances in the ModelInstance must have the same order as the factors.
 
         Parameters
@@ -124,15 +116,15 @@
         during_analysis
             Is this visualisation during analysis?
         """
         self.analysis.visualize(
             paths=paths, instance=instance, during_analysis=during_analysis
         )
         self.analysis.visualize_combined(
-            analyses=None, paths=paths, instance=instance, during_analysis=during_analysis
+            analyses=None,
+            paths=paths,
+            instance=instance,
+            during_analysis=during_analysis,
         )
 
-    def log_likelihood_function(
-            self,
-            instance: ModelInstance
-    ) -> float:
+    def log_likelihood_function(self, instance: ModelInstance) -> float:
         return self.analysis.log_likelihood_function(instance)
```

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/factor/hierarchical.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/factor/hierarchical.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/factor/prior.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/factor/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/graph.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/declarative/result.py` & `autofit-2023.7.5.2/autofit/graphical/declarative/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/ep_mean_field.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/ep_mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/factor_optimiser.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/factor_optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/history.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/history.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/optimiser.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/stochastic.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/stochastic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/expectation_propagation/visualise.py` & `autofit-2023.7.5.2/autofit/graphical/expectation_propagation/visualise.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/factor_graphs/abstract.py` & `autofit-2023.7.5.2/autofit/graphical/factor_graphs/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/factor_graphs/factor.py` & `autofit-2023.7.5.2/autofit/graphical/factor_graphs/factor.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/factor_graphs/graph.py` & `autofit-2023.7.5.2/autofit/graphical/factor_graphs/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/factor_graphs/jacobians.py` & `autofit-2023.7.5.2/autofit/graphical/factor_graphs/jacobians.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/factor_graphs/transform.py` & `autofit-2023.7.5.2/autofit/graphical/factor_graphs/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/laplace/line_search.py` & `autofit-2023.7.5.2/autofit/graphical/laplace/line_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/laplace/newton.py` & `autofit-2023.7.5.2/autofit/graphical/laplace/newton.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/laplace/optimiser.py` & `autofit-2023.7.5.2/autofit/graphical/laplace/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/mean_field.py` & `autofit-2023.7.5.2/autofit/graphical/mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/graphical/utils.py` & `autofit-2023.7.5.2/autofit/graphical/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/interpolator/abstract.py` & `autofit-2023.7.5.2/autofit/interpolator/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/interpolator/covariance.py` & `autofit-2023.7.5.2/autofit/interpolator/covariance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/interpolator/query.py` & `autofit-2023.7.5.2/autofit/interpolator/query.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/identifier.py` & `autofit-2023.7.5.2/autofit/mapper/identifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/mock/mock_model.py` & `autofit-2023.7.5.2/autofit/mapper/mock/mock_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/model.py` & `autofit-2023.7.5.2/autofit/mapper/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/model_mapper.py` & `autofit-2023.7.5.2/autofit/mapper/model_mapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/model_object.py` & `autofit-2023.7.5.2/autofit/mapper/model_object.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/operator.py` & `autofit-2023.7.5.2/autofit/mapper/operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/abstract.py` & `autofit-2023.7.5.2/autofit/mapper/prior/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/arithmetic.py` & `autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/assertion.py` & `autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/assertion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/arithmetic/compound.py` & `autofit-2023.7.5.2/autofit/mapper/prior/arithmetic/compound.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/deferred.py` & `autofit-2023.7.5.2/autofit/mapper/prior/deferred.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/gaussian.py` & `autofit-2023.7.5.2/autofit/mapper/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/log_gaussian.py` & `autofit-2023.7.5.2/autofit/mapper/prior/log_gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/log_uniform.py` & `autofit-2023.7.5.2/autofit/mapper/prior/log_uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/tuple_prior.py` & `autofit-2023.7.5.2/autofit/mapper/prior/tuple_prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/uniform.py` & `autofit-2023.7.5.2/autofit/mapper/prior/uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior/width_modifier.py` & `autofit-2023.7.5.2/autofit/mapper/prior/width_modifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/abstract.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1437,14 +1437,18 @@
     def paths(self) -> List[Path]:
         """
         A list of paths to all the priors in the model, ordered by their
         ids
         """
         return [path for path, _ in self.path_priors_tuples]
 
+    @property
+    def composition(self):
+        return [".".join(path) for path in self.paths]
+
     def sort_priors_alphabetically(self, priors: Iterable[Prior]) -> List[Prior]:
         """
         Sort priors by their paths according to this model.
 
         Parameters
         ----------
         priors
```

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/annotation.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/annotation.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/attribute_pair.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/attribute_pair.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/collection.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/prior_model.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/prior_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/prior_model/recursion.py` & `autofit-2023.7.5.2/autofit/mapper/prior_model/recursion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/variable.py` & `autofit-2023.7.5.2/autofit/mapper/variable.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mapper/variable_operator.py` & `autofit-2023.7.5.2/autofit/mapper/variable_operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/abstract.py` & `autofit-2023.7.5.2/autofit/messages/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/beta.py` & `autofit-2023.7.5.2/autofit/messages/beta.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/composed_transform.py` & `autofit-2023.7.5.2/autofit/messages/composed_transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/fixed.py` & `autofit-2023.7.5.2/autofit/messages/fixed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/gamma.py` & `autofit-2023.7.5.2/autofit/messages/gamma.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/interface.py` & `autofit-2023.7.5.2/autofit/messages/interface.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/normal.py` & `autofit-2023.7.5.2/autofit/messages/normal.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/transform.py` & `autofit-2023.7.5.2/autofit/messages/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/messages/utils.py` & `autofit-2023.7.5.2/autofit/messages/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/mock.py` & `autofit-2023.7.5.2/autofit/mock.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/abstract_search.py` & `autofit-2023.7.5.2/autofit/non_linear/abstract_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/analysis.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/combined.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         """
         self.child_results = results
 
     def __getattr__(self, item: str):
         """
         Get an attribute of the first `Result` object in the list of `Result` objects.
         """
+        if item in ("__getstate__", "__setstate__"):
+            raise AttributeError(item)
         return getattr(self.child_results[0], item)
 
     def __iter__(self):
         return iter(self.child_results)
 
     def __len__(self):
         return len(self.child_results)
@@ -200,20 +202,23 @@
         for each analysis path.
 
         Parameters
         ----------
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         """
+
         def func(child_paths, analysis):
             analysis.visualize_before_fit(child_paths, model)
 
         self._for_each_analysis(func, paths)
 
-    def visualize_before_fit_combined(self, analyses, paths: AbstractPaths, model: AbstractPriorModel):
+    def visualize_before_fit_combined(
+        self, analyses, paths: AbstractPaths, model: AbstractPriorModel
+    ):
         """
         Visualise images and quantities which are shared across all analyses.
 
         For example, each Analysis may have a different dataset, where the data in each dataset is intended to all
         be plotted on the same matplotlib subplot. This function can be overwritten to allow the visualization of such
         a plot.
 
@@ -249,15 +254,21 @@
         """
 
         def func(child_paths, analysis):
             analysis.visualize(child_paths, instance, during_analysis)
 
         self._for_each_analysis(func, paths)
 
-    def visualize_combined(self, analyses : List["Analysis"], instance, paths: AbstractPaths, during_analysis):
+    def visualize_combined(
+        self,
+        analyses: List["Analysis"],
+        instance,
+        paths: AbstractPaths,
+        during_analysis,
+    ):
         """
         Visualise the instance using images and quantities which are shared across all analyses.
 
         For example, each Analysis may have a different dataset, where the fit to each dataset is intended to all
         be plotted on the same matplotlib subplot. This function can be overwritten to allow the visualization of such
         a plot.
 
@@ -273,15 +284,15 @@
         during_analysis
             Is this visualisation during analysis?
         """
         self.analyses[0].visualize_combined(
             analyses=self.analyses,
             paths=paths,
             instance=instance,
-            during_analysis=during_analysis
+            during_analysis=during_analysis,
         )
 
     def profile_log_likelihood_function(
         self,
         paths: AbstractPaths,
         instance,
     ):
```

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/free_parameter.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/free_parameter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/indexed.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/indexed.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,26 +34,36 @@
         return self.analysis.log_likelihood_function(instance[self.index])
 
     # TODO : Add before fit methods here?
 
     def visualize(self, paths: AbstractPaths, instance, during_analysis):
         return self.analysis.visualize(paths, instance[self.index], during_analysis)
 
-    def visualize_combined(self, analyses, paths: AbstractPaths, instance, during_analysis):
-        return self.analysis.visualize_combined(analyses, paths, instance[self.index], during_analysis)
+    def visualize_combined(
+        self, analyses, paths: AbstractPaths, instance, during_analysis
+    ):
+        return self.analysis.visualize_combined(
+            analyses, paths, instance[self.index], during_analysis
+        )
 
     def profile_log_likelihood_function(self, paths: AbstractPaths, instance):
         return self.profile_log_likelihood_function(paths, instance[self.index])
 
     def __getattr__(self, item):
+        if item in ("__getstate__", "__setstate__"):
+            raise AttributeError(item)
         return getattr(self.analysis, item)
 
     def make_result(self, samples, model, sigma=3.0, use_errors=True, use_widths=True):
         return self.analysis.make_result(
-            samples, model, sigma=sigma, use_errors=use_errors, use_widths=use_widths,
+            samples,
+            model,
+            sigma=sigma,
+            use_errors=use_errors,
+            use_widths=use_widths,
         )
 
 
 class IndexCollectionAnalysis(CombinedAnalysis):
     def __init__(self, *analyses):
         """
         Collection of analyses where each analysis has a different
@@ -62,15 +72,18 @@
         Parameters
         ----------
         analyses
             A list of analyses each with a separate model
         """
         super().__init__(
             *[
-                IndexedAnalysis(analysis, index,)
+                IndexedAnalysis(
+                    analysis,
+                    index,
+                )
                 for index, analysis in enumerate(analyses)
             ]
         )
 
     def make_result(self, samples, model, sigma=1.0, use_errors=True, use_widths=False):
         """
         Associate each model with an analysis when creating the result.
```

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/model_analysis.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/model_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         analysis
         model
         """
         self.analysis = analysis
         self.model = model
 
     def __getattr__(self, item):
+        if item in ("__getstate__", "__setstate__"):
+            raise AttributeError(item)
         return getattr(self.analysis, item)
 
     def log_likelihood_function(self, instance):
         return self.analysis.log_likelihood_function(instance)
 
     def make_result(self, samples, model, sigma=1.0, use_errors=True, use_widths=False):
         """
```

### Comparing `autofit-2023.6.18.3/autofit/non_linear/analysis/multiprocessing.py` & `autofit-2023.7.5.2/autofit/non_linear/analysis/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/__init__.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/job.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/job.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/grid_search/result_builder.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/grid_search/result_builder.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/sensitivity.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/sensitivity.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/grid/simple_grid.py` & `autofit-2023.7.5.2/autofit/non_linear/grid/simple_grid.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/initializer.py` & `autofit-2023.7.5.2/autofit/non_linear/initializer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/abstract_mcmc.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/abstract_mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/auto_correlations.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/auto_correlations.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/emcee.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/emcee.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/plotter.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/emcee/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/emcee/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/plotter.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mcmc/zeus/zeus.py` & `autofit-2023.7.5.2/autofit/non_linear/mcmc/zeus/zeus.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mock/mock_analysis.py` & `autofit-2023.7.5.2/autofit/non_linear/mock/mock_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mock/mock_result.py` & `autofit-2023.7.5.2/autofit/non_linear/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mock/mock_samples.py` & `autofit-2023.7.5.2/autofit/non_linear/mock/mock_samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/mock/mock_search.py` & `autofit-2023.7.5.2/autofit/non_linear/mock/mock_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/abstract_nest.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/abstract_nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/abstract.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/dynamic.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/dynamic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/plotter.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/dynesty/static.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/dynesty/static.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/plotter.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/nest/ultranest/ultranest.py` & `autofit-2023.7.5.2/autofit/non_linear/nest/ultranest/ultranest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/abstract_optimize.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/abstract_optimize.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/drawer/drawer.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/drawer/drawer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/lbfgs.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/lbfgs.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/lbfgs/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/lbfgs/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/abstract.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/globe.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/globe.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/local.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/local.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/plotter.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/optimize/pyswarms/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/optimize/pyswarms/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/parallel/process.py` & `autofit-2023.7.5.2/autofit/non_linear/parallel/process.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/parallel/sneaky.py` & `autofit-2023.7.5.2/autofit/non_linear/parallel/sneaky.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/paths/abstract.py` & `autofit-2023.7.5.2/autofit/non_linear/paths/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/paths/database.py` & `autofit-2023.7.5.2/autofit/non_linear/paths/database.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/paths/directory.py` & `autofit-2023.7.5.2/autofit/non_linear/paths/directory.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/paths/null.py` & `autofit-2023.7.5.2/autofit/non_linear/paths/null.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/paths/sub_directory_paths.py` & `autofit-2023.7.5.2/autofit/non_linear/paths/sub_directory_paths.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/result.py` & `autofit-2023.7.5.2/autofit/non_linear/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/mcmc.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/nest.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/pdf.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/pdf.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/sample.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/sample.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/samples.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/samples/stored.py` & `autofit-2023.7.5.2/autofit/non_linear/samples/stored.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/settings.py` & `autofit-2023.7.5.2/autofit/non_linear/settings.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/non_linear/timer.py` & `autofit-2023.7.5.2/autofit/non_linear/timer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/plot/output.py` & `autofit-2023.7.5.2/autofit/plot/output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/plot/samples_plotters.py` & `autofit-2023.7.5.2/autofit/plot/samples_plotters.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/text/formatter.py` & `autofit-2023.7.5.2/autofit/text/formatter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/text/samples_text.py` & `autofit-2023.7.5.2/autofit/text/samples_text.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/text/text_util.py` & `autofit-2023.7.5.2/autofit/text/text_util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/tools/add_notebook_quotes.py` & `autofit-2023.7.5.2/autofit/tools/add_notebook_quotes.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/tools/update_identifiers.py` & `autofit-2023.7.5.2/autofit/tools/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit/tools/util.py` & `autofit-2023.7.5.2/autofit/tools/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/autofit.egg-info/SOURCES.txt` & `autofit-2023.7.5.2/autofit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/scripts/update_identifiers.py` & `autofit-2023.7.5.2/scripts/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/scripts/update_identifiers_from_file.py` & `autofit-2023.7.5.2/scripts/update_identifiers_from_file.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.6.18.3/setup.py` & `autofit-2023.7.5.2/setup.py`

 * *Files identical despite different names*

