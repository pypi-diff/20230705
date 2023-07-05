# Comparing `tmp/autolens-2023.6.18.3.tar.gz` & `tmp/autolens-2023.7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autolens-2023.6.18.3.tar", last modified: Sun Jun 18 22:19:15 2023, max compression
+gzip compressed data, was "autolens-2023.7.5.2.tar", last modified: Wed Jul  5 14:50:54 2023, max compression
```

## Comparing `autolens-2023.6.18.3.tar` & `autolens-2023.7.5.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.569561 autolens-2023.6.18.3/autolens/
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.569561 autolens-2023.6.18.3/autolens/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/aggregator/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/aggregator/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/aggregator/subhalo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/aggregator/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/analysis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/preloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/analysis/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/config/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/config/non_linear.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/config/visualize/plots.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/imaging/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/mock/mock_fit_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/imaging/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20654 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/imaging/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/imaging/plot/fit_imaging_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/interferometer/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.573561 autolens-2023.6.18.3/autolens/interferometer/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/interferometer/plot/fit_interferometer_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/lens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/lens/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/mock/mock_to_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/mock/mock_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/lens/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/plot/ray_tracing_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24518 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/ray_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/ray_tracing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/subhalo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/lens/to_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/point/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/point/fit_point/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/max_separation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/point_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/point_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/positions_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/fit_point/positions_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/point/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/mock/mock_point_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/point/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/model/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.577561 autolens-2023.6.18.3/autolens/point/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/plot/fit_point_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/plot/point_dataset_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/point_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    27183 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/point/point_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/autolens/quantity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/quantity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/quantity/fit_quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/autolens/quantity/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/quantity/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/quantity/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/quantity/model/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/autolens/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/autolens/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/autolens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-18 22:19:15.000000 autolens-2023.6.18.3/autolens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:19:15.581561 autolens-2023.6.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-18 22:19:01.000000 autolens-2023.6.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/CITATIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.254529 autolens-2023.7.5.2/autolens/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 14:50:44.000000 autolens-2023.7.5.2/autolens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.254529 autolens-2023.7.5.2/autolens/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/aggregator/fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/aggregator/fit_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/aggregator/subhalo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/aggregator/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.254529 autolens-2023.7.5.2/autolens/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/analysis/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/mock/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/preloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/analysis/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/config/non_linear.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/config/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/config/visualize/plots.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/imaging/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/mock/mock_fit_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/imaging/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20654 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/imaging/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/imaging/plot/fit_imaging_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/interferometer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/fit_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/interferometer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/interferometer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/interferometer/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/interferometer/plot/fit_interferometer_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/lens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/lens/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/mock/mock_to_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/mock/mock_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/lens/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/plot/ray_tracing_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24518 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/ray_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/ray_tracing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/subhalo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/lens/to_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.258529 autolens-2023.7.5.2/autolens/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/plot/abstract_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/plot/get_visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/plot/get_visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/plot/get_visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/plot/get_visuals/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/point/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/point/fit_point/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/max_separation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/point_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/point_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/positions_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/fit_point/positions_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/point/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/mock/mock_point_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/point/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/model/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/point/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/plot/fit_point_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/plot/point_dataset_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/point_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27183 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/point/point_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/quantity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/quantity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/quantity/fit_quantity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/quantity/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/quantity/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/quantity/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/quantity/model/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/autolens/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/autolens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-05 14:50:54.000000 autolens-2023.7.5.2/autolens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:50:54.262529 autolens-2023.7.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-05 14:50:43.000000 autolens-2023.7.5.2/setup.py
```

### Comparing `autolens-2023.6.18.3/CITATIONS.rst` & `autolens-2023.7.5.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/LICENSE` & `autolens-2023.7.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/PKG-INFO` & `autolens-2023.7.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autolens
-Version: 2023.6.18.3
+Version: 2023.7.5.2
 Summary: Open-Source Strong Lensing
 Home-page: https://github.com/Jammy2211/PyAutoLens
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autolens-2023.6.18.3/README.rst` & `autolens-2023.7.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/__init__.py` & `autolens-2023.7.5.2/autolens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,8 @@
 from . import mock as m
 from . import util
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.18.3"
+__version__ = "2023.7.5.2"
```

### Comparing `autolens-2023.6.18.3/autolens/aggregator/__init__.py` & `autolens-2023.7.5.2/autolens/aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/aggregator/fit_imaging.py` & `autolens-2023.7.5.2/autolens/aggregator/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/aggregator/fit_interferometer.py` & `autolens-2023.7.5.2/autolens/aggregator/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/aggregator/subhalo.py` & `autolens-2023.7.5.2/autolens/aggregator/subhalo.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/aggregator/tracer.py` & `autolens-2023.7.5.2/autolens/aggregator/tracer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/analysis.py` & `autolens-2023.7.5.2/autolens/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/mock/mock_result.py` & `autolens-2023.7.5.2/autolens/analysis/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/positions.py` & `autolens-2023.7.5.2/autolens/analysis/positions.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/preloads.py` & `autolens-2023.7.5.2/autolens/analysis/preloads.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/result.py` & `autolens-2023.7.5.2/autolens/analysis/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/setup.py` & `autolens-2023.7.5.2/autolens/analysis/setup.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/analysis/visualizer.py` & `autolens-2023.7.5.2/autolens/analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/config/non_linear.yaml` & `autolens-2023.7.5.2/autolens/config/non_linear.yaml`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/config/visualize/plots.yaml` & `autolens-2023.7.5.2/autolens/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/exc.py` & `autolens-2023.7.5.2/autolens/exc.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/fixtures.py` & `autolens-2023.7.5.2/autolens/fixtures.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/fit_imaging.py` & `autolens-2023.7.5.2/autolens/imaging/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/imaging.py` & `autolens-2023.7.5.2/autolens/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/mock/mock_fit_imaging.py` & `autolens-2023.7.5.2/autolens/imaging/mock/mock_fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/model/analysis.py` & `autolens-2023.7.5.2/autolens/imaging/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/model/result.py` & `autolens-2023.7.5.2/autolens/imaging/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/model/visualizer.py` & `autolens-2023.7.5.2/autolens/imaging/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/imaging/plot/fit_imaging_plotters.py` & `autolens-2023.7.5.2/autolens/imaging/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/fit_interferometer.py` & `autolens-2023.7.5.2/autolens/interferometer/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/interferometer.py` & `autolens-2023.7.5.2/autolens/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/model/analysis.py` & `autolens-2023.7.5.2/autolens/interferometer/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/model/result.py` & `autolens-2023.7.5.2/autolens/interferometer/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/model/visualizer.py` & `autolens-2023.7.5.2/autolens/interferometer/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/interferometer/plot/fit_interferometer_plotters.py` & `autolens-2023.7.5.2/autolens/interferometer/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/mock/mock_tracer.py` & `autolens-2023.7.5.2/autolens/lens/mock/mock_tracer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/plot/ray_tracing_plotters.py` & `autolens-2023.7.5.2/autolens/lens/plot/ray_tracing_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/ray_tracing.py` & `autolens-2023.7.5.2/autolens/lens/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/ray_tracing_util.py` & `autolens-2023.7.5.2/autolens/lens/ray_tracing_util.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/subhalo.py` & `autolens-2023.7.5.2/autolens/lens/subhalo.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/lens/to_inversion.py` & `autolens-2023.7.5.2/autolens/lens/to_inversion.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/plot/__init__.py` & `autolens-2023.7.5.2/autolens/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/plot/abstract_plotters.py` & `autolens-2023.7.5.2/autolens/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/plot/get_visuals/one_d.py` & `autolens-2023.7.5.2/autolens/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/plot/get_visuals/two_d.py` & `autolens-2023.7.5.2/autolens/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/fluxes.py` & `autolens-2023.7.5.2/autolens/point/fit_point/fluxes.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/max_separation.py` & `autolens-2023.7.5.2/autolens/point/fit_point/max_separation.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/point_dataset.py` & `autolens-2023.7.5.2/autolens/point/fit_point/point_dataset.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/point_dict.py` & `autolens-2023.7.5.2/autolens/point/fit_point/point_dict.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/positions_image.py` & `autolens-2023.7.5.2/autolens/point/fit_point/positions_image.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/fit_point/positions_source.py` & `autolens-2023.7.5.2/autolens/point/fit_point/positions_source.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/model/analysis.py` & `autolens-2023.7.5.2/autolens/point/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/plot/fit_point_plotters.py` & `autolens-2023.7.5.2/autolens/point/plot/fit_point_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/plot/point_dataset_plotters.py` & `autolens-2023.7.5.2/autolens/point/plot/point_dataset_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/point_dataset.py` & `autolens-2023.7.5.2/autolens/point/point_dataset.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/point/point_solver.py` & `autolens-2023.7.5.2/autolens/point/point_solver.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/quantity/fit_quantity.py` & `autolens-2023.7.5.2/autolens/quantity/fit_quantity.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/quantity/model/analysis.py` & `autolens-2023.7.5.2/autolens/quantity/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/quantity/model/result.py` & `autolens-2023.7.5.2/autolens/quantity/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens/util/__init__.py` & `autolens-2023.7.5.2/autolens/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/autolens.egg-info/SOURCES.txt` & `autolens-2023.7.5.2/autolens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.18.3/setup.py` & `autolens-2023.7.5.2/setup.py`

 * *Files identical despite different names*

