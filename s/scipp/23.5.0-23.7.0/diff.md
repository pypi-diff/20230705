# Comparing `tmp/scipp-23.5.0.tar.gz` & `tmp/scipp-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipp-23.5.0.tar", last modified: Wed May 31 10:20:11 2023, max compression
+gzip compressed data, was "scipp-23.7.0.tar", last modified: Wed Jul  5 06:15:11 2023, max compression
```

## Comparing `scipp-23.5.0.tar` & `scipp-23.7.0.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-31 10:19:47.000000 scipp-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-05-31 10:20:11.965467 scipp-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-31 10:19:47.000000 scipp-23.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.949467 scipp-23.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/_binding.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/_scipp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/binning/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/binning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/compat/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5935 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/pandas_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/xarray_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/configuration/config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/constants/
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/coords/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/coord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/coord_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5211 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/rule.py
--rw-r--r--   0 runner    (1001) docker     (122)    12893 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/transform_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/core/
--rw-r--r--   0 runner    (1001) docker     (122)     3967 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/_cpp_wrapper_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/argument_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/assignments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/bin_remapping.py
--rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/binning.py
--rw-r--r--   0 runner    (1001) docker     (122)    18006 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/bins.py
--rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/concepts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cpp_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    42413 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cpp_classes.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (122)    21420 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/data_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/domains.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/groupby.py
--rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/like.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/logical.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/math.py
--rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/reduction.py
--rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/shape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/structured.py
--rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/trigonometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/unary.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    29249 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/data/
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/extend_units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/format/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/formatting_datagroup_html.py
--rw-r--r--   0 runner    (1001) docker     (122)    16472 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/formatting_html.py
--rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/html/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/datagroup.css
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_atomic_row.html
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_collapsible_row.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_detail_list.html
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_repr.html
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/icons-svg-inline.html
--rw-r--r--   0 runner    (1001) docker     (122)     9794 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/style.css.template
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/io/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15758 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/object_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/displayable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure2d.py
--rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel.py
--rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/resampling_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view.py
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/integrate/
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/integrate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/interpolate/
--rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/interpolate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/ndimage/
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/ndimage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/optimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/signal/
--rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)    19028 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/spatial/
--rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/spatial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/sphinxext/autoplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/assertions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/units/
--rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/collapse_and_slices.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/pyshell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/to_string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-05 06:14:45.000000 scipp-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-05 06:15:11.581833 scipp-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-05 06:14:45.000000 scipp-23.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.565833 scipp-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/
+-rw-r--r--   0 runner    (1001) docker     (122)     8722 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/_binding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/_extend_units.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/_scipp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/binning/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/binning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6012 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/compat/dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/compat/pandas_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/compat/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/compat/xarray_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/configuration/config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.569833 scipp-23.7.0/src/scipp/coords/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/coord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/coord_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5213 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7452 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12557 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/coords/transform_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.573833 scipp-23.7.0/src/scipp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     6443 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/_cpp_wrapper_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/argument_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/assignments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/bin_remapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/binning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18163 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/bins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/cpp_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42476 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/cpp_classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21420 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/data_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/domains.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/logical.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/structured.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/trigonometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/unary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29376 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/core/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.573833 scipp-23.7.0/src/scipp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.573833 scipp-23.7.0/src/scipp/format/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/format/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/format/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.577833 scipp-23.7.0/src/scipp/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/formatting_datagroup_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16489 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/formatting_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.577833 scipp-23.7.0/src/scipp/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/datagroup.css
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/dg_atomic_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/dg_collapsible_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/dg_detail_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/dg_repr.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/icons-svg-inline.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9792 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/html/templates/style.css.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.577833 scipp-23.7.0/src/scipp/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15866 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/controller1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/controller2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/controller3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/displayable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/figure1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/figure2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/figure3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/model1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/panel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/panel1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/panel3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/resampling_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/view1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/plotting/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/integrate/
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/integrate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/interpolate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/ndimage/
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/ndimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/optimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/scipy/signal/
+-rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/scipy/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19469 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/spatial/
+-rw-r--r--   0 runner    (1001) docker     (122)    11960 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/spatial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/sphinxext/autoplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5075 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/testing/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7956 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/units/
+-rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 06:15:11.581833 scipp-23.7.0/src/scipp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/collapse_and_slices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/pyshell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-07-05 06:14:45.000000 scipp-23.7.0/src/scipp/utils/to_string.py
```

### Comparing `scipp-23.5.0/LICENSE` & `scipp-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/PKG-INFO` & `scipp-23.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipp
-Version: 23.5.0
+Version: 23.7.0
 Summary: Multi-dimensional data arrays with labeled dimensions
 Home-page: https://github.com/scipp/scipp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD-3-Clause
 Project-URL: Documentation, https://scipp.github.io/
 Project-URL: Bug Tracker, https://github.com/scipp/scipp/issues
 Project-URL: Changelog, https://scipp.github.io/about/release-notes.html
```

### Comparing `scipp-23.5.0/src/scipp/_binding.py` & `scipp-23.7.0/src/scipp/_binding.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/compat/dict.py` & `scipp-23.7.0/src/scipp/compat/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     """Convert a Scipp Variable to a python dict."""
     out = {
         "dims": _dims_to_strings(v.dims),
         "shape": v.shape,
         "unit": v.unit,
         "dtype": v.dtype,
     }
+    if not v.aligned:
+        out["aligned"] = False
 
     # Use defaultdict to return the raw values/variances by default
     dtype_parser = defaultdict(lambda: lambda x, y: x)
     # Using raw dtypes as dict keys doesn't appear to work, so we need to
     # convert to strings.
     dtype_parser.update(
         {
@@ -127,15 +129,15 @@
     scipp.to_dict
     """
     keys_as_set = set(dict_obj.keys())
     if {"coords", "data"}.issubset(keys_as_set):
         # Case of a DataArray-like dict (most-likely)
         return _dict_to_data_array(dict_obj)
     elif keys_as_set.issubset(
-        {"dims", "values", "variances", "unit", "dtype", "shape"}
+        {"dims", "values", "variances", "unit", "dtype", "shape", "aligned"}
     ):
         # Case of a Variable-like dict (most-likely)
         return _dict_to_variable(dict_obj)
     else:
         # Case of a Dataset-like dict
         out = Dataset()
         for key, item in dict_obj.items():
@@ -144,15 +146,15 @@
 
 
 def _dict_to_variable(d):
     """Convert a Python dict to a Scipp Variable."""
     d = dict(d)
     # The Variable constructor does not accept both `shape` and `values`. If
     # `values` is present, remove `shape` from the list.
-    keylist = list(d.keys())
+    keylist = set(d.keys())
     if "values" in keylist and "shape" in keylist:
         keylist.remove("shape")
     out = {}
 
     for key in keylist:
         if key == "dtype" and isinstance(d[key], str):
             out[key] = getattr(DType, d[key])
@@ -168,15 +170,16 @@
         if not out['dims']:
             out['value'] = out['values']
             del out['values']
             del out['dims']
         for key in ['dtype', 'variance', 'variances']:
             if key in out:
                 del out[key]
-    return make_var(**out)
+    var = make_var(**out)
+    return var
 
 
 def _dict_to_data_array(d):
     """Convert a Python dict to a Scipp DataArray."""
     d = dict(d)
     if "data" not in d:
         raise KeyError(
```

### Comparing `scipp-23.5.0/src/scipp/compat/pandas_compat.py` & `scipp-23.7.0/src/scipp/compat/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/compat/wrapping.py` & `scipp-23.7.0/src/scipp/compat/wrapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/compat/xarray_compat.py` & `scipp-23.7.0/src/scipp/compat/xarray_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/configuration/__init__.py` & `scipp-23.7.0/src/scipp/configuration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,7 +125,8 @@
 
     def items(self) -> Iterable[Tuple[str, Any]]:
         """Returns iterable over parameter names and values."""
         yield from self.get().items()
 
 
 config = Config()
+__all__ = ['config']
```

### Comparing `scipp-23.5.0/src/scipp/configuration/config_default.yaml` & `scipp-23.7.0/src/scipp/configuration/config_default.yaml`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/constants/__init__.py` & `scipp-23.7.0/src/scipp/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/coords/coord.py` & `scipp-23.7.0/src/scipp/coords/coord.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
 import dataclasses
-from enum import Enum, auto
 from typing import Optional
 
 from ..core import Variable
 
 
-class Destination(Enum):
-    coord = auto()
-    attr = auto()
-
-    @property
-    def other(self):
-        return Destination.attr if self == Destination.coord else Destination.coord
-
-
 @dataclasses.dataclass
 class Coord:
     dense: Optional[Variable]  # for dense variable or bin-coord
     event: Optional[Variable]
-    destination: Destination
+    aligned: bool
     usages: int = -1  # negative for unlimited usages
 
     @property
     def has_dense(self) -> bool:
         return self.dense is not None
 
     @property
```

### Comparing `scipp-23.5.0/src/scipp/coords/coord_table.py` & `scipp-23.7.0/src/scipp/coords/coord_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
 import dataclasses
 from typing import Dict, Iterable, List, Set, Tuple
 
-from .coord import Coord, Destination
+from .coord import Coord
 from .options import Options
 from .rule import FetchRule, RenameRule, Rule, rule_output_names
 
 
 class CoordTable:
     """
     Stores a dictionary of coordinates for use in coord transforms.
@@ -28,15 +28,15 @@
             self._total_usages[name] = -1
 
     def add(self, name: str, coord: Coord):
         self._coords[name] = dataclasses.replace(coord, usages=self.total_usages(name))
 
     def consume(self, name: str) -> Coord:
         coord = self._coords[name]
-        coord.destination = Destination.attr
+        coord.aligned = False
         coord.use()
         if coord.usages == 0:
             # The coord's data is no longer needed in the table.
             # But the caller of `consume` does need it, so return `coord` as is.
             self._coords[name] = dataclasses.replace(coord, dense=None, event=None)
         return coord
```

### Comparing `scipp-23.5.0/src/scipp/coords/graph.py` & `scipp-23.7.0/src/scipp/coords/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             rule = self._rule_for(out_name, da)
             for name in rule.out_names:
                 subgraph[name] = rule
             depth_first_stack.extend(rule.dependencies)
         return Graph(subgraph)
 
     def _rule_for(self, out_name: str, da: DataArray) -> Rule:
-        if _is_in_meta_data(out_name, da):
-            return FetchRule((out_name,), da.meta, da.bins.meta if da.bins else {})
+        if _is_in_coords(out_name, da):
+            return FetchRule((out_name,), da.coords, da.bins.coords if da.bins else {})
         try:
             return self._rules[out_name]
         except KeyError:
             raise KeyError(
                 f"Coordinate '{out_name}' does not exist in the input data "
                 "and no rule has been provided to compute it."
             ) from None
@@ -137,9 +137,9 @@
                 raise ValueError(
                     f'Duplicate output name defined in conversion graph: {product}'
                 )
             rule_graph[product] = rule
     return rule_graph
 
 
-def _is_in_meta_data(name: str, da: DataArray) -> bool:
-    return name in da.meta or (da.bins is not None and name in da.bins.meta)
+def _is_in_coords(name: str, da: DataArray) -> bool:
+    return name in da.coords or (da.bins is not None and name in da.bins.coords)
```

### Comparing `scipp-23.5.0/src/scipp/coords/rule.py` & `scipp-23.7.0/src/scipp/coords/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import inspect
 from abc import ABC, abstractmethod
 from copy import copy
 from functools import partial
 from typing import Any, Callable, Dict, Iterable, List, Mapping, Tuple
 
 from ..core import Variable
-from .coord import Coord, Destination
+from .coord import Coord
 
 try:
     from typing import Protocol as _Protocol
 
     # Importing CoordTable from coord_table.py would result in an import
     # cycle because that module import rule.py
     # CoordTable is only needed for type annotations here,
@@ -50,15 +50,15 @@
         return f'({", ".join(self.out_names)})'
 
 
 class FetchRule(Rule):
     """
     Get coords from the provided dict-like sources.
 
-    Can be used to abstract away retrieving coords and attrs from the input DataArray.
+    Can be used to abstract away retrieving coords from the input DataArray.
     """
 
     def __init__(
         self,
         out_names: Tuple[str, ...],
         dense_sources: Mapping[str, Variable],
         event_sources: Mapping[str, Variable],
@@ -68,15 +68,15 @@
         self._event_sources = event_sources
 
     def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
         return {
             out_name: Coord(
                 dense=self._dense_sources.get(out_name, None),
                 event=self._event_sources.get(out_name, None),
-                destination=Destination.coord,
+                aligned=True,
             )
             for out_name in self.out_names
         }
 
     @property
     def dependencies(self) -> Tuple[str]:
         return ()  # type: ignore
@@ -92,15 +92,15 @@
 
     def __init__(self, out_names: Tuple[str, ...], in_name: str):
         super().__init__(out_names)
         self._in_name = in_name
 
     def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
         # Shallow copy the _Coord object to allow the alias to have
-        # a different destination and usage count than the original.
+        # a different alignment and usage count than the original.
         return {
             out_name: copy(coords.consume(self._in_name)) for out_name in self.out_names
         }
 
     @property
     def dependencies(self) -> Tuple[str]:
         return tuple((self._in_name,))
@@ -135,15 +135,15 @@
                     outputs[name].dense = coord.dense
         return self._without_unrequested(outputs)
 
     def _compute_pure_dense(self, inputs):
         outputs = self._func(**{name: coord.dense for name, coord in inputs.items()})
         outputs = self._to_dict(outputs)
         return {
-            name: Coord(dense=var, event=None, destination=Destination.coord)
+            name: Coord(dense=var, event=None, aligned=True)
             for name, var in outputs.items()
         }
 
     def _compute_with_events(self, inputs):
         args = {
             name: coord.event if coord.has_event else coord.dense
             for name, coord in inputs.items()
@@ -151,15 +151,15 @@
         outputs = self._to_dict(self._func(**args))
         # Dense outputs may be produced as side effects of processing event
         # coords.
         outputs = {
             name: Coord(
                 dense=var if var.bins is None else None,
                 event=var if var.bins is not None else None,
-                destination=Destination.coord,
+                aligned=True,
             )
             for name, var in outputs.items()
         }
         return outputs
 
     def _without_unrequested(self, d: Dict[str, Any]) -> Dict[str, Any]:
         missing_outputs = [key for key in self.out_names if key not in d]
```

### Comparing `scipp-23.5.0/src/scipp/coords/transform_coords.py` & `scipp-23.7.0/src/scipp/coords/transform_coords.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 from dataclasses import fields
 from fractions import Fraction
 from typing import Callable, Dict, Iterable, List, Mapping, Optional, Set, Union
 
 from ..core import DataArray, Dataset, DimensionError, VariableError, bins, empty
 from ..logging import get_logger
-from .coord_table import Coord, CoordTable, Destination
+from .coord_table import Coord, CoordTable
 from .graph import Graph, GraphDict, rule_sequence
 from .options import Options
 from .rule import ComputeRule, FetchRule, RenameRule, Rule, rule_output_names
 
 
 def transform_coords(
     x: Union[DataArray, Dataset],
@@ -56,21 +56,21 @@
     rename_dims:
         Rename dimensions if the corresponding dimension coords
         are used as inputs and there is a single output coord
         that can be associated with that dimension.
         See the user guide for more details and examples.
         Default is True.
     keep_aliases:
-        If True, aliases for coords defined in graph are
-        included in the output. Default is True.
+        If True, include aliases in the output.
+        Default is True.
     keep_intermediate:
-        Keep attributes created as intermediate results.
+        If True, include intermediate results in the output.
         Default is True.
     keep_inputs:
-        Keep consumed input coordinates or attributes.
+        Include consumed input coordinates in the output.
         Default is True.
     quiet:
         If True, no log output is produced. Otherwise, ``transform_coords``
         produces a log of its actions.
     **kwargs:
         Mapping of coords to callables. This can be used as an alternate and brief
         way of specifying targets and graph. If provided, neither ``targets`` nor
@@ -186,15 +186,15 @@
     rules = rule_sequence(graph)
     working_coords = CoordTable(rules, targets, options)
     dim_coords = set()
     for rule in rules:
         for name, coord in rule(working_coords).items():
             working_coords.add(name, coord)
             # Check if coord is a dimension-coord. Need to also check if it is in the
-            # data dimensions because slicing can produce attrs with dims that are
+            # data dimensions because slicing can produce coords with dims that are
             # no longer in the data.
             if name in original.dims and coord.has_dim(name):
                 dim_coords.add(name)
 
     dim_name_changes = (
         _dim_name_changes(graph, dim_coords) if options.rename_dims else {}
     )
@@ -205,18 +205,18 @@
 
 
 def _transform_dataset(
     original: Dataset, targets: Set[str], graph: Graph, *, options: Options
 ) -> Dataset:
     # Note the inefficiency here in datasets with multiple items: Coord
     # transform is repeated for every item rather than sharing what is
-    # possible. Implementing this would be tricky and likely error-prone,
-    # since different items may have different attributes. Unless we have
-    # clear performance requirements we therefore go with the safe and
-    # simple solution
+    # possible. Implementing this used to be tricky and likely error-prone,
+    # since different items may have had different attributes. Unless we have
+    # clear performance requirements, we therefore went with the safe and
+    # simple solution.
     if len(original) > 0:
         return Dataset(
             data={
                 name: _transform_data_array(
                     original[name], targets=targets, graph=graph, options=options
                 )
                 for name in original
@@ -274,34 +274,25 @@
         '\n'.join(f'    {rule}' for rule in steps) if steps else '    None'
     )
 
     get_logger().info(message)
 
 
 def _store_coord(da: DataArray, name: str, coord: Coord) -> None:
-    def try_del(dest):
-        if dest == Destination.coord:
-            da.coords.pop(name, None)
-            if da.bins is not None:
-                da.bins.coords.pop(name, None)
-        else:
-            da.attrs.pop(name, None)
-            if da.bins is not None:
-                da.bins.attrs.pop(name, None)
+    def try_del():
+        da.coords.pop(name, None)
+        if da.bins is not None:
+            da.bins.coords.pop(name, None)
 
     def store(x, c):
-        if coord.destination == Destination.coord:
-            x.coords[name] = c
-        else:
-            x.attrs[name] = c
-
-    try_del(coord.destination.other)
+        x.coords[name] = c
+        x.coords.set_aligned(name, coord.aligned)
 
     if coord.usages == 0:
-        try_del(coord.destination)
+        try_del()
     else:
         if coord.has_dense:
             store(da, coord.dense)
         if coord.has_event:
             try:
                 store(da.bins, coord.event)
             except (DimensionError, VariableError):
@@ -312,15 +303,15 @@
 
 def _store_results(da: DataArray, coords: CoordTable, targets: Set[str]) -> DataArray:
     da = da.copy(deep=False)
     if da.bins is not None:
         da.data = bins(**da.bins.constituents)
     for name, coord in coords.items():
         if name in targets:
-            coord.destination = Destination.coord
+            coord.aligned = True
         _store_coord(da, name, coord)
     return da
 
 
 def _color_dims(graph: Graph, dim_coords: Set[str]) -> Dict[str, Dict[str, Fraction]]:
     colors = {
         coord: {dim: Fraction(0, 1) for dim in dim_coords} for coord in graph.nodes()
```

### Comparing `scipp-23.5.0/src/scipp/core/_cpp_wrapper_util.py` & `scipp-23.7.0/src/scipp/core/_cpp_wrapper_util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/_sizes.py` & `scipp-23.7.0/src/scipp/core/_sizes.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/argument_handlers.py` & `scipp-23.7.0/src/scipp/core/argument_handlers.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/arithmetic.py` & `scipp-23.7.0/src/scipp/core/arithmetic.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/assignments.py` & `scipp-23.7.0/src/scipp/core/assignments.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/bin_remapping.py` & `scipp-23.7.0/src/scipp/core/bin_remapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/binning.py` & `scipp-23.7.0/src/scipp/core/binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
       >>> y = sc.array(dims=['row'], unit='m', values=rng.random(100))
       >>> data = sc.ones(dims=['row'], unit='K', shape=[100])
       >>> table = sc.DataArray(data=data, coords={'x': x, 'y': y})
       >>> table.hist(x=2)
       <scipp.DataArray>
       Dimensions: Sizes[x:2, ]
       Coordinates:
-        x                         float64              [m]  (x [bin-edge])  [0.00313229, 0.497696, 0.992259]
+      * x                         float64              [m]  (x [bin-edge])  [0.00313229, 0.497696, 0.992259]
       Data:
                                   float64              [K]  (x)  [53, 47]
 
       >>> table.hist(x=sc.scalar(0.2, unit='m')).sizes
       {'x': 5}
 
       >>> table.hist(x=sc.linspace('x', 0.2, 0.8, num=10, unit='m')).sizes
```

### Comparing `scipp-23.5.0/src/scipp/core/bins.py` & `scipp-23.7.0/src/scipp/core/bins.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,19 @@
 
     @unit.setter
     def unit(self, unit: Union[_cpp.Unit, str]):
         """Set unit of the bin elements"""
         self.constituents['data'].unit = unit
 
     @property
+    def aligned(self) -> bool:
+        """Alignment flag for coordinates of bin elements."""
+        return self.constituents['data'].aligned
+
+    @property
     def constituents(self) -> Dict[str, Union[str, _cpp.Variable, _cpp.DataArray]]:
         """Constituents of binned data, as supported by :py:func:`sc.bins`."""
         return _call_cpp_func(_cpp.bins_constituents, self._data())
 
     def sum(self) -> Union[_cpp.Variable, _cpp.DataArray]:
         """Sum of events in each bin.
```

### Comparing `scipp-23.5.0/src/scipp/core/comparison.py` & `scipp-23.7.0/src/scipp/core/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/concepts.py` & `scipp-23.7.0/src/scipp/core/concepts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/counts.py` & `scipp-23.7.0/src/scipp/core/counts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/cpp_classes.pyi` & `scipp-23.7.0/src/scipp/core/cpp_classes.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1967,14 +1967,17 @@
 
     def round(self, *, out: Optional[VariableLike]=None) -> VariableLike:
         ...
 
     def save_hdf5(self, filename: Union[str, Path]) -> None:
         ...
 
+    def set_aligned(self, aligned: bool) -> None:
+        ...
+
     @property
     def shape(self) -> tuple:
         ...
 
     @property
     def size(self) -> int:
         ...
```

### Comparing `scipp-23.5.0/src/scipp/core/cumulative.py` & `scipp-23.7.0/src/scipp/core/cumulative.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/data_group.py` & `scipp-23.7.0/src/scipp/core/data_group.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/dataset.py` & `scipp-23.7.0/src/scipp/core/dataset.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/dimensions.py` & `scipp-23.7.0/src/scipp/core/dimensions.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/domains.py` & `scipp-23.7.0/src/scipp/core/domains.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/groupby.py` & `scipp-23.7.0/src/scipp/core/groupby.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/like.py` & `scipp-23.7.0/src/scipp/core/like.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/logical.py` & `scipp-23.7.0/src/scipp/core/logical.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/math.py` & `scipp-23.7.0/src/scipp/core/math.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/operations.py` & `scipp-23.7.0/src/scipp/core/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/reduction.py` & `scipp-23.7.0/src/scipp/core/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/shape.py` & `scipp-23.7.0/src/scipp/core/shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
       >>> x = sc.DataArray(sc.arange('x', 3), coords={'x': sc.arange('x', 3)})
       >>> y = sc.DataArray(100 * sc.arange('x', 3), coords={'x': 100 * sc.arange('x', 3)})
       >>> z = sc.concat([x, y], dim='x')
       >>> z
       <scipp.DataArray>
       Dimensions: Sizes[x:6, ]
       Coordinates:
-        x                           int64  [dimensionless]  (x)  [0, 1, ..., 100, 200]
+      * x                           int64  [dimensionless]  (x)  [0, 1, ..., 100, 200]
       Data:
                                     int64  [dimensionless]  (x)  [0, 1, ..., 100, 200]
       >>> z.values
       array([  0,   1,   2,   0, 100, 200])
     """
     if x and isinstance(x[0], data_group.DataGroup):
         return data_group._apply_to_items(concat, x, dim)
@@ -178,15 +178,15 @@
       <scipp.Variable> (y: 2, z: 3)      int64  [dimensionless]  [0, 1, ..., 4, 5]
 
       >>> a = sc.DataArray(0.1 * sc.arange('x', 6), coords={'x': sc.arange('x', 6)})
       >>> sc.fold(a, dim='x', sizes={'y': 2, 'z': 3})
       <scipp.DataArray>
       Dimensions: Sizes[y:2, z:3, ]
       Coordinates:
-        x                           int64  [dimensionless]  (y, z)  [0, 1, ..., 4, 5]
+      * x                           int64  [dimensionless]  (y, z)  [0, 1, ..., 4, 5]
       Data:
                                   float64  [dimensionless]  (y, z)  [0, 0.1, ..., 0.4, 0.5]
       >>> sc.fold(a, dim='x', sizes={'y': 2, 'z': 3}).data.values
       array([[0. , 0.1, 0.2],
              [0.3, 0.4, 0.5]])
       >>> sc.fold(a, dim='x', sizes={'y': 2, 'z': 3}).coords['x'].values
       array([[0, 1, 2],
@@ -285,26 +285,26 @@
       ...                'y': sc.arange('y', 3),
       ...                'xy': sc.array(dims=['x', 'y'],
       ...                               values=np.arange(6).reshape(2, 3))})
       >>> a
       <scipp.DataArray>
       Dimensions: Sizes[x:2, y:3, ]
       Coordinates:
-        x                           int64  [dimensionless]  (x)  [0, 1]
-        xy                          int64  [dimensionless]  (x, y)  [0, 1, ..., 4, 5]
-        y                           int64  [dimensionless]  (y)  [0, 1, 2]
+      * x                           int64  [dimensionless]  (x)  [0, 1]
+      * xy                          int64  [dimensionless]  (x, y)  [0, 1, ..., 4, 5]
+      * y                           int64  [dimensionless]  (y)  [0, 1, 2]
       Data:
                                   float64  [dimensionless]  (x, y)  [0, 0.1, ..., 0.4, 0.5]
       >>> sc.flatten(a, to='u')
       <scipp.DataArray>
       Dimensions: Sizes[u:6, ]
       Coordinates:
-        x                           int64  [dimensionless]  (u)  [0, 0, ..., 1, 1]
-        xy                          int64  [dimensionless]  (u)  [0, 1, ..., 4, 5]
-        y                           int64  [dimensionless]  (u)  [0, 1, ..., 1, 2]
+      * x                           int64  [dimensionless]  (u)  [0, 0, ..., 1, 1]
+      * xy                          int64  [dimensionless]  (u)  [0, 1, ..., 4, 5]
+      * y                           int64  [dimensionless]  (u)  [0, 1, ..., 1, 2]
       Data:
                                   float64  [dimensionless]  (u)  [0, 0.1, ..., 0.4, 0.5]
 
     """
     if to is None:
         # Note that this is a result of the fact that we want to support
         # calling flatten without kwargs, and that in this case it semantically
@@ -380,30 +380,29 @@
       >>> sc.squeeze(v)
       <scipp.Variable> (y: 3)      int64  [dimensionless]  [0, 1, 2]
       >>> sc.squeeze(v, 'z')
       <scipp.Variable> (x: 1, y: 3)      int64  [dimensionless]  [0, 1, 2]
       >>> sc.squeeze(v, ['x', 'z'])
       <scipp.Variable> (y: 3)      int64  [dimensionless]  [0, 1, 2]
 
-    Coordinates for squeezed dimensions are turned into attributes:
+    Coordinates for squeezed dimensions become unaligned:
 
       >>> da = sc.DataArray(v, coords={'x': sc.arange('x', 1),
       ...                              'y': sc.arange('y', 3)})
       >>> da
       <scipp.DataArray>
       Dimensions: Sizes[x:1, y:3, z:1, ]
       Coordinates:
-        x                           int64  [dimensionless]  (x)  [0]
-        y                           int64  [dimensionless]  (y)  [0, 1, 2]
+      * x                           int64  [dimensionless]  (x)  [0]
+      * y                           int64  [dimensionless]  (y)  [0, 1, 2]
       Data:
                                     int64  [dimensionless]  (x, y, z)  [0, 1, 2]
       >>> sc.squeeze(da)
       <scipp.DataArray>
       Dimensions: Sizes[y:3, ]
       Coordinates:
-        y                           int64  [dimensionless]  (y)  [0, 1, 2]
+        x                           int64  [dimensionless]  ()  0
+      * y                           int64  [dimensionless]  (y)  [0, 1, 2]
       Data:
                                     int64  [dimensionless]  (y)  [0, 1, 2]
-      Attributes:
-        x                           int64  [dimensionless]  ()  0
     """
     return _call_cpp_func(_cpp.squeeze, x, (dim,) if isinstance(dim, str) else dim)
```

### Comparing `scipp-23.5.0/src/scipp/core/structured.py` & `scipp-23.7.0/src/scipp/core/structured.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/trigonometry.py` & `scipp-23.7.0/src/scipp/core/trigonometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/unary.py` & `scipp-23.7.0/src/scipp/core/unary.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/util.py` & `scipp-23.7.0/src/scipp/core/util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/core/variable.py` & `scipp-23.7.0/src/scipp/core/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     *,
     dims: Sequence[str] = None,
     shape: Sequence[int] = None,
     sizes: dict = None,
     unit: Union[Unit, str, None] = default_unit,
     dtype: DTypeLike = DType.float64,
     with_variances: bool = False,
+    aligned: bool = True,
 ) -> Variable:
     """Constructs a :class:`Variable` with uninitialized values with given
     dimension labels and shape.
 
     The dims and shape can also be specified using a `sizes` dict.
 
     Warning
@@ -267,14 +268,16 @@
         Optional, dimension label to size map.
     unit:
         Unit of contents.
     dtype: scipp.typing.DTypeLike
         Type of underlying data.
     with_variances:
         If True includes uninitialized variances.
+    aligned:
+        Initial value for the alignment flag.
 
     Returns
     -------
     :
         A variable with uninitialized elements.
 
     See Also
@@ -290,14 +293,15 @@
       <scipp.Variable> (x: 4)    float64  [dimensionless]  [2, 2, 2, 2]
     """
     return _cpp.empty(
         **_parse_dims_shape_sizes(dims, shape, sizes),
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
+        aligned=aligned,
     )
 
 
 def full(
     *,
     value: Any,
     variance: Any = None,
@@ -390,15 +394,15 @@
 
       >>> sc.vector(value=[1, 2, 3])
       <scipp.Variable> ()    vector3  [dimensionless]  (1, 2, 3)
 
       >>> sc.vector(value=[4, 5, 6], unit='m')
       <scipp.Variable> ()    vector3              [m]  (4, 5, 6)
     """
-    return _cpp.vectors(dims=[], unit=unit, values=value)
+    return vectors(dims=(), values=value, unit=unit)
 
 
 def vectors(
     *,
     dims: Sequence[str],
     values: Union[_np.ndarray, list],
     unit: Union[Unit, str, None] = default_unit,
@@ -439,15 +443,15 @@
       >>> var.values
       array([[1., 2., 3.],
              [4., 5., 6.]])
 
       >>> sc.vectors(dims=['x'], values=[[1, 2, 3], [4, 5, 6]], unit='mm')
       <scipp.Variable> (x: 2)    vector3             [mm]  [(1, 2, 3), (4, 5, 6)]
     """
-    return _cpp.vectors(dims=dims, unit=unit, values=values)
+    return _cpp.Variable(dims=dims, values=values, unit=unit, dtype=DType.vector3)
 
 
 def array(
     *,
     dims: Iterable[str],
     values: ArrayLike,
     variances: Optional[ArrayLike] = None,
```

### Comparing `scipp-23.5.0/src/scipp/data/__init__.py` & `scipp-23.7.0/src/scipp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/format/_parse.py` & `scipp-23.7.0/src/scipp/format/_parse.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/format/formatter.py` & `scipp-23.7.0/src/scipp/format/formatter.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/geometry.py` & `scipp-23.7.0/src/scipp/geometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/__init__.py` & `scipp-23.7.0/src/scipp/html/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/formatting_datagroup_html.py` & `scipp-23.7.0/src/scipp/html/formatting_datagroup_html.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/formatting_html.py` & `scipp-23.7.0/src/scipp/html/formatting_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,20 +181,19 @@
         "<use xlink:href='#{0}'>"
         "</use>"
         "</svg>".format(icon_name)
     )
 
 
 def summarize_coord(dim, var, ds=None):
-    is_index = dim in var.dims
-    return summarize_variable(str(dim), var, is_index, embedded_in=ds)
+    return summarize_variable(str(dim), var, is_aligned=var.aligned, embedded_in=ds)
 
 
 def summarize_mask(dim, var, ds=None):
-    return summarize_variable(str(dim), var, is_index=False, embedded_in=ds)
+    return summarize_variable(str(dim), var, is_aligned=False, embedded_in=ds)
 
 
 def summarize_coords(coords, ds=None):
     vars_li = "".join(
         "<li class='sc-var-item'>" f"{summarize_coord(dim, var, ds)}" "</span></li>"
         for dim, var in _ordered_dict(coords).items()
     )
@@ -213,15 +212,15 @@
     attrs_li = "".join(
         "<li class='sc-var-item'>{}</li>".format(
             summarize_variable(
                 name,
                 var,
                 has_attrs=False,
                 embedded_in=embedded_in,
-                is_index=name in var.dims,
+                is_aligned=False,
             )
         )
         for name, var in _ordered_dict(attrs).items()
     )
     return f"<ul class='sc-var-list'>{attrs_li}</ul>"
 
 
@@ -290,27 +289,27 @@
         )
         for dim, size in zip(var.dims, var.shape)
     )
     return dims_text
 
 
 def _format_common(is_index):
-    cssclass_idx = " class='sc-has-index'" if is_index else ""
+    cssclass_aligned = " class='sc-aligned'" if is_index else ""
 
     # "unique" ids required to expand/collapse subsections
     attrs_id = "attrs-" + str(uuid.uuid4())
     data_id = "data-" + str(uuid.uuid4())
     attrs_icon = _icon("icon-file-text2")
     data_icon = _icon("icon-database")
 
-    return cssclass_idx, attrs_id, attrs_icon, data_id, data_icon
+    return cssclass_aligned, attrs_id, attrs_icon, data_id, data_icon
 
 
 def summarize_variable(
-    name, var, is_index=False, has_attrs=False, embedded_in=None, add_dim_size=False
+    name, var, is_aligned=False, has_attrs=False, embedded_in=None, add_dim_size=False
 ):
     """
     Formats the variable data into the format expected when displaying
     as a standalone variable (when a single variable or data array is
     displayed) or as part of a dataset.
     """
     dims_str = "({})".format(
@@ -333,24 +332,26 @@
         data_repr = "Values:<br>" + data_repr
     variances_preview = None
     if var.variances is not None:
         variances_preview = _make_row(inline_variable_repr(var, has_variances=True))
         data_repr += f"<br><br>Variances ({VARIANCES_SYMBOL}):<br>\
 {short_data_repr_html(var, variances=True)}"
 
-    cssclass_idx, attrs_id, attrs_icon, data_id, data_icon = _format_common(is_index)
+    cssclass_aligned, attrs_id, attrs_icon, data_id, data_icon = _format_common(
+        is_aligned
+    )
 
     if name is None:
         html = [
-            f"<div class='sc-standalone-var-name'><span{cssclass_idx}>"
+            f"<div class='sc-standalone-var-name'><span{cssclass_aligned}>"
             f"{escape(dims_str)}</span></div>"
         ]
     else:
         html = [
-            f"<div class='sc-var-name'><span{cssclass_idx}>{escape(str(name))}"
+            f"<div class='sc-var-name'><span{cssclass_aligned}>{escape(str(name))}"
             "</span></div>",
             f"<div class='sc-var-dims'>{escape(dims_str)}</div>",
         ]
     html += [
         f"<div class='sc-var-dtype'>{escape(str(var.dtype))}</div>",
         f"<div class='sc-var-unit'>{escape(unit)}</div>",
         f"<div class='sc-value-preview sc-preview'><span>{preview}</span>",
@@ -374,15 +375,15 @@
 
 def summarize_data(dataset):
     has_attrs = isinstance(dataset, sc.Dataset)
     vars_li = "".join(
         "<li class='sc-var-item'>{}</li>".format(
             summarize_variable(
                 name,
-                var,
+                var.data,
                 has_attrs=has_attrs,
                 embedded_in=dataset if has_attrs else None,
             )
         )
         for name, var in _ordered_dict(dataset).items()
     )
     return f"<ul class='sc-var-list'>{vars_li}</ul>"
```

### Comparing `scipp-23.5.0/src/scipp/html/resources.py` & `scipp-23.7.0/src/scipp/html/resources.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/table.py` & `scipp-23.7.0/src/scipp/html/table.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/datagroup.css` & `scipp-23.7.0/src/scipp/html/templates/datagroup.css`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/dg_atomic_row.html` & `scipp-23.7.0/src/scipp/html/templates/dg_atomic_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/dg_collapsible_row.html` & `scipp-23.7.0/src/scipp/html/templates/dg_collapsible_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/dg_detail_list.html` & `scipp-23.7.0/src/scipp/html/templates/dg_detail_list.html`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/dg_repr.html` & `scipp-23.7.0/src/scipp/html/templates/dg_repr.html`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/icons-svg-inline.html` & `scipp-23.7.0/src/scipp/html/templates/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/html/templates/style.css.template` & `scipp-23.7.0/src/scipp/html/templates/style.css.template`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 */
 .sc-dim-list li span,
 .sc-standalone-var-name > span span,
 .sc-var-name > span span {
   padding: 0 !important;
 }
 
-.sc-has-index {
+.sc-aligned {
   font-weight: bold;
 }
 
 .sc-var-list,
 .sc-var-item,
 .reveal .sc-var-list,
 .reveal .sc-var-item {
```

### Comparing `scipp-23.5.0/src/scipp/io/hdf5.py` & `scipp-23.7.0/src/scipp/io/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         _write_scipp_header(group, 'Variable')
         dset = cls._write_data(group, var)
         dset.attrs['dims'] = [str(dim) for dim in var.dims]
         dset.attrs['shape'] = var.shape
         dset.attrs['dtype'] = str(var.dtype)
         if var.unit is not None:
             dset.attrs['unit'] = _serialize_unit(var.unit)
+        dset.attrs['aligned'] = var.aligned
         return group
 
     @classmethod
     def read(cls, group):
         _check_scipp_header(group, 'Variable')
         from .._scipp import core as sc
         from .._scipp.core import DType as d
@@ -273,14 +274,15 @@
         contents = {key: values.attrs[key] for key in ['dims', 'shape']}
         contents['dtype'] = cls._dtypes[values.attrs['dtype']]
         if 'unit' in values.attrs:
             contents['unit'] = _read_unit_attr(values)
         else:
             contents['unit'] = None  # essential, otherwise default unit is used
         contents['with_variances'] = 'variances' in group
+        contents['aligned'] = values.attrs.get('aligned', True)
         if contents['dtype'] in [d.VariableView, d.DataArrayView, d.DatasetView]:
             var = BinDataIO.read(group)
         else:
             var = sc.empty(**contents)
             cls._read_data(group, var)
         return var
```

### Comparing `scipp-23.5.0/src/scipp/logging.py` & `scipp-23.7.0/src/scipp/logging.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/object_list.py` & `scipp-23.7.0/src/scipp/object_list.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/operations.py` & `scipp-23.7.0/src/scipp/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/__init__.py` & `scipp-23.7.0/src/scipp/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/controller.py` & `scipp-23.7.0/src/scipp/plotting/controller.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/controller1d.py` & `scipp-23.7.0/src/scipp/plotting/controller1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/controller2d.py` & `scipp-23.7.0/src/scipp/plotting/controller2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/controller3d.py` & `scipp-23.7.0/src/scipp/plotting/controller3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/dispatch.py` & `scipp-23.7.0/src/scipp/plotting/dispatch.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/displayable.py` & `scipp-23.7.0/src/scipp/plotting/displayable.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/figure.py` & `scipp-23.7.0/src/scipp/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/figure1d.py` & `scipp-23.7.0/src/scipp/plotting/figure1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/figure2d.py` & `scipp-23.7.0/src/scipp/plotting/figure2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/figure3d.py` & `scipp-23.7.0/src/scipp/plotting/figure3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/formatters.py` & `scipp-23.7.0/src/scipp/plotting/formatters.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/model.py` & `scipp-23.7.0/src/scipp/plotting/model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/model1d.py` & `scipp-23.7.0/src/scipp/plotting/model1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/model2d.py` & `scipp-23.7.0/src/scipp/plotting/model2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/model3d.py` & `scipp-23.7.0/src/scipp/plotting/model3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/objects.py` & `scipp-23.7.0/src/scipp/plotting/objects.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/panel.py` & `scipp-23.7.0/src/scipp/plotting/panel.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/panel1d.py` & `scipp-23.7.0/src/scipp/plotting/panel1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/panel3d.py` & `scipp-23.7.0/src/scipp/plotting/panel3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/plot1d.py` & `scipp-23.7.0/src/scipp/plotting/plot1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/plot2d.py` & `scipp-23.7.0/src/scipp/plotting/plot2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/plot3d.py` & `scipp-23.7.0/src/scipp/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/profile.py` & `scipp-23.7.0/src/scipp/plotting/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/resampling_model.py` & `scipp-23.7.0/src/scipp/plotting/resampling_model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/toolbar.py` & `scipp-23.7.0/src/scipp/plotting/toolbar.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/tools.py` & `scipp-23.7.0/src/scipp/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/view.py` & `scipp-23.7.0/src/scipp/plotting/view.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/view1d.py` & `scipp-23.7.0/src/scipp/plotting/view1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/view2d.py` & `scipp-23.7.0/src/scipp/plotting/view2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/view3d.py` & `scipp-23.7.0/src/scipp/plotting/view3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/widgets.py` & `scipp-23.7.0/src/scipp/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/plotting/wrapper.py` & `scipp-23.7.0/src/scipp/plotting/wrapper.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/reduction.py` & `scipp-23.7.0/src/scipp/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/scipy/integrate/__init__.py` & `scipp-23.7.0/src/scipp/scipy/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/scipy/interpolate/__init__.py` & `scipp-23.7.0/src/scipp/scipy/interpolate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,23 +141,23 @@
       >>> f = interp1d(da, 'x')
 
       >>> xnew = sc.linspace(dim='x', start=0.1, stop=1.4, num=12, unit='rad')
       >>> f(xnew)  # use interpolation function returned by `interp1d`
       <scipp.DataArray>
       Dimensions: Sizes[x:12, ]
       Coordinates:
-        x                         float64            [rad]  (x)  [0.1, 0.218182, ..., 1.28182, 1.4]
+      * x                         float64            [rad]  (x)  [0.1, 0.218182, ..., 1.28182, 1.4]
       Data:
                                   float64  [dimensionless]  (x)  [0.0998334, 0.211262, ..., 0.941144, 0.98545]
 
       >>> f(xnew, midpoints=True)
       <scipp.DataArray>
       Dimensions: Sizes[x:11, ]
       Coordinates:
-        x                         float64            [rad]  (x [bin-edge])  [0.1, 0.218182, ..., 1.28182, 1.4]
+      * x                         float64            [rad]  (x [bin-edge])  [0.1, 0.218182, ..., 1.28182, 1.4]
       Data:
                                   float64  [dimensionless]  (x)  [0.155548, 0.266977, ..., 0.918992, 0.963297]
 
     .. plot:: :context: close-figs
 
       >>> sc.plot({'original':da,
       ...          'interp1d':f(xnew),
```

### Comparing `scipp-23.5.0/src/scipp/scipy/ndimage/__init__.py` & `scipp-23.7.0/src/scipp/scipy/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/scipy/optimize/__init__.py` & `scipp-23.7.0/src/scipp/scipy/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/scipy/signal/__init__.py` & `scipp-23.7.0/src/scipp/scipy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/serialization.py` & `scipp-23.7.0/src/scipp/serialization.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/show.py` & `scipp-23.7.0/src/scipp/show.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,21 @@
         f'<svg width={_svg_width}em viewBox="{left} {top} {width} {height}"'
         ' class="sc-root">'
         f'<defs>{load_style()}</defs>{content}</svg>'
     )
 
 
 class VariableDrawer:
-    def __init__(self, variable, margin=1.0, target_dims=None):
+    def __init__(self, variable, margin=1.0, target_dims=None, show_alignment=False):
         self._margin = margin
         self._variable = variable
         self._target_dims = target_dims
         if self._target_dims is None:
             self._target_dims = self._dims()
+        self._show_alignment = show_alignment
         self._x_stride = 1
         if len(self._dims()) > 3:
             raise RuntimeError("Cannot visualize {}-D data".format(len(self._dims())))
 
     def _dims(self):
         dims = self._variable.dims
         return dims
@@ -231,25 +232,30 @@
             self._variable.dims,
             self._variable.shape,
             unit,
             self._variable.variances is not None,
         )
         x_pos = offset[0]
         y_pos = offset[1] + 0.6
+        weight = (
+            "font-weight: bold"
+            if self._show_alignment and self._variable.aligned
+            else ""
+        )
         if title is not None:
             # Crudely avoid label overlap, ignoring actual character width
             brief_title = _truncate_long_string(str(title), int(2.5 * self.size()[0]))
             svg = f'<text x="{x_pos}" y="{y_pos}" \
-                    class="sc-name" style="font-size:#normal-font"> \
+                    class="sc-name" style="font-size:#normal-font;{weight}"> \
                     {escape(brief_title)}</text>'
 
             svg += f'<title>{title}({escape(details)})</title>'
         else:
             svg = f'<text x="{x_pos}" y="{y_pos}" \
-                    class="sc-name" style="font-size:#small-font"> \
+                    class="sc-name" style="font-size:#small-font;{weight}"> \
                     {escape(details)}</text>'
 
         return svg
 
     def _draw_bins_buffer(self):
         if self._variable.bins is None:
             return ''
@@ -310,23 +316,26 @@
             0,
             max(_cubes_in_full_width, self.size()[0]),
             self.size()[1],
         )
 
 
 class DrawerItem:
-    def __init__(self, name, data, color):
+    def __init__(self, name, data, colors, show_alignment=False):
         self._name = name
         self._data = data
-        self._color = color
+        self._color = colors
+        self._show_alignment = show_alignment
 
     def append_to_svg(
         self, content, width, height, offset, layout_direction, margin, dims
     ):
-        drawer = VariableDrawer(self._data, margin, target_dims=dims)
+        drawer = VariableDrawer(
+            self._data, margin, target_dims=dims, show_alignment=self._show_alignment
+        )
         content += drawer.draw(color=self._color, offset=offset, title=self._name)
         size = drawer.size()
         width, height, offset = _new_size_and_offset(
             size, width, height, layout_direction
         )
         return content, width, height, offset
 
@@ -365,15 +374,15 @@
     def _dims(self):
         dims = self._dataset.dims
         if isinstance(self._dataset, sc.DataArray):
             # Handle, e.g., bin edges of a slice, where data lacks the edge dim
             for item in self._dataset.meta.values():
                 for dim in item.dims:
                     if dim not in dims:
-                        dims = [dim] + dims
+                        dims = (dim,) + dims
         if len(dims) > 3:
             raise RuntimeError("Cannot visualize {}-D data".format(len(dims)))
         return dims
 
     def make_svg(self, content_only=False):
         content = ''
         width = 0
@@ -403,20 +412,20 @@
         # coordinates, but in a static picture there is probably no other way.
         area_x = []
         area_y = []
         area_z = []
         area_xy = []
         area_0d = []
         if isinstance(self._dataset, sc.DataArray):
-            area_xy.append(DrawerItem('', self._dataset, config['colors']['data']))
+            area_xy.append(DrawerItem('', self._dataset.data, config['colors']['data']))
         else:
             # Render highest-dimension items last so coords are optically
             # aligned
             for name, data in sorted(self._dataset.items()):
-                item = DrawerItem(name, data, config['colors']['data'])
+                item = DrawerItem(name, data.data, config['colors']['data'])
                 # Using only x and 0d areas for 1-D dataset
                 if len(dims) == 1 or data.dims != dims:
                     if len(data.dims) == 0:
                         area_0d.append(item)
                     elif len(data.dims) != 1:
                         area_xy[-1:-1] = [item]
                     elif data.dims[0] == dims[-1]:
@@ -433,15 +442,17 @@
             categories = zip(
                 ['coords', 'masks', 'attrs'], [ds.coords, ds.masks, ds.attrs]
             )
         else:
             categories = zip(['coords'], [ds.coords])
         for what, items in categories:
             for name, var in sorted(items.items()):
-                item = DrawerItem(name, var, config['colors'][what])
+                item = DrawerItem(
+                    name, var, config['colors'][what], show_alignment=what == 'coords'
+                )
                 if len(var.dims) == 0:
                     area_0d.append(item)
                 elif var.dims[-1] == dims[-1]:
                     area_x.append(item)
                 elif var.dims[-1] == dims[-2]:
                     area_y.append(item)
                 else:
```

### Comparing `scipp-23.5.0/src/scipp/spatial/__init__.py` & `scipp-23.7.0/src/scipp/spatial/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Sequence, Union
 
 import numpy as _np
 import numpy as np
 
 from .. import units
 from .._scipp import core as _core_cpp
-from ..core import Unit, UnitError, Variable, vectors
+from ..core import DType, Unit, UnitError, Variable, vectors
 from ..core._cpp_wrapper_util import call_func as _call_cpp_func
 
 
 def _to_eigen_layout(a):
     # Numpy and scipp use row-major, but Eigen matrices use column-major,
     # transpose matrix axes for copying values.
     return _np.moveaxis(a, -1, -2)
@@ -87,15 +87,15 @@
         A list or NumPy array of 3 items
 
     Returns
     -------
     :
         A scalar variable of dtype ``translation3``.
     """
-    return _call_cpp_func(_core_cpp.translations, dims=[], unit=unit, values=value)
+    return translations(dims=(), unit=unit, values=value)
 
 
 def translations(
     *,
     dims: Sequence[str],
     unit: Union[Unit, str] = units.dimensionless,
     values: Union[_np.ndarray, list],
@@ -113,15 +113,17 @@
         A list or NumPy array of 3-vectors
 
     Returns
     -------
     :
         An array variable of dtype ``translation3``.
     """
-    return _call_cpp_func(_core_cpp.translations, dims=dims, unit=unit, values=values)
+    return _core_cpp.Variable(
+        dims=dims, unit=unit, values=values, dtype=DType.translation3
+    )
 
 
 def scaling_from_vector(*, value: Union[_np.ndarray, list]):
     """
     Creates a scaling transformation from a provided 3-vector.
 
     Parameters
@@ -190,15 +192,15 @@
         coefficients (x*i, y*j, z*k, w)
 
     Returns
     -------
     :
         A scalar variable of dtype ``rotation3``.
     """
-    return _call_cpp_func(_core_cpp.rotations, dims=[], values=value)
+    return rotations(dims=(), values=value)
 
 
 def rotations(*, dims: Sequence[str], values: Union[_np.ndarray, list]):
     """
     Creates a rotation-type variable from the provided quaternion coefficients.
 
     The quaternion coefficients are provided in scalar-last order (x, y, z, w), where
@@ -234,15 +236,15 @@
     values = np.asarray(values)
     if values.shape[-1] != 4:
         raise ValueError(
             "Inputs must be Quaternions to create a rotation, i.e., have "
             "4 components. If you want to pass a rotation matrix, use "
             "sc.linear_transforms instead."
         )
-    return _call_cpp_func(_core_cpp.rotations, dims=dims, values=values)
+    return _core_cpp.Variable(dims=dims, values=values, dtype=DType.rotation3)
 
 
 def rotations_from_rotvecs(rotation_vectors: Variable) -> Variable:
     """
     Creates rotation transformations from rotation vectors.
 
     This requires ``scipy`` to be installed, as is wraps
@@ -351,19 +353,19 @@
         An array of 4x4 matrices of affine coefficients.
 
     Returns
     -------
     :
         An array variable of dtype ``affine_transform3``.
     """
-    return _call_cpp_func(
-        _core_cpp.affine_transforms,
+    return _core_cpp.Variable(
         dims=dims,
         unit=unit,
         values=_to_eigen_layout(values),
+        dtype=DType.affine_transform3,
     )
 
 
 def linear_transform(
     *,
     unit: Union[Unit, str] = units.dimensionless,
     value: Union[_np.ndarray, list],
@@ -379,16 +381,18 @@
         Optional, unit. Default=dimensionless
 
     Returns
     -------
     :
         A scalar variable of dtype ``linear_transform3``.
     """
-    return _call_cpp_func(
-        _core_cpp.matrices, dims=[], unit=unit, values=_to_eigen_layout(value)
+    return linear_transforms(
+        dims=(),
+        unit=unit,
+        values=value,
     )
 
 
 def linear_transforms(
     *,
     dims: Sequence[str],
     unit: Union[Unit, str] = units.dimensionless,
@@ -407,16 +411,19 @@
         Optional, data unit. Default=dimensionless
 
     Returns
     -------
     :
         An array variable of dtype ``linear_transform3``.
     """
-    return _call_cpp_func(
-        _core_cpp.matrices, dims=dims, unit=unit, values=_to_eigen_layout(values)
+    return _core_cpp.Variable(
+        dims=dims,
+        unit=unit,
+        values=_to_eigen_layout(values),
+        dtype=DType.linear_transform3,
     )
 
 
 def inv(var: Variable) -> Variable:
     """Return the inverse of a spatial transformation.
 
     Parameters
```

### Comparing `scipp-23.5.0/src/scipp/sphinxext/autoplot.py` & `scipp-23.7.0/src/scipp/sphinxext/autoplot.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/testing/assertions.py` & `scipp-23.7.0/src/scipp/testing/assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,10 @@
     try:
         yield
     except AssertionError as exc:
         if hasattr(exc, 'add_note'):
             # Needs Python >= 3.11
             exc.add_note(f'PREPOSITION {loc.format(*args)}')
         raise
+
+
+__all__ = ['assert_identical']
```

### Comparing `scipp-23.5.0/src/scipp/testing/strategies.py` & `scipp-23.7.0/src/scipp/testing/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,7 +232,21 @@
     if coords is _NotSet:
         coords = data.dims
     if coords is not None:
         coord_dict = draw(coord_dicts(coords=coords, sizes=data.sizes, args=coord_args))
     else:
         coord_dict = {}
     return DataArray(data, coords=coord_dict)
+
+
+__all__ = [
+    'dims',
+    'sizes_dicts',
+    'units',
+    'integer_dtypes',
+    'floating_dtypes',
+    'scalar_numeric_dtypes',
+    'variables',
+    'n_variables',
+    'coord_dicts',
+    'dataarrays',
+]
```

### Comparing `scipp-23.5.0/src/scipp/typing.py` & `scipp-23.7.0/src/scipp/typing.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/units/__init__.py` & `scipp-23.7.0/src/scipp/units/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/collapse_and_slices.py` & `scipp-23.7.0/src/scipp/utils/collapse_and_slices.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/colors.py` & `scipp-23.7.0/src/scipp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/comparison.py` & `scipp-23.7.0/src/scipp/utils/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/profile.py` & `scipp-23.7.0/src/scipp/utils/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/pyshell.py` & `scipp-23.7.0/src/scipp/utils/pyshell.py`

 * *Files identical despite different names*

### Comparing `scipp-23.5.0/src/scipp/utils/to_string.py` & `scipp-23.7.0/src/scipp/utils/to_string.py`

 * *Files identical despite different names*

